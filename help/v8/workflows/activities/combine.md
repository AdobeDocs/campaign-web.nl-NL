---
audience: end-user
title: Werkstroomactiviteit combineren gebruiken
description: Leer hoe u de workflowactiviteit combineren gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: 98b4b43427266d5f9580733d4674db938713296d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 16%

---


# Combineren {#combine}

Deze activiteit staat u toe om reeksen op binnenkomende gegevens te verwerken. U kunt dus meerdere populaties combineren, een deel ervan uitsluiten of gegevens alleen gemeenschappelijk houden voor verschillende doelen. Hier volgen de beschikbare segmentatietypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* De **Unie** staat u toe om het resultaat van veelvoudige activiteiten in één enkel doel te hergroeperen.
* De **Intersectie** Hiermee kunt u alleen de elementen behouden die gemeenschappelijk zijn voor de verschillende binnenkomende populaties in de activiteit.
* De **Uitsluiting** kunt u elementen op basis van bepaalde criteria uitsluiten van één populatie.

## Configuratie

Voer de volgende stappen uit om de **Combineren** activiteit:

1. Meerdere activiteiten toevoegen, zoals **publiek opbouwen** activiteiten om ten minste twee verschillende uitvoerende bijkantoren te vormen.
1. Voeg een **Combineren** activiteit aan om het even welke vorige segmentatieovergangen.
1. Selecteer het segmentatietype: samenvoegen, doorsnijden of uitsluiten.
1. Klikken **Doorgaan**.
1. In de **Stelt in om te verbinden** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.

Voor de **Unie** en **Intersectie** selecteert u de **Type afstemming** om te bepalen hoe duplicaten worden verwerkt:

* Alleen toetsen: dit is de standaardmodus. De activiteit behoudt slechts één element wanneer elementen van de verschillende binnenkomende overgangen dezelfde sleutel hebben. Deze optie kan alleen worden gebruikt als de binnenkomende populaties homogeen zijn.
* Een selectie van kolommen: Selecteer deze optie om de lijst met kolommen te definiëren waarop de afstemming van gegevens wordt toegepast. U moet eerst de primaire set (de set met de brondata) selecteren en vervolgens de kolommen die u voor de samenvoeging wilt gebruiken.

Voor de **Intersectie** en **Uitsluiting**, kunt u de **Voltooiing genereren** als u de resterende populatie wilt verwerken. Het complement zal de samenvoeging bevatten van de resultaten van alle binnenkomende activiteiten min de doorsnede. Een extra uitgaande overgang zal dan aan de activiteit worden toegevoegd.

Voor de **Uitsluiting**, selecteert u de **Primaire set** van de binnenkomende overgangen, in **Stelt in om te verbinden** sectie. Dit is de set waaruit elementen worden uitgesloten. De andere sets komen overeen met de elementen voordat deze worden uitgesloten van de primaire set.

## Voorbeelden

In het volgende voorbeeld hebben we een **union** dat alle profielen van de twee vragen terugwint: personen tussen 18 en 27 jaar oud en personen tussen 34 en 40 jaar oud.

![](../assets/workflow-union-example.png)

In het volgende voorbeeld wordt het **intersection** tussen twee zoekactiviteiten. Het wordt hier gebruikt om profielen op te halen die tussen 18 en 27 jaar oud zijn en waarvan e-mailadres is verstrekt.

![](../assets/workflow-intersection-example.png)

Het volgende **uitsluiting** In het voorbeeld worden twee query&#39;s weergegeven die zijn geconfigureerd voor filterprofielen die 18 tot 27 jaar oud zijn en een e-maildomein van Adobe hebben. De profielen met een Adobe-e-maildomein worden dan uitgesloten van de eerste set.

![](../assets/workflow-exclusion-example.png)





