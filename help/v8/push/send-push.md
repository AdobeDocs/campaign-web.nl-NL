---
audience: end-user
title: Een pushmelding verzenden
description: Meer informatie over het verzenden van pushberichten via Adobe Campaign Web
badge: label="Alpha"
source-git-commit: c24b53ee17e81805f0717682202d2d4154c96c1e
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Een voorbeeld bekijken en een pushmelding verzenden {#send-push-delivery}

## Geef een voorvertoning van de pushmelding weer {#preview-push}

Nadat u de inhoud van uw bericht hebt gedefinieerd, kunt u testabonnees gebruiken om het bericht voor te vertonen en te testen. Als u gepersonaliseerde inhoud hebt opgenomen, kunt u onderzoeken hoe deze inhoud in het bericht wordt getoond door de gegevens van het testprofiel te gebruiken. Dit staat u toe om ervoor te zorgen dat het bericht correct wordt teruggegeven en dat de gepersonaliseerde elementen correct worden opgenomen.

De belangrijkste stappen voor een voorvertoning van uw SMS-levering zijn als volgt. Meer informatie over het bekijken van voorvertoningen vindt u in [deze sectie](../preview-test/preview-content.md).

1. Vanaf de pagina met inhoud voor levering gebruiken **[!UICONTROL Simulate content]** om een voorvertoning van uw persoonlijke inhoud weer te geven.

   ![](assets/push_send_1.png)

1. Klikken **[!UICONTROL Add subscribers(s)]** om een of meerdere profielen te selecteren om een voorvertoning van hun gegevens weer te geven in de inhoud van het pushbericht.


   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png)-->

1. In het rechterdeelvenster vindt u een voorvertoning van het pushbericht, waarin gepersonaliseerde elementen dynamisch worden vervangen door gegevens uit het geselecteerde profiel.

   ![](assets/push_send_7.png)

U kunt nu uw pushmelding bekijken en verzenden naar uw publiek.

## De levering van pushberichten testen {#test-push}

Gebruiken **Adobe Campaign**, kunt u pushmeldingen testen voordat u ze naar het hoofdpubliek stuurt. Deze stap is belangrijk voor het valideren van uw levering en het identificeren van eventuele problemen.
De ontvangers van de test kunnen elementen zoals verbindingen, beelden, en verpersoonlijkingsmontages herzien, die optimale prestaties verzekeren en om het even welke fouten ontdekken. Met dit proces kunt u uw pushmeldingen verfijnen en optimaliseren voordat u het grote publiek bereikt.

![](../assets/do-not-localize/book.png) Leer hoe u pushmeldingen voor tests verzendt in [deze sectie](../preview-test/proofs.md#subscribers).

![](assets/push_send_6.png)

## Verzend uw pushmelding {#send-push}

1. Nadat u de inhoud van uw pushmelding hebt aangepast, klikt u op **[!UICONTROL Review & send]** van uw **[!UICONTROL Delivery]** pagina.

   ![](assets/push_send_2.png)

1. Klikken **[!UICONTROL Prepare]**en toezicht houden op de geboekte vooruitgang en de verstrekte statistieken.

   Als er fouten optreden, raadpleegt u het menu Logs voor meer informatie over de fout.

   ![](assets/push_send_3.png)

1. De berichten verzenden door op **[!UICONTROL Send]** om door te gaan met het definitieve verzendingsproces.

1. Bevestig de verzendactie door op de knop **[!UICONTROL Send]** of **[!UICONTROL Send as scheduled]** knop.

   ![](assets/push_send_4.png)

Zodra uw levering wordt verzonden, kunt u uw KPIs (Zeer belangrijke Indicator van Prestaties) gegevens van uw leveringspagina en gegevens van volgen **[!UICONTROL Logs]** -menu.

U kunt nu de impact van uw bericht meten met ingebouwde rapporten. [Meer informatie](../reporting/push-report.md)
