---
title: Instructies en beperkingen in de gebruikersinterface van het campagneweb
description: Instructies en beperkingen in de gebruikersinterface van het campagneweb
badge: label="Beta"
source-git-commit: ff95b563784ae507245e6690feedda33ea6a111b
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Afvoerkanalen en beperkingen {#guardrails-limitations}

Wanneer u in de interface van het campagneweb werkt met componenten die zijn gemaakt of gewijzigd in de clientconsole van Campagne, zijn de onderstaande instructies en beperkingen van toepassing.

## Workflows {#wf-guardrails-limitations}

Dezelfde workflow is toegankelijk voor zowel de console- als de webinterface. Houd er echter rekening mee dat bepaalde beperkingen van toepassing zijn.

**Activity Edition**

* Wanneer u een consoleworkflow opent in de webinterface, kunt u alleen activiteiten wijzigen die compatibel zijn.

**Canvaseditie**

* Als een consolewerkschema veelvoudige beginknopen/takken of drijvende activiteiten heeft, moet u een beginactiviteit en een vork toevoegen om beginknopen aan de belangrijkste knoop aan te sluiten. U moet ook zwevende activiteiten verwijderen.

**Positie activiteit**

* De positionering van de knooppunten wordt pas opnieuw berekend (de eerste positionering van de activiteiten wordt daarom gewijzigd) wanneer een activiteit is toegevoegd of verwijderd (niet altijd).

**Onbelichte opties**

* Niet-compatibele opties worden niet weergegeven in de webinterface.

**Lussen**

* Workflows inclusief lussen worden niet weergegeven in de webinterface. Er wordt een foutbericht weergegeven.

**Verzoening en verrijking**

In de Campagne cliëntconsole, **Verrijking** deze activiteit kan zowel verzoening als verrijking tot stand brengen . In het Web UI van de Campagne, zijn de verzoeningsmogelijkheden nog niet beschikbaar. Als u verzoening in de consoleactiviteit hebt geplaatst, zal het als niet-compatibele activiteit in Web UI worden getoond.

* Als de **Verrijking** activiteit in de console voert slechts een verrijking uit, **Verrijking** activiteit wordt weergegeven op het web.
* Als de **Verrijking** de activiteit in de console voert slechts een verenigbaarheid uit, wordt een incompatibele activiteit getoond.

## Vooraf gedefinieerde filters {#filters-guardrails-limitations}


Bepaalde vooraf gedefinieerde filters zijn niet beschikbaar wanneer u het publiek van een levering selecteert of wanneer u een publiek maakt in een workflow. Er wordt een specifiek foutbericht weergegeven. U kunt de vraag nog gebruiken, en zien: de het filtreren voorwaarde en de resultaten, maar u kunt niet de nauwkeurige vraag in de regelbouwer bekijken, en kunt niet de filter uitgeven.

![](assets/filter-unavailable.png)
