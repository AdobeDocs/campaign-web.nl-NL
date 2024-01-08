---
audience: end-user
title: Algemene rapporten voor het SMS-kanaal
description: Werken met Global-rapporten voor het SMS-kanaal
badge: label="Beperkte beschikbaarheid"
source-git-commit: c5b4e1d44977b43324e85a7b5e173ef3154a620d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 1%

---

# Algemene rapporten voor het SMS-kanaal {#campaign-reports-sms}

De globale rapporten verstrekken gebruikers van een uitvoerig overzicht van verkeer en betrokkenheidsmetriek op kanaal-niveau.

Ga naar de **[!UICONTROL Reports]** in het menu **[!UICONTROL Reporting]** sectie. U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-sms}

### Overzicht van levering {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Overzicht van SMS-verzending"
>abstract="De **Overzicht van SMS-verzending** De KPIs verstrekt een grondig overzicht van uw levering van SMS, die gedetailleerde inzichten en specifieke gegevens aanbiedt. Het levert uitvoerige informatie over de prestaties, de doeltreffendheid, en de resultaten van uw levering."

De **[!UICONTROL Delivery Overview]** Het rapport biedt uitvoerige zeer belangrijke prestatiesindicatoren (KPIs) die diepgaand inzicht in de interactiepatronen van uw bezoekers met elke levering van SMS verstrekken. De volgende cijfers worden hieronder beschreven.

![](assets/global_report_sms_delivery_overview.png)

+++ Meer informatie over overzichtsmetriek voor levering.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Percentage berichten dat succesvol is verzonden, in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Click-through rate]**: Percentage duidelijke ontvangers die minstens één keer op een levering hebben geklikt.

* **[!UICONTROL Errors]**: Percentage fouten gecumuleerd tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten.

+++

### Gericht publiek {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="Doelpopulatie van SMS"
>abstract="De grafiek en tabel voor de **Gerichte opulatie** gegevens over uw SMS-publiek presenteren, waaronder informatie over te leveren berichten en uitsluitingen."

De **[!UICONTROL Targeted audience]** tabel en grafiek geven gegevens weer met betrekking tot uw ontvangers voor elke verzonden SMS-levering. De cijfers worden hieronder beschreven.

![](assets/global_report_sms_targeted_audience.png)

+++ Meer informatie over de meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: Totaal aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Leveringsstatistieken {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Sms-leveringsstatistieken"
>abstract="De **Leveringsstatistieken** Het rapport biedt uitgebreide inzichten in verzonden SMS en biedt een uitsplitsing van verschillende metingen, zoals succespercentages, voorvallen van fouten en in quarantaine geplaatste gebruikers. Deze gedetailleerde presentatie maakt een grondig onderzoek mogelijk van de algemene prestaties en resultaten van het SMS-leveringsproces."

De **[!UICONTROL Delivery statistics]** in de tabel wordt aangegeven hoe succesvol je levering via SMS is. De cijfers worden hieronder beschreven.

![](assets/global_report_sms_delivery_statistics.png)

+++ Meer informatie over de statistieken van de Levering metriek.

* **[!UICONTROL Total messages]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors / Bounces]**: Totaal aantal fouten bij leveringen en automatische oplevering in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (onbekend, ongeldig domein) in verhouding tot het aantal te leveren berichten.

  Typen SMS-fouten worden vermeld in het dialoogvenster [Adobe Campaign v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines){target="_blank"}.

+++

### Oorzaken van uitsluiting {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Sms-oorzaken van uitsluiting"
>abstract="De **Oorzaken van uitsluiting** de grafiek en de lijst illustreren de diverse redenen die gebruikersprofielen beletten de berichten van SMS te ontvangen."

De **[!UICONTROL Causes of exclusion]** de grafiek en de lijst tonen de redenen die gebruikersprofielen, die van de gerichte profielen werden uitgesloten, van het ontvangen van uw leveringen van SMS verhinderden.

Fouttypen worden vermeld in het dialoogvenster [Adobe Campaign v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types){target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png)

## Leveringsdoorvoer {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Productie van SMS-berichten"
>abstract="De **Leveringsdoorvoer** het rapport biedt uitgebreide inzichten in de efficiëntie van het systeem voor het leveren van SMS-berichten, met een gedetailleerd overzicht van het succes en de foutenpercentages binnen een bepaald tijdsbestek."

![](assets/global_report_sms_delivery_throughput.png)

De **[!UICONTROL Delivery Throughput]** het rapport biedt uitgebreide inzichten in de doeltreffendheid van het systeem voor de levering van SMS-berichten, met een gedetailleerde samenvatting van het succes en de foutenpercentages over een bepaalde periode.
