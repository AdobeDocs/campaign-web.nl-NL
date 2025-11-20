---
audience: end-user
title: Werken met workflowactiviteiten
description: Meer informatie over workflowactiviteiten
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 1%

---

# Workflowactiviteiten {#workflow-activities}

Workflowactiviteiten worden gegroepeerd in drie categorieën. Afhankelijk van de context kunnen de beschikbare activiteiten afwijken.

Alle activiteiten worden beschreven in de volgende onderdelen:

* [Gerichte activiteiten en gegevensbeheer](#targeting)
* [Kanaalactiviteiten](#channel)
* [Workflowbeheeractiviteiten](#flow-control)

![&#x200B; Overzicht van de activiteiten van het Werkschema &#x200B;](../assets/workflow-activities.png)

## Targetingactiviteiten {#targeting}

Deze activiteiten zijn specifiek gericht op de doelgroepen. U kunt hiermee een of meer doelgroepen maken door een publiek te definiëren en deze doelgroepen te splitsen of te combineren met een doorsnede, samenvoeging of uitsluitingsbewerking.

* [&#x200B; bouwt publiek &#x200B;](build-audience.md): Bepaal uw doelbevolking. Selecteer een bestaand publiek of gebruik de vraagmodeler om uw eigen vraag te bepalen.
* [&#x200B; gegevensbron van de Verandering &#x200B;](change-data-source.md): Verandering de gegevensbron voor de het werk lijst van uw werkschema.
* [&#x200B; dimensie van de Verandering &#x200B;](change-dimension.md): Verander de het richten dimensie terwijl het bouwen van uw werkschema.
* [&#x200B; combineren &#x200B;](combine.md): Voer segmentatie op uw binnenkomende bevolking uit. Gebruik een samenvoeging, een doorsnede of een uitsluiting.
* [&#x200B; Deduplicatie &#x200B;](deduplication.md): Verwijder duplicaten in de resultaten van binnenkomende activiteiten.
* [&#x200B; Verrijking &#x200B;](enrichment.md): Bepaal extra gegevens om in uw werkschema te verwerken. Vorm de activiteit om de outputovergang met extra gegevens te voltooien.
* [&#x200B; Incrementele vraag &#x200B;](incremental-query.md): Vraag het gegevensbestand op een geplande basis. Telkens wanneer deze activiteit loopt, sluit het resultaten van vorige uitvoeringen uit, die slechts nieuwe elementen richten.
* [&#x200B; Verzoening &#x200B;](reconciliation.md): Bepaal het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in een het werklijst, zoals gegevens die van een extern dossier worden geladen.
* [&#x200B; sparen publiek &#x200B;](save-audience.md): Werk een bestaand publiek bij of creeer een nieuw publiek van de bevolking die stroomopwaarts in een werkschema wordt berekend.
* [&#x200B; Gesplitst &#x200B;](split.md): Segment de inkomende bevolking in verscheidene ondergroepen.

## Gegevensbeheeractiviteiten {#data}

Deze activiteiten zijn specifiek gericht op het manipuleren en verrijken van bevolkingsgegevens.

* [&#x200B; Extraheer dossier &#x200B;](extract-file.md): De gegevens van de uitvoer van Adobe Campaign aan een ander systeem als extern dossier.
* [&#x200B; het dossier van de Lading &#x200B;](load-file.md): Het werk met profielen en gegevens die in een extern dossier worden opgeslagen.
* [&#x200B; dossier van de Overdracht &#x200B;](transfer-file.md): Ontvang of verzend dossiers, test voor dossieraanwezigheid, of lijstdossiers op een server. Het gebruikte protocol kan of server-aan-server protocol of het protocol van HTTP zijn.
* [&#x200B; code van JavaScript &#x200B;](javascript-code.md): Voer een de codefragment van JavaScript binnen de context van een werkschema uit.
* [&#x200B; de diensten van het Abonnement &#x200B;](subscription-services.md): Abonneer of unsubscribe veelvoudige profielen aan of van de dienst in één enkele actie.
* [&#x200B; gegevens van de Update &#x200B;](update-data.md): Voer massa-updates op gebieden in het gegevensbestand uit. Met verschillende opties kunt u de gegevensupdate aanpassen.

## Kanaalactiviteiten {#channel}

Met Adobe Campaign Web kunt u marketingcampagnes op meerdere kanalen automatiseren en uitvoeren. U kunt kanaalactiviteiten combineren tot het canvas om kanaalworkflows te maken die acties activeren op basis van het gedrag van de klant. De volgende **activiteiten van het Kanaal** zijn beschikbaar: E-mail, SMS, Android, en de Push van iOS berichten. [&#x200B; Leer hoe te opstelling een levering in de context van een werkschema &#x200B;](channels.md).

## Workflowbeheeractiviteiten {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Eindactiviteit"
>abstract="Het **Eind** activiteit staat u toe om het eind van een werkschema grafisch te merken. Deze activiteit heeft geen functioneel effect en is daarom optioneel."

De volgende activiteiten zijn specifiek voor het organiseren en uitvoeren van workflows. Hun voornaamste taak is de coördinatie van de andere activiteiten:

* [&#x200B; en-lid &#x200B;](and-join.md): Synchroniseer veelvoudige uitvoertakken van een werkschema.
* **Eind**: Merk grafisch het eind van een werkschema. Deze activiteit heeft geen functioneel effect en is daarom optioneel.
* [&#x200B; Extern signaal &#x200B;](external-signal.md): Trigger de uitvoering van een werkschema van een ander werkschema of een API vraag.
* [&#x200B; Fork &#x200B;](fork.md): Creeer uitgaande overgangen om verscheidene activiteiten gelijktijdig te beginnen.
* [&#x200B; Planner &#x200B;](scheduler.md): Plan wanneer het werkschema begint.
* [&#x200B; Test &#x200B;](test.md): laat overgangen toe die op gespecificeerde voorwaarden worden gebaseerd.
* [&#x200B; wacht &#x200B;](wait.md): De uitvoering van de pauze van een deel van een werkschema tijdelijk.