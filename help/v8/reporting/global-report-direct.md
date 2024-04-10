---
audience: end-user
title: Algemene rapporten voor het directe-mailkanaal
description: Meer informatie over Global-rapporten voor het directe e-mailkanaal
exl-id: a42536fe-375b-4169-8775-d47ed26692f8
source-git-commit: 98a0ce67682f8e1ab412be91b5af01e35c638f99
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Algemene rapporten voor het directe-mailkanaal {#global-report-direct}

De wereldwijde rapporten van Direct Mail bieden gebruikers een uitgebreid overzicht van verkeers- en servicemetriek op kanaalniveau.

Ga naar de **[!UICONTROL Reports]** in het menu **[!UICONTROL Reporting]** sectie. U kunt de gegevens filteren op basis van de rapportdatum, -map of -regels. [Meer informatie](global-reports.md)

## Leveringsoverzicht {#delivery-summary-direct}

### Overzicht van levering {#delivery-overview-direct}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_overview_direct_mail"
>title="Overzicht van levering"
>abstract="De **Overzicht van levering** biedt belangrijke prestatiemetriek (KPIs) die diepgaande inzichten van de interactie van uw bezoekers met elke directe postlevering aanbieden. De meetgegevens worden hieronder beschreven."

De **[!UICONTROL Delivery Overview]** biedt belangrijke prestatiemetriek (KPIs) die diepgaande inzichten van de interactie van uw bezoekers met elke directe postlevering aanbieden. De meetgegevens worden hieronder beschreven.

![](assets/global_report_direct_mail_delivery_overview.png){zoomable=&quot;yes&quot;}{align="center"}

+++ Meer informatie over overzichtsmetriek voor levering.

* **[!UICONTROL Messages to deliver]**: Het totale aantal berichten dat tijdens de voorbereiding van de levering wordt verwerkt.

* **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

* **[!UICONTROL Errors]**: Totaal aan fouten gecumuleerd tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten.

* **[!UICONTROL Unsubscribes]**: Aantal ontvangers die op abonnementen hebben geklikt.
+++

### Gericht publiek {#delivery-summary-direct-initial-target}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_graph"
>title="Gericht publiek"
>abstract="De gegevens en de berichtinformatie van de ontvanger worden getoond in **Gericht publiek** grafiek, die de analyse van de voorbereiding van de levering weergeeft."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_target_audience_direct_mail_table"
>title="Gericht publiek"
>abstract="De **Gericht publiek** de lijst verstrekt een gedetailleerde specificatie van uw ontvangers en de overeenkomstige berichten, die op de resultaten van het leveringsvoorbereidingsproces worden gebaseerd."

De tabel en grafiek voor **[!UICONTROL Targeted Audience]** showcase-gegevens over uw ontvangers, met gedetailleerde hieronder verstrekte gegevens.

![](assets/global_report_direct_mail_targeted_audience.png){zoomable=&quot;yes&quot;}{align="center"}

+++ Meer informatie over de meetgegevens voor doelgroepen.

* **[!UICONTROL Targeted audience]**: Totaal aantal beoogde ontvangers.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Exclusion]**: Het totale aantal adressen dat tijdens de analyse wordt genegeerd wanneer het toepassen van regels: adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

### Leveringsstatistieken {#delivery-summary-direct-exec-stats}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_graph"
>title="Leveringsstatistieken"
>abstract="De **Leveringsstatistieken** de grafiek verstrekt inzicht in de doeltreffendheid van uw directe postleveringen, met inbegrip van succesvolle leveringen en om het even welke ontmoet fouten."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_delivery_statistics_summary_direct_mail_table"
>title="Leveringsstatistieken"
>abstract="De **Leveringsstatistieken** in de tabel worden het succes van de levering via e-mail en de gemaakte fouten weergegeven."

De **[!UICONTROL Delivery statistics]** de grafiek en de tabel geven een overzicht van het succes van elke directe postbestelling , met de hieronder beschreven gedetailleerde cijfers .

+++ Meer informatie over de statistieken van de Levering metriek.

* **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

* **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL Errors / Bounces]**: Totaal aantal fouten bij leveringen en automatische oplevering in verhouding tot het aantal te leveren berichten.

* **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (onbekend, ongeldig domein) in verhouding tot het aantal te leveren berichten.

+++

### Oorzaken van uitsluiting {#causes-exclusion}

>[!CONTEXTUALHELP]
>id="acw_global_reporting_exclusions_direct_mail_table"
>title="Uitsluitingen"
>abstract="De **Oorzaken van uitsluiting** de lijst toont een gedetailleerde uitsplitsing, door regel, van berichten die tijdens het leveringsvoorbereidingsproces werden verworpen."

>[!CONTEXTUALHELP]
>id="acw_global_reporting_causes_exclusion_direct_mail_graph"
>title="Oorzaken van uitsluiting"
>abstract="De **Oorzaken van uitsluiting** de grafiek illustreert de distributie van verworpen berichten tijdens de voorbereiding voor levering, die door elke regel wordt gecategoriseerd."

![](assets/global_report_direct_mail_exclusions.png){zoomable=&quot;yes&quot;}{align="center"}

In de grafiek en de tabel met uitsluitingen worden de redenen weergegeven waarom gebruikersprofielen, die zijn uitgesloten van de doelprofielen, het bericht niet hebben ontvangen.

+++Meer informatie over oorzaken van uitsluitingsmetingen.

* **[!UICONTROL Address in quarantine]**: Fouttype dat wordt gegenereerd wanneer het adres in quarantaine wordt geplaatst.

* **[!UICONTROL Address not specified]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het adres niet bestaat.

* **[!UICONTROL Bad quality address]**: Fouttype dat wordt gegenereerd wanneer de kwaliteitsbeoordeling van het postadres te laag is.

* **[!UICONTROL Denylisted address]**: Het type van Fout produceerde toen de ontvanger werd gevoegd op lijst van gewenste personen toen de levering werd uitgevoerd.

* **[!UICONTROL Double]**: Fouttype dat is gegenereerd toen de ontvanger werd uitgesloten, omdat de sleutelwaarden niet uniek waren.

* **[!UICONTROL Control group]**: Het adres van de ontvanger maakt deel uit van de controlegroep.

* **[!UICONTROL Target limited in size]**: De maximale leveringsgrootte is bereikt voor de ontvanger.

+++
