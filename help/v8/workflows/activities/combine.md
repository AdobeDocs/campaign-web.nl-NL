---
audience: end-user
title: Werkstroomactiviteit combineren gebruiken
description: Leer hoe u de workflowactiviteit combineren gebruikt
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 11%

---


# Combineren {#combine}

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine"
>title="Combineer activiteit"
>abstract="De **Combineren** activiteit is **Targeting** activiteit. Deze activiteit staat u toe om segmentatie op uw binnenkomende bevolking uit te voeren. U kunt dus meerdere populaties combineren, een deel ervan uitsluiten of gegevens alleen gemeenschappelijk houden voor meerdere doelen."


De **Combineren** activiteit is **Targeting** activiteit. Deze activiteit staat u toe om segmentatie op uw binnenkomende bevolking uit te voeren. U kunt dus meerdere populaties combineren, een deel ervan uitsluiten of gegevens alleen gemeenschappelijk houden voor verschillende doelen. Hier volgen de beschikbare segmentatietypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* De **Unie** staat u toe om het resultaat van veelvoudige activiteiten in één enkel doel te hergroeperen.
* De **Intersectie** Hiermee kunt u alleen de elementen behouden die gemeenschappelijk zijn voor de verschillende binnenkomende populaties in de activiteit.
* De **Uitsluiting** kunt u elementen op basis van bepaalde criteria uitsluiten van één populatie.

## Algemene configuratie {#general}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_merging_options"
>title="Samenvoegopties voor doorsnede"
>abstract="Met de doorsnede kunt u alleen de elementen behouden die gemeenschappelijk zijn voor de verschillende binnenkomende populaties in de activiteit. Controleer in de sectie Sets to join alle vorige activiteiten waaraan u wilt deelnemen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_merging_options"
>title="Samenvoegopties voor uitsluiting"
>abstract="Met deze uitsluiting kunt u elementen op basis van bepaalde criteria uitsluiten van één populatie. Controleer in de sectie Sets to join alle vorige activiteiten waaraan u wilt deelnemen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_options"
>title="Selecteer het segmentatietype"
>abstract="Selecteer hoe u het publiek wilt combineren: verenigen, doorsnijden of uitsluiten."

Voer de volgende algemene stappen uit om de configuratie van de **Combineren** activiteit:

1. Meerdere activiteiten toevoegen, zoals **publiek opbouwen** activiteiten om ten minste twee verschillende uitvoerende bijkantoren te vormen.
1. Voeg een **Combineren** activiteiten aan een van de vorige bijkantoren.
1. Selecteer het segmentatietype: [union](#union), [intersection](#intersection) of [uitsluiting](#exclusion).
1. Klikken **Doorgaan**.
1. In de **Stelt in om te verbinden** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.

## Samenvoegen {#union}

>[!CONTEXTUALHELP]
>id="acw_orchestration_intersection_reconciliation_options"
>title="Doorsnede afstemmingsopties"
>abstract="Selecteer het afstemmingstype om te bepalen hoe duplicaten worden verwerkt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_reconciliation"
>title="Afstemmingsopties"
>abstract="Selecteer de **Type afstemming** om te definiëren hoe duplicaten moeten worden verwerkt."

In de **Combineren** activiteit, kunt u vormen **Unie**. Hiervoor moet u de optie **Type afstemming** om te bepalen hoe duplicaten worden verwerkt:

* **Alleen toetsen**: dit is de standaardmodus. De activiteit behoudt slechts één element wanneer elementen van de verschillende binnenkomende overgangen dezelfde sleutel hebben. Deze optie kan alleen worden gebruikt als de binnenkomende populaties homogeen zijn.
* **Een selectie van kolommen**: selecteer deze optie om de lijst met kolommen te definiëren waarop de afstemming van gegevens wordt toegepast. U moet eerst de primaire set (de set met de brondata) selecteren en vervolgens de kolommen die u voor de samenvoeging wilt gebruiken.

## Doorsnede {#intersection}

In de **Combineren** activiteit, kunt u vormen **Intersectie**. Hiervoor moet u de volgende extra stappen volgen:

1. Selecteer de **Type afstemming** om te bepalen hoe duplicaten worden verwerkt. Zie de [Unie](#union) sectie.
1. U kunt de **Voltooiing genereren** als u de resterende populatie wilt verwerken. Het complement zal de samenvoeging bevatten van de resultaten van alle binnenkomende activiteiten min de doorsnede. Een extra uitgaande overgang zal dan aan de activiteit worden toegevoegd.

## Uitsluiting {#exclusion}

>[!CONTEXTUALHELP]
>id="acw_orchestration_exclusion_options"
>title="Uitsluitingsregels"
>abstract="Indien nodig, kunt u binnenkomende lijsten manipuleren. Om een doel van een andere dimensie uit te sluiten, moet dit doel worden teruggebracht naar dezelfde doeldimensie als het hoofddoel. Om dit te doen, voegt de klik een regel in de sectie van de Regels van de Uitsluiting toe en specificeert de voorwaarden van de afmetingsverandering. Afstemming van gegevens vindt plaats via een attribuut of een join-functie."

>[!CONTEXTUALHELP]
>id="acw_orchestration_combine_sets"
>title="Te combineren sets selecteren"
>abstract="In de **Stelt in om te verbinden** selecteert u de **Primaire set** van de binnenkomende overgangen. Dit is de set waaruit elementen worden uitgesloten. De andere sets komen overeen met de elementen voordat deze worden uitgesloten van de primaire set."


In de **Combineren** activiteit, kunt u vormen **Uitsluiting**. Hiervoor moet u de volgende extra stappen volgen:

1. In de **Stelt in om te verbinden** selecteert u de **Primaire set** van de binnenkomende overgangen. Dit is de set waaruit elementen worden uitgesloten. De andere sets komen overeen met de elementen voordat deze worden uitgesloten van de primaire set.
1. Indien nodig, kunt u binnenkomende lijsten manipuleren. Om een doel van een andere dimensie uit te sluiten, moet dit doel worden teruggebracht naar dezelfde doeldimensie als het hoofddoel. Om dit te doen, klik **Een regel toevoegen** in de **Uitsluitingsregels** en geeft u de voorwaarden voor het wijzigen van de dimensie op. Afstemming van gegevens vindt plaats via een attribuut of een join-functie.
1. U kunt de **Voltooiing genereren** als u de resterende populatie wilt verwerken. Zie de [Intersectie](#intersection) sectie.

## Voorbeelden

In het volgende voorbeeld gebruiken we een **Combineren** en wij voegen een **union** om alle profielen van de twee vragen op te halen : personen tussen 18 en 27 jaar en personen tussen 34 en 40 jaar oud .

![](../assets/workflow-union-example.png)

In het volgende voorbeeld wordt het **intersection** tussen twee zoekactiviteiten. Het wordt hier gebruikt om profielen op te halen die tussen 18 en 27 jaar oud zijn en waarvan e-mailadres is verstrekt.

![](../assets/workflow-intersection-example.png)

Het volgende **uitsluiting** Het voorbeeld toont twee vragen die aan filterprofielen worden gevormd die tussen 18 en 27 jaar oud zijn en een Adobe e-maildomein hebben. De profielen met een Adobe e-maildomein worden dan uitgesloten van de eerste set.

![](../assets/workflow-exclusion-example.png)


