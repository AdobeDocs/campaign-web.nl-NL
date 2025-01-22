---
audience: end-user
title: Een e-mail voorbereiden en verzenden
description: Leer hoe u een e-mail voorbereidt en verzendt met de gebruikersinterface van het Web voor campagne
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: 58f25a6b41c89e97c0f721f4437b5245d16b3757
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 1%

---


# Uw e-mail voorbereiden en verzenden {#prepare-send}

## De verzending voorbereiden {#prepare}

Wanneer u uw [ inhoud ](../email/edit-content.md), [ publiek ](../audience/add-audience.md), en [ programma ](../msg/gs-messages.md#schedule-the-delivery-sending-gs-schedule) hebt bepaald, bent u bereid om uw e-maillevering voor te bereiden.

Tijdens de voorbereiding van de levering, wordt de doelbevolking berekend en de berichtinhoud geproduceerd voor elk profiel inbegrepen in het doel. Zodra de voorbereiding is voltooid, zijn de berichten klaar om te worden verzonden, of onmiddellijk of op de geplande datum en tijd.

De bevestigingsregels die tijdens leveringsvoorbereiding worden gebruikt worden beschreven in de [ Campagne v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/emails/send.html) {target="_blank"}.

De belangrijkste stappen voor het voorbereiden van de verzending worden hieronder vermeld.

1. Klik op **[!UICONTROL Review and send]** van het leveringdashboard.

   ![](assets/email-review-and-send.png){zoomable="yes"}


1. Klik op de knop **[!UICONTROL Prepare]** in de rechterbovenhoek en bevestig de selectie.

   ![](assets/email-prepare.png){zoomable="yes"}

   >[!NOTE]
   >
   >Als u de levering hebt gepland en de optie **[!UICONTROL Enable confirmation before sending]** hebt uitgeschakeld, worden de voorbereidings- en verzendstappen gegroepeerd onder de knop **[!UICONTROL Prepare and send]** . [ leer meer bij het plannen ](../msg/gs-deliveries.md#gs-schedule)

1. De voortgang van de voorbereiding wordt weergegeven. Afhankelijk van de omvang van de doelpopulatie kan deze operatie enige tijd duren.

   U kunt de voorbereiding op elk gewenst moment stoppen met de knop **[!UICONTROL Stop preparation]** .

   ![](assets/email-stop-preparation.png){zoomable="yes"}

   >[!NOTE]
   >Tijdens de voorbereidingsfase worden geen berichten verzonden. U kunt dit daarom starten of stoppen zonder het risico te lopen iets te beïnvloeden.

1. Controleer de PKI&#39;s wanneer de bereiding is voltooid. Als het aantal berichten dat u wilt verzenden niet overeenkomt met uw verwachtingen, wijzigt u het publiek en start u de voorbereiding opnieuw.

   ![](assets/email-preparation-complete.png){zoomable="yes"}

   Hier worden de verschillende KPI&#39;s weergegeven:

   * **[!UICONTROL Targeted]** : het aantal doelontvangers.
   * **[!UICONTROL To deliver]** : het aantal berichten dat wordt verzonden.
   * **[!UICONTROL To exclude]**: het aantal berichten die door a [ worden uitgesloten typologieregel ](../advanced-settings/delivery-settings.md#typology).

1. Klik op de knop **[!UICONTROL Logs]** en controleer of er geen fout optreedt. In het laatste logbericht worden foutberichten en het aantal fouten weergegeven. [Meer informatie](delivery-logs.md)

   ![](assets/email-prepare-logs.png){zoomable="yes"}

1. Als in het preparaat een kritieke fout wordt aangetroffen waardoor de levering niet kan worden verzonden, wordt de status van het preparaat in het leveringsdashboard weergegeven als mislukt.

   ![](assets/email-prepare-error.png){zoomable="yes"}

1. Als u na de bereiding wijzigingen aanbrengt in uw aflevering, moet u de voorbereiding opnieuw starten om met deze wijzigingen rekening te houden.

Zodra de voorbereiding zonder fout volledig is, is uw bericht klaar om te worden verzonden.

## Bericht verzenden {#send}


Zodra de [ voorbereiding ](#prepare) volledig is, kunt u uw e-mail nu verzenden.

Als het bericht gepland is, zal het op de bepaalde datum en de tijd worden verzonden. [Meer informatie](../msg/gs-deliveries.md#gs-schedule)

### Direct verzenden {#send-immediately}

Voer de onderstaande stappen uit als u direct een e-mail wilt verzenden.

1. Klik in het dashboard voor levering op de knop **[!UICONTROL Send]** in de rechterbovenhoek.

   ![](assets/email-send.png){zoomable="yes"}

1. Bevestig deze actie om het bericht aan het belangrijkste doel onmiddellijk te verzenden.

1. De verzendvoortgang wordt weergegeven.

### Het verzenden plannen {#schedule-the-send}

Voer de onderstaande stappen uit als u uw e-mail op een latere datum en tijd wilt verzenden.

1. Voordat u op de knop **[!UICONTROL Review and send]** klikt, moet u controleren of u een planning voor uw e-mail hebt gedefinieerd. [Meer informatie](../msg/gs-deliveries.md#gs-schedule)

1. Klik in het dashboard voor levering op de knop **[!UICONTROL Send as scheduled button]** in de rechterbovenhoek.

   ![](assets/email-send-as-scheduled.png){zoomable="yes"}

1. Klik op **[!UICONTROL Confirm sending]**. De levering zal op de geplande datum aan het belangrijkste doel worden verzonden.

   >[!NOTE]
   >
   >Als u de optie **[!UICONTROL Enable confirmation before sending]** hebt uitgeschakeld, worden de voorbereidings- en verzendstappen gegroepeerd onder de knop **[!UICONTROL Prepare and send]** . [ leer meer bij het plannen ](../msg/gs-deliveries.md#gs-schedule)

## De verzending onderbreken of stoppen {#pause-stop-sending}

Of uw levering gepland of niet <!--TBC--> is, kunnen twee acties op elk ogenblik tijdens het verzendende proces worden uitgevoerd:

* Klik op **[!UICONTROL Pause sending]** om het verzenden van de berichten te onderbreken. U kunt het verzenden op elk gewenst moment hervatten.

* Klik op **[!UICONTROL Stop sending]** om het verzenden direct te onderbreken. Na stopzetting kan noch de bereiding noch de verzending worden hervat.

![](assets/email-send-pause-or-stop.png){zoomable="yes"}

## De KPI&#39;s controleren {#check-kpis}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_delivered"
>title="Geleverd"
>abstract="Het aantal berichten dat is afgeleverd. Deze indicator wordt elke 5 minuten bijgewerkt. Het getoonde percentage is gebaseerd op het totale aantal verzonden berichten."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="KPI&#39;s begrijpen"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_opens"
>title="Geopende items"
>abstract="Het aantal geopende berichten. Deze indicator wordt elke 5 minuten bijgewerkt. Het getoonde percentage is de verhouding van het aantal verschillende opent in vergelijking met het aantal geleverde berichten."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="KPI&#39;s begrijpen"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_clicks"
>title="Klikken"
>abstract="Het aantal ontvangers dat ten minste één keer in de e-mail heeft geklikt. Deze indicator wordt elke 5 minuten bijgewerkt. Het getoonde percentage is de verhouding van het aantal verschillende kliks in vergelijking met het aantal geleverde berichten."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="KPI&#39;s begrijpen"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_sent"
>title="Verzonden"
>abstract="Het totale aantal berichten dat tijdens de leveringsanalyse wordt verwerkt."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="KPI&#39;s begrijpen"


>[!CONTEXTUALHELP]
>id="acw_deliveries_email_metrics_errors"
>title="Fouten"
>abstract="Totaal van fouten die tijdens levering en automatische terugkeerverwerking met betrekking tot het totale aantal verzonden berichten worden gecumuleerd."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/reports/kpis" text="KPI&#39;s begrijpen"


Zodra verzenden volledig is, kunt u getoonde KPIs controleren:

![](assets/email-send-kpis.png){zoomable="yes"}

* **[!UICONTROL Sent]** : het aantal geleverde berichten. Het getoonde percentage is gebaseerd op het totale aantal te leveren berichten.

* **[!UICONTROL Delivered]** : het aantal berichten dat is afgeleverd. Het getoonde percentage is gebaseerd op het totale aantal verzonden berichten.

* **[!UICONTROL Opens]** : het aantal geopende berichten. Het getoonde percentage is het aantal verschillende opent in vergelijking met het aantal geleverde berichten.

* **[!UICONTROL Clicks]**: het aantal ontvangers dat ten minste één keer in de e-mail heeft geklikt. Het getoonde percentage is het aantal verschillende kliks in vergelijking met het aantal geleverde berichten.

* **[!UICONTROL Errors]** : het aantal e-mails met de foutstatus. Het getoonde percentage is gebaseerd op het totale aantal verzonden berichten.

>[!NOTE]
>
>Alle indicatoren worden elke 5 minuten na de start van de levering bijgewerkt. De indicatoren voor de voorbereiding van de levering zijn realtime.

Leer meer over KPIs in [ deze pagina ](../reporting/kpis.md).

U kunt ook de logbestanden controleren. [Meer informatie](delivery-logs.md)