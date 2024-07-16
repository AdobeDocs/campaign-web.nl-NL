---
audience: end-user
title: Campagnerapporten voor het SMS-kanaal
description: Campagnerapporten voor het kanaal van SMS begrijpen
exl-id: 0df9b999-84c8-4e42-b5da-857b2ef0dd75
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Campagnerapporten voor het SMS-kanaal {#campaign-reports-sms-channel}

Elk campagnerapport is verdeeld in verschillende widgets waarin het succes en de fouten van uw campagne worden beschreven. Voor het kanaal van SMS, zijn de rapporten en de metriek gedetailleerd hieronder. Leer hoe te om tot uw campagnerapporten in [ toegang te hebben deze pagina ](campaign-reports.md).

## Leveringsoverzicht {#delivery-summary-sms}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_deliveries_overview"
>title="Overzicht van levering"
>abstract="Het **Overzicht van de Levering** rapport verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over geven hoe uw bezoekers met uw levering van SMS in dienst nemen."


Het **[!UICONTROL Delivery Overview]** -rapport bevat prestatie-indicatoren (KPI&#39;s) die gedetailleerde informatie geven over de manier waarop bezoekers uw SMS-levering gebruiken. De cijfers worden hieronder beschreven.

![](assets/campaign_report_sms_1.png){zoomable="yes"}

+++Meer weten over de metriek van het SMS-campagnerapport?

* **[!UICONTROL Total sent]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Errors]**: Totaal aantal fouten gecumuleerd tijdens levering en automatische retourverwerking in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer in een levering heeft geklikt.

+++


### Eerste doelstatistieken {#delivery-summary-sms-initial-target}

>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_target"
>title="Eerste doelstatistieken"
>abstract="De **Aanvankelijke statistieken van het doelpubliek** lijst toont gegevens met betrekking tot uw ontvangers"

In de tabel **[!UICONTROL Initial target audience statistics]** worden gegevens weergegeven die relatief zijn ten opzichte van de ontvangers. De cijfers worden hieronder beschreven.


![](assets/campaign_report_sms_2.png){zoomable="yes"}

+++Meer weten over de metriek van het SMS-campagnerapport?

* **[!UICONTROL Initial audience]**: het totale aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Rejected by rules]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++


### Uitvoeringsstatistieken {#delivery-summary-sms-exec-stats}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_exec_stats"
>title="Uitvoeringsstatistieken"
>abstract="De **statistieken van de Uitvoering** lijst specificeert het succes van uw levering: berichten om te leveren, succes, fouten, en nieuwe quarantines."


In de tabel **[!UICONTROL Execution statistics]** wordt aangegeven hoe succesvol de levering is. De cijfers worden hieronder beschreven.


![](assets/campaign_report_sms_3.png){zoomable="yes"}

+++Meer weten over de metriek van het SMS-campagnerapport?

* **[!UICONTROL Message to deliver]**: Het totale aantal berichten dat na de voorbereiding van de levering moet worden geleverd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors]**: Het totale aantal fouten dat tijdens leveringen is gecumuleerd en de automatische oplaadbewerking in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (onbekend, ongeldig domein) in verhouding tot het aantal te leveren berichten.

  De de foutentypes van SMS zijn vermeld in de [ Adobe Campaign v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/delivery-failures.html#sms-quarantines) {target="_blank"}.

+++

### Gegenereerde klikstromen {#delivery-summary-sms-click-streams}


>[!CONTEXTUALHELP]
>id="acw_campaign_reporting_sms_click_streams"
>title="Gegenereerde klikstromen"
>abstract="De **Gegenereerde klikstromen** lijst toont de beschikbare gegevens met betrekking tot hoe uw ontvangers met uw levering interactie hadden."

In de tabel **[!UICONTROL Generated click streams]** worden gegevens weergegeven die relatief zijn ten opzichte van de manier waarop de ontvangers met de levering hebben gewerkt. De cijfers worden hieronder beschreven.

![](assets/campaign_report_sms_4.png){zoomable="yes"}

+++Meer weten over de metriek van het SMS-campagnerapport?

* **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer in een levering heeft geklikt.

* **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

* **[!UICONTROL Reactivity]**: Verhouding van het aantal beoogde ontvangers dat op een levering heeft geklikt, in verhouding tot het geschatte aantal beoogde ontvangers dat een levering heeft geopend.

+++
