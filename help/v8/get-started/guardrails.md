---
title: Instructies en beperkingen in de gebruikersinterface van het campagneweb
description: Instructies en beperkingen in de gebruikersinterface van het campagneweb
badge: label="Beta"
source-git-commit: 86d87e9a3ac9028634a08c2c0969cd232dff15f5
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 0%

---


# Afvoerkanalen en beperkingen {#guardrails-limitations}

Wanneer u in de interface van het campagneweb werkt met componenten die zijn gemaakt of gewijzigd in de clientconsole van Campagne, zijn de onderstaande instructies en beperkingen van toepassing.

## Workflows {#wf-guardrails-limitations}

**Activiteiten**

* Workflowactiviteiten die nog niet in de webinterface worden ondersteund, zijn alleen-lezen. U kunt de workflow nog steeds uitvoeren, berichten verzenden, de logbestanden controleren, enz. De activiteiten van het werkschema die zowel in WebUI als de cliëntconsole beschikbaar zijn zijn editable.

| Console | Webinterface |
| --- | --- |
| ![](assets/limitations-activities-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){width="50%" align="left" zoomable="yes"} |

**Canvas**

* Wanneer u een nieuwe workflow maakt in de webinterface, ondersteunt het canvas slechts één ingangspunt. Nochtans, als u een werkstroom in de console met veelvoudige ingangspunten creeerde,

Maar zelfs als uw workflow is gemaakt in het canvas van de clientconsole met meerdere ingangspunten, kan deze ook worden bewerkt in de webinterface. U kunt nog steeds openen en bewerken



Om dit scenario te proberen, creeer een werkschema van de cliëntconsole met veelvoudige ingangspunten en open het van Web UI om het resultaat te zien.



Natuurlijk kunt u de activiteiten bewerken en de workflow zoals gebruikelijk starten en uitvoeren.



**Positie activiteit**

* De positionering van de knooppunten wordt pas opnieuw berekend (de eerste positionering van de activiteiten wordt daarom gewijzigd) wanneer een activiteit is toegevoegd of verwijderd (niet altijd).

**Onbelichte opties**

* Niet-compatibele opties worden niet weergegeven in de webinterface.

**Lussen**

* Lussen zijn nog niet beschikbaar in de webinterface. Als u een werkstroom met een lijn gebruikend de console creeerde, kunt u tot het niet van Web UI toegang hebben. Er wordt een foutbericht weergegeven.

| Console | Webinterface |
| --- | --- |
| ![](assets/limitations-loops-console.png){width="50%" align="left" zoomable="yes"} | ![](assets/limitations-loops-web.png){width="50%" align="left" zoomable="yes"} |

**Verzoening en verrijking**

In de Campagne cliëntconsole, **Verrijking** deze activiteit kan zowel verzoening als verrijking tot stand brengen . In het Web UI van de Campagne, zijn de verzoeningsmogelijkheden nog niet beschikbaar. Als u verzoening in de consoleactiviteit hebt geplaatst, zal het als niet-compatibele activiteit in Web UI worden getoond.

* Als de **Verrijking** activiteit in de console voert slechts een verrijking uit, **Verrijking** activiteit wordt weergegeven op het web.
* Als de **Verrijking** de activiteit in de console voert slechts een verenigbaarheid uit, wordt een incompatibele activiteit getoond.

## Vooraf gedefinieerde filters {#filters-guardrails-limitations}

In die versie van het product zijn sommige vooraf gedefinieerde filters niet beschikbaar in de gebruikersinterface wanneer u het publiek van een levering selecteert of wanneer u een publiek in een workflow maakt.

Er wordt een specifiek foutbericht weergegeven. Zelfs als u niet de grafische vertegenwoordiging van de vraag in de regelbouwer kunt bekijken, en niet de filter kunt uitgeven, kunt u het nog gebruiken, en de het filtreren voorwaarden, en de resultaten zien. U kunt de SQL-query ook openen om de exacte instellingen te controleren.

![](assets/filter-unavailable.png){width="70%" align="left"}

Merk op dat als u een filter in de interface van het Web bouwt en het in de console met niet gestaafde attributen wijzigt, de grafische vertegenwoordiging niet meer in de interface van het Web beschikbaar kan zijn. In elk geval kunt u het filter nog steeds gebruiken.

Niet-ondersteunde kenmerken worden hieronder weergegeven.

### Niet-ondersteunde gegevenstypen {#unsupported-data-type}

De volgende gegevenstypes beschikbaar in de cliëntconsole worden niet gesteund wanneer het tonen van een filter of een regel in de interface van het Web:

* datetime
* tijd
* timespan
* double
* zweven

### Niet-ondersteunde filtermogelijkheden {#unsupported-filtering-capabilities}

Wanneer een filter met complexe uitdrukkingen en functies in de cliëntconsole wordt gebouwd, kan het niet in de interface van het Web worden uitgegeven.

Bovendien worden de volgende operatoren niet ondersteund:

* Numerieke tekst
   * is opgenomen in
   * geen in

* Het type String
   * groter dan
   * minder dan
   * groter dan of gelijk aan
   * kleiner dan of gelijk aan
   * leuk
   * niet leuk

* Het type Date
   * op of na
   * op of voor
   * niet gelijk aan
   * is leeg
   * is niet leeg
   * is opgenomen in
   * niet in
   * laatste

* 1-N koppelingen
   * COUNT, SUM, AVG, MIN, MAX