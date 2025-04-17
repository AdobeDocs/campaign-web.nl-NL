---
audience: end-user
title: Werken met de querymodelfunctie
description: Leer hoe u met Adobe Campaign Web query modeler werkt.
exl-id: 56708a66-f654-413a-80ed-1865077b3c0a
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '693'
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
| **bepaalt publiek**: Specificeer de bevolking u in uw berichten of werkschema&#39;s wilt richten, en creeer moeiteloos nieuw publiek dat aan uw behoeften wordt aangepast. [ Leer hoe te om publiek te bouwen ](../audience/one-time-audience.md) | ![](assets/access-audience.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [ Beeld die hoe te om tot de interface van de publieksverwezenlijking toegang te hebben ] |
| **pas werkschemaactiviteiten** aan: Pas regels binnen werkschemaactiviteiten, zoals **Gesplitste** en **Verzoening** toe, om op uw specifieke vereisten te richten. [ leer meer over werkschemaactiviteiten ](../workflows/activities/about-activities.md) | ![](assets/access-workflow.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [ Beeld dat hoe te om tot de opties van de werkschemaaanpassing toegang te hebben ] |
| **vooraf bepaalde filters**: Creeer vooraf bepaalde filters die als kortere weg tijdens diverse het filtreren verrichtingen dienen, of u met gegevenslijsten werkt of het publiek voor een levering vormt. [ Leer hoe te met vooraf bepaalde filters ](../get-started/predefined-filters.md) te werken | ![](assets/access-predefined-filter.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [ Beeld die tonen hoe te om tot vooraf bepaalde filters ] toegang te hebben |
| **de rapporten van de Filter gegevens**: Voeg regels toe om de gegevens te filtreren die in rapporten worden getoond. [ Leer hoe te met rapporten ](../reporting/gs-reports.md) te werken | ![](assets/access-reports.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [ Beeld dat hoe te om gegevens in rapporten ] toont te filtreren |
| **pas lijsten** aan: Creeer douaneregels om de gegevens te filtreren die in lijsten zoals ontvangers of leveringslijsten worden getoond. [ Leer hoe te om lijsten ](../get-started/list-filters.md#list-built-in-filters) te filtreren | ![](assets/access-lists.png){zoomable="yes"}{width="200" align="center" zoomable="yes"} [ Beeld dat hoe te om lijstfilters ] aan te passen toont |
| **bouwt voorwaardelijke inhoud**: Maak e-mailinhoud dynamisch door voorwaarden te creëren die bepalen welke inhoud aan verschillende ontvangers zou moeten worden getoond, die gepersonaliseerd en relevant overseinen verzekeren. [ Leer hoe te om voorwaardelijke inhoud te bouwen ](../personalization/conditions.md) | ![](assets/conditional-content.png){width="200" align="center" zoomable="yes"} [ Beeld dat hoe te om voorwaardelijke inhoud ] te creëren toont |

>[!NOTE]
>
>Wanneer u een object opent dat is gemaakt in de clientconsole waarop regels zijn toegepast, zoals een publiek of een vooraf gedefinieerd filter, wordt de sectie **[!UICONTROL Refine target]** mogelijk weergegeven. Dit betekent dat de extra parameters zijn gevormd om het regeldoel te verfijnen. Deze parameters kunnen alleen in de console worden gewijzigd.
>
>![ Beeld dat een waarschuwing over het raffineren van doelstellingen toont ](assets/target-warning.png){zoomable="yes"}

## Query-modellerinterface {#interface}

De vraagmodeler verstrekt een centraal canvas waar u uw vraag en een juiste ruit bouwt die informatie over uw vraag verstrekt.

>[!CONTEXTUALHELP]
>id="acw_rule_builder_switch_button"
>title="Nieuwe gebruikerservaring"
>abstract="Gebruik deze knevel om tussen de klassieke vraagmodeler en de nieuwe ervaring van de regelbouwer te schakelen."

![ Beeld dat de interface van de vraagmodeller toont ](assets/query-interface.png){zoomable="yes"}

### Het centrale canvas {#canvas}

Het centrale canvas van de vraagmodeler is waar u toevoegt en de verschillende componenten combineert om uw vraag te bouwen. [ Leer hoe te om een vraag ](build-query.md) te bouwen

De werkbalk in de rechterbovenhoek van het canvas bevat opties waarmee u de querycomponenten eenvoudig kunt manipuleren en door het canvas kunt navigeren:

* **Veelvoudige selectiemodus**: Selecteer veelvoudige het filtreren componenten om hen bij de plaats van uw keus te kopiëren en te kleven.
* **roteer**: Verdraai verticaal het canvas.
* **Passend aan het scherm**: Pas het het gezoemniveau van het canvas aan uw scherm aan.
* **Gezoem uit** / **Gezoem binnen**: Gezoem uit of binnen op het canvas.
* **kaart van de Vertoning**: Open een momentopname van het canvas die uw huidige plaats tonen.

### Het deelvenster Eigenschappen van regel {#rule-properties}

Aan de rechterkant bevat het deelvenster **[!UICONTROL Rule properties]** informatie over de query. Het staat u toe om diverse handelingen uit te voeren om de vraag te controleren en ervoor te zorgen het uw behoeften aanpast. Dit deelvenster wordt weergegeven wanneer u een query samenstelt om een publiek te maken. [ leer hoe te om uw vraag te controleren en te bevestigen ](build-query.md#check-and-validate-your-query)