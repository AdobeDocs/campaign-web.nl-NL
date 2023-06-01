---
audience: end-user
title: Werkstroomactiviteit combineren gebruiken
description: Leer hoe u de workflowactiviteit combineren gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: 2172d159b9d43b18ebb56f5bbbb806884db14346
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 21%

---


# Combineren {#combine}

Deze activiteit staat u toe om reeksen op binnenkomende gegevens te verwerken. U kunt dus meerdere populaties combineren, een deel ervan uitsluiten of gegevens alleen gemeenschappelijk houden voor verschillende doelen. Hier volgen de beschikbare segmentatietypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* De **Unie** staat u toe om het resultaat van veelvoudige activiteiten in één enkel doel te hergroeperen.
* De **Intersectie** Hiermee kunt u alleen de elementen behouden die gemeenschappelijk zijn voor de verschillende binnenkomende populaties in de activiteit.
* De **Uitsluiting** kunt u elementen op basis van bepaalde criteria uitsluiten van één populatie.

Voer de volgende stappen uit om de **Combineren** activiteit:

1. Voeg uw **Combineren** activiteit aan om het even welke vorige segmentatieovergangen.
1. Selecteer het segmentatietype: samenvoegen, doorsnijden of uitsluiten.
1. Klikken **Doorgaan**.
1. In de **Stelt in om te verbinden** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.

Voor de **Unie** en **Intersectie** selecteert u de **Type afstemming** om te bepalen hoe duplicaten worden verwerkt:

    * Alleen toetsen: dit is de standaardmodus. De activiteit behoudt slechts één element wanneer elementen van de verschillende binnenkomende overgangen dezelfde sleutel hebben. Deze optie kan alleen worden gebruikt als de binnenkomende populaties homogeen zijn.
    * Een selectie van kolommen: Selecteer deze optie om de lijst met kolommen te definiëren waarop de afstemming van gegevens wordt toegepast. U moet eerst de primaire set (de set met de brondata) selecteren en vervolgens de kolommen die u voor de samenvoeging wilt gebruiken.

Voor de **Intersectie** en **Uitsluiting**, kunt u de **Voltooiing genereren** als u de resterende populatie wilt verwerken. Het complement zal de samenvoeging bevatten van de resultaten van alle binnenkomende activiteiten min de doorsnede. Een extra uitgaande overgang zal dan aan de activiteit worden toegevoegd.

Voor de **Uitsluiting**, selecteert u de **Primaire set** van de binnenkomende overgangen, in **Stelt in om te verbinden** sectie. Dit is de set waaruit elementen worden uitgesloten. De andere sets komen overeen met de elementen voordat deze worden uitgesloten van de primaire set.
