---
audience: end-user
title: Test-e-mails verzenden
description: Leer teste-mails definiëren en verzenden
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 8438c7ab35c2423beddbb36db2fcf52f661876bf
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Test-e-mails verzenden {#send-proofs}

![](../assets/do-not-localize/badge.png)

Het verzenden van e-mails over tests is een belangrijke stap in het valideren van uw e-mailcampagne en het identificeren van mogelijke problemen. Door teste-mails te verzenden, kunt u verschillende elementen controleren, zoals koppelingen, opt-out-koppelingen, afbeeldingen en spiegelpagina&#39;s, en eventuele fouten opsporen.

U kunt teste-mails verzenden naar twee typen ontvangers:

* **Testprofielen**: teste-mails sturen naar zaadadressen, die aanvullende en fictieve ontvangers in de database zijn;
* **Vervangende profielen**: U kunt teste-mails verzenden naar een specifiek e-mailadres terwijl u een bestaand profiel imiteert. Zo kunt u het e-mailbericht net zo ervaren als de ontvangers, zodat u het bericht dat het profiel ontvangt, op de juiste wijze kunt weergeven.

## Ontvangers met proefdrukken selecteren {#recipients}

1. Open het scherm voor het maken van e-mailinhoud en klik vervolgens op **[!UICONTROL Simulate content]**.

1. Klik op de knop **[!UICONTROL Test]** en gebruikt vervolgens de knop **[!UICONTROL Mode]** vervolgkeuzelijst om het type ontvangers te kiezen dat de proefdrukken ontvangt:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Proefdrukken naar testprofielen verzenden

1. Kies de optie **[!UICONTROL Use test profiles]** in.

1. Voeg de testprofielen toe waarop de e-mails over de test worden weergegeven.

   <!--FOR BETA: You can also build an audience to select test profiles based on your own criteria using the **[!UICONTROL Add test audience]** button.-->

   ![](assets/test-profiles-audience.png)

### Proefdrukken naar vervangingsprofielen verzenden

1. Kies de optie **[!UICONTROL Substitution from target]** in.

1. Voeg het e-mailadres of de e-mailadressen toe waarop de proefdrukken worden weergegeven.

   >[!NOTE]
   >
   >U kunt elk e-mailadres opgeven. Op deze manier kunt u proefdrukken naar alle gebruikers verzenden, zelfs als zij geen gebruikers van Adobe Campaign V8 zijn.

1. Selecteer voor elk e-mailadres het profiel in het doel dat u wilt gebruiken. U kunt Adobe Campaign ook een willekeurig profiel van het doel laten selecteren.

   ![](assets/substitution.png)

Nadat de proefontvangers zijn geselecteerd, kunt u de teste-mail verzenden. [Ontdek hoe u proeven verzendt](#send)

>[!NOTE]
>
>Als u het laatste e-mailbericht naar de ontvangers van de proefdrukken wilt verzenden, schakelt u de optie **[!UICONTROL Include test population in the main target]** optie ingeschakeld.

## Proefdrukken verzenden {#send}

Als u de proefdrukken naar de geselecteerde ontvangers wilt verzenden, klikt u op **[!UICONTROL Send test email]** bevestig vervolgens de verzending.

![](assets/send-proof.png)

Verzend zoveel proefdrukken als nodig zijn tot u de inhoud van uw levering hebt voltooid. Zodra dit wordt gedaan, kunt u e-mail naar het belangrijkste doel verzenden. [Leer hoe u uw e-mail voorbereidt en verzendt](../monitor/prepare-send.md)

## Toegang verzonden proefdrukken {#access-proofs}

Zodra de proefdrukken zijn verzonden, kunt u tot specifieke logboeken van toegang hebben **[!UICONTROL View test email log]** knop. Deze logboeken staan u toe om tot alle proeven toegang te hebben die voor de geselecteerde levering worden verzonden, en om specifieke statistieken met betrekking tot hun het verzenden te visualiseren.

![](assets/proof-log.png)

U kunt ook proefdrukken vanuit de lijst met leveringen openen, net als bij elke levering.

![](assets/delivery-list.png)
