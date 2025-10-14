---
audience: end-user
title: Een pushmelding verzenden
description: Meer informatie over het verzenden van pushberichten via Adobe Campaign Web
exl-id: 16b3b33b-36db-4635-8e44-707694b859db
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Een pushbericht voorvertonen en verzenden {#send-push-delivery}

## Geef een voorvertoning van de pushmelding weer {#preview-push}

Als u de inhoud van uw bericht hebt gedefinieerd, gebruikt u testabonnees om het bericht voor te vertonen en te testen. Als gepersonaliseerde inhoud wordt omvat, onderzoek hoe deze inhoud in het bericht door de gegevens van het testprofiel te gebruiken wordt getoond. Dit verzekert het bericht correct wordt teruggegeven en de gepersonaliseerde elementen geschikt worden opgenomen.

De belangrijkste stappen voor een voorvertoning van uw pushmelding zijn als volgt. Meer details op hoe te voorproef zijn de leveringen beschikbaar in [&#x200B; deze sectie &#x200B;](../preview-test/preview-content.md).

1. Gebruik **[!UICONTROL Simulate content]** om een voorvertoning van uw gepersonaliseerde inhoud weer te geven vanaf de pagina met de inhoud van de levering.

   ![&#x200B; previewing gepersonaliseerde inhoud in de pagina van de leveringsinhoud &#x200B;](assets/push_send_1.png){zoomable="yes"}

1. Klik op **[!UICONTROL Add subscribers(s)]** om een of meerdere profielen te selecteren om een voorvertoning van hun gegevens weer te geven in de inhoud van het pushbericht.

   <!--Once your test subscribers are selected, click **[!UICONTROL Select]**.
    ![](assets/push_send_5.png){zoomable="yes"}-->

1. In het rechterdeelvenster vindt u een voorvertoning van het pushbericht, waarin gepersonaliseerde elementen dynamisch worden vervangen door gegevens uit het geselecteerde profiel.

   ![&#x200B; ruit van de Voorproef die gepersonaliseerde die elementen tonen met profielgegevens worden vervangen &#x200B;](assets/push_send_7.png){zoomable="yes"}

Bekijk en verzend uw pushmelding naar uw publiek.

## De levering van pushberichten testen {#test-push}

Gebruikend **Adobe Campaign**, verzend proef alvorens hen aan uw belangrijkste publiek te leveren. Deze stap valideert uw levering en identificeert om het even welke kwesties.

Testprofielen fungeren als proefontvangers. Componenten en instellingen zoals koppelingen, afbeeldingen en personalisatie worden gecontroleerd en gevalideerd, zodat u optimale prestaties krijgt en fouten kunt opsporen. Dit proces verfijnt en optimaliseert uw pushmeldingen voordat u het grote publiek bereikt. [&#x200B; leer hoe te om proefdrukken &#x200B;](../preview-test/test-deliveries.md#subscribers) te verzenden.

![&#x200B; het Testen duw bericht levering met proefontvangers &#x200B;](assets/push_send_6.png){zoomable="yes"}

## Verzend uw pushmelding {#send-push}

1. Nadat u de inhoud van uw pushmelding hebt aangepast, klikt u op **[!UICONTROL Review & send]** op de **[!UICONTROL Delivery]** -pagina.

   ![&#x200B; Overzicht en verzend knoop op de leveringspagina &#x200B;](assets/push_send_2.png){zoomable="yes"}

1. Klik op **[!UICONTROL Prepare]** en controleer de voortgang en de beschikbare statistieken.

   Als er fouten optreden, raadpleegt u het menu Logs voor meer informatie over de fout.

   ![&#x200B; de voorbereidingsvooruitgang en statistieken van de Controle &#x200B;](assets/push_send_3.png){zoomable="yes"}

1. Verzend de berichten door op **[!UICONTROL Send]** te klikken om door te gaan met het laatste verzendproces.

1. Bevestig de verzendactie door op **[!UICONTROL Send]** te klikken.

   Klik op de knop **[!UICONTROL Send as scheduled]** als de levering aan de drukknop gepland is. Leer meer over levering het plannen in [&#x200B; deze sectie &#x200B;](../msg/gs-messages.md#schedule-the-delivery-sending).

   ![&#x200B; verzend als geplande knoop voor geplande duplevering &#x200B;](assets/push_send_4.png){zoomable="yes"}

Zodra uw levering wordt verzonden, volg uw Zeer belangrijke Gegevens van de Indicator van Prestaties (KPI) van uw leveringspagina en gegevens van het **[!UICONTROL Logs]** menu.

Begin het effect van uw bericht met ingebouwde rapporten te meten. [Meer informatie](../reporting/push-report.md).