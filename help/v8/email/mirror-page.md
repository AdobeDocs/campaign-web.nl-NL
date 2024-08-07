---
audience: end-user
title: Een koppeling toevoegen aan de spiegelpagina
description: Leer hoe u de koppeling naar de spiegel toevoegt en beheert
exl-id: 0c22357f-0465-4fdc-833e-5fda5805fe42
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Een koppeling toevoegen aan de spiegelpagina{#mirror-page}

De spiegelpagina is een online versie van uw e-mail.

Hoewel de meeste e-mailclients afbeeldingen zonder problemen renderen, kunnen bepaalde voorinstellingen om beveiligingsredenen voorkomen dat afbeeldingen worden weergegeven. Gebruikers kunnen naar de spiegelpagina van een e-mailbericht bladeren, bijvoorbeeld als ze problemen ondervinden met het renderen of als ze afbeeldingen proberen te bekijken in hun Postvak IN. Het wordt ook aanbevolen om een onlineversie aan te bieden om toegankelijkheidsredenen of om sociaal delen aan te moedigen.

De spiegelpagina die door Adobe Campaign wordt gegenereerd, bevat alle aanpassingsgegevens.

![ de steekproef van de spiegelverbinding ](assets/mirror-page-link.png){width="600" align="left"}

## Een koppeling toevoegen aan de spiegelpagina{#link-to-mirror-page}

Het invoegen van een koppeling naar de spiegelpagina is een goede gewoonte. Deze koppeling kan bijvoorbeeld &#39;Deze e-mail weergeven in uw browser&#39; of &#39;Deze online lezen&#39; zijn. Deze bevindt zich vaak in de kop- of voettekst van de e-mail.

In Adobe Campaign, kunt u een verbinding aan de spiegelpagina in de e-mailinhoud opnemen gebruikend het specifieke **verpersoonlijkingsblok**. De ingebouwde **Verbinding aan spiegelpagina** verpersoonlijkingsblok neemt de volgende code in uw e-mailinhoud op: `<%@ include view='MirrorPage' %>`.

Een koppeling toevoegen aan een spiegel in uw e-mail:

1. Selecteer een element en klik op **[!UICONTROL Insert link]** op de contextuele werkbalk.

   ![](assets/message-tracking-mirror-page.png){zoomable="yes"}

1. Selecteer het pictogram **[!UICONTROL Add personalization]** voor toegang tot het menu voor aanpassing.

   ![](assets/message-tracking-mirror-page_2.png){zoomable="yes"}

1. Selecteer **[!UICONTROL Mirror page URL]** in het menu **[!UICONTROL Fragments]** en klik op **[!UICONTROL Add]** . [ Leer hoe te om uitdrukkingsfragmenten ](../content/use-expression-fragments.md) te gebruiken

   ![](assets/message-tracking-mirror-page_3.png){zoomable="yes"}

De spiegelpagina wordt automatisch gemaakt.

>[!IMPORTANT]
>
>Koppelingen naar spiegelpagina&#39;s worden automatisch gegenereerd en kunnen niet worden bewerkt. Ze bevatten alle gecodeerde, gepersonaliseerde gegevens die nodig zijn om de oorspronkelijke e-mail te renderen. Als gevolg hiervan kan het gebruik van gepersonaliseerde kenmerken met grote waarden langdurige spiegel-pagina&#39;s-URL&#39;s genereren, waardoor de koppeling niet kan werken in webbrowsers met een maximale URL-lengte.

Wanneer de e-mail is verzonden en de ontvangers op de koppeling voor de spiegelpagina klikken, wordt de inhoud van de e-mail in hun standaardwebbrowser weergegeven.

>[!NOTE]
>
>In de proefdruk die naar de testprofielen wordt verzonden, is de verbinding aan de spiegelpagina niet actief. Deze wordt alleen geactiveerd in de laatste berichten.

Standaard is de retentieperiode voor een spiegel 60 dagen. Na die vertraging is de spiegelpagina niet meer beschikbaar.


## Pagina genereren spiegelen{#mirror-page-generation}

Standaard wordt de spiegelpagina automatisch gegenereerd door Adobe Campaign als de e-mailinhoud niet leeg is en als deze een koppeling naar de spiegelpagina bevat (ook wel de koppeling Mirror genoemd).

U kunt de generatiemodus van de spiegel voor e-mail bepalen. De opties zijn beschikbaar in de leveringseigenschappen. [Meer informatie](../advanced-settings/delivery-settings.md#mirror)
