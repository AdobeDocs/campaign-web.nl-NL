---
audience: end-user
title: E-mailleveringsrapporten
description: Leer hoe u rapporten over e-maillevering kunt openen en gebruiken
badge: label="Beta"
source-git-commit: f80a224665e8c70c2efce3af9a8f60a07fadd5dc
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 1%

---

# E-mailleveringsrapport {#email-report}

De **E-mailleveringsrapport** biedt uitgebreide inzichten en gegevens die specifiek zijn voor het e-mailkanaal. Het biedt gedetailleerde informatie over de prestaties, effectiviteit en resultaten van uw afzonderlijke leveringen, zodat u een uitgebreid overzicht krijgt.

## Leveringsoverzicht {#delivery-summary-email}

* **[!UICONTROL Initial target audience statistics]** de lijst toont gegevens met betrekking tot uw ontvangers:

  ![](assets/reporting_email_1.png){align="left" zoomable="yes"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Initial audience]**: Totaal aantal beoogde ontvangers.

   * **[!UICONTROL To deliver]**: Totaal aantal berichten dat na de voorbereiding van de levering moet worden bezorgd.

   * **[!UICONTROL Exclusion]**: Het totale aantal berichten dat is uitgesloten van het verzonden doel.
+++

* **[!UICONTROL Delivery statistics]** in de tabel wordt aangegeven hoe succesvol de levering is .

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

Dit rapport bevat gedetailleerde informatie over de leveringstijd van het gehele platform binnen een opgegeven tijdsbestek. Primaire metrisch die wordt gebruikt om de snelheid van berichtlevering te meten is het aantal berichten per uur worden verzonden.

## Uitzendstatistieken {#broadcast-statistics}

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

* **[!UICONTROL User activities]** toont de uitsplitsing van opent en klikt in de vorm van een grafiek. U kunt de tijdsperiode kiezen waarin de gegevens moeten worden opgenomen: laatste dag, afgelopen uur of 30 minuten.

  ![](assets/reporting_email_10.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

+++

## Statistieken bijhouden {#tracking-statistics}


* **[!UICONTROL Tracking Statistics]** de grafiek verstrekt statistieken over opent en klikt. U kunt het specifieke tijdkader selecteren voor het opgeven van gegevens.

  ![](assets/reporting_email_11.png){align="center"}

  +++Meer informatie over de afmetingen van het e-mailleveringsrapport.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens één keer hebben geopend.

+++

## Indeling van openen {#breakdown-opens}

In dit rapport wordt de uitsplitsing van de openingen per besturingssysteem, apparaat en browser voor de betrokken periode weergegeven. Voor elke categorie worden twee grafieken gebruikt. De eerste toont statistieken betreffende opent op een computer en mobiele apparaten. In het tweede voorbeeld worden alleen statistieken weergegeven over het openen op mobiele apparaten.
U hebt de flexibiliteit om over te schakelen van **[!UICONTROL Fix & mobile]** uitsluitend **[!UICONTROL Mobile only]** voor een nauwkeuriger doelgerichtheid.

![](assets/reporting_email_13.png){align="center"}

## Hotclicks {#hotclicks}

Dit rapport toont de berichtinhoud (HTML en/of tekst) met, op elke verbinding, het percentage klikt op verbindingen. De belemmeringen van de verpersoonlijking unsubscription verbindingen, spiegelpaginakoppelingen en aanbiedingsverbindingen worden in de totale gecumuleerde kliks in aanmerking genomen maar niet getoond in het rapport.

![](assets/reporting11.png)
