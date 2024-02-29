---
audience: end-user
title: Werken met workflowactiviteiten
description: Meer informatie over workflowactiviteiten
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# Workflowactiviteiten {#workflow-activities}

Workflowactiviteiten worden gegroepeerd in drie categorieën. Afhankelijk van de context kunnen de beschikbare activiteiten afwijken.

Alle activiteiten worden beschreven in de volgende onderdelen:

* [Gerichte activiteiten en gegevensbeheer](#targeting)
* [Kanaalactiviteiten](#channel)
* [Stroombeheeractiviteiten](#flow-control)

![](../assets/workflow-activities.png)

## Gerichte activiteiten en gegevensbeheer {#targeting}

Deze activiteiten zijn specifiek gericht op het richten, manipuleren en verrijken van bevolkingsgegevens. Met deze instructies kunt u een of meer doelen maken door een publiek te definiëren en deze soorten publiek te splitsen of te combineren met een doorsnede-, samenvoegings- of uitsluitingsbewerking.

* Gebruik de [Adviezen opslaan](save-audience.md) activiteit om een bestaand publiek bij te werken of een nieuw publiek van de bevolking te creëren die stroomopwaarts in een werkschema wordt berekend.
* Gebruik de [publiek opbouwen](build-audience.md) activiteit om uw doelpopulatie te bepalen. U kunt of een bestaand publiek selecteren of de vraagmodeler gebruiken om uw eigen vraag te bepalen.
* Gebruik de [Combineren](combine.md) activiteit om segmentatie op uw binnenkomende bevolking uit te voeren. U kunt een samenvoeging, een doorsnede of een uitsluiting gebruiken.
* Gebruik de [Splitsen](split.md) activiteit om de binnenkomende bevolking in verschillende subgroepen te segmenteren.
* Gebruik de [Verzoening](reconciliation.md) activiteit om de verbinding tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in een het werklijst te bepalen, bijvoorbeeld gegevens die van een extern dossier worden geladen.
* Gebruik de [Verrijking](enrichment.md) om aanvullende gegevens te definiëren die in uw workflow moeten worden verwerkt. Met deze activiteit, kunt u hefboomwerking de binnenkomende overgang en de activiteit vormen om de outputovergang met extra gegevens te voltooien.
* Gebruik de [Deduplicatie](deduplication.md) activiteit om duplicaten in het resultaat(en) van de binnenkomende activiteiten te verwijderen.
* Gebruik de [Dimensie wijzigen](change-dimension.md) activiteit om de het richten dimensie te veranderen aangezien u uw werkschema bouwt.
* Gebruik de [Bestand laden](load-file.md) om te werken met profielen en gegevens die in een extern bestand zijn opgeslagen.

## Kanaalactiviteiten {#channel}

Met Adobe Campaign Web kunt u marketingcampagnes op meerdere kanalen automatiseren en uitvoeren. U kunt kanaalactiviteiten in het canvas combineren om kanaalworkflows te maken die acties op basis van klantgedrag kunnen activeren. Het volgende **Kanaal** activiteiten zijn beschikbaar: e-mail-, SMS-, Android- en iOS Push-berichten. [Leer hoe u een levering instelt in de context van een workflow](channels.md).

## Stroombeheeractiviteiten {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Eindactiviteit"
>abstract="De **Einde** Met activiteit kunt u het einde van een werkstroom grafisch markeren. Deze activiteit heeft geen functioneel effect en is daarom optioneel."

De volgende activiteiten zijn specifiek voor het organiseren en uitvoeren van workflows. Hun voornaamste taak is de coördinatie van de andere activiteiten:

* Gebruik de [Planner](scheduler.md) activiteit om te plannen wanneer de werkstroom begint.
* Gebruik de [En-join](and-join.md) activiteit om veelvoudige uitvoertakken van een werkschema te synchroniseren.
* Een **Einde** activiteit om het einde van een werkstroom grafisch te markeren. Deze activiteit heeft geen functioneel effect en is daarom optioneel.
* Gebruik de [Vork](fork.md) activiteit om uitgaande overgangen tot stand te brengen om verscheidene activiteiten tezelfdertijd te beginnen.
* Voeg een [Wachten](wait.md) activiteit om de uitvoering van een deel van een werkstroom tijdelijk te pauzeren.

<!--
## Data management activities {#data-management}

overview: what they're used for
which use case you can perform with them

list available activites + short description + ref to section
-->

