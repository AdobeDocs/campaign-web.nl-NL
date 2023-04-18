---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
exl-id: 687b13a4-7ec8-4d07-9d20-53eb4ebefd28
source-git-commit: d9d1666e0903d78560230dd81af32b53608686c5
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Belangrijkste principes voor het maken van werkstromen {#gs-workflow-creation}

Een werkstroom is een procesdefinitie: het werkstroomdiagram, dat een weergave is van wat er moet gebeuren. Een workflow is ook een instantie van dit proces: een werkstroominstantie, die een voorstelling is van wat er eigenlijk gebeurt.

In het werkstroomsjabloon worden de verschillende taken beschreven die moeten worden uitgevoerd en wordt beschreven hoe deze aan elkaar zijn gekoppeld. De taakmalplaatjes worden genoemd activiteiten en door pictogrammen vertegenwoordigd. Ze zijn aan elkaar gekoppeld door overgangen.

screenshot TBD

## Wat zit er in een workflow?

Elke werkstroom bevat:

* **Activiteiten**: Een activiteit beschrijft een taakmalplaatje. De verschillende beschikbare activiteiten worden op het diagram weergegeven door pictogrammen. Elk type heeft gemeenschappelijke eigenschappen en specifieke eigenschappen.

   In een werkschemadiagram, kan een bepaalde activiteit veelvoudige taken veroorzaken, in het bijzonder wanneer er een lijn of terugkerende acties is.

* **Overgangen**: Met overgangen kunt u activiteiten koppelen en de volgorde ervan definiëren. Een overgang koppelt een bronactiviteit aan een bestemmingsactiviteit.

* **Worktables**: De werktabel bevat alle informatie die door de overgang wordt overgedragen. Voor elke workflow worden meerdere werktabellen gebruikt. De gegevens in deze tabellen kunnen gedurende de gehele levenscyclus van de werkstroom worden versneld en gebruikt, zolang deze niet worden gewist. Onbenodigde tabellen worden immers gewist wanneer de workflow wordt gepassiveerd en mogelijk tijdens de uitvoering van de grootste workflows om overbelasting van de server te voorkomen.

## Zelfstandige workflows en workflows voor campagnes

Workflows kunnen als zelfstandige workflows of vanuit een campagne worden gemaakt.

TBD: specifieke details tussen standalone &amp; campagneworkflows.

## Belangrijkste stappen om een workflow te maken

De belangrijkste stappen voor het maken van workflows zijn:

TBD: afbeelding die het hele proces weergeeft met uitleg en verwijzing naar documentpagina&#39;s