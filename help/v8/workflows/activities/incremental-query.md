---
audience: end-user
title: De incrementele activiteit van de querywerkstroom gebruiken
description: Leer hoe te om de Incrementele activiteit van het vraagwerkschema te gebruiken
exl-id: 72bd307b-eba2-42a0-9744-05e089c34925
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 5%

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

De **Incrementele vraag** activiteit is a **richtend** activiteit die u toestaat om het gegevensbestand op een geplande basis te vragen. Telkens wanneer deze activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten. Hierdoor kunt u alleen nieuwe elementen als doel instellen.

>[!NOTE]
>
>Terwijl de de cliëntconsole van de Campagne de **[!UICONTROL Incremental query]** activiteit met een ingebouwde planner integreert, behandelt het Gebruikersinterface van het Web van de Campagne deze functionaliteit afzonderlijk. Als u incrementele query-uitvoeringen wilt plannen, voegt u een **[!UICONTROL Scheduler]** -activiteit toe in de workflow vóór de **[!UICONTROL Incremental query]** -activiteit. [&#x200B; Leer hoe te om een activiteit van de Planner te vormen &#x200B;](scheduler.md)

De **[!UICONTROL Incremental query]** -activiteit kan voor verschillende doeleinden worden gebruikt:

* Het segmenteren van individuen om het doel van een bericht, een publiek, of andere verrichtingen te bepalen.
* Gegevens exporteren. U kunt bijvoorbeeld de activiteit gebruiken om regelmatig nieuwe aanmeldbestanden te exporteren. Dit is nuttig voor externe rapportering of bedrijfsintelligentiegereedschappen.

De bevolking die al het doelwit is van eerdere uitvoeringen, wordt opgeslagen in de workflow. Twee werkschema&#39;s begonnen van het zelfde malplaatje delen niet het zelfde logboek. Nochtans, gebruiken twee taken die op de zelfde stijgende vraag in het zelfde werkschema worden gebaseerd het zelfde logboek.

Als het resultaat van een stijgende vraag 0 tijdens één van zijn uitvoeringen evenaart, pauzeert het werkschema tot de volgende geprogrammeerde uitvoering van de vraag. De overgangen en activiteiten die volgen op de incrementele query worden niet verwerkt vóór de volgende uitvoering.

## Vorm de Incrementele vraagactiviteit {#incremental-query-configuration}

Volg deze stappen om de **Incrementele vraag** activiteit te vormen:

[ Beschrijving: Schermschot die de configuratieinterface voor de Incrementele vraagactiviteit in Adobe Campaign tonen.]\
![](../assets/incremental-query.png)

1. Voeg een **Incrementele vraag** activiteit in uw werkschema toe.

1. In de **[!UICONTROL Audience]** sectie, kies de **Doelende afmeting**, dan klik **[!UICONTROL Continue]**.

   De doelgerichte dimensie definieert de bevolking waarop de actie gericht is, zoals ontvangers, begunstigden van contracten, exploitanten of abonnees. Standaard is het doel geselecteerd bij de ontvangers. [&#x200B; leer meer over het richten van dimensies &#x200B;](../../audience/about-recipients.md#targeting-dimensions)

1. Gebruik de vraagmodeler om uw vraag te bepalen, gelijkend op hoe u een publiek wanneer het ontwerpen van een nieuwe e-mail creeert. [&#x200B; Leer hoe te met de vraagmodelaar &#x200B;](../../query/query-modeler-overview.md) te werken

1. Selecteer in de sectie **[!UICONTROL Processed data]** de incrementele modus die u wilt gebruiken:

   * **[!UICONTROL Exclude results of previous execution]**: Telkens wanneer de activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten.

     Records die al in eerdere uitvoeringen zijn bedoeld, kunnen worden geregistreerd gedurende een maximumaantal dagen vanaf de dag waarop ze als doel zijn genomen. Stel deze waarde in in het veld **[!UICONTROL History in days]** . Als deze waarde nul is, worden de ontvangers nooit gezuiverd van het logboek.

   * **[!UICONTROL Use a date field]**: deze optie sluit resultaten uit van eerdere uitvoeringen op basis van een bepaald datumveld. Kies het gewenste datumveld in de lijst met kenmerken die beschikbaar zijn voor de geselecteerde doeldimensie. Bij volgende uitvoeringen van de workflow worden alleen gegevens opgehaald die na de laatste uitvoeringsdatum zijn gewijzigd of gemaakt.

     Na de eerste uitvoering van de workflow wordt het veld **[!UICONTROL Last execution date]** beschikbaar. Hiermee wordt de datum aangegeven die wordt gebruikt voor de volgende uitvoering en wordt deze automatisch bijgewerkt telkens wanneer de workflow wordt uitgevoerd. U kunt deze waarde handmatig overschrijven om aan uw wensen te voldoen.

   >[!NOTE]
   >
   >De modus **[!UICONTROL Use a date field]** biedt meer flexibiliteit, afhankelijk van het geselecteerde datumveld. Als het opgegeven veld bijvoorbeeld overeenkomt met een wijzigingsdatum, haalt de datumveldmodus de onlangs bijgewerkte gegevens op. In de andere modus zijn geen opnamen opgenomen die al eerder als doel waren ingesteld, zelfs niet als deze zijn gewijzigd sinds de laatste uitvoering van de workflow.

## Voorbeeld {#incremental-query-example}

In het volgende voorbeeld ziet u de configuratie van een workflow die profielen in de Adobe Campaign-database elke week filtert. Het is gericht op personen die zijn geabonneerd op de Yoga Newsletter-service en stuurt hen een welkome e-mail.

![&#x200B; Screenshot van een configuratie van het voorbeeldwerkschema voor het filtreren van profielen die aan de dienst van het Nieuwsbrief Yoga worden ingetekend.](../assets/incremental-query-example.png)

De workflow bevat de volgende elementen:

* Een **[!UICONTROL Scheduler]** -activiteit die de workflow elke maandag om 6.00 uur uitvoert.
* Een **[!UICONTROL Incremental query]** activiteit, die alle huidige abonnees tijdens de eerste uitvoering en slechts nieuwe abonnees tijdens verdere uitvoeringen richt.
* Een **[!UICONTROL Email delivery]** activiteit.