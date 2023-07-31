---
audience: end-user
title: Testleveringen verzenden
description: Leer hoe u testleveringen definieert en verzendt
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alfa"
source-git-commit: 31f74f1a0cb04ca08abc9f455183f7ea1cbb1cb5
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 1%

---

# Testleveringen verzenden {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Voorvertoningsmodus"
>abstract="Geef een voorvertoning van het bericht weer en test het bericht door de testpopulatie op te nemen in het hoofddoel."

**[!UICONTROL Adobe Campaign]** Hiermee kunt u een bericht testen voordat u het naar het hoofdpubliek stuurt.

Het verzenden van testleveringen (voorheen &#39;proefdrukken&#39; genoemd) is een belangrijke stap in het valideren van uw campagne en het identificeren van mogelijke problemen.

De ontvangers van een test kunnen diverse elementen controleren zoals verbindingen, opt-out verbindingen, beelden, of spiegelpagina&#39;s, evenals om het even welke fouten in het teruggeven, de inhoud, verpersoonlijkingsmontages en leveringsconfiguratie ontdekken.

## Selecteer de testontvangers {#test-recipients}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Testpopulatie"
>abstract="Selecteer een testpopulatiemodus."

Afhankelijk van het kanaal dat u gebruikt, kunnen testberichten naar drie soorten ontvangers worden verzonden:

* [Testprofielen](#test-profiles) - Verzenden **e-mails en SMS testen** aan zaadadressen, die extra ontvangers in het gegevensbestand zijn.

  Ze kunnen worden gemaakt in de [!DNL Campaign] in de **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** map. Meer informatie in [Campagne v8 (console)-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

* [Vervangen van hoofddoel](#substitution-profiles) - Verzenden **e-mails en SMS testen** naar een specifiek e-mailadres of telefoonnummer wanneer u een bestaand profiel imiteert.

  Op deze manier kunt u het bericht net zo ervaren als de ontvangers, zodat u een nauwkeurige weergave krijgt van de inhoud die het profiel zal ontvangen.

* [Abonnees](#subscribers) - Verzenden **pushmeldingen testen** aan fictieve abonnees toegevoegd aan het gegevensbestand.

  Net als testprofielen kunnen ze worden gemaakt in het dialoogvenster [!DNL Campaign] in de **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** map. Meer informatie in [Campagne v8 (console)-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

Als u de ontvangers van een testlevering wilt selecteren, volgt u de onderstaande stappen op basis van het type profielen dat u wilt gebruiken.

### Test profiles {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Doel van het bewijs"
>abstract="U kunt een tweede bestand uploaden als &#39;doel van de proefdruk&#39; als u de levering wilt testen voordat u het hoofddoel bereikt."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Profielen uploaden"
>abstract="U kunt een tweede bestand met aanvullende profielen uploaden als u de levering wilt testen met een andere set dan de set die u voor het hoofddoel hebt gebruikt."

1. Blader naar het scherm Inhoud bewerken van uw e-mail- of SMS-verzending en klik vervolgens op de knop **[!UICONTROL Simulate content]** knop.

1. Klik op de knop **[!UICONTROL Test]**.

   >[!NOTE]
   >
   >Als u al profielen hebt geselecteerd voor [voorvertoning van levering](preview-content.md), worden deze weergegeven in het linkervenster.

   ![](assets/simulate-test-button-email.png)

1. Van de **[!UICONTROL Mode]** vervolgkeuzelijst kiest u **[!UICONTROL Test profiles]** om fictieve ontvangers te richten die de test e-mail of levering van SMS zullen ontvangen.

   ![](assets/simulate-profile-mode.png)

1. Als u al profielen hebt geselecteerd voor [voorvertoning van het bericht](preview-content.md) in het scherm van de inhoudsimulatie, worden die profielen pre-geselecteerd als testontvangers. U kunt uw selectie wissen en/of extra ontvangers toevoegen met de opdracht **[!UICONTROL Add test profile(s)]** knop.

   >[!NOTE]
   >
   >Standaard worden de **[!UICONTROL Use test profiles]** is geselecteerd.

1. Om het definitieve bericht aan de ontvangers van de testlevering ook te verzenden, selecteer **[!UICONTROL Include test population in the main target]** -optie.

1. Nadat de testprofielen zijn geselecteerd, kunt u [verzendt de testlevering](#send-test).

### Vervangende profielen {#substitution-profiles}

Een test-e-mail of -SMS verzenden naar een specifiek e-mailadres of telefoonnummer terwijl gegevens uit een bestaand profiel van het deelvenster [!DNL Campaign] database, gebruik vervangende profielen.

1. Alvorens een test te verzenden, zorg ervoor u een doelpubliek voor u levering bepaalt. [Meer informatie](../audience/about-audiences.md)

1. Blader naar het scherm Inhoud bewerken van uw e-mail- of SMS-verzending en klik vervolgens op de knop **[!UICONTROL Simulate content]** knop.

1. Klik op de knop **[!UICONTROL Test]**.

   ![](assets/simulate-test-button-email.png)

1. Van de **[!UICONTROL Mode]** vervolgkeuzelijst kiest u **[!UICONTROL Substitute from main target]** om een test naar een specifiek e-mailadres of telefoonnummer te verzenden terwijl de gegevens van een bestaand profiel worden weergegeven.

   >[!CAUTION]
   >
   >Als u geen [publiek](../audience/about-audiences.md) voor uw levering, **[!UICONTROL Substitute from main target]** Deze optie wordt grijs weergegeven en u kunt geen vervangingsprofielen selecteren.

1. Klik op de knop **[!UICONTROL Add address]** en geeft u het e-mailadres of telefoonnummer op dat de testlevering ontvangt.

   ![](assets/simulate-add-substitution-address.png)

   >[!NOTE]
   >
   >U kunt elk e-mailadres of telefoonnummer invoeren. Hierdoor kunt u testleveringen naar alle ontvangers verzenden, zelfs als deze geen gebruikers van [!DNL Adobe Campaign].

1. Selecteer het profiel in het doel dat u voor de levering hebt gedefinieerd om als vervangend profiel te gebruiken. U kunt ook [!DNL Adobe Campaign] Selecteer een willekeurig profiel in het doel. De profielgegevens van het geselecteerde profiel worden in de testlevering weergegeven.

1. Bevestig de ontvanger en herhaal de bewerking om zoveel e-mailadressen of telefoonnummers toe te voegen als nodig is.

   ![](assets/simulate-profile-substitute.png)

1. Om het definitieve bericht aan de ontvangers van de testlevering ook te verzenden, selecteer **[!UICONTROL Include test population in the main target]** -optie.

1. Als de vervangende profielen zijn geselecteerd, kunt u [verzendt de testlevering](#send-test).

### Abonnees {#subscribers}

Als u werkt met pushberichten, kunnen testleveringen alleen naar abonnees worden verzonden. Volg onderstaande stappen om deze te selecteren.

1. Blader naar het scherm Inhoud bewerken van uw levering en klik vervolgens op de knop **[!UICONTROL Simulate content]** knop.

1. Klik op de knop **[!UICONTROL Test]**.

   ![](assets/simulate-test-button-push.png)

1. Als u al abonnees hebt geselecteerd op [voorvertoning van de levering](preview-content.md) in het scherm van de inhoudsimulatie, worden die profielen pre-geselecteerd als testabonnees.

   U kunt uw selectie wissen en/of extra abonnees toevoegen met behulp van de toegewezen knop.

   ![](assets/simulate-test-subscribers.png)

1. Als u het laatste pushbericht ook naar de testabonnees wilt verzenden, selecteert u de optie **[!UICONTROL Include test population in the main target]** -optie.

1. Als de abonnees zijn geselecteerd, kunt u [verzendt de testlevering](#send-test).

## De testlevering verzenden {#send-test}

Volg onderstaande stappen om de testlevering naar de geselecteerde ontvangers te verzenden.

1. Klik op de knop **[!UICONTROL Send test]**.

1. Bevestig de verzendende.

   ![](assets/simulate-send-test.png)

1. Verzend zoveel tests als nodig zijn tot u de inhoud van uw levering hebt voltooid.

Als u klaar bent, kunt u de levering voorbereiden en naar het hoofddoel verzenden. Leer hoe in de speciale secties hieronder:

* [Uw e-mail verzenden](../monitor/prepare-send.md)
* [Uw pushmelding verzenden](../push/send-push.md#send-push)
* [Verstuur je SMS-verzending](../sms/send-sms.md#send-sms)

## Toegang verzonden testleveringen {#access-proofs}

Zodra de testleveringen zijn verzonden, kunt u toegang krijgen tot toegewezen logbestanden van de **[!UICONTROL View test log]** knop.

Deze logboeken staan u toe om tot alle tests toegang te hebben die voor de geselecteerde levering worden verzonden, en om specifieke statistieken met betrekking tot hun verzending te visualiseren. [Leer hoe u leveringslogboeken kunt controleren](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

U kunt tot verzonden tests van ook toegang hebben [leveringslijst](../msg/gs-messages.md), zoals elke levering.

![](assets/simulate-deliveries-list.png)
