---
title: Werken met GenStudio for Performance Marketing in Adobe Campaign
description: Leren werken met GenStudio for Performance Marketing in Adobe Campaign
feature: Email Design
topic: Content Management, Artificial Intelligence
role: User
level: Beginner, Intermediate
exl-id: c22a44a8-e4e2-453a-9ca2-b80f7c0edc19
source-git-commit: 61e6dcf13fc6a405f5e25328bf336e863701b2fe
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Werken met GenStudio for Performance Marketing {#genstudio}

>[!CONTEXTUALHELP]
>id="ac_genstudio_button"
>title="Een sjabloon gebruiken die is gebouwd met GenStudio"
>abstract="Dankzij de naadloze integratie met Adobe GenStudio for Performance Marketing kunt u eenvoudig een GenStudio-sjabloon importeren die is verbeterd met de Adobe AI-technologie."

## Aan de slag met GenStudio {#gs-genstudio}

[&#x200B; Adobe GenStudio for Performance Marketing &#x200B;](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home){target="_blank"} is een generatieve AI-eerste toepassing die marketingteams hun eigen advertenties en e-mails laat maken om impactful, gepersonaliseerde marketing campagnes te drijven die aan uw merknormen voldoen en aan uw ondernemingsbeleid voldoet. Door gebruik te maken van Adobe AI-technologie, biedt deze technologie een uitgebreide reeks hulpmiddelen die de complexiteit van het maken en beheren van content vereenvoudigen, zodat creatieve mensen zich kunnen richten op innovatie.

>[!AVAILABILITY]
>
>Deze mogelijkheid is alleen beschikbaar voor het e-mailkanaal.

Om marketing efficiency te verbeteren en merkconsistentie te handhaven, kunt u [!DNL **GenStudio for Performance Marketing**] ervaringen met [!DNL **Adobe Campaign**] foutloos integreren. Zo kunt u de AI-kracht van [!DNL GenStudio] gebruiken om inhoud te maken, naast de geavanceerde orchestratiemogelijkheden van [!DNL Adobe Campaign] .

>[!INFO]
>
>Om verder te gaan, controleer dit [&#x200B; overzicht &#x200B;](https://business.adobe.com/products/genstudio-for-performance-marketing.html#watch-overview){target="_blank"} en a [&#x200B; demo &#x200B;](https://business.adobe.com/products/genstudio-for-performance-marketing.html#demo){target="_blank"} van [!DNL Adobe GenStudio for Performance Marketing].

## GenStudio-mogelijkheden gebruiken in Adobe Campaign {#use-genstudio}

Dankzij de [!DNL GenStudio for Performance Marketing] - en [!DNL Adobe Campaign] -integratie kunt u marketers van uw bedrijf beter laten samenwerken om processen te stroomlijnen.

Een technische markeerteken, die [!DNL Adobe Campaign] bijvoorbeeld gebruikt om e-mailcampagnes te ontwikkelen en te automatiseren, kan samenwerken met een prestatiemarkering die inhoud maakt met [!DNL GenStudio] .

Met deze integratie kunnen beide toepassingen samenwerken om on-brand-inhoud van [!DNL GenStudio] in [!DNL Adobe Campaign] eenvoudig te integreren, waardoor aantrekkelijke e-mails worden geleverd die gericht zijn op specifieke klantsegmenten en de verkoop stimuleren.

### Een HTML-sjabloon exporteren van Adobe Campaign naar GenStudio {#export-from-campaign-to-genstudio}

Eerst kunt u een [!DNL Adobe Campaign] HTML-sjabloon met instructies van uw merk exporteren naar [!DNL GenStudio for Performance Marketing] . Voer de onderstaande stappen uit.

1. Open in [!DNL Adobe Campaign] de inhoud van uw e-mail. [&#x200B; leer hoe &#x200B;](../email/create-email.md#create-content)

1. Selecteer in de Designer-mailtoepassing **[!UICONTROL Export HTML]** op de knop **[!UICONTROL More]** .

   ![](assets/genstudio-export-template.png){zoomable="yes"}

1. Upload deze geëxporteerde HTML-sjabloon naar [!DNL GenStudio for Performance Marketing] . <!--Make sure you detect the fields that the generative AI uses to insert content in order to create an actionable template.-->

   >[!NOTE]
   >
   >Leer hoe te om een malplaatje van HTML in [!DNL GenStudio] in de [&#x200B; 2&rbrace; specifieke sectie van de Gids van de Gebruiker van Adobe GenStudio for Performance Marketing te uploaden.](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/content/templates/use-templates#templates-from-ajo-and-marketo){target="_blank"}<!--GenStudio doc to be updated with Campaign-->

1. In GenStudio gebruikt u deze sjabloon om verschillende e-mailvariaties te maken met AI-herinneringen en deze op te slaan.

   >[!NOTE]
   >
   >Leer hoe te om e-mailervaringen in GenStudio te creëren specifieke [&#x200B; sectie &#x200B;](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/create/create-email-experience){target="_blank"}.

### GenStudio-ervaringen in Adobe Campaign benutten {#leverage-genstudio-experiences}

Volg onderstaande stappen om de e-mailvariaties die u zojuist hebt gemaakt door deze te importeren in [!DNL GenStudio] , te benutten.[!DNL Adobe Campaign]

1. In [!DNL Adobe Campaign], [&#x200B; creeer een e-maillevering &#x200B;](../email/create-email.md).

1. Klik op de knop **[!UICONTROL Edit content]** in het dashboard voor e-maillevering. [Meer informatie](../email/create-email.md#create-content)

1. Selecteer **[!UICONTROL Import HTML]** op de startpagina van e-mail Designer en klik op de knop **[!UICONTROL Adobe GenStudio for Performance Marketing]** .

   ![](assets/genstudio-pem-import-email.png){zoomable="yes"}

1. Blader naar de ervaringen van GenStudio om uw inhoud te gaan samenstellen. U kunt de ervaringen filteren op verschillende criteria, zoals producten, personen, merken of zelfs kleuren.

   <!--![](assets/genstudio-filter-experiences.png){zoomable="yes"}-->

1. Selecteer een ervaring en klik op **[!UICONTROL Use]** .

   ![](assets/genstudio-use-experience.png){zoomable="yes"}

1. Selecteer de map waarin u de GenStudio-ervaring wilt importeren.

   ![](assets/genstudio-choose-destination.png){zoomable="yes"}

1. De geselecteerde inhoud wordt weergegeven in de e-mailtoepassing van de Designer.

   ![](assets/genstudio-email-content.png){zoomable="yes"}

   >[!NOTE]
   >
   >De ervaringen van GenStudio [&#x200B; die van a  [!DNL Adobe Campaign]  worden gecreeerd malplaatje &#x200B;](#export-from-ajo-to-genstudio) worden direct ingevoerd in E-mailDesigner. De ervaringen van GenStudio die zonder a [!DNL Adobe Campaign] malplaatje worden gecreeerd worden ingevoerd in [&#x200B; verenigbaarheidswijze &#x200B;](../email/existing-content.md).

   Gebruik de [&#x200B; e-mailinhoud het uitgeven hulpmiddelen &#x200B;](../email/create-email-content.md) en [&#x200B; verpersoonlijkingsgebieden &#x200B;](../personalization/personalize.md) om uw e-mail uit te geven zoals gewenst. Sla uw inhoud op.

<!--Detail a use case with A/B testing to import other GenStudio variations and track how your tratments are performing.-->


<!--
## How-to video {#video}

Discover the process of exporting an email template from Adobe Campaign to GenStudio for Performance Marketing, crafting brand-compliant emails using the template in GenStudio, and importing them seamlessly back into Adobe Campaign.

>[!VIDEO](https://video.tv.adobe.com/v/3456038/?quality=12)
TO REPLACE WITH CAMPAIGN VIDEO WHEN/IF RELEASED
-->