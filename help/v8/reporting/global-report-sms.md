---
audience: end-user
title: Algemene rapporten voor het SMS-kanaal
description: Werken met wereldwijde rapporten voor het SMS-kanaal
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 1%

---

# Algemene rapporten voor het SMS-kanaal {#campaign-reports-sms}

De globale rapporten verstrekken gebruikers een uitvoerig overzicht van verkeer en betrokkenheidsmetriek op kanaal-niveau.

Navigeer naar het menu **[!UICONTROL Reports]** in de sectie **[!UICONTROL Reporting]** . U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-sms}

### Overzicht van levering {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Overzicht van SMS-verzending"
>abstract="Het **de leveringsoverzicht van SMS** KPIs verstrekt een grondige samenvatting van uw levering van SMS, die gedetailleerde inzichten en specifieke gegevens aanbieden. Het levert uitvoerige informatie over de prestaties, de doeltreffendheid, en de resultaten van uw levering."

Het **[!UICONTROL Delivery Overview]** -rapport bevat uitgebreide prestatie-indicatoren (KPI&#39;s) die diepgaande inzichten bieden in de interactiepatronen van uw bezoekers bij elke SMS-levering. De volgende cijfers worden hieronder beschreven.

![](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++ Meer informatie over overzichtsmetriek voor levering.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: percentage berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Click-through rate]**: percentage duidelijke ontvangers die minstens één keer in een levering hebben geklikt.

* **[!UICONTROL Errors]**: percentage fouten gecumuleerd tijdens levering en automatische retourverwerking in verhouding tot het totale aantal verzonden berichten.

+++

### Gericht publiek {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="Doelpopulatie van SMS"
>abstract="De grafiek en de lijst voor de **Gerichte bevolking** huidige gegevens met betrekking tot uw publiek van SMS, met inbegrip van informatie over te leveren berichten en uitsluitingen."

De tabel en grafiek van **[!UICONTROL Targeted audience]** bevatten gegevens die betrekking hebben op uw ontvangers voor elke verzonden SMS-levering. De cijfers worden hieronder beschreven.

![](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++ Meer informatie over de meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: het totale aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Leveringsstatistieken {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Sms-leveringsstatistieken"
>abstract="Het **Statistieken van de Levering** rapport verstrekt uitvoerige inzichten in verzonden SMS, die een verdeling van diverse metriek zoals succespercentages, foutenvoorkomen, en publiek aanbieden dat in quarantaine wordt geplaatst. Deze gedetailleerde presentatie maakt een grondig onderzoek mogelijk van de algemene prestaties en resultaten van het SMS-leveringsproces."

In de tabel **[!UICONTROL Delivery statistics]** ziet u hoe succesvol uw SMS-berichten zijn. De cijfers worden hieronder beschreven.

![](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++ Meer informatie over de statistieken van de Levering metriek.

* **[!UICONTROL Total messages]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors / Bounces]**: Het totale aantal fouten dat tijdens leveringen is gecumuleerd en de automatische oplaadbewerking in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (onbekend, ongeldig domein) in verhouding tot het aantal te leveren berichten.

  De de foutentypes van SMS zijn vermeld in de [ Adobe Campaign v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines) {target="_blank"}.

+++

### Oorzaken van uitsluiting {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Sms-oorzaken van uitsluiting"
>abstract="De **Oorzaken van uitsluiting** grafiek en lijst illustreren de diverse redenen die gebruikersprofielen verhinderden de berichten van SMS te ontvangen."

In de grafiek en tabel van **[!UICONTROL Causes of exclusion]** ziet u waarom gebruikersprofielen, die zijn uitgesloten van de beoogde profielen, uw SMS-berichten niet konden ontvangen.

De types van fouten zijn vermeld in [ Adobe Campaign v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#email-error-types) {target="_blank"}.

![](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## Leveringsdoorvoer {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Productie van SMS-berichten"
>abstract="Het **rapport van de productie van 0} Levering {verstrekt uitgebreide inzichten in de efficiency van het systeem van de berichtlevering van SMS, die een gedetailleerd overzicht van succes en foutentarieven binnen een gespecificeerd tijdskader voorstellen.**"

![](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

Het **[!UICONTROL Delivery Throughput]** -rapport biedt uitgebreide inzichten in de effectiviteit van het systeem voor het verzenden van SMS-berichten en biedt een gedetailleerde samenvatting van het succes en de foutenpercentages over een bepaalde periode.
