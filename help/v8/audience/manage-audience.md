---
audience: end-user
title: Het publiek bewaken en beheren
description: Leer hoe u het publiek in Adobe Campaign Web kunt bewaken en beheren
exl-id: ce0785a0-6af5-4ea1-ace7-0ce9d3ff065f
source-git-commit: 0f83fa69847bbabbf725f95ff29ed9b09db915b6
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Het publiek bewaken en beheren {#monitor-manage}

## Wat is een publiek? {#what}

Het publiek is het belangrijkste doel van uw levering: de ontvangers die de berichten ontvangen. Het type publiek hangt van de doelafbeelding af die in het leveringsmalplaatje wordt bepaald. Meer informatie over leveringssjablonen vindt u in [deze pagina](../msg/delivery-template.md).

Om de populatie van een publiek te bepalen, kunt u:

* [Nieuw publiek maken](create-audience.md) van de **[!UICONTROL Audiences]** menu,
* [Bestaande doelgroep selecteren](add-audience.md) gemaakt als een lijst in de clientconsole of afkomstig uit Adobe Experience Platform;
* [Een nieuw publiek maken](../query/query-modeler-overview.md) met het vraagmodel door filtercriteria te definiëren en te combineren,
* [Een publiek uit een extern bestand gebruiken](file-audience.md). Deze optie is alleen beschikbaar voor zelfstandige e-mailleveringen en kan niet worden gebruikt in campagneleveringen.

Wanneer u zich richt op een publiek, kunt u ook definiëren **controlegroepen** om te voorkomen dat berichten naar een deel van uw publiek worden verzonden en om de impact van uw campagnes te meten. [Leer hoe u een controlegroep instelt](control-group.md)

>[!NOTE]
>
>Wanneer het verzenden van berichten in de context van een campagnewerkschema, wordt het publiek bepaald in een specifiek **publiek opbouwen** workflowactiviteit. In deze context kunt u geen publiek uit een bestand laden voor e-maillevering en wordt het publiek alleen gedefinieerd in deze toegewijde activiteit. Leer hoe u het publiek van uw levering kunt definiëren in een campagneworkflow in [deze sectie](../workflows/activities/build-audience.md)

## publiek monitoren {#monitor}

>[!CONTEXTUALHELP]
>id="acw_audiences_properties"
>title="Properties"
>abstract="Hier vindt u een overzicht van de publiekseigenschappen, zoals de oorsprong, opslagmap of de status. Klik op de koppeling in het dialoogvenster **Laatste workflow** om de workflow te openen die is gebruikt om het publiek te maken."

>[!CONTEXTUALHELP]
>id="acw_audiences_count"
>title="Grootte publiek"
>abstract="Hier kunt u het totale aantal profielen in het publiek vinden. Klik op de knop Berekenen om de resultaten van het publiek bij te werken en opnieuw te berekenen."

>[!CONTEXTUALHELP]
>id="acw_audiences_workflow_error_data_execution"
>title="Auditiefout"
>abstract="Poortgegevens zijn niet beschikbaar. Wacht tot de workflow is voltooid."

De lijst met publiek beschikbaar voor gebruik in het Web van de Campagne is toegankelijk van **[!UICONTROL Audiences]** -menu.

![](assets/audiences-list.png){zoomable=&quot;yes&quot;}

Het publiek kan uit veelvoudige bronnen voortkomen. De **[!UICONTROL Origin]** kolommen geven aan waar een bepaald publiek is gemaakt:

* **[!UICONTROL Adobe Campaign]**: Deze soorten publiek worden gemaakt in de Adobe Campaign V8-console. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dit publiek wordt gecreeerd binnen Adobe Experience Platform en is geïntegreerd in het Web van de Campagne gebruikend de Adobe Bronnen en de integratie van Doelen. Leer hoe u deze integratie instelt in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

  ➡️ [Deze functie in video detecteren](#video)

* **[!UICONTROL Adobe Campaign WebUI]**: Deze doelgroepen worden gemaakt met de workflows voor het publiek van Campagne Web. [Leer hoe u een publiek kunt maken](create-audience.md)

Voor meer informatie over een publiek opent u deze vanuit de lijst. De publiekseigenschappen worden weergegeven, samen met het aantal profielen dat is opgenomen in het publiek. U kunt het aantal gebruikers op elk gewenst moment vernieuwen met de opdracht **[!UICONTROL Calculate]** knop.

De **[!UICONTROL Data]** kunt u de profielen die deel uitmaken van het publiek, vizualiseren. U kunt deze weergave aanpassen door meer kolommen toe te voegen of geavanceerde filters te gebruiken om de weergegeven gegevens te verfijnen.

![](assets/audiences-details.png){zoomable=&quot;yes&quot;}

Om een publiek te dupliceren of te schrappen, klik **[!UICONTROL More action]** in de lijst met soorten publiek naast de naam van het publiek of in het scherm met publieksdetails.

## Hoe kan ik-video {#video}

Leer hoe te om een bestemming tot stand te brengen om een publiek van het Experience Platform in het gebruikersinterface van het Web van Adobe Campaign te gebruiken.

>[!VIDEO](https://video.tv.adobe.com/v/3427635?quality=12)

Gedetailleerde informatie over hoe te opstelling is de Adobe van Bronnen en Doelen integratie beschikbaar in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.
