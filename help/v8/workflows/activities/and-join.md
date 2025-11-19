---
audience: end-user
title: De activiteit van de AND-join-workflow gebruiken
description: Leer hoe u de workflowactiviteit AND-join gebruikt
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# AND-join {#join}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join-activiteit"
>abstract="De **en-sluit zich aan** activiteit staat u toe om veelvoudige uitvoeringstakken van een werkschema te synchroniseren. De regeling wordt in werking gesteld zodra alle voorgaande activiteiten zijn beëindigd. Zo weet u zeker dat bepaalde activiteiten zijn voltooid voordat u doorgaat met het uitvoeren van de workflow."

De **en-sluit zich aan** activiteit is de controle **activiteit van de a** Stroom. Meerdere uitvoeringstakken van een workflow worden gesynchroniseerd.

Deze activiteit activeert zijn uitgaande overgang slechts nadat alle binnenkomende overgangen worden geactiveerd. Met andere woorden, het activeert zodra alle voorgaande activiteiten zijn voltooid. Zo zorgt u ervoor dat bepaalde activiteiten zijn voltooid voordat u doorgaat met het uitvoeren van de workflow.

## Vorm en verbind activiteit {#and-join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Samenvoegopties"
>abstract="Selecteer de activiteiten waaraan u wilt deelnemen. In de **Primaire reeks** drop-down, kies welke binnenkomende overgangspopulatie u wilt houden."

Voer de volgende stappen uit om de **EN-lid** activiteit te vormen:

![ Screenshot die de configuratieinterface voor de EN-sluit zich aan activiteit tonen.](../assets/workflow-andjoin.png)

1. Voeg meerdere activiteiten toe, zoals kanaalactiviteiten, om minstens twee verschillende uitvoeringstakken te vormen.
1. Voeg **toe EN-sluit** activiteit aan om het even welke takken.
1. In de **het samenvoegen opties** sectie, controleer alle vorige activiteiten u zich wilt aansluiten.
1. In de **Primaire reeks** drop-down, kies welke binnenkomende overgangspopulatie om te houden. De uitgaande overgang kan slechts één van de binnenkomende overgangspopulaties bevatten.

## Voorbeeld {#and-join-example}

In het volgende voorbeeld worden twee workflowvertakkingen getoond met een e-mail- en sms-levering. AND-sluit aanzettrekkers aan wanneer beide binnenkomende overgangen worden toegelaten. Pushmeldingen worden alleen verzonden nadat beide leveringen zijn voltooid.

![ Voorbeeld van een werkschema met twee takken, die e-mail en levering van SMS door dupberichten tonen.](../assets/workflow-andjoin-example.png){zoomable="yes"}