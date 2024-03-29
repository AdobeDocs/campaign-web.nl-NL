---
audience: end-user
title: Een pushmelding verzenden
description: Meer informatie over het verzenden van pushberichten via Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Een pushbericht voorvertonen en verzenden {#send-push-delivery}

## Geef een voorvertoning van de pushmelding weer {#preview-push}

Nadat u de inhoud van uw bericht hebt gedefinieerd, kunt u testabonnees gebruiken om het bericht voor te vertonen en te testen. Als u gepersonaliseerde inhoud hebt opgenomen, kunt u onderzoeken hoe deze inhoud in het bericht wordt getoond door de gegevens van het testprofiel te gebruiken. Dit staat u toe om ervoor te zorgen dat het bericht correct wordt teruggegeven en dat de gepersonaliseerde elementen correct worden opgenomen.

De belangrijkste stappen voor een voorvertoning van uw pushmelding zijn als volgt. Meer informatie over het bekijken van voorvertoningen vindt u in [deze sectie](../preview-test/preview-content.md).

1. Vanaf de pagina met inhoud voor levering gebruiken **[!UICONTROL Simulate content]** om een voorvertoning van uw persoonlijke inhoud weer te geven.

   ![](assets/push_send_1.png){zoomable=&quot;yes&quot;}

1. Klikken **[!UICONTROL Add subscribers(s)]** om een of meerdere profielen te selecteren om een voorvertoning van hun gegevens weer te geven in de inhoud van het pushbericht.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. In het rechterdeelvenster vindt u een voorvertoning van het pushbericht, waarin gepersonaliseerde elementen dynamisch worden vervangen door gegevens uit het geselecteerde profiel.

   ![](assets/push_send_7.png){zoomable=&quot;yes&quot;}

U kunt nu uw pushmelding bekijken en verzenden naar uw publiek.

## De levering van pushberichten testen {#test-push}

Gebruiken **Adobe Campaign**, kunt u proefdrukken verzenden voordat u deze naar het grote publiek stuurt. Deze stap is belangrijk voor het valideren van uw levering en het identificeren van eventuele problemen.

Testprofielen zijn de proefontvangers. Ze kunnen componenten en instellingen zoals koppelingen, afbeeldingen en personalisatie controleren en valideren, zodat u optimale prestaties krijgt en eventuele fouten kunt opsporen. Met dit proces kunt u uw pushmeldingen verfijnen en optimaliseren voordat u het grote publiek bereikt. [Meer informatie over het verzenden van proefdrukken](../preview-test/test-deliveries.md#subscribers)

![](assets/push_send_6.png){zoomable=&quot;yes&quot;}

## Verzend uw pushmelding {#send-push}

1. Klik op **[!UICONTROL Review & send]** van uw **[!UICONTROL Delivery]** pagina.

   ![](assets/push_send_2.png){zoomable=&quot;yes&quot;}

1. Klikken **[!UICONTROL Prepare]** en toezicht te houden op de geboekte vooruitgang en de verstrekte statistieken.

   Als er fouten optreden, raadpleegt u het menu Logs voor meer informatie over de fout.

   ![](assets/push_send_3.png){zoomable=&quot;yes&quot;}

1. Verzend de berichten door op te klikken **[!UICONTROL Send]** om door te gaan met het definitieve verzendingsproces.

1. Bevestig de verzendactie door op de knop **[!UICONTROL Send]**.

   Als de aflevering is gepland, klikt u op de knop **[!UICONTROL Send as scheduled]** knop. Meer informatie over de planning van de levering in [deze sectie](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![](assets/push_send_4.png){zoomable=&quot;yes&quot;}

Zodra uw levering wordt verzonden, kunt u uw KPIs (Zeer belangrijke Indicator van Prestaties) gegevens van uw leveringspagina en gegevens van volgen **[!UICONTROL Logs]** -menu.

U kunt nu beginnen de impact van uw bericht te meten met ingebouwde rapporten. [Meer informatie](../reporting/push-report.md)
