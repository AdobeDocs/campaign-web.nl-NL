---
title: Tijdzonebeheer
description: Leer hoe de UI van het Web van Adobe Campaign datum en tijdwaarden toont die op browser, exploitant, werkschema, en de gebieden van de servertijd worden gebaseerd.
source-git-commit: 357d2014ade1e783b3bf1e1c363894084199738d
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 2%

---

# Tijdzonebeheer {#timezone-management}

Het Web UI van Adobe Campaign toont alle datum en tijdwaarden volgens de **lokale tijdzone van Webbrowser van de gebruiker**. Dit gedrag kan tot verschillen leiden wanneer het vergelijken van tijdstempels tussen het Web UI en de Console van de Cliënt.

Deze sectie verklaart verwachte verschillen tussen het **Web UI**, **Console van de Cliënt**, en **werkschemauitvoering** tijdstreken.

>[!NOTE]
>
>Er worden geen gegevens op de server opgeslagen. Alleen de weergave in de interface verandert.

## Belangrijkste concepten

* **tijdzone van de Server**: de streek van de servertijd beantwoordt aan de tijdzone die op het werkende systeem van de server wordt gevormd. Alle tijdstempels worden intern opgeslagen in UTC op de server.

* **gedrag van de Console van de Cliënt**: De vertoningen timestamps van de Console van de Cliënt gebruikend de **tijdzone van de exploitant**, die in de montages van de exploitant wordt bepaald. Door gebrek, beantwoordt dit aan de **tijdzone van de server**.

* **het gedrag van UI van het Web**: Het Web UI toont timestamps gebruikend de **lokale tijdzone van browser**. Wanneer een gebruiker de browser of de tijdzone van het systeem wijzigt, worden de weergegeven datum-/tijdwaarden automatisch bijgewerkt.

* **het gedrag van het Werkschema**: de werkschema&#39;s interpreteren lokale tijdstempels die op de **worden gebaseerd gevormde tijdzone van het werkschema**. Als gespecificeerd niet, wordt de **tijdzone van de server** gebruikt door gebrek.

## Voorbeeld

| Interface | Tijdzone gebruikt | Voorbeeld weergeven |
|------------|----------------|-----------------|
| Clientconsole | Operatoren (standaard = server) | `2025-10-20 14:00:00` |
| Webinterface | Lokale tijdzone van browser | `2025-10-20 21:00:00` (voor browser in UTC +7) |

In dit voorbeeld verwijzen beide interfaces naar dezelfde onderliggende UTC-tijdstempel, maar wordt deze elk weergegeven met een andere tijdzone.

## Gevolgen

De verschillen in weergegeven tijden kunnen worden weergegeven in:

* Profiel of gegevensvelden met `datetime` waarden
* Leveringslogboeken of contactdatums
* Tijdstempels voor workflowuitvoering en importeren

De onderliggende gegevens blijven identiek. Het verschil is slechts in **teruggevend**.

>[!NOTE]
>
>Als gebruikers uit meerdere regio&#39;s aan dezelfde instantie samenwerken, kunnen er duidelijke discrepanties optreden tussen de webinterface en de consolesjablonen.

## Aanbevelingen

Als u de weergavewaarden wilt uitlijnen op verschillende interfaces, kunt u:

* Verander uw **browser tijdzone** om de **exploitant of server tijdzone** aan te passen.
* Zorg bij het exporteren van gegevens (voor exporteren gebruik van UTC) voor consistente conversie in rapportagegereedschappen.
* Wanneer het ontwerpen van werkschema&#39;s, plaats uitdrukkelijk de **tijdzone van de werkschematijd** in activiteiteneigenschappen voor voorspelbaar het plannen en de invoer gedrag.
* Communiceer aan bedrijfsgebruikers dat timestamp verschillen tussen de meningen van UI van het Web en van de Console van de Cliënt **normaal en verwacht** zijn.
