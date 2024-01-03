---
audience: end-user
title: Algemene rapporten voor het directe-mailkanaal
description: Meer informatie over Global-rapporten voor het directe e-mailkanaal
badge: label="Beperkte beschikbaarheid"
source-git-commit: 6fbc6d477aac54e8cb7a1eeba40f7c32903c261f
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 1%

---

# Algemene rapporten voor het directe-mailkanaal {#global-report-direct}

De globale rapporten verstrekken gebruikers van een uitvoerig overzicht van verkeer en betrokkenheidsmetriek op kanaal-niveau.

Ga naar de **[!UICONTROL Reports]** in het menu **[!UICONTROL Reporting]** sectie. U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-direct}

### Overzicht van levering {#delivery-overview-direct}

De **[!UICONTROL Delivery Overview]** biedt belangrijke prestatiemetriek (KPIs) die diepgaande inzichten in de interactie van uw bezoekers met elke e-maillevering aanbieden. De meetgegevens worden hieronder beschreven.

![](assets/global_report_email_delivery_overview.png){align="center"}

+++ Meer informatie over overzichtsmetriek voor levering.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Errors]**: Totaal aan fouten gecumuleerd tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten.

* **[!UICONTROL Unsubscribes]**: Aantal ontvangers die op abonnementen hebben geklikt.
+++

### Gericht publiek {#delivery-summary-direct-initial-target}

De tabel en grafiek voor **[!UICONTROL Targeted Audience]** showcase-gegevens over uw ontvangers, met gedetailleerde hieronder verstrekte gegevens.

![](assets/global_report_email_targeted_audience.png){align="center"}

+++ Meer informatie over de meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: Totaal aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Leveringsstatistieken {#delivery-summary-direct-exec-stats}

De **[!UICONTROL Delivery statistics]** de tabel geeft een overzicht van het succes van elke directe postbestelling , met de hieronder beschreven gedetailleerde cijfers .

![](assets/global_report_email_delivery_statistics.png){align="center"}

+++ Meer informatie over de statistieken van de Levering metriek.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors / Bounces]**: Totaal aantal fouten bij leveringen en automatische oplevering in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (onbekend, ongeldig domein) in verhouding tot het aantal te leveren berichten.

+++

### Oorzaken van uitsluiting {#causes-exclusion}

![](assets/global_report_email_exclusions.png){align="center"}

In de grafiek en de tabel met uitsluitingen worden de redenen weergegeven waarom gebruikersprofielen, die zijn uitgesloten van de doelprofielen, het bericht niet hebben ontvangen.

## Leveringsdoorvoer {#delivery-throughput}

Dit rapport bevat uitgebreide informatie over de leveringstijd binnen een opgegeven tijdsperiode. De belangrijkste metrische waarde die wordt gebruikt om de snelheid van berichtlevering te meten is het aantal berichten die per uur worden verzonden.

## Niet-te leveren items {#non-deliverables-direct}

### Uitsplitsing van fouten per type {#delivery-summary-direct-breakdown-per-type}

De **[!UICONTROL Breakdown of errors per type]** in tabel en grafiek worden de gegevens weergegeven die betrekking hebben op mogelijke fouten op verschillende gebieden , met specifieke cijfers die hieronder worden gegeven .

De fouten die in dit rapport worden weergegeven, activeren het quarantaineproces. Voor meer informatie over quarantainebeheer raadpleegt u [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++ Meer informatie over de uitsplitsing van fouten per type metriek.

* **[!UICONTROL User unknown]**: Fouttype dat tijdens de levering wordt gegenereerd om aan te geven dat het adres ongeldig is.

* **[!UICONTROL Invalid domain]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het domein van het adres onjuist is of niet bestaat.

* **[!UICONTROL Mailbox full]**: Fouttype dat wordt gegenereerd na vijf leveringspogingen om aan te geven dat het postvak van de ontvanger te veel berichten bevat.

* **[!UICONTROL Account disabled]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het adres niet langer bestaat.

* **[!UICONTROL Refused]**: Fouttype dat wordt gegenereerd wanneer een adres wordt afgewezen door de IAP (Internet Access Provider), bijvoorbeeld na toepassing van een beveiligingsregel (anti-spamsoftware).

* **[!UICONTROL Unreachable]**: Het type van fout dat in het koord van de berichtdistributie voorkomt: incident op het relais SMTP, domein tijdelijk onbereikbaar etc.

* **[!UICONTROL Not connected]**: Fouttype om aan te geven dat de mobiele telefoon van de ontvanger op het moment van verzending wordt uitgeschakeld of losgekoppeld van het netwerk.

+++

### Uitsplitsing van fouten per domein {#delivery-summary-email-breakdown-per-domain}

De **[!UICONTROL Breakdown of errors per domain]** in tabel en grafiek worden de gegevens weergegeven die betrekking hebben op mogelijke fouten binnen elk domein. De metriek is gemeenschappelijk met **[!UICONTROL Breakdown of errors per type]** tabel en grafiek hierboven.

