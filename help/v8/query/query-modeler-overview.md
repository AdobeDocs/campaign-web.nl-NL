---
audience: end-user
title: Werken met de querymodelfunctie
description: Leer hoe u met Adobe Campaign Web query modeler werkt.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: 1a5f49cfdf56a21faedcef3029b62b88ebd81c8d
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# Werken met de querymodelfunctie {#segment-builder}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card5"
>title="New Query modeler"
>abstract="Het Web van Adobe Campaign kenmerkt een vraagmodeler die het proces van het filtreren van gegevensbestanden vereenvoudigt om specifieke doelstellingen te selecteren die op diverse criteria worden gebaseerd. Dit omvat het gebruik van geavanceerde expressies en operatoren. De vraagmodeler is beschikbaar in elke context waar u regels aan filtergegevens moet bepalen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_querymessage"
>title="Query-modelleraar"
>abstract="Bepaal het filtreren criteria voor ontvangers of om het even welke andere gericht afmeting van het gegevensbestand. Profiteer van uw Adobe Experience Platform-publiek om uw doelgroep verder te verfijnen en de impact van uw campagne te maximaliseren."

>[!CONTEXTUALHELP]
>id="acw_deliveries_refine_target"
>title="Doel verfijnen"
>abstract="Deze regels kunnen slechts in de cliëntconsole worden veranderd."

De gebruikersinterface van het Web van Adobe Campaign kenmerkt een vraagmodeler die het proces vereenvoudigt om het gegevensbestand te filtreren dat op diverse criteria wordt gebaseerd. Het verzekert volledige verenigbaarheid met de vragen die in de cliëntconsole worden gecreeerd, die een naadloze overgang aan het Webgebruikersinterface vergemakkelijkt.

Bovendien, beheert het vraagmodel zeer complexe en lange vragen efficiënt, die grotere flexibiliteit en precisie aanbieden. Het steunt ook vooraf bepaalde filters binnen voorwaarden, die gebruikers machtigen om vragen te verfijnen terwijl het gebruiken van geavanceerde uitdrukkingen en exploitanten voor uitvoerige publiek richtend en segmenteringsstrategieën.

## Heb toegang tot de vraagmodeller

De vraagmodeler is beschikbaar in elke context waar u regels aan filtergegevens moet bepalen.

| Gebruik | Voorbeeld |
|  ---  |  ---  |
| **bepaalt publiek**: Specificeer de bevolking u in uw berichten of werkschema&#39;s wilt richten, en creeer moeiteloos nieuw publiek dat aan uw behoeften wordt aangepast. [ Leer hoe te om publiek te bouwen ](../audience/one-time-audience.md) | ![ Beeld die tonen hoe te om tot de interface van de publieksverwezenlijking toegang te hebben ](assets/access-audience.png){width="200" align="center" zoomable="yes"} |
| **pas werkschemaactiviteiten** aan: Pas regels binnen werkschemaactiviteiten, zoals **Gesplitste** en **Verzoening** toe, om op uw specifieke vereisten te richten. [ leer meer over werkschemaactiviteiten ](../workflows/activities/about-activities.md) | ![ Beeld die hoe te om tot de opties van de werkschemaaanpassing toegang te hebben ](assets/access-workflow.png){width="200" align="center" zoomable="yes"} toont |
| **vooraf bepaalde filters**: Creeer vooraf bepaalde filters die als kortere weg tijdens diverse het filtreren verrichtingen dienen, of u met gegevenslijsten werkt of het publiek voor een levering vormt. [ Leer hoe te met vooraf bepaalde filters ](../get-started/predefined-filters.md) te werken | ![ Beeld die tonen hoe te om tot vooraf bepaalde filters toegang te hebben ](assets/access-predefined-filter.png){width="200" align="center" zoomable="yes"} |
| **de rapporten van de Filter gegevens**: Voeg regels toe om de gegevens te filtreren die in rapporten worden getoond. [ Leer hoe te met rapporten ](../reporting/gs-reports.md) te werken | ![ Beeld dat hoe te om gegevens in rapporten ](assets/access-reports.png){width="200" align="center" zoomable="yes"} toont te filtreren |
| **pas lijsten** aan: Creeer douaneregels om de gegevens te filtreren die in lijsten zoals ontvangers of leveringslijsten worden getoond. [ Leer hoe te om lijsten ](../get-started/list-filters.md#list-built-in-filters) te filtreren | ![ Beeld die hoe te om lijstfilters ](assets/access-lists.png){width="200" align="center" zoomable="yes"} tonen aan te passen |
| **bouwt voorwaardelijke inhoud**: Maak e-mailinhoud dynamisch door voorwaarden te creëren die bepalen welke inhoud aan verschillende ontvangers zou moeten worden getoond, die gepersonaliseerd en relevant overseinen verzekeren. [ Leer hoe te om voorwaardelijke inhoud te bouwen ](../personalization/conditions.md) | ![ Beeld dat hoe te om voorwaardelijke inhoud ](assets/conditional-content.png){width="200" align="center" zoomable="yes"} te creëren toont |

>[!NOTE]
>
>Wanneer u een object opent dat is gemaakt in de clientconsole waarop regels zijn toegepast, zoals een publiek of een vooraf gedefinieerd filter, wordt de sectie **[!UICONTROL Refine target]** mogelijk weergegeven. Dit betekent dat de extra parameters zijn gevormd om het regeldoel te verfijnen. Deze parameters kunnen alleen in de console worden gewijzigd.
>
>![ Beeld dat een waarschuwing over het raffineren van doelstellingen toont ](assets/target-warning.png){zoomable="yes"}

## Query-modellerinterface {#interface}

De vraagmodeler verstrekt een centraal canvas waar u uw vraag en een juiste ruit bouwt die informatie over uw vraag verstrekt.

>[!IMPORTANT]
>
>Er is een gloednieuwe interface beschikbaar voor het Query-model. De Nieuwe regelbouwer staat u toe om uw vraag met meer gemak dankzij zijn vereenvoudigde interface te bouwen. Druk op de schakelknop in de rechterbovenhoek om naar deze ervaring over te schakelen. U kunt naar de klassieke modelleerling van de Vraag terugkeren wanneer u wilt door eenvoudig de knevel terug te duwen om de nieuwe interface onbruikbaar te maken. U kunt de zelfde principes toepassen zoals vraagmodeler in deze nieuwe interface.
>&#x200B;>![Beeld die knevel voor de nieuwe interface van de regelbouwer tonen ](assets/query-modeler-toggle.png){zoomable="yes"}


>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="Nieuwe ervaring voor het maken van regels"
>abstract="Gebruik deze knevel om tussen de Klassieke modelleerling van de Vraag en de Nieuwe ervaring van de regelbouwer te schakelen. De nieuwe regelbouwer staat u toe om uw vraag gemakkelijker te bouwen, dankzij zijn vereenvoudigde en intuïtieve interface."

![ Beeld dat de interface van de vraagmodeller toont ](assets/query-interface.png){zoomable="yes"}

### Het centrale canvas {#canvas}

Het centrale canvas van de vraagmodeler is waar u toevoegt en de verschillende componenten combineert om uw vraag te bouwen. [ Leer hoe te om een vraag ](build-query.md) te bouwen

>[!BEGINTABS]

>[!TAB  Klassieke modelleerling van de Vraag ]

De werkbalk in de rechterbenedenhoek van het canvas bevat opties waarmee u de querycomponenten eenvoudig kunt manipuleren en door het canvas kunt navigeren:

* **Veelvoudige selectiemodus**: Selecteer veelvoudige het filtreren componenten om hen bij de plaats van uw keus te kopiëren en te kleven.
* **roteer**: Verdraai verticaal het canvas.
* **Passend aan het scherm**: Pas het het gezoemniveau van het canvas aan uw scherm aan.
* **Gezoem uit** / **Gezoem binnen**: Gezoem uit of binnen op het canvas.
* **kaart van de Vertoning**: Open een momentopname van het canvas die uw huidige plaats tonen.

>[!TAB  Nieuwe ervaring van de regelbouwer ]

De werkbalk in de rechterbovenhoek van het canvas bevat opties waarmee u de querycomponenten eenvoudig kunt manipuleren en door het canvas kunt navigeren:

* **Beweeg omhoog selectie**: Beweeg de component omhoog een rij.
* **Beweging onderaan selectie**: Beweeg de component onderaan een rij.
* **selectie van de Groep**: Zet twee componenten in een groep.
* **ungroup selectie**: Scheid de componenten van één enkele groep.
* **breid alle** uit: Breid alle groepen uit.
* **Vouw alle** samen: Vouw alle groepen samen.
* **verwijder alle**: Verwijder alle groepen en componenten.

>[!ENDTABS]

### Het deelvenster Eigenschappen van regel {#rule-properties}

Aan de rechterkant bevat het deelvenster **[!UICONTROL Rule properties]** informatie over de query. Het staat u toe om diverse handelingen uit te voeren om de vraag te controleren en ervoor te zorgen het uw behoeften aanpast. Dit deelvenster wordt weergegeven wanneer u een query samenstelt om een publiek te maken. [ leer hoe te om uw vraag te controleren en te bevestigen ](build-query.md#check-and-validate-your-query)
