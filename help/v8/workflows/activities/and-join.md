---
audience: end-user
title: De activiteit van de AND-join-workflow gebruiken
description: Leer hoe u de workflowactiviteit AND-join gebruikt
badge: label="Beta"
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# AND-join {#join}


>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join-activiteit"
>abstract="De **En-join** Met activiteit kunt u meerdere uitvoertakken van een workflow synchroniseren. De regeling wordt in werking gesteld zodra alle voorgaande activiteiten zijn beëindigd. Op deze manier kunt u ervoor zorgen dat bepaalde activiteiten zijn voltooid voordat u doorgaat met het uitvoeren van de workflow."

De **En-join** activiteit is **Stroomregeling** activiteit. Hiermee kunt u meerdere uitvoeringstakken van een workflow synchroniseren.

Deze activiteit brengt slechts zijn uitgaande overgang teweeg zodra alle binnenkomende overgangen worden geactiveerd, met andere woorden, zodra alle voorafgaande activiteiten zijn geëindigd. Op deze manier kunt u ervoor zorgen dat bepaalde activiteiten zijn voltooid voordat u doorgaat met het uitvoeren van de workflow.

## Vorm en verbind activiteit{#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Vorm EN-verbind activiteit"
>abstract="Selecteer de activiteiten waaraan u wilt deelnemen. In de **Primaire set** keuzelijst, kies welke binnenkomende overgangspopulatie u wilt houden."

Voer de volgende stappen uit om de **AND-join** activiteit:

![](../assets/workflow-andjoin.png)

1. Voeg veelvoudige activiteiten zoals kanaalactiviteiten toe om minstens twee verschillende uitvoertakken te vormen.
1. Een **AND-join** activiteiten aan een van de bijkantoren.
1. In de **Samenvoegopties** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.
1. In de **Primaire set** keuzelijst, kies welke binnenkomende overgangspopulatie u wilt houden. De uitgaande overgang kan slechts één van de binnenkomende overgangspopulaties bevatten.

## Voorbeeld{#and-join-example}

In het volgende voorbeeld worden twee workflowvertakkingen getoond met een e-mail- en sms-levering. EN-toetreden zal teweegbrengen wanneer beide binnenkomende overgangen worden toegelaten. De pushberichten worden dan pas verzonden nadat beide leveringen zijn voltooid.

![](../assets/workflow-andjoin-example.png)
