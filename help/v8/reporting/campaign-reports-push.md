---
audience: end-user
title: Campagnerapporten voor het pushkanaal
description: Campagnerapporten begrijpen voor het Push-kanaal
exl-id: 5e7ac2b8-b543-427b-846c-7c0b489cc21c
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Campagnerapporten voor het pushkanaal {#campaign-reports-push-channel}

Elk campagnerapport is verdeeld in verschillende widgets waarin het succes en de fouten van uw campagne worden beschreven. Voor het pushkanaal worden de rapporten en metriek hieronder beschreven. Leer hoe te om tot uw campagnerapporten op [&#x200B; toegang te hebben deze pagina &#x200B;](campaign-reports.md).

## Leveringsoverzicht {#delivery-summary-push}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_deliveries_overview"
>title="Overzicht van levering"
>abstract="Het **Overzicht van de Levering** rapport verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over geven hoe uw bezoekers met uw levering van het dupbericht in dienst nemen."

Het **[!UICONTROL Delivery Overview]** -rapport bevat prestatie-indicatoren (KPI&#39;s) die gedetailleerde informatie geven over de manier waarop bezoekers de pushmelding uitvoeren. De cijfers worden hieronder beschreven.

![&#x200B; Summiere metriek van de Levering die in het rapport van het Overzicht van de Levering &#x200B;](assets/campaign-reporting-push-summary.png){zoomable="yes"} wordt getoond

+++Meer weten over de cijfers van het pushcampagnerapport?

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Errors]**: Het totale aantal fouten dat is geaccumuleerd tijdens de levering en automatische retourverwerking, in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Total clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer in een levering heeft geklikt.

+++

### Eerste doelstatistieken {#delivery-summary-push-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_target"
>title="Eerste doelstatistieken"
>abstract="De **Aanvankelijke statistieken van het doelpubliek** lijst toont gegevens met betrekking tot uw ontvangers."

In de tabel **[!UICONTROL Initial target audience statistics]** worden gegevens weergegeven die relatief zijn ten opzichte van de ontvangers. De cijfers worden hieronder beschreven.

![&#x200B; Aanvankelijke statistieken van het doelpubliek die in het rapport &#x200B;](assets/campaign-reporting-push-target.png){zoomable="yes"} worden getoond

+++Meer weten over de cijfers van het pushcampagnerapport?

* **[!UICONTROL Initial audience]**: het totale aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Rejected by rules]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels, zoals adres mist, quarantined, of op lijst van gewezen personen.

+++

### Uitvoeringsstatistieken {#delivery-summary-push-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_exec_stats"
>title="Uitvoeringsstatistieken"
>abstract="De **statistieken van de Uitvoering** lijst specificeert het succes van uw levering: berichten om te leveren, succes, fouten, en nieuwe quarantines."

In de tabel **[!UICONTROL Execution statistics]** wordt aangegeven hoe succesvol de levering is. De cijfers worden hieronder beschreven.

![&#x200B; statistieken van de Uitvoering die in het rapport &#x200B;](assets/campaign-reporting-push-exec.png){zoomable="yes"} worden getoond

+++Meer weten over de cijfers van het pushcampagnerapport?

* **[!UICONTROL Message to deliver]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt, in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors]**: Het totale aantal fouten dat is geaccumuleerd tijdens leveringen en automatische oplaadbewerking, in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (bijvoorbeeld ongeldige registratie, berichtafwijzing of payload fout), in verhouding tot het aantal te leveren berichten.

  De types van de de berichtfouten van de duw zijn vermeld in [&#x200B; Adobe Campaign v8 (cliëntconsole) documentatie &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html?lang=nl-NL#push-error-types){target="_blank"}.

+++

### Gegenereerde klikstromen {#delivery-summary-push-click-streams}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_push_click_streams"
>title="Gegenereerde klikstromen"
>abstract="De **Gegenereerde klikstromen** lijst toont de beschikbare gegevens met betrekking tot hoe uw ontvangers met uw levering interactie hadden."

In de tabel **[!UICONTROL Generated click streams]** worden gegevens weergegeven die relatief zijn ten opzichte van de manier waarop de ontvangers met de levering hebben gewerkt. De cijfers worden hieronder beschreven.

![&#x200B; Gegenereerde klikstromen die in het rapport &#x200B;](assets/campaign-reporting-push-clicks.png){zoomable="yes"} worden getoond

+++Meer weten over de cijfers van het pushcampagnerapport?

* **[!UICONTROL Unique clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer in een levering heeft geklikt.

* **[!UICONTROL Total clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Reactivity]**: Verhouding van het aantal beoogde ontvangers die op een levering hebben geklikt, ten opzichte van het geschatte aantal beoogde ontvangers dat een levering heeft geopend.

+++