---
title: Aangepaste velden
description: Leer hoe u aangepaste velden configureert
exl-id: 34e7e0b7-3981-43b1-95a5-6c672adafdc9
source-git-commit: 728bc032614067bc420b80a4cac634a08f594ff8
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---

# Aangepaste velden configureren {#custom-fields}

Aangepaste velden zijn aanvullende kenmerken die via de Adobe Campaign-console aan de out-of-the-box-schema&#39;s worden toegevoegd. Leer meer in de [ Adobe Campaign v8 documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema.html) {target="_blank"}

Deze aangepaste velden worden op verschillende schermen weergegeven, bijvoorbeeld de details van een profiel of een testprofiel.

In de webgebruikersinterface kunt u geen aangepaste velden maken, maar kunt u de manier wijzigen waarop ze worden weergegeven. Wijzigingen zijn van toepassing op alle campagnegebruikers.

>[!NOTE]
>
>U moet beheerdersrechten hebben om aangepaste velden te kunnen wijzigen.

Aangepaste velden zijn beschikbaar in de volgende schema&#39;s:

* Ontvangers (nms)
* Campagnes (nms)
* Leveringen (nms)
* Zaadadressen (nms)

Voer de volgende stappen uit om aangepaste velden te configureren:

1. Onder **Beleid**, klik **Schema&#39;s**.

   ![](assets/custom-fields.png){zoomable="yes"}

1. Bepaal de plaats van het gewenste schema, bijvoorbeeld het **Ontvangers (nms)** schema.

   ![](assets/custom-fields2.png){zoomable="yes"}

1. Klik de **Meer acties** knoop en selecteer **uitgeven douanedetails**.

   ![](assets/custom-fields3.png){zoomable="yes"}

   **geeft het scherm van het douanedetail** alle douanevelden en hun type uit.

   ![](assets/custom-fields4.png){zoomable="yes"}

   In dit scherm kunt u de volgende handelingen uitvoeren:

   * Wijzig de volgorde van de verschillende velden met de pijl-omhoog en -omlaag.
   * maak het gebied verplicht: controleer het **Verplicht** vakje.
   * maak het gebied zichtbaar of verberg het: klik **Zichtbare** knoop.
   * Voeg een zichtbaarheidsvoorwaarde toe: klik **Zichtbaar als** knoop en schrijf uw xtk uitdrukking gebruikend de beschikbare xtk functies.

1. Navigeer naar het scherm waarop het aangepaste veld wordt weergegeven. In ons voorbeeld is dit het scherm met profieldetails.

   ![](assets/custom-fields5.png){zoomable="yes"}
