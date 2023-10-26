---
audience: end-user
title: Verzend een SMS-levering
description: Meer informatie over het verzenden van SMS via Adobe Campaign Web
badge: label="Beta"
exl-id: 901faf3b-fcdd-4a4e-8de7-7d088686250f
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Een SMS-verzending bekijken en verzenden {#send-sms-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_metrics_newquarantines"
>title="Nieuwe metrische quarantines"
>abstract="Het totale aantal adressen quarantined na een ontbroken levering (onbekend gebruiker, ongeldig domein) met betrekking tot het aantal te leveren berichten."

## Je SMS-aanbieding bekijken{#preview-sms}

Nadat u de inhoud van uw bericht hebt gedefinieerd, kunt u testprofielen gebruiken om een voorbeeld van de inhoud weer te geven en deze te testen. Als u gepersonaliseerde inhoud hebt opgenomen, kunt u onderzoeken hoe deze inhoud in het bericht wordt getoond door de gegevens van het testprofiel te gebruiken. Op deze manier kunt u ervoor zorgen dat het bericht op de gewenste manier wordt weergegeven en dat alle gepersonaliseerde gegevens correct worden weergegeven.

De belangrijkste stappen voor een voorvertoning van uw SMS-levering zijn als volgt. Meer informatie over het bekijken van voorvertoningen vindt u in [deze sectie](../preview-test/preview-content.md).

1. Vanaf de pagina met inhoud voor levering gebruiken **[!UICONTROL Simulate content]** om een voorvertoning van uw persoonlijke inhoud weer te geven.

   ![](assets/sms_send_1.png)

1. Klikken **[!UICONTROL Add test profile(s)]** om een of meerdere testprofielen of profielen te selecteren.

   <!--
    Once your test profiles are selected, click **[!UICONTROL Select]**.
    ![](assets/sms_send_2.png)
    -->

1. In het rechterdeelvenster vindt u een voorbeeld van de SMS-levering, waar gepersonaliseerde elementen dynamisch worden vervangen door gegevens uit het geselecteerde profiel.

   ![](assets/sms_send_3.png)

Je kunt je SMS-bericht nu bekijken en naar je publiek sturen.

## Je SMS-levering testen {#test-sms}

Met **Adobe Campaign**, kunt u een bericht testen voordat u het naar het hoofdpubliek stuurt. Dit is een essentiële stap voor het valideren van uw e-mailcampagne en het identificeren van mogelijke problemen.

Het verzenden van testSMS is een belangrijke stap in het verzekeren van de kwaliteit en de doeltreffendheid van uw levering. De ontvangers van de test kunnen diverse elementen zoals verbindingen, opt-out verbindingen en beelden herzien, evenals om het even welke fouten in het teruggeven, inhoud, verpersoonlijkingsmontages, en de configuratie van SMS identificeren. Dit proces helpt u uw SMS grondig evalueren en optimaliseren alvorens uw belangrijkste publiek te bereiken.

![](../assets/do-not-localize/book.png) Leer hoe je SMS-test verzendt in [deze sectie](../preview-test/test-deliveries.md).

![](assets/sms_send_6.png)

## Verstuur je SMS-verzending {#send-sms}

1. Nadat u de SMS-inhoud hebt aangepast, klikt u op **[!UICONTROL Review & send]** van uw **[!UICONTROL Delivery]** pagina.

   ![](assets/sms_send_4.png)

1. Klikken **[!UICONTROL Prepare]** en toezicht te houden op de geboekte vooruitgang en de verstrekte statistieken.

   Als er fouten optreden, raadpleegt u het menu Logs voor meer informatie over de fout.

1. Verzend de berichten door op te klikken **[!UICONTROL Send]** om door te gaan met het definitieve verzendingsproces.

   ![](assets/sms_send_5.png)

   Als de levering van SMS gepland is, klik **[!UICONTROL Send as scheduled]** knop. Meer informatie over de planning van de levering in [deze sectie](../msg/gs-messages.md#schedule-the-delivery-sending).


1. Bevestig de verzendactie door op de knop **[!UICONTROL Send]** knop.

Zodra uw levering wordt verzonden, kunt u uw KPIs (Zeer belangrijke Indicator van Prestaties) gegevens van uw leveringspagina en gegevens van volgen **[!UICONTROL Logs]** -menu.

U kunt nu beginnen de impact van uw bericht te meten met ingebouwde rapporten. [Meer informatie](../reporting/sms-report.md)
