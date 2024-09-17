---
audience: end-user
title: Een pushmelding verzenden
description: Meer informatie over het verzenden van pushberichten via Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Een pushbericht voorvertonen en verzenden {#send-push-delivery}

## Geef een voorvertoning van de pushmelding weer {#preview-push}

Nadat u de inhoud van uw bericht hebt gedefinieerd, kunt u testabonnees gebruiken om het bericht voor te vertonen en te testen. Als u gepersonaliseerde inhoud hebt opgenomen, kunt u onderzoeken hoe deze inhoud in het bericht wordt getoond door de gegevens van het testprofiel te gebruiken. Dit staat u toe om ervoor te zorgen dat het bericht correct wordt teruggegeven en dat de gepersonaliseerde elementen correct worden opgenomen.

De belangrijkste stappen voor een voorvertoning van uw pushmelding zijn als volgt. Meer details op hoe te voorproef zijn de leveringen beschikbaar in [ deze sectie ](../preview-test/preview-content.md).

1. Gebruik **[!UICONTROL Simulate content]** om een voorvertoning van uw gepersonaliseerde inhoud weer te geven vanaf de pagina met de inhoud van de levering.

   ![](assets/push_send_1.png){zoomable="yes"}

1. Klik op **[!UICONTROL Add subscribers(s)]** om een of meerdere profielen te selecteren om een voorvertoning van hun gegevens weer te geven in de inhoud van het pushbericht.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. In het rechterdeelvenster vindt u een voorvertoning van het pushbericht, waarin gepersonaliseerde elementen dynamisch worden vervangen door gegevens uit het geselecteerde profiel.

   ![](assets/push_send_7.png){zoomable="yes"}

U kunt nu uw pushmelding bekijken en verzenden naar uw publiek.

## De levering van pushberichten testen {#test-push}

Gebruikend **Adobe Campaign**, hebt u de capaciteit om proeven te verzenden alvorens hen naar uw belangrijkste publiek te verzenden. Deze stap is belangrijk voor het valideren van uw levering en het identificeren van eventuele problemen.

Testprofielen zijn de proefontvangers. Ze kunnen componenten en instellingen zoals koppelingen, afbeeldingen en personalisatie controleren en valideren, zodat u optimale prestaties krijgt en eventuele fouten kunt opsporen. Met dit proces kunt u uw pushmeldingen verfijnen en optimaliseren voordat u het grote publiek bereikt. [ Leer hoe te om proefdrukken ](../preview-test/test-deliveries.md#subscribers) te verzenden

![](assets/push_send_6.png){zoomable="yes"}

## Verzend uw pushmelding {#send-push}

1. Nadat u de inhoud van uw pushmelding hebt aangepast, klikt u op **[!UICONTROL Review & send]** op de **[!UICONTROL Delivery]** -pagina.

   ![](assets/push_send_2.png){zoomable="yes"}

1. Klik op **[!UICONTROL Prepare]** en controleer de voortgang en de beschikbare statistieken.

   Als er fouten optreden, raadpleegt u het menu Logs voor meer informatie over de fout.

   ![](assets/push_send_3.png){zoomable="yes"}

1. Verzend de berichten door op **[!UICONTROL Send]** te klikken om verder te gaan met het laatste verzendproces.

1. Bevestig de verzendactie door op **[!UICONTROL Send]** te klikken.

   Als de aflevering is gepland, klikt u op de knop **[!UICONTROL Send as scheduled]** . Leer meer over levering het plannen in [ deze sectie ](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![](assets/push_send_4.png){zoomable="yes"}

Zodra uw levering wordt verzonden, kunt u uw gegevens van KPIs (Zeer belangrijke Indicator van Prestaties) van uw leveringspagina en gegevens van het **[!UICONTROL Logs]** menu volgen.

U kunt nu beginnen de impact van uw bericht te meten met ingebouwde rapporten. [Meer informatie](../reporting/push-report.md)
