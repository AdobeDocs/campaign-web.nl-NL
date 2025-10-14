---
audience: end-user
title: Een voorbeeld bekijken en een direct mailbericht verzenden
description: Leer hoe u een voorbeeld kunt bekijken van een levering via e-mail via Adobe Campaign Web
exl-id: 06ce7535-e84d-4aed-bea9-b85b4ee0d008
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 1%

---

# Een voorbeeld bekijken en een direct mailbericht verzenden {#send-direct-mail}

Als u het extractiebestand hebt geconfigureerd voor directe verzending via e-mail, gebruikt u testprofielen om een voorvertoning weer te geven. Als gepersonaliseerde inhoud wordt opgenomen, onderzoek hoe deze inhoud in de kolommen gebruikend de gegevens van het testprofiel verschijnt. Hierdoor wordt ervoor gezorgd dat de bestandsinhoud correct wordt gerenderd en dat aangepaste elementen worden opgenomen.

Als het extractiebestand gereed is, verzendt u de directe-maillevering om het bestand te genereren en deelt u het met uw directe-mailprovider. [&#x200B; Leer hoe te om uw directe postlevering te verzenden &#x200B;](#dm-send)

## Een voorbeeld van het extractiebestand bekijken {#preview-dm}

De belangrijkste stappen voor een voorvertoning van het extractiebestand zijn als volgt. Meer details op hoe te voorproef zijn de leveringen beschikbaar in [&#x200B; deze sectie &#x200B;](../preview-test/preview-content.md).

1. Gebruik **[!UICONTROL Simulate content]** om een voorvertoning van uw gepersonaliseerde inhoud weer te geven vanaf de pagina met de inhoud van de levering.

   ![&#x200B; Schermafbeelding die de simulatie inhoudsoptie in de pagina van de leveringsinhoud tonen &#x200B;](assets/dm-simulate.png){zoomable="yes"}

1. Klik op **[!UICONTROL Add test profile(s)]** om een of meerdere profielen te selecteren en een voorvertoning van de gegevens weer te geven in de inhoud van het extractiebestand.

1. In het rechterdeelvenster bekijkt u een voorvertoning van het extractiebestand, waarin gepersonaliseerde elementen dynamisch worden vervangen door gegevens uit het geselecteerde profiel.

   ![&#x200B; Schermschot die de voorproef van het extractiedossier in de juiste ruit tonen &#x200B;](assets/dm-preview-right.png){zoomable="yes"}

## Proefdrukken verzenden {#test-dm}

Gebruikend **Adobe Campaign**, verzend proef alvorens hen aan uw belangrijkste publiek te leveren. Deze stap valideert uw levering en identificeert om het even welke kwesties. De ontvangers van de test herzien elementen zoals verpersoonlijkingsmontages, die optimale prestaties verzekeren en fouten ontdekken. Met dit proces wordt het extractiebestand verfijnd en geoptimaliseerd voordat u het grote publiek bereikt.

Voor direct-mailleveringen wordt bij het verzenden van proefdrukken een voorbeeld van het extractiebestand gegenereerd op basis van gegevens uit de geselecteerde testprofielen. Ga als volgt te werk om het bestand te openen:

1. Klik in het scherm Inhoud simuleren op de knop **[!UICONTROL Send proof]** en voer dezelfde stappen uit als voor elk type levering om een proefdruk te verzenden. [&#x200B; Leer hoe te om proefdrukken &#x200B;](../preview-test/test-deliveries.md) te verzenden

1. Zodra de proefdruk is verzonden, opent u deze via de knop **[!UICONTROL View proofs]** of vanuit de lijst met leveringen. [&#x200B; Leer hoe te om tot verzonden proeven toegang te hebben &#x200B;](../preview-test/test-deliveries.md#access-test-deliveries)

1. Klik in het dashboard voor de proefdruklevering op de knop **[!UICONTROL Preview file]** om een voorvertoning van het extractiebestand te openen.

   ![&#x200B; Schermschot die de optie van het voorproefdossier in het dashboard van de proeflevering tonen &#x200B;](assets/dm-proof.png){zoomable="yes"}

   >[!NOTE]
   >
   >Alleen de eerste 100 regels worden weergegeven in het voorvertoningsbestand.

## Verzend uw direct-maillevering {#send-dm}

Zodra uw direct-mail klaar is om naar uw klanten te worden verzonden, verzend de levering om de gegevensextractie in het gespecificeerde extractiedossier te beginnen. Ga als volgt te werk om dit te doen:

1. Nadat u de inhoud van het extractiebestand hebt ontworpen, klikt u op **[!UICONTROL Review & send]** op de pagina **[!UICONTROL Delivery]** .

   ![&#x200B; Schermafbeelding die het overzicht toont en optie in de leveringspagina verzendt &#x200B;](assets/dm-review-send.png){zoomable="yes"}

1. Klik op **[!UICONTROL Prepare]** en controleer de voortgang en de beschikbare statistieken.

   Als er fouten optreden, raadpleegt u het menu **[!UICONTROL Logs]** voor meer informatie over de fout.

   ![&#x200B; Schermafbeelding die de voor- optie en logboekenmenu toont &#x200B;](assets/dm-prepare.png){zoomable="yes"}

1. Verzend de berichten door op **[!UICONTROL Send]** te klikken om door te gaan met het laatste verzendproces.

1. Bevestig de verzendactie door op **[!UICONTROL Send]** te klikken.

   Klik op de knop **[!UICONTROL Send as scheduled]** als de levering via e-mail gepland is. Leer meer over levering het plannen in [&#x200B; deze sectie &#x200B;](../msg/gs-messages.md#schedule-the-delivery-sending).

Zodra uw levering wordt verzonden, wordt het extractiedossier automatisch geproduceerd en uitgevoerd naar de plaats die in de **[!UICONTROL Routing]** externe rekening wordt gespecificeerd die in de 1&rbrace; wordt geselecteerd geavanceerde montages van het leveringsmalplaatje [&#128279;](../advanced-settings/delivery-settings.md).

Houd uw PKIs (Zeer belangrijke Indicator van Prestaties) gegevens van uw leveringspagina en gegevens van het **[!UICONTROL Logs]** menu bij.

Begin het effect van uw bericht met ingebouwde rapporten te meten. [Meer informatie](../reporting/direct-mail.md)