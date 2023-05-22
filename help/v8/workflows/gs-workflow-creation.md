---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---


# Belangrijkste principes voor het maken van werkstromen {#gs-workflow-creation}

Met Campagne v8 Web, kunt u werkschema&#39;s in een visueel canvas bouwen om kanaalprocessen zoals segmentatie, campagneuitvoering, dossierverwerking te ontwerpen.

Workflows kunnen worden gemaakt als zelfstandige workflows, in het menu Workflows of vanuit een campagne in het menu Campagnes.

TBD: specifieke details tussen standalone &amp; campagneworkflows.

## Wat zit er in een workflow?

Het workflowdiagram is een weergave van wat er moet gebeuren. Hierin worden de verschillende taken beschreven die moeten worden uitgevoerd en hoe deze aan elkaar zijn gekoppeld.

Elke werkstroom bevat:

* **Activiteiten**: Een activiteit is een uit te voeren taak. De verschillende activiteiten worden op het diagram weergegeven door pictogrammen. Elke activiteit heeft specifieke eigenschappen en andere eigenschappen die voor alle activiteiten gemeenschappelijk zijn.

   In een werkschemadiagram, kan een bepaalde activiteit veelvoudige taken veroorzaken, in het bijzonder wanneer er een lijn of terugkerende acties is.

* **Overgangen**: Overgangen koppelen een bronactiviteit aan een bestemmingsactiviteit en bepalen hun opeenvolging.

* **Worktables**: De werktabel bevat alle informatie die door de overgang wordt overgedragen. Voor elke workflow worden meerdere werktabellen gebruikt. De gegevens in deze tabellen kunnen gedurende de gehele levenscyclus van de werkstroom worden versneld en gebruikt, zolang deze niet worden gewist. Onbenodigde tabellen worden immers gewist wanneer de workflow wordt gepassiveerd en mogelijk tijdens de uitvoering van de grootste workflows om overbelasting van de server te voorkomen.

## Belangrijkste stappen om een workflow te maken

De belangrijkste stappen voor het maken van workflows zijn:

TBD: afbeelding die het hele proces weergeeft met uitleg en verwijzing naar documentpagina&#39;s

eigenschappen maken en definiëren > activiteiten op het canvas ordenen > indien nodig instellingen configureren > de uitvoering starten en controleren