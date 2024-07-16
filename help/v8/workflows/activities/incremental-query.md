---
audience: end-user
title: De incrementele activiteit van de querywerkstroom gebruiken
description: Leer hoe te om de Incrementele activiteit van het vraagwerkschema te gebruiken
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '716'
ht-degree: 20%

---

# Incrementele query {#incremental-query}



>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery"
>title="Incrementele query"
>abstract="De **Incrementele vraag** activiteit is a **richtend** activiteit die u toestaat om het gegevensbestand te vragen gebruikend de modelleur van de Vraag. Telkens wanneer deze activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten. Zo kunt u doelgericht alleen nieuwe elementen benaderen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_history"
>title="Incrementele querygeschiedenis"
>abstract="Incrementele querygeschiedenis"

>[!CONTEXTUALHELP]
>id="acw_orchestration_incrementalquery_processeddata"
>title="Incrementele query verwerkte gegevens"
>abstract="Incrementele query verwerkte gegevens"

De **Incrementele vraag** activiteit is a **richtend** activiteit die u toestaat om het gegevensbestand op een geplande basis te vragen. Telkens wanneer deze activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten. Zo kunt u doelgericht alleen nieuwe elementen benaderen.

>[!NOTE]
>
>Terwijl de de cliëntconsole van de Campagne de **[!UICONTROL Incremental query]** activiteit met een ingebouwde planner integreert, behandelt het Gebruikersinterface van het Web van de Campagne deze functionaliteit afzonderlijk. Als u incrementele query-uitvoeringen wilt plannen, moet u een **[!UICONTROL Scheduler]** -activiteit in de workflow toevoegen voordat de **[!UICONTROL Incremental query]** -activiteit plaatsvindt. [ Leer hoe te om een activiteit van de Planner te vormen ](scheduler.md)

De activiteit **[!UICONTROL Incremental query]** kan voor diverse doeleinden worden gebruikt:

* Individuele gebruikers segmenteren om het doel van een bericht, doelgroep, enz te bepalen.
* Gegevens exporteren. U kunt de activiteit bijvoorbeeld gebruiken om regelmatig nieuwe aanmeldbestanden te exporteren. Het kan nuttig zijn als u uw logboekgegevens in externe rapportering of hulpmiddelen wilt gebruiken BI.

De bevolking die al het doelwit is van eerdere uitvoeringen, wordt opgeslagen in de workflow. Dit betekent dat twee werkschema&#39;s die van het zelfde malplaatje begonnen zijn niet het zelfde logboek delen. Nochtans, gebruiken twee taken die op de zelfde stijgende vraag in het zelfde werkschema worden gebaseerd het zelfde logboek.

Als het resultaat van een stijgende vraag aan 0 tijdens één van zijn uitvoeringen gelijk is, wordt het werkschema gepauzeerd tot de volgende geprogrammeerde uitvoering van de vraag. De overgangen en de activiteiten die volgen op de stijgende vraag worden daarom niet verwerkt vóór de volgende uitvoering.

## Vorm de Incrementele vraagactiviteit {#incremental-query-configuration}

Volg deze stappen om de **Incrementele vraag** activiteit te vormen:

![](../assets/incremental-query.png)

1. Voeg een **Incrementele vraag** activiteit in uw werkschema toe.

1. In de **[!UICONTROL Audience]** sectie, kies de **Doelende afmeting** dan klik **[!UICONTROL Continue]**.

   Met de doeldimensie kunt u de doelgroep van de actie definiëren: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. Standaard is het doel geselecteerd bij de ontvangers. [ leer meer over het richten van dimensies ](../../audience/about-recipients.md#targeting-dimensions)

1. Gebruik de vraagmodeler om uw vraag te bepalen, de zelfde manier u creeert een publiek wanneer het ontwerpen van een nieuwe e-mail. [ Leer hoe te met de vraagmodelaar ](../../query/query-modeler-overview.md) te werken

1. Selecteer in de sectie **[!UICONTROL Processed data]** de incrementele modus die u wilt gebruiken:

   * **[!UICONTROL Exclude results of previous execution]**: Telkens wanneer de activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten.

     Records die al in eerdere uitvoeringen zijn bedoeld, kunnen worden geregistreerd gedurende een maximumaantal dagen vanaf de dag waarop ze als doel zijn gebruikt. Gebruik hiervoor het veld **[!UICONTROL History in days]** . Als deze waarde nul is, worden de ontvangers nooit gezuiverd van het logboek.

   * **[!UICONTROL Use a date field]**: met deze optie kunt u resultaten uitsluiten van vorige uitvoeringen op basis van een bepaald datumveld. Hiervoor kiest u het gewenste datumveld in de lijst met kenmerken die beschikbaar zijn voor de geselecteerde doeldimensie. Bij de volgende uitvoeringen van de workflow worden alleen gegevens opgehaald die na de laatste uitvoeringsdatum zijn gewijzigd of gemaakt.

     Na de eerste uitvoering van de workflow wordt het veld **[!UICONTROL Last execution date]** beschikbaar. Hiermee wordt de datum aangegeven die wordt gebruikt voor de volgende uitvoering en die automatisch wordt bijgewerkt telkens wanneer de workflow wordt uitgevoerd. U kunt deze waarde ook overschrijven door handmatig een nieuwe waarde in te voeren die beter aan uw behoeften voldoet.

   >[!NOTE]
   >
   >In de modus **[!UICONTROL Use a date field]** is meer flexibiliteit mogelijk, afhankelijk van het datumveld dat is geselecteerd. Als het opgegeven veld bijvoorbeeld overeenkomt met een wijzigingsdatum, kunt u in de modus Datumveld gegevens ophalen die onlangs zijn bijgewerkt, terwijl in de andere modus alleen opnamen worden uitgesloten die in een vorige uitvoering al als doel waren ingesteld, zelfs als deze zijn gewijzigd sinds de laatste uitvoering van de workflow.

## Voorbeeld {#incremental-query-example}

In het volgende voorbeeld ziet u de configuratie van een workflow die elke week de profielen in de Adobe Campaign-database filtert die zijn geabonneerd op de Yoga Newsletter-service en die hen een welkome e-mail stuurt.

![](../assets/incremental-query-example.png)

De workflow bestaat uit de volgende elementen:

* Een activiteit **[!UICONTROL Scheduler]**, om de workflow elke maandag om 6.00 uur uit te voeren.
* Een activiteit **[!UICONTROL Incremental query]**, die zich tijdens de eerste uitvoering richt op alle huidige abonnees en daarna alleen op de nieuwe abonnees van die week tijdens de volgende uitvoeringen.
* Een **[!UICONTROL Email delivery]** activiteit.
