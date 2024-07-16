---
audience: end-user
title: Globale rapporten voor het kanaal van de Duw
description: Werken met algemene rapporten voor het pushkanaal
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 1%

---

# Globale rapporten voor het kanaal van de Duw {#campaign-reports-push}

De globale rapporten verstrekken gebruikers een uitvoerig overzicht van verkeer en betrokkenheidsmetriek op kanaal-niveau.

Navigeer naar het menu **[!UICONTROL Reports]** in de sectie **[!UICONTROL Reporting]** . U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-push}

### Overzicht van levering {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Overzicht van pushbezorging"
>abstract="Het duwen **leveringsoverzicht** KPIs verstrekt een grondig onderzoek van uw dupleveringen, leverend gedetailleerde inzichten en specifieke gegevens. Het verstrekt uitvoerige details betreffende de prestaties, de doeltreffendheid, en de resultaten van leveringen."

Het **[!UICONTROL Delivery Overview]** -rapport bevat prestatie-indicatoren (KPI&#39;s) die gedetailleerde informatie geven over hoe uw bezoekers omgaan met elke levering van pushberichten. De cijfers worden hieronder beschreven.

![](assets/global_report_push_delivery_overview.png){zoomable="yes"}

+++ Meer informatie over overzichtsmetriek voor levering.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Total clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer in een levering heeft geklikt.

* **[!UICONTROL Errors]**: Totaal aantal fouten gecumuleerd tijdens levering en automatische retourverwerking in verhouding tot het totale aantal verzonden berichten.

+++

### Gericht publiek {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Doelpopulatie duwen"
>abstract="De **gerichte bevolking** grafiek en lijst showcase gegevens met betrekking tot uw publiek van het duwingsoverseinen, die informatie over te leveren berichten en uitsluitingen presenteren."

De tabel en grafiek van **[!UICONTROL Targeted audience]** bevatten gegevens die betrekking hebben op uw ontvangers voor elke verzonden pushmelding. De cijfers worden hieronder beschreven.

![](assets/global_report_push_targeted_audience.png){zoomable="yes"}

+++ Meer informatie over de meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: het totale aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Leveringsstatistieken {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Statistieken betreffende onder druk geleverde goederen"
>abstract="Het **Algemene statistische** rapport verstrekt informatie over verzonden dupberichten, met inbegrip van succespercentages, fouten, en quarantines."

In de tabel **[!UICONTROL Delivery statistics]** ziet u het succes van elke pushmelding. De cijfers worden hieronder beschreven.

![](assets/global_report_push_delivery_statistics.png){zoomable="yes"}

+++ Meer informatie over de statistieken van de Levering metriek.

* **[!UICONTROL Total messages]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors / Bounces]**: Het totale aantal fouten dat tijdens leveringen is gecumuleerd en de automatische oplaadbewerking in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat na een mislukte levering in quarantaine is geplaatst (ongeldige registratie, berichtafwijzing, payload fout, bijvoorbeeld.) met betrekking tot het aantal te leveren berichten.

  De types van de de berichtfouten van de duw zijn vermeld in [ Adobe Campaign v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types) {target="_blank"}.

+++

### Oorzaken van uitsluiting {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Uitsluitingsoorzaken"
>abstract="De **Oorzaken van de grafiek en de lijst van de Uitsluiting** illustreren de diverse redenen die gebruikersprofielen verhinderden de duimberichten te ontvangen."

In de grafiek en tabel van **[!UICONTROL Causes of exclusion]** ziet u waarom gebruikersprofielen, die waren uitgesloten van de doelprofielen, het bericht niet konden ontvangen.

De types van de de berichtfouten van de duw zijn vermeld in [ Adobe Campaign v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types) {target="_blank"}.

## Leveringsdoorvoer {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Leveringsrapport"
>abstract="Het **rapport van de productie van de Levering** stelt gedetailleerde informatie betreffende de productie van de dupmelding van de levering van het volledige platform binnen een gespecificeerde timeframe voor."

![](assets/global_report_push_delivery_throughput.png){zoomable="yes"}

Het **[!UICONTROL Delivery Throughput]** -rapport biedt uitgebreide inzichten in de doeltreffendheid van het systeem voor de levering van pushberichten, waarmee u een gedetailleerde samenvatting kunt geven van het succes en de foutenpercentages over een bepaalde periode.
