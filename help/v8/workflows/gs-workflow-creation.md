---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: 748fef18a91a61f5ed956f65762a979e7dacabf3
workflow-type: tm+mt
source-wordcount: '251'
ht-degree: 0%

---


# Belangrijkste principes voor het maken van werkstromen {#gs-workflow-creation}

Met Campagne v8 Web, kunt u werkschema&#39;s in een visueel canvas bouwen om kanaalprocessen zoals segmentatie, campagneuitvoering, dossierverwerking te ontwerpen.

Workflows kunnen worden gemaakt als zelfstandige workflows, via het menu Workflows of rechtstreeks in een campagne. In dat geval wordt de workflow gekoppeld aan de campagne en uitgevoerd samen met alle workflows van de andere campagne.

## Wat zit er in een workflow?

Het workflowdiagram is een weergave van wat er moet gebeuren. Hierin worden de verschillende taken beschreven die moeten worden uitgevoerd en hoe deze aan elkaar zijn gekoppeld.

![](assets/workflow-example.png)

Elke werkstroom bevat:

* **Activiteiten**: Een activiteit is een uit te voeren taak. De verschillende activiteiten worden op het diagram weergegeven door pictogrammen. Elke activiteit heeft specifieke eigenschappen en andere eigenschappen die voor alle activiteiten gemeenschappelijk zijn.

   In een werkschemadiagram, kan een bepaalde activiteit veelvoudige taken veroorzaken, in het bijzonder wanneer er een lijn of terugkerende acties is.

* **Overgangen**: Overgangen koppelen een bronactiviteit aan een bestemmingsactiviteit en bepalen hun opeenvolging.

* **Worktables**: De werktabel bevat alle informatie die door de overgang wordt overgedragen. Voor elke workflow worden meerdere werktabellen gebruikt. De gegevens in deze tabellen kunnen gedurende de gehele levenscyclus van de workflow worden gebruikt.

## Belangrijkste stappen om een workflow te maken

De belangrijkste stappen voor het maken van workflows zijn:

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="create-workflow.md#create">
<img alt="Lood" src="assets/do-not-localize/workflow-process-1 .jpeg">
</a>
<div><a href="create-workflow.md#create"><strong>De workflow maken</strong>
</div>
<p>
</td>
<td>
<a href="create-workflow.md#build">
<img alt="Onfrequent" src="assets/do-not-localize/workflow-process-2.jpeg">
</a>
<div>
<a href="create-workflow.md#build"><strong>Orchestraten</strong></a>
</div>
<p></td>
<td>
<a href="workflow-settings.md">
<img alt="Validatie" src="assets/do-not-localize/workflow-process-3.jpeg">
</a>
<div>
<a href="workflow-settings.md"><strong>Geavanceerde instellingen configureren (optioneel)</strong></a>
</div>
<p>
</td>
<td>
<a href="start-monitor-workflows.md">
<img alt="workflows starten en controleren" src="assets/do-not-localize/workflow-process-4.jpeg">
</a>
<div>
<a href="start-monitor-workflows.md"><strong>De workflowuitvoering starten en controleren</strong></a>
</div>
<p>
</td>
</tr></table>