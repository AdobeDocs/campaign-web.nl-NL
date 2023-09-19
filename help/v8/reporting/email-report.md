---
audience: end-user
title: E-mailleveringsrapporten
description: Leer hoe u rapporten over e-maillevering kunt openen en gebruiken
badge: label="Beta"
source-git-commit: 5307387d63df5ae3af1b849fa0a1181c42cc1879
workflow-type: tm+mt
source-wordcount: '1659'
ht-degree: 0%

---

# E-mailleveringsrapport {#email-report}

De **E-mailleveringsrapport** biedt uitgebreide inzichten en gegevens die specifiek zijn voor het e-mailkanaal. Het biedt gedetailleerde informatie over de prestaties, effectiviteit en resultaten van uw afzonderlijke leveringen, zodat u een uitgebreid overzicht krijgt.

## Leveringsoverzicht {#delivery-summary-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_sending_email"
>title="Rapportage verzenden"
>abstract="Het menu Verzenden in uw rapport biedt diepgaande inzichten in de interacties van uw bezoekers met uw leveringen en eventuele fouten die deze hebben aangetroffen."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_initial_target"
>title="Oorspronkelijke doelpopulatie-widget"
>abstract="De aanvankelijke grafiek van de doelpopulatie toont gegevens met betrekking tot uw ontvangers en het succes van uw levering."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_summary"
>title="Widget Afleveringsstatistieken"
>abstract="De grafiek van de statistiek van de Levering detailleert het succes van uw levering en fouten die voorkwamen."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_exclusion"
>title="Widget Afleveringsstatistieken"
>abstract="In de grafiek en de tabel van de oorzaken van de uitsluiting wordt de uitsplitsing per regel van de tijdens de voorbereiding afgewezen berichten weergegeven."

* **[!UICONTROL Initial target audience population]** de grafiek toont gegevens met betrekking tot uw ontvangers:

  ![](assets/reporting_email_1.png){align="left" zoomable="yes"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Initial audience]**: Totaal aantal beoogde ontvangers.

   * **[!UICONTROL To deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

   * **[!UICONTROL Exclusion]**: Het totale aantal berichten dat is uitgesloten van het verzonden doel.
+++

* **[!UICONTROL Delivery statistics]** grafiek geeft het succes van uw levering aan.

  ![](assets/reporting_email_2.png){align="left"}

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Message sent]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

   * **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL Errors]**: Totaal aantal fouten bij leveringen en automatische oplevering in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL New quarantines]**: Het totale aantal adressen dat in quarantaine wordt geplaatst na een mislukte levering (onbekend, ongeldig domein) in verhouding tot het aantal te leveren berichten.

+++

* **[!UICONTROL Causes of exclusion]** de grafiek en de tabel geven de uitsplitsing per regel van de tijdens de analyse afgewezen berichten weer.

  ![](assets/reporting_email_3.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL User unknown]**: Fouttype dat tijdens de levering wordt gegenereerd om aan te geven dat het e-mailadres ongeldig is.

   * **[!UICONTROL Invalid domain]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het domein van het e-mailadres onjuist is of niet bestaat.

   * **[!UICONTROL Mailbox full]**: Fouttype dat wordt gegenereerd na vijf leveringspogingen om aan te geven dat het postvak van de ontvanger te veel berichten bevat.

   * **[!UICONTROL Account disabled]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het adres niet langer bestaat.

   * **[!UICONTROL Refused]**: Fouttype dat wordt gegenereerd wanneer een adres wordt afgewezen door de IAP (Internet Access Provider), bijvoorbeeld na toepassing van een beveiligingsregel (anti-spamsoftware).

   * **[!UICONTROL Unreachable]**: Het type van fout dat in het koord van de berichtdistributie voorkomt: incident op het relais SMTP, domein tijdelijk onbereikbaar etc.

   * **[!UICONTROL Not connected]**: Fouttype om aan te geven dat de mobiele telefoon van de ontvanger op het moment van verzending wordt uitgeschakeld of losgekoppeld van het netwerk.

+++

## Leveringsdoorvoer {#delivery-throughtput}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_throughput_email"
>title="Widget voor productie"
>abstract="Het rapport Productie-doorvoer bevat gedetailleerde informatie over de leveringstijd van het gehele platform binnen een opgegeven tijdsbestek."

Dit rapport bevat gedetailleerde informatie over de leveringstijd van het gehele platform binnen een opgegeven tijdsbestek. Primaire metrisch die wordt gebruikt om de snelheid van berichtlevering te meten is het aantal berichten per uur worden verzonden.

## Uitzendstatistieken {#broadcast-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_broadcast_statistics"
>title="Widget statistiek uitzenden"
>abstract="De lijst van de statistiek van de Uitzending bevat de beschikbare gegevens voor mogelijke fouten die met elk domein worden ontmoet."

* **[!UICONTROL Broadcast statistics]** de tabel bevat de beschikbare gegevens voor mogelijke fouten die met elk domein zijn aangetroffen.

  ![](assets/reporting_email_4.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Processed emails]**: Het totale aantal berichten dat door de leveringsserver wordt verwerkt.

   * **[!UICONTROL Delivered]**: Percentage van het aantal succesvol verwerkte berichten vergeleken met het totale aantal verwerkte berichten.

   * **[!UICONTROL Hard bounces]**: Percentage van het aantal &#39;harde&#39; grenzen, permanente fouten, zoals een onjuist e-mailadres, in vergelijking met het totale aantal verwerkte berichten.

   * **[!UICONTROL Soft bounces]**: Percentage van het aantal &quot;zachte&quot; grenzen, tijdelijke fouten zoals een volledig postvak, vergeleken met het totale aantal verwerkte berichten

   * **[!UICONTROL Opens]**: Percentage van het aantal beoogde ontvangers die een bericht ten minste eenmaal hebben geopend in vergelijking met het aantal berichten dat met succes is verwerkt.

   * **[!UICONTROL Clicks]**: Percentage van het aantal personen dat ten minste eenmaal op een levering heeft geklikt in verhouding tot het aantal berichten dat met succes is verwerkt.

   * **[!UICONTROL Unsubscriptions]**: Percentage van het aantal klikken op een koppeling zonder abonnement in verhouding tot het aantal berichten dat met succes is verwerkt.
+++

## Niet-leverbare items en niet-bezorgingen {#non-deliverables-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_type"
>title="Uitsplitsing van fouten per widget type"
>abstract="De indeling van fouten per tabel en grafiek bevat de beschikbare gegevens voor elk aangetroffen fouttype."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_error_domain"
>title="Uitsplitsing van fouten per domeinwidget"
>abstract="De indeling van fouten per tabel en grafiek bevat de beschikbare gegevens voor elk type fout dat afhankelijk van elk domein wordt aangetroffen."

* **[!UICONTROL Breakdown of errors per type]** en **[!UICONTROL Breakdown of errors per domain]** tabellen en grafieken bevatten de beschikbare gegevens voor mogelijke fouten die met elk domein worden aangetroffen.

  De fouten die in dit rapport worden weergegeven, activeren het quarantaineproces. Voor meer informatie over quarantainebeheer raadpleegt u [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html){target="_blank"}.

  ![](assets/campaign_report_email_6.png)

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL User unknown]**: Fouttype dat tijdens de levering wordt gegenereerd om aan te geven dat het e-mailadres ongeldig is.

   * **[!UICONTROL Invalid domain]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het domein van het e-mailadres onjuist is of niet bestaat.

   * **[!UICONTROL Mailbox full]**: Fouttype dat wordt gegenereerd na vijf leveringspogingen om aan te geven dat het postvak van de ontvanger te veel berichten bevat.

   * **[!UICONTROL Account disabled]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het adres niet langer bestaat.

   * **[!UICONTROL Refused]**: Fouttype dat wordt gegenereerd wanneer een adres wordt afgewezen door de IAP (Internet Access Provider), bijvoorbeeld na toepassing van een beveiligingsregel (anti-spamsoftware).

   * **[!UICONTROL Unreachable]**: Het type van fout dat in het koord van de berichtdistributie voorkomt: incident op het relais SMTP, domein tijdelijk onbereikbaar etc.

   * **[!UICONTROL Not connected]**: Fouttype om aan te geven dat de mobiele telefoon van de ontvanger op het moment van verzending wordt uitgeschakeld of losgekoppeld van het netwerk.

+++

## Trackingsindicatoren {#tracking-indicators-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_tracking_email"
>title="Reeksspatiëring rapporteren"
>abstract="Het lusje van het Volgen binnen uw rapport biedt waardevolle gegevens, met inbegrip van ontvankelijk gedrag per verbinding, onderbreking van opent en klikt, evenals gedetailleerde informatie over meest vaak klikte URLs tijdens een levering."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_delivery_statistics_indicators"
>title=" Widget Afleveringsstatistieken"
>abstract="De widget voor leveringsstatistieken biedt belangrijke prestatie-indicatoren (KPI&#39;s) die gedetailleerde informatie geven over gegevens die beschikbaar zijn voor verzonden e-mails."

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_open_clickthrough"
>title="Widget voor Open- en doorkliksnelheid"
>abstract="In de tabel met Open- en Doorklikfrequenties worden gegevens weergegeven die betrekking hebben op de betrokkenheid van uw ontvangers bij uw levering."

* **[!UICONTROL Delivery statistics]** biedt prestatiekernindicatoren (KPI&#39;s) die gedetailleerde informatie geven over gegevens die beschikbaar zijn voor verzonden e-mails.

  ![](assets/reporting_email_5.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Success]**: Het aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL Distinct opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste eenmaal heeft geopend.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

   * **[!UICONTROL Clicks on the opt-out link]**: Het aantal klikken op de koppeling voor het opzeggen van abonnementen.

   * **[!UICONTROL Clicks on the mirror link]**: Het aantal klikken op de koppeling naar de spiegelpagina.

   * **[!UICONTROL Estimation of forwards]**: Schatting van het aantal e-mails dat door de beoogde ontvangers is doorgestuurd.
+++

* **[!UICONTROL Open and click-through rate]** de lijst toont gegevens met betrekking tot uw ontvangers.

  ![](assets/reporting_email_6.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Sent]**: Totaal aantal verzonden berichten.

   * **[!UICONTROL Complaints]**: Het aantal berichten voor dit domein dat door de ontvanger als ongewenst is gemeld.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

   * **[!UICONTROL Clicks]**: Aantal verschillende beoogde ontvangers die minstens één keer op dezelfde levering hebben geklikt.

   * **[!UICONTROL Raw reactivity]**: Percentage van het aantal ontvangers dat ten minste één keer op een levering heeft geklikt in vergelijking met het aantal ontvangers dat een levering ten minste één keer heeft geopend.
+++

## URL&#39;s en klikpaden {#url-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_urls_clickstreams"
>title="URL&#39;s en klik op de widget Streams"
>abstract="URLs en klik stromen verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over URLs geven die het meest tijdens een levering werden geklikt."

* **[!UICONTROL URLs and click streams]** verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over URLs geven die het meest tijdens een levering werden geklikt.

  ![](assets/reporting_email_7.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Reactivity]**: Verhouding van het aantal beoogde ontvangers dat op een levering heeft geklikt, in verhouding tot het geschatte aantal beoogde ontvangers dat een levering heeft geopend.

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Platform average]** : Dit gemiddelde tarief, dat onder elk tarief wordt getoond (reactiviteit, verschillende kliks, en gecumuleerde kliks), wordt berekend voor leveringen die in de voorafgaande zes maanden werden verzonden. Alleen leveringen met dezelfde typologie en op hetzelfde kanaal worden in aanmerking genomen. Proefdrukken zijn uitgesloten.

+++

* **[!UICONTROL Top 10 most visited links]** de grafiek en de lijst bevatten de beschikbare gegevens voor ontvankelijk gedrag per verbinding.

  ![](assets/reporting_email_8.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Percentage]**: Percentage gebruikers dat interactie had met de levering.

+++

* **[!UICONTROL Breakdown of clicks over time]** de grafiek bevat de beschikbare gegevens voor het gedrag van de ontvanger per koppeling.

  ![](assets/reporting_email_9.png){align="center"}

## Gebruikersactiviteiten {#user-activities-email}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_user_activities"
>title="Widget gebruikersactiviteiten"
>abstract="In de grafiek Gebruikersactiviteiten wordt de uitsplitsing van geopend en geklikt in de vorm van een diagram. U kunt de tijdsperiode kiezen waarin de gegevens moeten worden opgenomen: laatste dag, afgelopen uur of 30 minuten."

* **[!UICONTROL User activities]** toont de uitsplitsing van opent en klikt in de vorm van een grafiek. U kunt de tijdsperiode kiezen waarin de gegevens moeten worden opgenomen: laatste dag, afgelopen uur of 30 minuten.

  ![](assets/reporting_email_10.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

+++

## Statistieken bijhouden {#tracking-statistics}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_statistics"
>title="Widget Statistieken bijhouden"
>abstract="De grafiek van de Statistieken van het Volgen verstrekt statistieken over opent en klikt. U kunt het specifieke tijdkader selecteren voor het opgeven van gegevens."

* **[!UICONTROL Tracking Statistics]** de grafiek verstrekt statistieken over opent en klikt. U kunt het specifieke tijdkader selecteren voor het opgeven van gegevens.

  ![](assets/reporting_email_11.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

+++

## Indeling van openen {#breakdown-opens}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_device"
>title="Onderverdeling per apparaatwidget"
>abstract="De indeling per apparaat"

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_breakdown_os"
>title="Onderverdeling op besturingssysteemwidget"
>abstract="Uitsplitsing door besturingssysteem"

In dit rapport wordt de uitsplitsing van de openingen per besturingssysteem, apparaat en browser voor de betrokken periode weergegeven. Voor elke categorie worden twee grafieken gebruikt. De eerste toont statistieken betreffende opent op een computer en mobiele apparaten. In het tweede voorbeeld worden alleen statistieken weergegeven over het openen op mobiele apparaten.
U hebt de flexibiliteit om over te schakelen van **[!UICONTROL Fix & mobile]** uitsluitend **[!UICONTROL Mobile only]** voor een nauwkeuriger doelgerichtheid.

![](assets/reporting_email_13.png){align="center"}

## Hotclicks {#hotclicks}

>[!CONTEXTUALHELP]
>id="acw_delivery_reporting_hotclicks"
>title="Hotclicks-rapport"
>abstract="Het rapport Hotclicks geeft de inhoud van het bericht weer met het percentage klikken op elke koppeling."

Dit rapport toont de berichtinhoud (HTML en/of tekst) met, op elke verbinding, het percentage klikt op verbindingen. De belemmeringen van de verpersoonlijking unsubscription verbindingen, spiegelpaginakoppelingen en aanbiedingsverbindingen worden in de totale gecumuleerde kliks in aanmerking genomen maar niet getoond in het rapport.

![](assets/reporting11.png)
