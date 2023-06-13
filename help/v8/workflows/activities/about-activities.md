---
audience: end-user
title: Werken met workflowactiviteiten
description: Meer informatie over workflowactiviteiten
badge: label="Alpha"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: b66afeedbfcb342102c833899756afc35de9d504
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 5%

---


# Workflowactiviteiten {#workflow-activities}

Workflowactiviteiten worden gegroepeerd in drie categorieën. Afhankelijk van de context kunnen de beschikbare activiteiten afwijken.

Alle activiteiten worden beschreven in de volgende onderdelen:

* [Targetingactiviteiten](#targeting)
* [Kanaalactiviteiten](#channel)
* [Stroombeheeractiviteiten](#flow-control)

![](../assets/workflow-activities.png)

## Targetingactiviteiten {#targeting}

Deze activiteiten zijn specifiek gericht op het richten, manipuleren en verrijken van bevolkingsgegevens. Met deze instructies kunt u een of meer doelen maken door een publiek te definiëren en deze soorten publiek te splitsen of te combineren met een doorsnede, samenvoeging of uitsluitingsactie.

* De [publiek opbouwen](build-audience.md) Met activiteit kunt u de doelpopulatie definiëren. U kunt of een bestaand publiek selecteren of de regelbouwer gebruiken om uw eigen vraag te bepalen.
* De [Combineren](combine.md) activiteit staat toe om segmentatie op uw binnenkomende bevolking uit te voeren. U kunt een samenvoeging, een doorsnede of een uitsluiting gebruiken.
* De [Verrijking](enrichment.md) Met activiteiten kunt u aanvullende gegevens definiëren die in uw workflow moeten worden verwerkt. Met deze activiteit, kunt u hefboomwerking de binnenkomende overgang en de activiteit vormen om de outputovergang met extra gegevens te voltooien.

## Kanaalactiviteiten {#channel}

Met Adobe Campaign Web kunt u marketingcampagnes automatiseren en uitvoeren op meerdere kanalen, zoals e-mail, SMS of push. U kunt kanaalactiviteiten in het canvas combineren om kanaalworkflows te maken die acties op basis van klantgedrag kunnen activeren.

Het volgende **Kanaal** de activiteiten zijn beschikbaar :

* Email
* Push
* Sms

Zie dit [sectie](enrichment.md).

## Stroombeheeractiviteiten {#flow-control}

De volgende activiteiten zijn specifiek voor het organiseren en uitvoeren van workflows. Hun voornaamste taak is de coördinatie van de andere activiteiten:

* De [En-join](and-join.md) Met activiteit kunt u meerdere uitvoertakken van een workflow synchroniseren.
* De **Einde** Met activiteit kunt u het einde van een werkstroom grafisch markeren. Deze activiteit heeft geen functioneel effect en is daarom optioneel.
* De [Vork](fork.md) de activiteit staat u toe om uitgaande overgangen tot stand te brengen om verscheidene activiteiten tezelfdertijd te beginnen.
* De [Wachten](wait.md) activiteit onderbreekt tijdelijk het uitvoeren van een deel van een werkstroom.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

