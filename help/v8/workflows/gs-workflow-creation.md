---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Beta"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 53148300ecb5d52d89875519c44ae979d29a4d76
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---


# Belangrijkste principes voor het maken van werkstromen {#gs-workflow-creation}

Met Campagne v8 Web, kunt u werkschema&#39;s in een visueel canvas bouwen om kanaalprocessen zoals segmentatie, campagneuitvoering, dossierverwerking te ontwerpen.


## Wat zit er in een workflow? {#gs-workflow-inside}

Het workflowdiagram is een weergave van wat er moet gebeuren. Hierin worden de verschillende taken beschreven die moeten worden uitgevoerd en hoe deze aan elkaar zijn gekoppeld.

![](assets/workflow-example.png)

Elke werkstroom bevat:

* **Activiteiten**: Een activiteit is een uit te voeren taak. De verschillende activiteiten worden op het diagram weergegeven door pictogrammen. Elke activiteit heeft specifieke eigenschappen en andere eigenschappen die voor alle activiteiten gemeenschappelijk zijn.

  In een werkschemadiagram, kan een bepaalde activiteit veelvoudige taken veroorzaken, in het bijzonder wanneer er een lijn of terugkerende acties is.

* **Overgangen**: Overgangen koppelen een bronactiviteit aan een doelactiviteit en definiëren hun volgorde.

* **Worktables**: De werktabel bevat alle informatie die door de overgang wordt overgedragen. Voor elke workflow worden meerdere werktabellen gebruikt. De gegevens in deze tabellen kunnen gedurende de gehele levenscyclus van de workflow worden gebruikt.

## Belangrijke stappen om een workflow te maken {#gs-workflow-steps}


Met campagnes kunt u op twee manieren een workflow maken:

1. Workflows kunnen worden gemaakt als zelfstandige workflows, op basis van de **Workflows** -menu.

   ![](assets/create-a-standalone-wf.png)

1. Workflows kunnen rechtstreeks binnen een campagne worden gemaakt, via de **Workflow** tabblad van de campagne. Wanneer inbegrepen in een campagne, wordt het werkschema uitgevoerd samen met alle andere werkschema&#39;s van de campagne, en de rapporteringsmetriek zijn allen gegroepeerd op het campagnereniveau.

   ![](assets/create-a-wf-from-a-campaign.png)


De belangrijkste stappen voor het maken van workflows zijn als volgt:

![](assets/workflow-creation-process.png)

Deze stappen worden beschreven in de volgende sectie:

1. [Uw workflow maken en de eigenschappen ervan definiëren](create-workflow.md)
1. [Activiteiten ordenen en configureren](orchestrate-activities.md)
1. [Geavanceerde workflowinstellingen configureren](workflow-settings.md)
1. [Start uw workflow en controleer de uitvoering ervan](start-monitor-workflows.md)

