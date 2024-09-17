---
audience: end-user
title: Een voorbeeld bekijken en een direct mailbericht verzenden
description: Leer hoe u een voorbeeld kunt bekijken van een levering via e-mail via Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: 5cedffdc504ef82cbd3a262beb80d3c55f2831ab
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# Een voorbeeld bekijken en een direct mailbericht verzenden {#send-direct-mail}

Nadat u het extractiebestand hebt geconfigureerd voor directe verzending via e-mail, kunt u testprofielen gebruiken om een voorvertoning van het bestand weer te geven. Als u gepersonaliseerde inhoud hebt opgenomen, kunt u onderzoeken hoe deze inhoud in de kolommen wordt getoond door de gegevens van het testprofiel te gebruiken. Op deze manier kunt u ervoor zorgen dat de bestandsinhoud correct wordt gerenderd en dat de gepersonaliseerde elementen op de juiste wijze worden opgenomen.

Wanneer het extractiebestand gereed is, kunt u de directe-maillevering verzenden om het bestand te genereren en het te delen met uw directe-mailprovider. [ Leer hoe te om uw directe postlevering te verzenden ](#dm-send)

## Een voorbeeld van het extractiebestand bekijken {#preview-dm}

De belangrijkste stappen voor een voorvertoning van het extractiebestand zijn als volgt. Meer details op hoe te voorproef zijn de leveringen beschikbaar in [ deze sectie ](../preview-test/preview-content.md).

1. Gebruik **[!UICONTROL Simulate content]** om een voorvertoning van uw gepersonaliseerde inhoud weer te geven vanaf de pagina met de inhoud van de levering.

   ![](assets/dm-simulate.png){zoomable="yes"}

1. Klik op **[!UICONTROL Add test profile(s)]** om een of meerdere profielen te selecteren voor een voorvertoning van de gegevens in de inhoud van het extractiebestand.

1. In het rechterdeelvenster vindt u een voorvertoning van het extractiebestand, waarin gepersonaliseerde elementen dynamisch worden vervangen door gegevens uit het geselecteerde profiel.

   ![](assets/dm-preview-right.png){zoomable="yes"}

## Proefdrukken verzenden {#test-dm}

Gebruikend **Adobe Campaign**, hebt u de capaciteit om proeven te verzenden alvorens hen naar uw belangrijkste publiek te verzenden. Deze stap is belangrijk voor het valideren van uw levering en het identificeren van eventuele problemen. De ontvangers van de test kunnen elementen zoals verpersoonlijkingsmontages herzien, die optimale prestaties verzekeren en om het even welke fouten ontdekken. Met dit proces kunt u het extractiebestand verfijnen en optimaliseren voordat u het grote publiek bereikt.

Voor direct-mailleveringen wordt bij het verzenden van proefdrukken een voorbeeld van het extractiebestand gegenereerd op basis van gegevens uit de geselecteerde testprofielen. Ga als volgt te werk om het bestand te openen:

1. Klik in het scherm Inhoud simuleren op de knop **[!UICONTROL Send proof]** en voer dezelfde stappen uit als voor elk type levering om een proefdruk te verzenden. [ Leer hoe te om proefdrukken ](../preview-test/test-deliveries.md) te verzenden

1. Zodra de proefdruk is verzonden, kunt u deze openen via de knop **[!UICONTROL View proofs]** of vanuit de lijst met leveringen. [ Leer hoe te om tot verzonden proeven toegang te hebben ](../preview-test/test-deliveries.md#access-test-deliveries)

1. Klik in het dashboard voor de proefaflevering op de knop **[!UICONTROL Preview file]** om een voorbeeld van het extractiebestand te openen.

   ![](assets/dm-proof.png){zoomable="yes"}

   >[!NOTE]
   >
   >Alleen de eerste 100 regels worden weergegeven in het voorvertoningsbestand.

## Verzend uw direct-maillevering {#send-dm}

Zodra u direct-mail klaar is om naar uw klanten te worden verzonden, kunt u de levering verzenden om de gegevensextractie in het gespecificeerde extractiedossier te beginnen. Ga als volgt te werk om dit te doen:

1. Nadat u de inhoud van het extractiebestand hebt ontworpen, klikt u op **[!UICONTROL Review & send]** op de pagina **[!UICONTROL Delivery]** .

   ![](assets/dm-review-send.png){zoomable="yes"}

1. Klik op **[!UICONTROL Prepare]** en controleer de voortgang en de beschikbare statistieken.

   Als er fouten optreden, raadpleegt u het menu **[!UICONTROL Logs]** voor meer informatie over de fout.

   ![](assets/dm-prepare.png){zoomable="yes"}

1. Verzend de berichten door op **[!UICONTROL Send]** te klikken om verder te gaan met het laatste verzendproces.

1. Bevestig de verzendactie door op **[!UICONTROL Send]** te klikken.

   Klik op de knop **[!UICONTROL Send as scheduled]** als de levering via e-mail gepland is. Leer meer over levering het plannen in [ deze sectie ](../msg/gs-messages.md#schedule-the-delivery-sending).

Zodra uw levering wordt verzonden, wordt het extractiedossier automatisch geproduceerd en uitgevoerd naar de plaats die in de **[!UICONTROL Routing]** externe rekening wordt gespecificeerd die in de 1} wordt geselecteerd geavanceerde montages van het leveringsmalplaatje ](../advanced-settings/delivery-settings.md).[

U kunt uw KPIs (de Zeer belangrijke Indicator van Prestaties) gegevens van uw leveringspagina en gegevens van het **[!UICONTROL Logs]** menu volgen.

U kunt ook beginnen de impact van uw bericht te meten met ingebouwde rapporten. [Meer informatie](../reporting/direct-mail.md)
