---
audience: end-user
title: De werkstroomactiviteit Splitsen gebruiken
description: Leer hoe u de activiteit van de gesplitste workflow gebruikt
exl-id: 4457c70d-bc92-476f-90a3-d51e26ada8f1
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 0%

---

# Splitsen {#split}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split"
>title="Gesplitste activiteit"
>abstract="De **Splitsen** met activiteit kunt u inkomende populaties segmenteren in meerdere subsets op basis van verschillende selectiecriteria, zoals filterregels of populatiegrootte."

De **Splitsen** activiteit is **Targeting** activiteit die u toestaat om inkomende populaties in veelvoudige subsets te segmenteren die op verschillende selectiecriteria, zoals het filtreren regels of populatiegrootte worden gebaseerd.

## De activiteit Splitsen configureren {#split-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_segments"
>title="Segmenten voor splitsingsactiviteit"
>abstract="Voeg zoveel subsets toe als u wilt om de binnenkomende populatie te segmenteren.<br/></br>Wanneer de **Splitsen** de activiteit wordt uitgevoerd, wordt de populatie over de verschillende subsets verdeeld in de volgorde waarin ze aan de activiteit worden toegevoegd. Voordat u de workflow start, moet u de subsets in de gewenste volgorde ordenen met de pijlknoppen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_filter"
>title="Activiteitsfilter splitsen"
>abstract="Als u een filtervoorwaarde op de subset wilt toepassen, klikt u op **[!UICONTROL Create filter]** en vorm de gewenste het filtreren regel gebruikend de vraagmodeler. Neem bijvoorbeeld profielen op van de binnenkomende populatie waarvan het e-mailadres voorkomt in de database."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Werken met de querymodelfunctie"

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_limit"
>title="Limiet voor gesplitste activiteit"
>abstract="Als u het aantal profielen dat door de subset is geselecteerd, wilt beperken, schakelt u het **[!UICONTROL Enable limit]** en geeft het aantal of de percentages van de populatie aan die moeten worden opgenomen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_sorting"
>title="Splitsen op activiteit"
>abstract="Wanneer u een populatielimiet voor een subset instelt, kunt u de geselecteerde profielen op basis van een specifiek profielkenmerk in oplopende of aflopende volgorde rangschikken. Om dit te doen, knevel op **Sorteren inschakelen** -optie. U kunt bijvoorbeeld een subset beperken tot alleen de bovenste 50 profielen met het hoogste aankoopbedrag."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_complement"
>title="Splitsen genereert complement"
>abstract="Zodra u alle subsets hebt gevormd, kunt u de resterende populatie selecteren die geen van de subsets aanpast en hen in een extra uitgaande overgang omvat. Om dit te doen, knevel op **Complement genereren** -optie."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_generatesubsets"
>title="Alle subsets in dezelfde tabel genereren"
>abstract="Schakel deze optie in en uit om alle subsets te groeperen in één uitvoerovergang."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_emptytransition"
>title="Lege overgang overslaan"
>abstract="Schakelen tussen **[!UICONTROL Skip empty transition]** optie aan om de outputovergang voor deze ondergroep onbruikbaar te maken als de inkomende bevolking leeg is."

>[!CONTEXTUALHELP]
>id="acw_orchestration_split_enable_overlapping"
>title="Overlappende uitvoerpopulaties inschakelen"
>abstract="Overlappende uitvoerpopulaties inschakelen"

Voer de volgende stappen uit om de **Splitsen** activiteit:

1. Voeg een **Splitsen** activiteit aan uw werkschema.

1. Het deelvenster voor activiteitenconfiguratie wordt geopend met een standaardsubset. Klik op de knop **Segment toevoegen** om zoveel subsets toe te voegen als gewenst om de binnenkomende populatie te segmenteren.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Wanneer de **Splitsen** de activiteit wordt uitgevoerd, wordt de populatie over de verschillende subsets verdeeld in de volgorde waarin ze aan de activiteit worden toegevoegd. Als de eerste subset bijvoorbeeld 70% van de oorspronkelijke populatie herstelt, past de volgende toegevoegde subset zijn selectiecriteria alleen toe op de resterende 30%, enzovoort.
   >
   >Voordat u de workflow start, moet u ervoor zorgen dat u de subsets in de gewenste volgorde hebt geplaatst. Hiervoor gebruikt u de pijlknoppen om de positie van een subset te wijzigen.

1. Nadat subsets zijn toegevoegd, toont de activiteit evenveel uitvoerovergangen als er subsets zijn. We raden u ten zeerste aan het label van elke subset te wijzigen om deze gemakkelijk te identificeren in het werkstroomcanvas.

1. Vorm hoe elke ondergroep de inkomende bevolking zou moeten filtreren. Ga als volgt te werk om dit te doen:

   1. Open de subset om de eigenschappen ervan weer te geven.

   1. Als u een filtervoorwaarde op de subset wilt toepassen, klikt u op **[!UICONTROL Create filter]** en vorm de gewenste het filtreren regel gebruikend de vraagmodeler. Neem bijvoorbeeld profielen op van de binnenkomende populatie waarvan het e-mailadres voorkomt in de database. [Leer hoe te met vraagmodeler te werken](../../query/query-modeler-overview.md)

   1. Als u het aantal profielen dat door de subset is geselecteerd, wilt beperken, schakelt u het **[!UICONTROL Enable limit]** en geeft het aantal of de percentages van de populatie aan die moeten worden opgenomen.

   1. Om een overgang onbruikbaar te maken als de inkomende bevolking leeg is, knevel **[!UICONTROL Skip empty transition]** optie ingeschakeld. Als geen profiel overeenkomt met de subset, gaat de workflow niet naar de volgende activiteit.

      ![](../assets/workflow-split-subset.png)


      >[!NOTE]
      >
      >Wanneer u een populatielimiet voor een subset instelt, kunt u de geselecteerde profielen op basis van een specifiek profielkenmerk in oplopende of aflopende volgorde rangschikken. Om dit te doen, knevel op **[!UICONTROL Enable sorting]** -optie. U kunt bijvoorbeeld een subset beperken tot alleen de bovenste 50 profielen met het hoogste aankoopbedrag.

1. Zodra u alle subsets hebt gevormd, kunt u de resterende populatie selecteren die geen van de subsets aanpast en hen in een extra uitgaande overgang omvat. Om dit te doen, knevel op **[!UICONTROL Generate complement]** -optie.

   ![](../assets/workflow-split-complement.png)

   >[!NOTE]
   >
   >De **[!UICONTROL Generate all subsets in the same table]** kunt u alle subsets groeperen in één uitvoerovergang.

De activiteit wordt nu gevormd. Bij de uitvoering van de workflow wordt de populatie opgedeeld in de verschillende subsets, in de volgorde waarin ze aan de activiteit zijn toegevoegd.

## Voorbeeld{#split-example}

In het volgende voorbeeld wordt **[!UICONTROL Split]** De activiteit wordt gebruikt om een publiek in verschillende subsets te segmenteren die op het communicatiekanaal worden gebaseerd dat wij willen gebruiken:

* **Subset 1 &quot;push&quot;**: Deze subset bestaat uit alle profielen die onze mobiele toepassing hebben geïnstalleerd.
* **Subset 2 &quot;sms&quot;**: Gebruikers van mobiele telefoons: voor de resterende populatie die niet in Subset 1 viel, past subset 2 een filterregel toe op het selecteren van profielen met mobiele telefoons in de database.
* **Overgang aanvullen**: Deze overgang legt alle resterende profielen vast die niet overeenkomen met Subset 1 of Subset 2. Het bevat met name profielen die de mobiele toepassing niet hebben geïnstalleerd en geen mobiele telefoon hebben, zoals gebruikers die de mobiele app niet hebben geïnstalleerd of die geen geregistreerd mobiel nummer hebben.

![](../assets/workflow-split-example.png)
