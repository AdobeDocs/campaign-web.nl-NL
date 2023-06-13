---
audience: end-user
title: Campagnerapporten
description: Meer informatie over het openen en gebruiken van campagnerapporten
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 1%

---

# Campagnerapporten {#campaign-reports}

Het campagnerapport bestaat uit verschillende widgets waarin het succes en de fouten van uw campagne worden beschreven.

De pagina van het campagnerapport zal met de volgende lusjes worden getoond:

* [E-mailkanaal](#email-channel)
* [Sms-kanaal](#sms-channel)
* [Push-kanaal](#push-channel)

Als u het campagnerapport wilt openen, klikt u op Rapporten op het dashboard van uw campagne.

![](assets/campaign_report_email_13.png)

## E-mailkanaal {#email-channel}

### Leveringsoverzicht {#delivery-summary-email}

* **[!UICONTROL Delivery Overview]** Hier vindt u belangrijke prestatie-indicatoren (KPI&#39;s) die gedetailleerde informatie geven over de manier waarop bezoekers uw e-maillevering uitvoeren.

  ![](assets/campaign_report_email_1.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Total sent]**: Het totale aantal berichten dat tijdens de leveringsanalyse wordt verwerkt.

   * **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

   * **[!UICONTROL Bounces]**: Totaal van fouten die tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten worden gecumuleerd.

   * **[!UICONTROL Distinct opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste één keer heeft geopend.

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

+++

* **[!UICONTROL Initial target audience statistics]** de lijst toont gegevens met betrekking tot uw ontvangers:

  ![](assets/campaign_report_email_2.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Initial audience]**: Totaal aantal beoogde ontvangers.

   * **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na leveringsanalyse moet worden bezorgd.

   * **[!UICONTROL Rejected by rules]**: Totaal aantal adressen genegeerd tijdens de analyse wanneer het toepassen van regels: het adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

* **[!UICONTROL Execution statistics]** de tabel geeft het succes van uw levering aan .

  ![](assets/campaign_report_email_3.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na leveringsanalyse moet worden bezorgd.

   * **[!UICONTROL Success]**: Aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL Errors]**: Het totale aantal fouten dat tijdens leveringen is gecumuleerd en de automatische oplaadbewerking in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL New quarantines]**: Het totale aantal adressen quarantined na een ontbroken levering (onbekend gebruiker, ongeldig domein) met betrekking tot het aantal te leveren berichten.

+++

* **[!UICONTROL Reaction statistics]** de lijst bevat de beschikbare gegevens voor ontvankelijke activiteit voor uw levering.

  ![](assets/campaign_report_email_4.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Distinct opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste één keer heeft geopend.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens eenmaal hebben geopend.

   * **[!UICONTROL Unsubscriptions]**: Aantal ontvangers dat op afboekingen voor de betrokken periode heeft geklikt.

   * **[!UICONTROL Mirror page]**: Aantal ontvangers die op de verbinding van de spiegelpagina klikte.

   * **[!UICONTROL Forwards]**: Aantal ontvangers dat heeft geklikt en het e-mailbericht heeft doorgestuurd.
+++

* **[!UICONTROL Generated click streams]** de lijst toont gegevens met betrekking tot hoe uw ontvangers met uw levering interactie hadden.

  ![](assets/campaign_report_email_5.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Reactivity]**: Verhouding van het aantal ontvangers voor wie de levering is bedoeld en waarop op de levering is geklikt, in verhouding tot het geschatte aantal ontvangers voor wie de levering is geopend.

+++

### Niet-te leveren items {#non-deliverables-email}

* **[!UICONTROL Breakdown of errors per type]** en **[!UICONTROL Breakdown of errors per domain]** tabellen en grafieken bevatten de beschikbare gegevens voor mogelijke fouten die met elk domein worden aangetroffen.

  De fouten die in dit rapport worden weergegeven, activeren het quarantaineproces. Voor meer informatie over quarantainebeheer raadpleegt u [Quarantainebeheer](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html).

  ![](assets/campaign_report_email_6.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL User unknown]**: Fouttype dat tijdens de levering wordt gegenereerd om aan te geven dat het e-mailadres ongeldig is.

   * **[!UICONTROL Invalid domain]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het domein van het e-mailadres onjuist is of niet bestaat.

   * **[!UICONTROL Mailbox full]**: Het type van fout na vijf leveringspogingen wordt geproduceerd om erop te wijzen dat de ontvangers&#39; inbox teveel berichten bevat.

   * **[!UICONTROL Account disabled]**: Fouttype dat wordt gegenereerd bij het verzenden van een levering om aan te geven dat het adres niet langer bestaat.

   * **[!UICONTROL Refused]**: Het type van fout produceerde wanneer een adres door IAP (Internet Access Provider) wordt verworpen, bijvoorbeeld na de toepassing van een veiligheidsregel (anti-spamsoftware).

   * **[!UICONTROL Unreachable]**: Fouttype dat optreedt in de tekenreeks voor berichtdistributie: incident op het SMTP relais, tijdelijk onbereikbaar domein, enz.

   * **[!UICONTROL Not connected]**: Fouttype om aan te geven dat de mobiele telefoon van de ontvanger op het moment van verzending wordt uitgeschakeld of losgekoppeld van het netwerk.

+++

### Trackingsindicatoren {#tracking-indicators-email}

* **[!UICONTROL Delivery statistics]** biedt prestatiekernindicatoren (KPI&#39;s) die gedetailleerde informatie geven over gegevens die beschikbaar zijn voor verzonden e-mails.

  ![](assets/campaign_report_email_7.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Success]**: Aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL Distinct opens]**: Het totale aantal beoogde ontvangers dat een bericht ten minste één keer heeft geopend.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens eenmaal hebben geopend.

   * **[!UICONTROL Clicks on the opt-out link]**: Aantal klikken op de verbinding van het unsubscription.

   * **[!UICONTROL Clicks on the mirror link]**: Aantal klikken op de verbinding aan de spiegelpagina.

   * **[!UICONTROL Estimation of forwards]**: Schatting van het aantal e-mails dat door de beoogde ontvangers is doorgestuurd.
+++

* **[!UICONTROL Initial target audience statistics]** de lijst toont gegevens met betrekking tot uw ontvangers.

  ![](assets/campaign_report_email_8.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Sent]**: Het totale aantal verzonden berichten.

   * **[!UICONTROL Complaints]**: Aantal berichten voor dit domein die als ongewenst door de ontvanger zijn gemeld.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens eenmaal hebben geopend.

   * **[!UICONTROL Clicks]**: Aantal afzonderlijke beoogde ontvangers die minstens één keer op dezelfde levering hebben geklikt.

   * **[!UICONTROL Raw reactivity]**: Percentage van het aantal ontvangers dat ten minste één keer op een levering heeft geklikt in vergelijking met het aantal ontvangers dat een levering ten minste één keer heeft geopend.
+++

### URL&#39;s en klikpaden {#url-email}

* **[!UICONTROL URLs and click streams]** verstrekt zeer belangrijke prestatiesindicatoren (KPIs) die gedetailleerde informatie over URLs geven die het meest tijdens een levering werden geklikt.

  ![](assets/campaign_report_email_9.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Reactivity]**: Verhouding van het aantal ontvangers voor wie de levering is bedoeld en waarop op de levering is geklikt, in verhouding tot het geschatte aantal ontvangers voor wie de levering is geopend.

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Platform average]** : Dit gemiddelde tarief, dat onder elk tarief wordt getoond (reactiviteit, verschillende kliks, en gecumuleerde kliks), wordt berekend voor leveringen die in de voorafgaande zes maanden werden verzonden. Alleen leveringen met dezelfde typologie en op hetzelfde kanaal worden in aanmerking genomen. Proefdrukken zijn uitgesloten.
+++

* **[!UICONTROL Top 10 most visited links]** de grafiek en de lijst bevatten de beschikbare gegevens voor ontvankelijk gedrag per verbinding.

  ![](assets/campaign_report_email_10.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Percentage]**: Percentage gebruikers dat interactie had met de levering.

+++

* **[!UICONTROL Breakdown of clicks over time]** de grafiek bevat de beschikbare gegevens voor het gedrag van de ontvanger per koppeling.

  ![](assets/campaign_report_email_11.png)

### Gebruikersactiviteiten {#user-activities-email}

* **[!UICONTROL User activities]** toont de uitsplitsing van opent en klikt in de vorm van een grafiek.

  ![](assets/campaign_report_email_12.png)

  +++Meer informatie over de afmetingen van het campagnerapport voor e-mail.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Opens]**: Aantal verschillende beoogde ontvangers voor dit domein die een bericht minstens eenmaal hebben geopend.

+++

## Sms-kanaal {#sms-channel}

### Leveringsoverzicht {#delivery-summary-sms}

* **[!UICONTROL Delivery Overview]** biedt prestatiekernindicatoren (KPI&#39;s) die gedetailleerde informatie geven over de manier waarop bezoekers uw SMS-levering gebruiken.

  ![](assets/campaign_report_sms_1.png)

  +++Meer weten over de metriek van het SMS-campagnerapport?

   * **[!UICONTROL Total sent]**: Het totale aantal berichten dat tijdens de leveringsanalyse wordt verwerkt.

   * **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

   * **[!UICONTROL Errors]**: Totaal van fouten die tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten worden gecumuleerd.

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

+++

* **[!UICONTROL Initial target audience statistics]** de lijst toont gegevens met betrekking tot uw ontvangers:

  ![](assets/campaign_report_sms_2.png)

  +++Meer weten over de metriek van het SMS-campagnerapport?

   * **[!UICONTROL Initial audience]**: Totaal aantal beoogde ontvangers.

   * **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na leveringsanalyse moet worden bezorgd.

   * **[!UICONTROL Rejected by rules]**: Totaal aantal adressen genegeerd tijdens de analyse wanneer het toepassen van regels: het adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

* **[!UICONTROL Execution statistics]** de tabel geeft het succes van uw levering aan :

  ![](assets/campaign_report_sms_3.png)

  +++Meer weten over de metriek van het SMS-campagnerapport?

   * **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na leveringsanalyse moet worden bezorgd.

   * **[!UICONTROL Success]**: Aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL Errors]**: Het totale aantal fouten dat tijdens leveringen is gecumuleerd en de automatische oplaadbewerking in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL New quarantines]**: Het totale aantal adressen quarantined na een ontbroken levering (onbekend gebruiker, ongeldig domein) met betrekking tot het aantal te leveren berichten.

+++

* **[!UICONTROL Generated click streams]** de lijst toont gegevens met betrekking tot hoe uw ontvangers met uw levering interactie hadden:

  ![](assets/campaign_report_sms_4.png)

  +++Meer weten over de metriek van het SMS-campagnerapport?

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Reactivity]**: Verhouding van het aantal ontvangers voor wie de levering is bedoeld en waarop op de levering is geklikt, in verhouding tot het geschatte aantal ontvangers voor wie de levering is geopend.

+++

## Push-kanaal {#push-channel}

### Leveringsoverzicht {#delivery-summary-push}

* **[!UICONTROL Delivery Overview]** biedt prestatiekernindicatoren (KPI&#39;s) die gedetailleerde informatie geven over de manier waarop bezoekers de pushmelding verzenden.

  +++Meer weten over cijfers voor pushcampagnerapporten?

   * **[!UICONTROL Total sent]**: Het totale aantal berichten dat tijdens de leveringsanalyse wordt verwerkt.

   * **[!UICONTROL Delivered]**: Het aantal berichten dat is verzonden in verhouding tot het totale aantal verzonden berichten.

   * **[!UICONTROL Errors]**: Totaal van fouten die tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten worden gecumuleerd.

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

+++

* **[!UICONTROL Initial target audience statistics]** de lijst toont gegevens met betrekking tot uw ontvangers:

  +++Meer weten over cijfers voor pushcampagnerapporten?

   * **[!UICONTROL Initial audience]**: Totaal aantal beoogde ontvangers.

   * **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na leveringsanalyse moet worden bezorgd.

   * **[!UICONTROL Rejected by rules]**: Totaal aantal adressen genegeerd tijdens de analyse wanneer het toepassen van regels: het adres ontbreekt, quarantined, op lijst van gewezen personen, enz.

+++

* **[!UICONTROL Execution statistics]** de tabel geeft het succes van uw levering aan :

  +++Meer weten over cijfers voor pushcampagnerapporten?

   * **[!UICONTROL Message to deliver]**: Totaal aantal berichten dat na leveringsanalyse moet worden bezorgd.

   * **[!UICONTROL Success]**: Aantal berichten dat met succes is verwerkt in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL Errors]**: Het totale aantal fouten dat tijdens leveringen is gecumuleerd en de automatische oplaadbewerking in verhouding tot het aantal te leveren berichten.

   * **[!UICONTROL New quarantines]**: Het totale aantal adressen quarantined na een ontbroken levering (onbekend gebruiker, ongeldig domein) met betrekking tot het aantal te leveren berichten.

+++

* **[!UICONTROL Generated click streams]** de lijst toont gegevens met betrekking tot hoe uw ontvangers met uw levering interactie hadden:

  +++Meer weten over cijfers voor pushcampagnerapporten?

   * **[!UICONTROL Distinct clicks]**: Het totale aantal verschillende ontvangers dat minstens één keer op een levering heeft geklikt.

   * **[!UICONTROL Clicks]**: Het totale aantal klikken op koppelingen in leveringen.

   * **[!UICONTROL Reactivity]**: Verhouding van het aantal ontvangers voor wie de levering is bedoeld en waarop op de levering is geklikt, in verhouding tot het geschatte aantal ontvangers voor wie de levering is geopend.

+++
