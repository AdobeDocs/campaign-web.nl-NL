---
audience: end-user
title: Globale rapporten voor het kanaal van de Duw
description: Werken met algemene rapporten voor het pushkanaal
exl-id: 829a9b68-5c41-47dd-843c-412b6d255e8b
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 1%

---

# Globale rapporten voor het kanaal van de Duw {#campaign-reports-push}

De globale rapporten verstrekken gebruikers een uitvoerig overzicht van verkeer en betrokkenheidsmetriek op kanaal-niveau.

Ga naar de **[!UICONTROL Reports]** in het menu **[!UICONTROL Reporting]** sectie. U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-push}

### Overzicht van levering {#delivery-overview-push}

>[!CONTEXTUALHELP]
>id="acw_push_global_report_overview"
>title="Overzicht van pushbezorging"
>abstract="De toets **leveringsoverzicht** De KPIs verstrekt een grondig onderzoek van uw dupleveringen, die gedetailleerde inzichten en specifieke gegevens leveren. Het verstrekt uitvoerige details betreffende de prestaties, de doeltreffendheid, en de resultaten van leveringen."

De **[!UICONTROL Delivery Overview]** biedt prestatiekernindicatoren (KPI&#39;s) die gedetailleerde informatie geven over hoe uw bezoekers omgaan met elke levering van pushberichten. De cijfers worden hieronder beschreven.

![](assets/global_report_push_delivery_overview.png){zoomable=&quot;yes&quot;}

+++ Meer informatie over overzichtsmetriek voor levering.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Total clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

* **[!UICONTROL Errors]**: Totaal aan fouten gecumuleerd tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten.

+++

### Gericht publiek {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_targeted_audience"
>title="Doelpopulatie duwen"
>abstract="De **Doelpopulatie** grafiek en lijst showcase gegevens met betrekking tot uw publiek van het drukkend overseinen, presenterend informatie over te leveren berichten en uitsluitingen."

De **[!UICONTROL Targeted audience]** tabel en grafiek geven gegevens weer met betrekking tot uw ontvangers voor elke verzonden pushmelding. De cijfers worden hieronder beschreven.

![](assets/global_report_push_targeted_audience.png){zoomable=&quot;yes&quot;}

+++ Meer informatie over de meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: Totaal aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Leveringsstatistieken {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_delivery_stats"
>title="Statistieken betreffende onder druk geleverde goederen"
>abstract="De **Algemene statistieken** het rapport biedt informatie over verzonden pushmeldingen, zoals succespercentages, fouten en quarantines."

De **[!UICONTROL Delivery statistics]** de lijst specificeert het succes van elke Push berichtlevering. De cijfers worden hieronder beschreven.

![](assets/global_report_push_delivery_statistics.png){zoomable=&quot;yes&quot;}

+++ Meer informatie over de statistieken van de Levering metriek.

* **[!UICONTROL Total messages]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors / Bounces]**: Totaal aantal fouten bij leveringen en automatische oplevering in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat na een mislukte levering in quarantaine is geplaatst (ongeldige registratie, berichtafwijzing, payload fout, bijvoorbeeld.) met betrekking tot het aantal te leveren berichten.

  Typen pushmeldingen worden weergegeven in het dialoogvenster [Adobe Campaign v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

+++

### Oorzaken van uitsluiting {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_push_exclusion"
>title="Uitsluitingsoorzaken"
>abstract="De **Uitsluitingsoorzaken** de grafiek en de lijst illustreren de diverse redenen die gebruikersprofielen beletten om de dupberichten te ontvangen."

De **[!UICONTROL Causes of exclusion]** de grafiek en de lijst tonen de redenen die gebruikersprofielen, die van de gerichte profielen werden uitgesloten, het bericht ontvingen.

Typen pushmeldingen worden weergegeven in het dialoogvenster [Adobe Campaign v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#push-error-types){target="_blank"}.

## Leveringsdoorvoer {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_push"
>title="Leveringsrapport"
>abstract="De **Leveringsdoorvoer** het rapport bevat gedetailleerde informatie over de doorvoer van de pushmelding van het gehele platform binnen een opgegeven tijdsbestek."

![](assets/global_report_push_delivery_throughput.png){zoomable=&quot;yes&quot;}

De **[!UICONTROL Delivery Throughput]** het rapport biedt uitgebreide inzichten in de doeltreffendheid van het systeem voor de levering van pushberichten, met een gedetailleerde samenvatting van het succes en de foutenpercentages over een bepaalde periode.
