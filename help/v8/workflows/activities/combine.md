---
audience: end-user
title: Werkstroomactiviteit combineren gebruiken
description: Leer hoe u de workflowactiviteit combineren gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: bdf569913dfcf9bee549c6ae3252f5a92a5f34e8
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 13%

---


# Combineren {#combine}

Deze activiteit staat u toe om segmentatie op uw binnenkomende bevolking uit te voeren. U kunt dus meerdere populaties combineren, een deel ervan uitsluiten of gegevens alleen gemeenschappelijk houden voor verschillende doelen. Hier volgen de beschikbare segmentatietypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* De **Unie** staat u toe om het resultaat van veelvoudige activiteiten in één enkel doel te hergroeperen.
* De **Intersectie** Hiermee kunt u alleen de elementen behouden die gemeenschappelijk zijn voor de verschillende binnenkomende populaties in de activiteit.
* De **Uitsluiting** kunt u elementen op basis van bepaalde criteria uitsluiten van één populatie.

## Algemene configuratie {#general}

Voer de volgende algemene stappen uit om de configuratie van de **Combineren** activiteit:

1. Meerdere activiteiten toevoegen, zoals **publiek opbouwen** activiteiten om ten minste twee verschillende uitvoerende bijkantoren te vormen.
1. Voeg een **Combineren** activiteiten aan een van de vorige bijkantoren.
1. Selecteer het segmentatietype: [union](#union), [intersection](#intersection) of [uitsluiting](#exclusion).
1. Klikken **Doorgaan**.
1. In de **Stelt in om te verbinden** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.

## Samenvoegen {#union}

Voor de **Unie** selecteert u de **Type afstemming** om te bepalen hoe duplicaten worden verwerkt:

* **Alleen toetsen**: dit is de standaardmodus. De activiteit behoudt slechts één element wanneer elementen van de verschillende binnenkomende overgangen dezelfde sleutel hebben. Deze optie kan alleen worden gebruikt als de binnenkomende populaties homogeen zijn.
* **Een selectie van kolommen**: Selecteer deze optie om de lijst met kolommen te definiëren waarop de afstemming van gegevens wordt toegepast. U moet eerst de primaire set (de set met de brondata) selecteren en vervolgens de kolommen die u voor de samenvoeging wilt gebruiken.

## Doorsnede {#intersection}

Voor de **Intersectie**, moet u deze extra stappen volgen:

1. Selecteer **Type afstemming** om te bepalen hoe duplicaten worden verwerkt. Zie de [Unie](#union) sectie.
1. U kunt de **Voltooiing genereren** als u de resterende populatie wilt verwerken. Het complement zal de samenvoeging bevatten van de resultaten van alle binnenkomende activiteiten min de doorsnede. Een extra uitgaande overgang zal dan aan de activiteit worden toegevoegd.

## Uitsluiting {#exclusion}

Voor de **Uitsluiting**, moet u deze extra stappen volgen:

1. In de **Stelt in om te verbinden** selecteert u de **Primaire set** van de binnenkomende overgangen. Dit is de set waaruit elementen worden uitgesloten. De andere sets komen overeen met de elementen voordat deze worden uitgesloten van de primaire set.
1. Indien nodig, kunt u binnenkomende lijsten manipuleren. Om een doel van een andere dimensie uit te sluiten, moet dit doel worden teruggebracht naar dezelfde doeldimensie als het hoofddoel. Klik op **Een regel toevoegen** in de **Uitsluitingsregels** en geeft u de voorwaarden voor het wijzigen van de dimensie op. Afstemming van gegevens vindt plaats via een attribuut of een join-functie.
1. U kunt de **Voltooiing genereren** als u de resterende populatie wilt verwerken. Zie de [Intersectie](#intersection) sectie.

## Voorbeelden

In het volgende voorbeeld hebben we een **union** dat alle profielen van de twee vragen terugwint: personen tussen 18 en 27 jaar oud en personen tussen 34 en 40 jaar oud.

![](../assets/workflow-union-example.png)

In het volgende voorbeeld wordt het **intersection** tussen twee zoekactiviteiten. Het wordt hier gebruikt om profielen op te halen die tussen 18 en 27 jaar oud zijn en waarvan e-mailadres is verstrekt.

![](../assets/workflow-intersection-example.png)

Het volgende **uitsluiting** In het voorbeeld worden twee query&#39;s weergegeven die zijn geconfigureerd voor filterprofielen die 18 tot 27 jaar oud zijn en een e-maildomein van Adobe hebben. De profielen met een Adobe-e-maildomein worden dan uitgesloten van de eerste set.

![](../assets/workflow-exclusion-example.png)





