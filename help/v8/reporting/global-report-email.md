---
audience: end-user
title: Algemene rapporten voor het e-mailkanaal
description: Meer informatie over Global-rapporten voor het e-mailkanaal
badge: label="Beperkte beschikbaarheid"
source-git-commit: a6d42e0abb64f87aecb2912cb469ba269aa02515
workflow-type: tm+mt
source-wordcount: '1063'
ht-degree: 1%

---

# Algemene rapporten voor het e-mailkanaal {#global-report-direct}

De globale rapporten verstrekken gebruikers van een uitvoerig overzicht van verkeer en betrokkenheidsmetriek op kanaal-niveau.

Ga naar de **[!UICONTROL Reports]** in het menu **[!UICONTROL Reporting]** sectie. U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-email}

### Overzicht van levering {#delivery-overview-email}

De **[!UICONTROL Delivery Overview]** biedt belangrijke prestatiemetriek (KPIs) die diepgaande inzichten in de interactie van uw bezoekers met elke e-maillevering aanbieden. De meetgegevens worden hieronder beschreven.

![](assets/global_report_email_delivery_overview.png){align="center"}

+++ Meer informatie over overzichtsmetriek voor levering.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Total opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste eenmaal heeft geopend.

* **[!UICONTROL Total clicks]**: Het totale aantal ontvangers dat minstens één keer op een levering heeft geklikt.

* **[!UICONTROL Bounces & errors]**: Totaal aan fouten gecumuleerd tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten.

* **[!UICONTROL Unsubscribes]**: Aantal ontvangers die op abonnementen hebben geklikt.
+++

### Gericht publiek {#delivery-summary-email-initial-target}

De tabel en grafiek voor **[!UICONTROL Targeted Audience]** showcase-gegevens over uw ontvangers, met gedetailleerde hieronder verstrekte gegevens.

![](assets/global_report_email_targeted_audience.png){align="center"}

+++ Meer informatie over de meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: Totaal aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Leveringsstatistieken {#delivery-summary-email-exec-stats}

De **[!UICONTROL Delivery statistics]** tabel geeft een overzicht van het succes van elke e-maillevering , met gedetailleerde cijfers die hieronder worden beschreven .

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

E-mailfouttypen worden weergegeven in het dialoogvenster [Adobe Campaign v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

## Leveringsdoorvoer {#delivery-throughput}

![](assets/global_report_email_delivery_throughput.png){align="center"}

Dit rapport bevat uitgebreide informatie over de leveringstijd binnen een opgegeven tijdsperiode.

## Niet-te leveren items {#non-deliverables-email}

### Uitsplitsing van fouten per type {#delivery-summary-email-breakdown-per-type}

![](assets/global_report_email_breakdown_type.png){align="center"}

De **[!UICONTROL Breakdown of errors per type]** in tabel en grafiek worden de gegevens weergegeven die betrekking hebben op mogelijke fouten op verschillende gebieden , met specifieke cijfers die hieronder worden gegeven .

De fouten die in dit rapport worden weergegeven, activeren het quarantaineproces. Voor meer informatie over quarantainebeheer raadpleegt u [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

+++ Meer informatie over de uitsplitsing van fouten per type metriek.

* **[!UICONTROL User unknown]**: Fouttype dat tijdens de levering wordt gegenereerd om aan te geven dat het e-mailadres ongeldig is.

* **[!UICONTROL Invalid domain]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het domein van het e-mailadres onjuist is of niet bestaat.

* **[!UICONTROL Mailbox full]**: Fouttype dat wordt gegenereerd na vijf leveringspogingen om aan te geven dat het postvak van de ontvanger te veel berichten bevat.

* **[!UICONTROL Account disabled]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het adres niet langer bestaat.

* **[!UICONTROL Refused]**: Fouttype dat wordt gegenereerd wanneer een adres wordt afgewezen door de IAP (Internet Access Provider), bijvoorbeeld na toepassing van een beveiligingsregel (anti-spamsoftware).

* **[!UICONTROL Unreachable]**: Het type van fout dat in het koord van de berichtdistributie voorkomt: incident op het relais SMTP, domein tijdelijk onbereikbaar etc.

* **[!UICONTROL Not connected]**: Fouttype om aan te geven dat de mobiele telefoon van de ontvanger op het moment van verzending wordt uitgeschakeld of losgekoppeld van het netwerk.

+++

### Uitsplitsing van fouten per domein {#delivery-summary-email-breakdown-per-domain}

![](assets/global_report_email_breakdown_domain.png){align="center"}

De **[!UICONTROL Breakdown of errors per domain]** in tabel en grafiek worden de gegevens weergegeven die betrekking hebben op mogelijke fouten binnen elk domein. De metriek is gemeenschappelijk met **[!UICONTROL Breakdown of errors per type]** tabel en grafiek hierboven.

## Trackingsindicatoren {#tracking-indicators-email}

### Leveringsstatistieken {#delivery-summary-email-statistics}

De **[!UICONTROL Delivery statistics]** De metriek biedt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie betreffende de gegevens verstrekken verbonden aan elke e-maillevering. Hieronder vindt u nadere informatie over deze cijfers.

![](assets/global_report_email_delivery_statistics_tracking.png){align="center"}

+++ Meer informatie over de statistieken van de Levering metriek.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Unique opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste eenmaal heeft geopend.

* **[!UICONTROL Total Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

* **[!UICONTROL Clicks on the opt-out link]**: Het aantal klikken op de koppeling voor het opzeggen van abonnementen.

* **[!UICONTROL Clicks on the mirror link]**: Het aantal klikken op de koppeling naar de spiegelpagina.

* **[!UICONTROL Estimation of forwards]**: Schatting van het aantal e-mails dat door de beoogde ontvangers is doorgestuurd.
+++

### Openen en klikken op dalingssnelheid {#delivery-summary-open-rate}

De **[!UICONTROL Open and click-trough rate]** de lijst toont gegevens met betrekking tot uw ontvangers. De cijfers worden hieronder beschreven.

![](assets/global_report_email_opens.png){align="center"}

+++ Meer informatie over Open en klik-dalingssnelheden.

* **[!UICONTROL Sent]**: Totaal aantal verzonden berichten.

* **[!UICONTROL Complaints]**: Aantal en percentage berichten voor dit domein die door de ontvanger als ongewenst zijn gemeld.

* **[!UICONTROL Unique Opens]**: Aantal en percentage verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

* **[!UICONTROL Unique Clicks]**: Aantal en percentage verschillende beoogde ontvangers die minstens één keer op dezelfde levering hebben geklikt.

* **[!UICONTROL Raw reactivity]**: Percentage van het aantal ontvangers dat ten minste één keer op een levering heeft geklikt in vergelijking met het aantal ontvangers dat een levering ten minste één keer heeft geopend.
+++

## URL&#39;s en klikpaden {#url-email}

### URL&#39;s en klik op streams KPI&#39;s {#url-email-kpis}

De **[!UICONTROL URLs and click streams]** Het rapport verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde inzichten in URLs verstrekken die het hoogste aantal kliks tijdens een levering ontvingen. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_9.png){align="center"}

+++Leer meer op URLs en klik stromen metriek.

* **[!UICONTROL Reactivity]**: Verhouding van het aantal beoogde ontvangers dat op een levering heeft geklikt, in verhouding tot het geschatte aantal beoogde ontvangers dat een levering heeft geopend.

* **[!UICONTROL Unique clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

* **[!UICONTROL Total Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Platform average]** : Dit gemiddelde tarief, dat onder elk tarief wordt getoond (reactiviteit, verschillende kliks, en gecumuleerde kliks), wordt berekend voor leveringen die in de voorafgaande zes maanden werden verzonden. Alleen leveringen met dezelfde typologie en op hetzelfde kanaal worden in aanmerking genomen. Proefdrukken zijn uitgesloten.
+++

### De tien meest bezochte koppelingen bovenaan {#top10-campaign-report-email}

De **[!UICONTROL Top 10 most visited links]** de grafiek en de lijst bevatten de beschikbare gegevens voor ontvankelijk gedrag per verbinding. De cijfers worden hieronder beschreven.

![](assets/global_report_email_top10.png){align="center"}

+++Meer informatie over de tien meest bezochte koppelingen vindt u in de statistieken.

* **[!UICONTROL Total Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Percentage]**: Percentage gebruikers dat interactie had met de levering.

+++

### Uitsplitsing van klikken in de tijd {#campaign-report-email-breakdown-clicks}

De **[!UICONTROL Breakdown of clicks over time]** de grafiek bevat de beschikbare gegevens voor het gedrag van de ontvanger per koppeling.

![](assets/global_report_email_breakdown_clicks.png){align="center"}

## Gebruikersactiviteiten {#user-activities-email}

De **[!UICONTROL User activities]** het rapport toont de uitsplitsing van opent en klikt in de vorm van een grafiek. De cijfers voor dit rapport worden hieronder beschreven.

![](assets/global_report_email_user.png){align="center"}

+++ Meer informatie over de metriek van gebruikersactiviteiten.

* **[!UICONTROL Total Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Total Opens]**: Het totale aantal verschillende beoogde ontvangers voor dit domein dat ten minste één bericht heeft geopend.

+++