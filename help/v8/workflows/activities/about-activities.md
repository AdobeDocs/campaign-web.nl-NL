---
audience: end-user
title: Werken met workflowactiviteiten
description: Meer informatie over workflowactiviteiten
badge: label="Alpha" type="Positief"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c842829915784654b7130563d36dea188e84ff3d
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 4%

---


# Workflowactiviteiten {#workflow-activities}

Workflowactiviteiten worden gegroepeerd in drie categorieën. Afhankelijk van de context kunnen de beschikbare activiteiten afwijken.

Alle activiteiten worden beschreven in de volgende onderdelen:

* [Targetingactiviteiten](#targeting)
* [Kanaalactiviteiten](#channel)
* [Stroombeheeractiviteiten](#flow-control)

![](../assets/wokflow-activities.png)

## Targetingactiviteiten {#targeting}

Deze activiteiten zijn specifiek gericht op het richten, manipuleren en verrijken van bevolkingsgegevens. Met deze instructies kunt u een of meer doelen maken door een publiek te definiëren en deze soorten publiek te splitsen of te combineren met een doorsnede, samenvoeging of uitsluitingsactie.

* De [publiek opbouwen](build-audience.md) Met activiteit kunt u de doelpopulatie definiëren. U kunt of een bestaand publiek selecteren of de regelbouwer gebruiken om uw eigen vraag te bepalen.
* De [Combineren](combine.md) activiteit staat toe om segmentatie op uw binnenkomende bevolking uit te voeren. U kunt een samenvoeging, een doorsnede of een uitsluiting gebruiken.
* De [Verrijking](enrichment.md) Met activiteiten kunt u aanvullende gegevens definiëren die in uw workflow moeten worden verwerkt. Met deze activiteit, kunt u hefboomwerking de binnenkomende overgang en de activiteit vormen om de outputovergang met extra gegevens te voltooien.

## Kanaalactiviteiten {#channel}

Met Adobe Campaign Web kunt u marketingcampagnes automatiseren en uitvoeren op meerdere kanalen, zoals e-mail, SMS of push. Met Adobe Campaign-workflows kunt u kanaalactiviteiten combineren tot het canvas om kanaalworkflows te maken die acties op basis van klantgedrag kunnen activeren.

U kunt bijvoorbeeld een welkomstcampagne voor e-mail maken met een reeks berichten via verschillende kanalen, zoals e-mail, SMS en push. U kunt ook een e-mail verzenden nadat een klant een aankoop heeft voltooid of een gepersonaliseerd verjaardagsbericht via SMS naar een klant sturen.

Door kanaalactiviteiten te gebruiken, kunt u uitvoerige, gepersonaliseerde campagnes tot stand brengen die klanten over veelvoudige touchpoints en aandrijvingsomzettingen in dienst nemen.

* [Email](email.md)
* [Push](push.md)
* [Sms](sms.md)

## Stroombeheeractiviteiten {#flow-control}

De volgende activiteiten zijn specifiek voor het organiseren en uitvoeren van workflows. Hun voornaamste taak is de coördinatie van de andere activiteiten:

* De [En-join](and-join.md) Met activiteit kunt u meerdere uitvoertakken van een workflow synchroniseren.
* De [Einde](end.md) Met activiteit kunt u het einde van een werkstroom grafisch markeren. Deze activiteiten hebben geen functioneel effect en zijn daarom optioneel.
* De [Vork](fork.md) de activiteit staat u toe om uitgaande overgangen tot stand te brengen om verscheidene activiteiten tezelfdertijd te beginnen.
* De [Wachten](wait.md) activiteit onderbreekt tijdelijk het uitvoeren van een deel van een werkstroom.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

