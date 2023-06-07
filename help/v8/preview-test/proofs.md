---
audience: end-user
title: Test-e-mails verzenden
description: Leer teste-mails definiëren en verzenden
exl-id: b2677579-c95d-443d-b207-466af364c208
badge: label="Alpha" type="Positief"
source-git-commit: c6ebdf23c22cb197a816684108c782aa2180dc1e
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 1%

---

# Test-e-mails verzenden {#send-test-emails}

**[!UICONTROL Adobe Campaign]** Hiermee kunt u een bericht testen voordat u het naar het hoofdpubliek stuurt.

Het verzenden van e-mails over tests is een belangrijke stap in het valideren van uw e-mailcampagne en het identificeren van mogelijke problemen.

De ontvangers van een test kunnen verschillende elementen controleren, zoals verbindingen, opt-out verbindingen, beelden, en spiegel pagina&#39;s, evenals om het even welke fouten in het teruggeven, inhoud, verpersoonlijkingsmontages en e-mailconfiguratie ontdekken.

## Selecteer de testontvangers {#test-recipients}

U kunt teste-mails verzenden naar twee typen ontvangers:

* **Testprofielen** - teste-mails sturen naar zaadadressen, die aanvullende en fictieve ontvangers in de database zijn. Ze kunnen worden gemaakt in de [!DNL Campaign] in de **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** map. [Meer informatie](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/creating-seed-addresses.html){target="_blank"}

* **Vervangen van hoofddoel** - stuur teste-mails naar een specifiek e-mailadres terwijl u een bestaand profiel imiteert. Zo kunt u het e-mailbericht net zo ervaren als de ontvangers, zodat u het bericht dat het profiel ontvangt, op de juiste wijze kunt weergeven.

Volg onderstaande stappen om de ontvangers van de e-mailtest te selecteren.

1. Toegang tot de e-mail [Inhoud bewerken](../content/edit-content.md) of de [E-mailontwerper](../content/get-started-email-designer.md)klikt u op de knop **[!UICONTROL Simulate content]** knop.

1. Klik op de knop **[!UICONTROL Test]**.

   ![](assets/simulate-test-button.png)

1. Gebruik de **[!UICONTROL Mode]** vervolgkeuzelijst om het type ontvangers te kiezen die de teste-mail ontvangen:

   * **Testprofielen** om fictieve ontvangers te richten

   * **Vervangen van hoofddoel** om een test naar een specifiek e-mailadres te verzenden terwijl de gegevens van een bestaand profiel worden weergegeven.

   ![](assets/simulate-profile-mode.png)

   >[!NOTE]
   >
   >Standaard worden de **[!UICONTROL Use test profiles]** is geselecteerd. Als u al profielen hebt geselecteerd om een voorvertoning van de e-mail weer te geven in het scherm voor het simuleren van de inhoud, worden deze profielen vooraf geselecteerd als testontvangers. U kunt uw selectie wissen en/of extra ontvangers toevoegen.

1. Kies de optie **[!UICONTROL Substitute from target]** en voert u de volgende stappen uit:

   1. Klik op de knop **[!UICONTROL Add address]** en geeft u het e-mailadres op dat de teste-mail ontvangt.

      U kunt elk e-mailadres invoeren. Op deze manier kunt u teste-mails sturen naar gebruikers, zelfs als zij geen gebruikers zijn van [!DNL Adobe Campaign].

   1. Selecteer het profiel in het doel dat u als vervanging wilt gebruiken. U kunt ook [!DNL Adobe Campaign] Selecteer een willekeurig profiel in het doel. De profielgegevens van het geselecteerde profiel worden weergegeven in de test-e-mail.

   1. Bevestig de ontvanger en herhaal de bewerking om zoveel adressen toe te voegen als nodig is.

      ![](assets/simulate-profile-substitute.png)

1. Nadat de testontvangers zijn geselecteerd, kunt u [de test-e-mail verzenden](#send-test).

   >[!NOTE]
   >
   >Als u het laatste e-mailbericht ook naar de ontvangers van de teste-mail wilt verzenden, selecteert u de optie **[!UICONTROL Include test population in the main target]** optie.

## De test-e-mail verzenden {#send-test}

Voer de onderstaande stappen uit om het testbericht naar de geselecteerde ontvangers te verzenden.

1. Klik op **[!UICONTROL Send test email]**.

1. Bevestig de verzendende.

   ![](assets/simulate-send-test.png)

1. U kunt zoveel teste-mails verzenden als u nodig hebt, totdat u de inhoud van uw levering hebt voltooid.

Zodra dit wordt gedaan, kunt u [e-mail voorbereiden en verzenden](../monitor/prepare-send.md) tot het hoofddoel.

## E-mails over verzonden testberichten openen {#access-proofs}

Zodra de teste-mails zijn verzonden, hebt u toegang tot toegewezen logbestanden via de **[!UICONTROL View test email log]** knop.

Met deze logboeken hebt u toegang tot alle teste-mails die voor de geselecteerde levering zijn verzonden en kunt u specifieke statistieken over het verzenden van deze mails visualiseren. [Leer hoe u leveringslogboeken kunt controleren](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png)

U kunt ook e-mails over een test openen via het [leveringslijst](../msg/gs-messages.md), zoals elke levering.

![](assets/simulate-deliveries-list.png)
