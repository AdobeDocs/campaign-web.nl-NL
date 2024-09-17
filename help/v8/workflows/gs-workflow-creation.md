---
audience: end-user
title: Belangrijkste principes voor het maken van werkstromen
description: Belangrijke principes van workflows leren met Adobe Campaign Web
exl-id: ac6e63fb-34f2-474f-b364-d2af44f649b1
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Belangrijkste principes voor het maken van werkstromen {#gs-workflow-creation}

Met Adobe Campaign Web, kunt u werkschema&#39;s in een visueel canvas bouwen om kanaalprocessen zoals segmentatie, campagneuitvoering, dossierverwerking te ontwerpen.

## Wat zit er in een workflow? {#gs-workflow-inside}

Het workflowdiagram is een weergave van wat er moet gebeuren. Hierin worden de verschillende taken beschreven die moeten worden uitgevoerd en hoe deze aan elkaar zijn gekoppeld.

![](assets/workflow-example.png){zoomable="yes"} {zoomable="yes"}

Elke werkstroom bevat:

* **Activiteiten**: Een activiteit is een uit te voeren taak. De verschillende activiteiten worden op het diagram weergegeven door pictogrammen. Elke activiteit heeft specifieke eigenschappen en andere eigenschappen die voor alle activiteiten gemeenschappelijk zijn.

  In een werkschemadiagram, kan een bepaalde activiteit veelvoudige taken veroorzaken, in het bijzonder wanneer er een lijn of terugkerende acties is.

* **Overgangen**: De overgangen verbinden een bronactiviteit met een bestemmingsactiviteit en bepalen hun opeenvolging.

* **Worktables**: De werklijst bevat alle informatie die door de overgang wordt gedragen. Voor elke workflow worden meerdere werktabellen gebruikt. De gegevens in deze tabellen kunnen gedurende de gehele levenscyclus van de workflow worden gebruikt.

## Belangrijke stappen om een workflow te maken {#gs-workflow-steps}


Met campagnes kunt u op twee manieren een workflow maken:

1. De werkschema&#39;s kunnen als standalone werkschema&#39;s, van het **menu van de Werkschema&#39;s** worden gecreeerd.

   ![](assets/create-a-standalone-wf.png){zoomable="yes"}

1. De werkschema&#39;s kunnen direct binnen een campagne, van het **1} lusje van het Werkschema {van de campagne worden gecreeerd.** Wanneer inbegrepen in een campagne, wordt het werkschema uitgevoerd samen met alle andere werkschema&#39;s van de campagne, en de rapporteringsmetriek zijn allen gegroepeerd op het campagnereniveau.

   ![](assets/create-a-wf-from-a-campaign.png){zoomable="yes"}

De belangrijkste stappen voor het maken van workflows zijn als volgt:

![](assets/workflow-creation-process.png){zoomable="yes"}

Deze stappen worden beschreven in de volgende sectie:

1. [Uw workflow maken en de eigenschappen ervan definiëren](create-workflow.md)
1. [Activiteiten ordenen en configureren](orchestrate-activities.md)
1. [Geavanceerde workflowinstellingen configureren](workflow-settings.md)
1. [Start uw workflow en controleer de uitvoering ervan](start-monitor-workflows.md)
