---
audience: end-user
title: De activiteit van de AND-join-workflow gebruiken
description: Leer hoe u de workflowactiviteit AND-join gebruikt
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 1%

---


# AND-join {#join}

De **En-join** activiteit is **Stroomregeling** activiteit. Hiermee kunt u meerdere uitvoeringstakken van een workflow synchroniseren.

Deze activiteit brengt slechts zijn uitgaande overgang teweeg zodra alle binnenkomende overgangen worden geactiveerd, met andere woorden, zodra alle voorafgaande activiteiten zijn geëindigd. Op deze manier kunt u ervoor zorgen dat bepaalde activiteiten zijn voltooid voordat u doorgaat met het uitvoeren van de workflow.

## Configuratie

Voer de volgende stappen uit om de **AND-join** activiteit:

1. Voeg veelvoudige activiteiten zoals kanaalactiviteiten toe om minstens twee verschillende uitvoertakken te vormen.
1. Een **AND-join** activiteiten aan een van de bijkantoren.
1. In de **Samenvoegopties** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.
1. In de **Primaire set** keuzelijst, kies welke binnenkomende overgangspopulatie u wilt houden. De uitgaande overgang kan slechts één van de binnenkomende overgangspopulaties bevatten.

## Voorbeeld

In het volgende voorbeeld worden twee workflowvertakkingen getoond met een e-mail- en sms-levering. EN-toetreden zal teweegbrengen wanneer beide binnenkomende overgangen worden toegelaten. De pushberichten worden dan pas verzonden nadat beide leveringen zijn voltooid.

![](../assets/workflow-andjoin-example.png)