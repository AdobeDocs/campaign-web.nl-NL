---
audience: end-user
title: Verzend proeven
description: Campagne v8 Webdocumentatie
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 28cada1d6b645bd6f0c365528c9302bf4b03ad65
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 2%

---

# Verzend proeven {#send-proofs}

>[!NOTE]
>
>Deze documentatie is in opbouw en wordt regelmatig bijgewerkt. De definitieve versie van deze inhoud zal in Januari 2023 klaar zijn.

Door proefdrukken te verzenden, kunt u uw e-mail valideren en verschillende elementen controleren, zoals koppelingen, opt-out-koppelingen en het spiegelen van pagina&#39;s, afbeeldingen en mogelijke fouten opsporen.

De proefdrukken kunnen naar twee soorten ontvangers worden verzonden:

* **Testprofielen/publiek**: Verzend proef naar zaadadressen, die extra ontvangers in het gegevensbestand zijn die geen deel van het e-maildoel uitmaken,

* **Vervangende profielen**: proefdrukken naar een specifiek e-mailadres verzenden met een bestaand profiel. Op deze manier kunt u uzelf in de positie van de profielen plaatsen en een exacte weergave krijgen van het bericht dat het profiel ontvangt.

## Ontvangers met proefdrukken selecteren {#recipients}

1. Open het scherm voor het maken van e-mailinhoud en klik vervolgens op **[!UICONTROL Simulate content]**.

1. Klik op de knop **[!UICONTROL Test]** en gebruikt vervolgens de knop **[!UICONTROL Mode]** vervolgkeuzelijst om het type ontvangers te kiezen dat de proefdrukken ontvangt:

<!-- to check: by default, profiles selected in previous screen are pre-selected for proofs. Can add addtitional profiles + remove preselected?-->

### Proefdrukken naar testprofielen verzenden

1. Kies de optie **[!UICONTROL Use test profiles]** in.

1. Voeg de testprofielen toe waarop de e-mails over de test worden weergegeven.

   U kunt ook een publiek maken om testprofielen te selecteren op basis van uw eigen criteria met de opdracht **[!UICONTROL Add test audience]** knop.

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

Zodra de proefdrukken zijn verzonden, kunt u tot specifieke logboeken van toegang hebben **[!UICONTROL View test email log]** knop. Met deze logboeken hebt u toegang tot de verzonden proefdrukken en tot specifieke statistieken over het verzenden van bewijzen.

![](assets/proof-log.png)

Verzend zoveel proefdrukken als nodig zijn tot u de inhoud van uw levering hebt voltooid. Zodra dit wordt gedaan, kunt u e-mail naar het belangrijkste doel verzenden. [Leer hoe u uw e-mail voorbereidt en verzendt](../monitor/prepare-send.md)
