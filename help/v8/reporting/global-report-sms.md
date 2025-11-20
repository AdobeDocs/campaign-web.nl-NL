---
audience: end-user
title: Algemene rapporten voor het SMS-kanaal
description: Werken met wereldwijde rapporten voor het SMS-kanaal
exl-id: 346cf2ff-b6e4-4d8f-ba26-197eadeaf5e6
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Algemene rapporten voor het SMS-kanaal {#campaign-reports-sms}

De globale rapporten verstrekken gebruikers een uitvoerig overzicht van verkeer en betrokkenheidsmetriek op kanaalniveau.

Navigeer naar het menu **[!UICONTROL Reports]** in de sectie **[!UICONTROL Reporting]** . U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-sms}

### Overzicht van levering {#delivery-overview-sms}

>[!CONTEXTUALHELP]
>id="acw_sms_global_report_overview"
>title="Overzicht van SMS-verzending"
>abstract="Het **de leveringsoverzicht van SMS** KPIs verstrekt een grondige samenvatting van uw levering van SMS, die gedetailleerde inzichten en specifieke gegevens aanbieden. Het levert uitvoerige informatie over de prestaties, de doeltreffendheid, en de resultaten van uw levering."

Het **[!UICONTROL Delivery Overview]** -rapport bevat uitgebreide prestatiekernindicatoren (KPI&#39;s) die diepgaande inzichten bieden in de interactiepatronen van uw bezoekers bij elke SMS-levering. De volgende cijfers worden hieronder beschreven.

![&#x200B; A screenshot van het rapport van het Overzicht van de Levering, die zeer belangrijke prestatiesindicatoren voor levering van SMS tonen.](assets/global_report_sms_delivery_overview.png){zoomable="yes"}

+++Meer weten over de maatstaven van het leveringsoverzicht?

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: percentage berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Click-through rate]**: percentage duidelijke ontvangers die minstens één keer in een levering hebben geklikt.

* **[!UICONTROL Errors]**: percentage fouten dat is geaccumuleerd tijdens levering en automatische terugkeerverwerking, in verhouding tot het totale aantal verzonden berichten.

+++

### Gericht publiek {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_targeted_audience"
>title="Doelpopulatie van SMS"
>abstract="De grafiek en de lijst voor de **Gerichte populatie** huidige gegevens met betrekking tot uw publiek van SMS, met inbegrip van informatie over te leveren berichten en uitsluitingen."

De tabel en grafiek van **[!UICONTROL Targeted audience]** bevatten gegevens die betrekking hebben op uw ontvangers voor elke verzonden SMS-levering. De cijfers worden hieronder beschreven.

![&#x200B; A screenshot van het gerichte rapport van het Publiek, die gegevens over ontvangers en uitsluitingen voor de leveringen van SMS tonen.](assets/global_report_sms_targeted_audience.png){zoomable="yes"}

+++Meer informatie over meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: het totale aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels, zoals adres mist, quarantined, of op een lijst van gewezen personen.

+++

### Leveringsstatistieken {#delivery-summary-sms-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_delivery_stats"
>title="Sms-leveringsstatistieken"
>abstract="Het **Statistieken van de Levering** rapport verstrekt uitvoerige inzichten in verzonden SMS, die een verdeling van diverse metriek zoals succespercentages, foutenvoorkomen, en publiek aanbieden dat in quarantaine wordt geplaatst. Deze gedetailleerde presentatie maakt een grondig onderzoek mogelijk van de algemene prestaties en resultaten van het SMS-leveringsproces."

In de tabel **[!UICONTROL Delivery statistics]** ziet u hoe succesvol elke SMS-levering is. De cijfers worden hieronder beschreven.

![&#x200B; A screenshot van het rapport van de Statistieken van de Levering, die succespercentages, fouten, en quarantines voor de leveringen van SMS tonen.](assets/global_report_sms_delivery_statistics.png){zoomable="yes"}

+++Meer weten over statistieken over levering?

* **[!UICONTROL Total messages]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt, in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors / Bounces]**: Het totale aantal fouten dat is geaccumuleerd tijdens leveringen en automatische oplaadbewerking, in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat na een mislukte levering in quarantaine is geplaatst (bv. onbekende gebruiker, ongeldig domein), in verhouding tot het aantal te leveren berichten.

  De de foutentypes van SMS zijn vermeld in [&#x200B; Adobe Campaign v8 (cliëntconsole) documentatie &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=nl-NL#sms-quarantines){target="_blank"}.

+++

### Oorzaken van uitsluiting {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sms_exclusions"
>title="Sms-oorzaken van uitsluiting"
>abstract="De **Oorzaken van uitsluiting** grafiek en lijst illustreren de diverse redenen die gebruikersprofielen verhinderden de berichten van SMS te ontvangen."

In de grafiek en tabel van **[!UICONTROL Causes of exclusion]** ziet u waarom gebruikersprofielen, die zijn uitgesloten van de beoogde profielen, uw SMS-berichten niet konden ontvangen.

De types van fouten zijn vermeld in [&#x200B; Adobe Campaign v8 (cliëntconsole) documentatie &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=nl-NL#email-error-types){target="_blank"}.

![&#x200B; A screenshot van de Oorzaken van het rapport van de Uitsluiting, die redenen voor de leveringsuitsluitingen van SMS tonen.](assets/global_report_sms_causes_exclusion.png){zoomable="yes"}

## Leveringsdoorvoer {#delivery-throughput-sms}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_throughput_sms"
>title="Productie van SMS-berichten"
>abstract="Het **rapport van de productie van 0&rbrace; Levering &lbrace;verstrekt uitgebreide inzichten in de efficiency van het systeem van de berichtlevering van SMS, die een gedetailleerd overzicht van succes en foutentarieven binnen een gespecificeerd tijdskader voorstellen.**"

![&#x200B; A screenshot van het rapport van de Output van de Levering, die succes en foutenpercentages voor de leveringen van SMS in tijd tonen.](assets/global_report_sms_delivery_throughput.png){zoomable="yes"}

Het **[!UICONTROL Delivery Throughput]** -rapport biedt uitgebreide inzichten in de effectiviteit van het SMS-systeem voor het verzenden van berichten en biedt een gedetailleerde samenvatting van het succes en de foutenpercentages over een bepaalde periode.