---
audience: end-user
title: Campagnerapporten voor het e-mailkanaal
description: Meer informatie over campagnerapporten voor het e-mailkanaal
exl-id: c44c91f8-1f88-4087-8417-34be64a2ab19
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 0%

---

# Campagnerapporten voor het e-mailkanaal {#campaign-reports-email-channel}

Elk campagnerapport is verdeeld in verschillende widgets waarin het succes en de fouten van uw campagne worden beschreven. Voor het e-mailkanaal worden de rapporten en metriek hieronder beschreven. Leer hoe u uw campagnerapporten kunt openen in [deze pagina](campaign-reports.md).

## Leveringsoverzicht {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_overview"
>title="Overzicht van levering"
>abstract="De **Overzicht van levering** Hier vindt u belangrijke prestatie-indicatoren (KPI&#39;s) die gedetailleerde informatie geven over de manier waarop bezoekers uw e-maillevering uitvoeren."

### Overzicht van levering {#delivery-summary-email-ovv}

De **[!UICONTROL Delivery Overview]** biedt prestatiekernindicatoren (KPI&#39;s) die gedetailleerde informatie geven over hoe uw bezoekers uw e-maillevering uitvoeren. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_1.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Bounces]**: Totaal aan fouten gecumuleerd tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten.

* **[!UICONTROL Total opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste eenmaal heeft geopend.

* **[!UICONTROL Total clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

+++

### Eerste doelstatistieken {#delivery-summary-email-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_deliveries_target"
>title="Eerste doelstatistieken"
>abstract="De aanvankelijke lijst van de doelpublieksstatistieken toont gegevens met betrekking tot uw ontvangers."

De **[!UICONTROL Initial target audience statistics]** de lijst toont gegevens met betrekking tot uw ontvangers. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_2.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL Initial audience]**: Totaal aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Rejected by rules]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Uitvoeringsstatistieken {#delivery-summary-email-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_exec_stats"
>title="Uitvoeringsstatistieken"
>abstract="De **Uitvoeringsstatistieken** de lijst detailleert het succes van uw levering: te leveren berichten, succes, fouten, en nieuwe quarantines."

De **[!UICONTROL Execution statistics]** in de tabel wordt aangegeven hoe succesvol de levering is . De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_3.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors]**: Totaal aantal fouten bij leveringen en automatische oplevering in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (onbekend, ongeldig domein) in verhouding tot het aantal te leveren berichten.

  E-mailfouttypen worden weergegeven in het dialoogvenster [Adobe Campaign v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

+++

### Reactiestatistieken {#delivery-summary-email-reaction-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_reaction_stats"
>title="Reactiestatistieken"
>abstract="De **Reactiestatistieken** de lijst toont de beschikbare gegevens voor ontvankelijke activiteit voor uw levering: aantal opent, abonnementen, unsubscriptions, klikt om paginakoppeling te weerspiegelen."

De **[!UICONTROL Reaction statistics]** de lijst bevat de beschikbare gegevens voor ontvankelijke activiteit voor uw levering. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_4.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL Unique opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste eenmaal heeft geopend.

* **[!UICONTROL Total Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

* **[!UICONTROL Unsubscriptions]**: Aantal ontvangers die op afboekingen voor de betrokken periode hebben geklikt.

* **[!UICONTROL Mirror page]**: Aantal ontvangers die op de koppeling van de spiegelpagina hebben geklikt.

* **[!UICONTROL Forwards]**: Aantal ontvangers dat heeft geklikt en het e-mailbericht heeft doorgestuurd.
+++

### Gegenereerde klikstromen {#delivery-summary-email-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_email_click_streams"
>title="Gegenereerde klikstromen"
>abstract="De **Gegenereerde klikstromen** de lijst toont de beschikbare gegevens met betrekking tot hoe uw ontvangers met uw levering interactie hadden."

De **[!UICONTROL Generated click streams]** de lijst toont gegevens met betrekking tot hoe uw ontvangers met uw levering interactie hadden. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_5.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL Unique clicks]**: Het totale aantal unieke ontvangers dat ten minste één keer in een levering heeft geklikt.

* **[!UICONTROL Total Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Reactivity]**: Verhouding van het aantal beoogde ontvangers dat op een levering heeft geklikt, in verhouding tot het geschatte aantal beoogde ontvangers dat een levering heeft geopend.

+++

## Niet-te leveren items {#non-deliverables-email}

### Uitsplitsing van fouten per type {#delivery-summary-email-breakdown-per-type}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_type"
>title="Uitsplitsing van fouten per type"
>abstract="De **Uitsplitsing van fouten per type** de lijst en de grafiek bevatten de beschikbare gegevens voor elk aangetroffen foutentype: onbekende gebruiker, brievenbus volledig, ongeldig domein, en meer."

De **[!UICONTROL Breakdown of errors per type]** tabel en grafiek bevatten de beschikbare gegevens voor mogelijke fouten die voor elk type domein zijn aangetroffen. De cijfers worden hieronder beschreven.

De fouten die in dit rapport worden weergegeven, activeren het quarantaineproces. Voor meer informatie over quarantainebeheer raadpleegt u [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

![](assets/campaign_report_email_6.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL User unknown]**: Fouttype dat tijdens de levering wordt gegenereerd om aan te geven dat het e-mailadres ongeldig is.

* **[!UICONTROL Invalid domain]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het domein van het e-mailadres onjuist is of niet bestaat.

* **[!UICONTROL Mailbox full]**: Fouttype dat wordt gegenereerd na vijf leveringspogingen om aan te geven dat het postvak van de ontvanger te veel berichten bevat.

* **[!UICONTROL Account disabled]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het adres niet langer bestaat.

* **[!UICONTROL Refused]**: Fouttype dat wordt gegenereerd wanneer een adres wordt afgewezen door de IAP (Internet Access Provider), bijvoorbeeld na toepassing van een beveiligingsregel (anti-spamsoftware).

* **[!UICONTROL Unreachable]**: Het type van fout dat in het koord van de berichtdistributie voorkomt: incident op het relais SMTP, domein tijdelijk onbereikbaar etc.

* **[!UICONTROL Not connected]**: Fouttype om aan te geven dat de mobiele telefoon van de ontvanger op het moment van verzending wordt uitgeschakeld of losgekoppeld van het netwerk.

+++

### Uitsplitsing van fouten per domein {#delivery-summary-email-breakdown-per-domain}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_error_domain"
>title="Uitsplitsing van fouten per domein"
>abstract="De **Uitsplitsing van fouten per domein** de tabel en de grafiek geven de beschikbare gegevens weer voor elk fouttype dat afhankelijk van elk domein wordt aangetroffen."

De **[!UICONTROL Breakdown of errors per domain]** tabel en grafiek bevatten de beschikbare gegevens voor mogelijke fouten die met elk domein worden aangetroffen. De metriek is gemeenschappelijk met **[!UICONTROL Breakdown of errors per type]** tabel en grafiek hierboven.

## Trackingsindicatoren {#tracking-indicators-email}

### Leveringsstatistieken {#delivery-summary-email-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_delivery_statistics_summary"
>title="Leveringsstatistieken"
>abstract="De **Leveringsstatistieken** de grafiek geeft het succes van uw levering, en fouten die voorkwamen."

De **[!UICONTROL Delivery statistics]** metriek verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over gegevens beschikbaar voor verzonden e-mail verstrekken. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_7.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL Message(s) to deliver]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Unique opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste eenmaal heeft geopend.

* **[!UICONTROL Total Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

* **[!UICONTROL Clicks on the opt-out link]**: Het aantal klikken op de koppeling voor het opzeggen van abonnementen.

* **[!UICONTROL Clicks on the mirror link]**: Het aantal klikken op de koppeling naar de spiegelpagina.

* **[!UICONTROL Estimation of forwards]**: Schatting van het aantal e-mails dat door de beoogde ontvangers is doorgestuurd.
+++

### Openen en klikken op dalingssnelheid {#delivery-summary-open-rate}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_open_clickthrough"
>title="Open- en doorklikfrequentie"
>abstract="De **Open- en doorklikfrequentie** in de tabel worden gegevens weergegeven die betrekking hebben op de betrokkenheid van uw ontvangers bij uw levering."

De **[!UICONTROL Open and click-trough rate]** de lijst toont gegevens met betrekking tot uw ontvangers. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_8.png){zoomable=&quot;yes&quot;}

+++ Meer weten over de maatstaven van het e-mailcampagnerapport?

* **[!UICONTROL Sent]**: Totaal aantal verzonden berichten.

* **[!UICONTROL Complaints]**: Aantal en percentage berichten voor dit domein die door de ontvanger als ongewenst zijn gemeld.

* **[!UICONTROL Unique Opens]**: Aantal en percentage verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

* **[!UICONTROL Unique Clicks]**: Aantal en percentage verschillende beoogde ontvangers die minstens één keer op dezelfde levering hebben geklikt.

* **[!UICONTROL Raw reactivity]**: Percentage van het aantal ontvangers dat ten minste één keer op een levering heeft geklikt in vergelijking met het aantal ontvangers dat een levering ten minste één keer heeft geopend.

+++

## URL&#39;s en klikpaden {#url-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams"
>title="URL&#39;s en klikpaden"
>abstract="De **URL&#39;s en klik op streams** Het rapport verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over URLs geven die het meest tijdens een levering werden geklikt."

De **[!UICONTROL URLs and click streams]** Het rapport verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over URLs geven die het meest tijdens een levering werden geklikt. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_9.png){zoomable=&quot;yes&quot;}

+++ Meer weten over de maatstaven van het e-mailcampagnerapport?

* **[!UICONTROL Reactivity]**: Verhouding van het aantal beoogde ontvangers dat op een levering heeft geklikt, in verhouding tot het geschatte aantal beoogde ontvangers dat een levering heeft geopend.

* **[!UICONTROL Unique clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

* **[!UICONTROL Total Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Platform average]** : Dit gemiddelde tarief, dat onder elk tarief wordt getoond (reactiviteit, verschillende kliks, en gecumuleerde kliks), wordt berekend voor leveringen die in de voorafgaande zes maanden werden verzonden. Alleen leveringen met dezelfde typologie en op hetzelfde kanaal worden in aanmerking genomen. Proefdrukken zijn uitgesloten.

+++

### De tien meest bezochte koppelingen bovenaan {#top10-campaign-report-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_urls_clickstreams_top10"
>title="De tien meest bezochte koppelingen bovenaan"
>abstract="De **De tien meest bezochte koppelingen bovenaan** De alinea en de tabel bevatten de beschikbare gegevens voor het gedrag van de ontvanger per koppeling."

De **[!UICONTROL Top 10 most visited links]** de grafiek en de lijst bevatten de beschikbare gegevens voor ontvankelijk gedrag per verbinding. De cijfers worden hieronder beschreven.

![](assets/campaign_report_email_10.png){zoomable=&quot;yes&quot;}

+++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

* **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Percentage]**: Percentage gebruikers dat interactie had met de levering.

+++

### Uitsplitsing van klikken in de tijd {#campaign-report-email-breakdown-clicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_campaign_urls_click_breakdown"
>title="Uitsplitsing van klikken in de tijd"
>abstract="De **Uitsplitsing van klikken in de tijd** in de grafiek worden de beschikbare gegevens voor het gedrag van de ontvanger per koppeling weergegeven."

De **[!UICONTROL Breakdown of clicks over time]** de grafiek bevat de beschikbare gegevens voor het gedrag van de ontvanger per koppeling.

![](assets/campaign_report_email_11.png){zoomable=&quot;yes&quot;}

## Gebruikersactiviteiten {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_user_activities"
>title="Gebruikersactiviteiten"
>abstract="De **Gebruikersactiviteiten** de grafiek toont de uitsplitsing van opent en klikt in de vorm van een grafiek."

De **[!UICONTROL User activities]** het rapport toont de uitsplitsing van opent en klikt in de vorm van een grafiek. De cijfers voor dit rapport worden hieronder beschreven.

![](assets/campaign_report_email_user_activities.png){zoomable=&quot;yes&quot;}{align="center"}

+++Meer informatie over de afmetingen van het e-mailleveringsrapport.

* **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

+++
