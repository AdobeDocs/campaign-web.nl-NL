---
audience: end-user
title: Werken met workflowactiviteiten
description: Meer informatie over workflowactiviteiten
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---


# Workflowactiviteiten {#workflow-activities}

Workflowactiviteiten worden gegroepeerd in drie categorieën. Afhankelijk van de context kunnen de beschikbare activiteiten afwijken.

Alle activiteiten worden beschreven in de volgende onderdelen:

* [Gerichte activiteiten en gegevensbeheer](#targeting)
* [Kanaalactiviteiten](#channel)
* [Stroombeheeractiviteiten](#flow-control)

![](../assets/workflow-activities.png)

## Gerichte activiteiten {#targeting}

Deze activiteiten zijn specifiek gericht op de doelgroepen. Met deze instructies kunt u een of meer doelen maken door een publiek te definiëren en deze soorten publiek te splitsen of te combineren met een doorsnede-, samenvoegings- of uitsluitingsbewerking.

* [publiek opbouwen](build-audience.md): Definieer de doelpopulatie. U kunt of een bestaand publiek selecteren of de vraagmodeler gebruiken om uw eigen vraag te bepalen.
* [Gegevensbron wijzigen](change-data-source.md): Wijzig de gegevensbron voor de werktabel van uw workflow.&quot;
* [Dimensie wijzigen](change-dimension.md): Wijzig de doeldimensie terwijl u uw workflow maakt.
* [Combineren](combine.md): Voer segmentatie op uw binnenkomende bevolking uit. U kunt een samenvoeging, een doorsnede of een uitsluiting gebruiken.
* [Deduplicatie](deduplication.md): Verwijder duplicaten van de resultaten van de binnenkomende activiteiten.
* [Verrijking](enrichment.md): Definieer aanvullende gegevens die in uw workflow moeten worden verwerkt. Met deze activiteit, kunt u hefboomwerking de binnenkomende overgang en de activiteit vormen om de outputovergang met extra gegevens te voltooien.
* [Incrementele query](incremental-query.md): Vraag de database op een geplande basis op. Telkens wanneer deze activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten. Zo kunt u doelgericht alleen nieuwe elementen benaderen.
* [Verzoening](reconciliation.md): Definieer de koppeling tussen de gegevens in de Adobe Campaign-database en de gegevens in een werktabel, bijvoorbeeld gegevens die uit een extern bestand zijn geladen.
* [Adviezen opslaan](save-audience.md): Werk een bestaand publiek bij of maak een nieuw publiek van de populatie die stroomopwaarts in een werkstroom wordt berekend.
* [Splitsen](split.md): Segmenteer de binnenkomende populatie in verschillende subsets.

## Gegevensbeheeractiviteiten {#data}

Deze activiteiten zijn specifiek gericht op het manipuleren en verrijken van bevolkingsgegevens.

* [Bestand uitpakken](extract-file.md): Exporteer gegevens van Adobe Campaign naar een ander systeem als een extern bestand.
* [Bestand laden](load-file.md): Werken met profielen en gegevens die zijn opgeslagen in een extern bestand.
* [Bestand overbrengen](transfer-file.md): Ontvang of verzend dossiers, test op dossieraanwezigheid, of lijstdossiers op een server. Het gebruikte protocol kan of server-aan-server protocol of het protocol van HTTP zijn.
* [JavaScript-code](javascript-code.md): Een JavaScript-codefragment uitvoeren in de context van een workflow.
* [Abonnementsdiensten](subscription-services.md): U kunt meerdere profielen in één handeling aan een service toewijzen of het abonnement op de service opzeggen.
* [Gegevens bijwerken](update-data.md): Hiermee voert u massa-updates uit op velden in de database. Met verschillende opties kunt u de gegevensupdate aanpassen.

## Kanaalactiviteiten {#channel}

Met Adobe Campaign Web kunt u marketingcampagnes op meerdere kanalen automatiseren en uitvoeren. U kunt kanaalactiviteiten in het canvas combineren om kanaalworkflows te maken die acties op basis van klantgedrag kunnen activeren. Het volgende **Kanaal** activiteiten zijn beschikbaar: e-mail-, SMS-, Android- en iOS Push-berichten. [Leer hoe u een levering instelt in de context van een workflow](channels.md).

## Stroombeheeractiviteiten {#flow-control}

>[!CONTEXTUALHELP]
>id="acw_orchestration_end"
>title="Eindactiviteit"
>abstract="De **Einde** Met activiteit kunt u het einde van een werkstroom grafisch markeren. Deze activiteit heeft geen functioneel effect en is daarom optioneel."

De volgende activiteiten zijn specifiek voor het organiseren en uitvoeren van workflows. Hun voornaamste taak is de coördinatie van de andere activiteiten:

* [En-join](and-join.md): Meerdere uitvoeringstakken van een workflow synchroniseren.
* **Einde**: Geeft grafisch het einde van een workflow aan. Deze activiteit heeft geen functioneel effect en is daarom optioneel
* [Extern signaal](external-signal.md): Trigger de uitvoering van een werkstroom van een andere werkschema, of een API vraag.
* [Vork](fork.md): Maak uitgaande overgangen om meerdere activiteiten tegelijk te starten.
* [Planner](scheduler.md): Plan wanneer de workflow wordt gestart.
* [Testen](test.md): Schakel overgangen in op basis van opgegeven voorwaarden.
* [Wachten](wait.md): Onderbreek tijdelijk de uitvoering van een deel van een workflow.
