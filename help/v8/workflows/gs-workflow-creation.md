---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 5c4ace1fc8d299048c398fcce14900c797ef6207
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Belangrijkste principes voor het maken van werkstromen {#gs-workflow-creation}

Met Campagne v8 Web, kunt u werkschema&#39;s in een visueel canvas bouwen om kanaalprocessen zoals segmentatie, campagneuitvoering, dossierverwerking te ontwerpen.

Workflows kunnen als zelfstandige workflows worden gemaakt op basis van de **Workflows** of rechtstreeks in een campagne, in welk geval de workflow wordt gekoppeld aan de campagne en samen met alle workflows van de andere campagne wordt uitgevoerd.

## Wat zit er in een workflow? {#gs-workflow-inside}

Het workflowdiagram is een weergave van wat er moet gebeuren. Hierin worden de verschillende taken beschreven die moeten worden uitgevoerd en hoe deze aan elkaar zijn gekoppeld.

![](assets/workflow-example.png)

Elke werkstroom bevat:

* **Activiteiten**: Een activiteit is een uit te voeren taak. De verschillende activiteiten worden op het diagram weergegeven door pictogrammen. Elke activiteit heeft specifieke eigenschappen en andere eigenschappen die voor alle activiteiten gemeenschappelijk zijn.

  In een werkschemadiagram, kan een bepaalde activiteit veelvoudige taken veroorzaken, in het bijzonder wanneer er een lijn of terugkerende acties is.

* **Overgangen**: Overgangen koppelen een bronactiviteit aan een doelactiviteit en definiëren hun volgorde.

* **Worktables**: De werktabel bevat alle informatie die door de overgang wordt overgedragen. Voor elke workflow worden meerdere werktabellen gebruikt. De gegevens in deze tabellen kunnen gedurende de gehele levenscyclus van de workflow worden gebruikt.

## Belangrijke stappen om een workflow te maken {#gs-workflow-steps}

De belangrijkste stappen voor het maken van workflows zijn als volgt:

![](assets/workflow-creation-process.png)

Deze stappen worden beschreven in de volgende sectie:

1. [Uw workflow maken en de eigenschappen ervan definiëren](create-workflow.md)
1. [Activiteiten ordenen en configureren](orchestrate-activities.md)
1. [Geavanceerde workflowinstellingen configureren](workflow-settings.md)
1. [Start uw workflow en controleer de uitvoering ervan](start-monitor-workflows.md)

