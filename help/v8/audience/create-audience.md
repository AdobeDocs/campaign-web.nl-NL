---
audience: end-user
title: Soorten publiek maken en beheren
description: Leer hoe u publiek kunt maken en beheren in Adobe Campaign Web
badge: label="Beta"
source-git-commit: d81c143b5ba45bf02558856a250868d43679a63a
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---


# Soorten publiek maken {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Doelgroepen"
>abstract="Via dit scherm hebt u toegang tot de lijst met alle soorten publiek waarop u zich kunt richten. Klikken **Maken** nieuwe soorten publiek maken in een visueel canvas met behulp van diverse workflowactiviteiten, zoals **Splitsen** of **Uitsluiten**."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Instellingen voor publiek"
>abstract="Voer de naam van het publiek en aanvullende opties in en klik op de knop **Publiek maken** knop."

Met Campagne Web kunt u nieuwe soorten publiek maken tot een visueel workflowcanvas. U kunt workflowactiviteiten niet alleen helemaal vanaf het begin gebruiken om een eenvoudig publiek te maken, maar ook om het publiek te verfijnen. U kunt bijvoorbeeld meerdere soorten publiek combineren tot één publiek, uw publiek verrijken met externe kenmerken of een publiek opsplitsen in meerdere soorten publiek op basis van uw eigen regels.

Zodra u uw werkschema hebt gecreeerd, worden de resulterende publiek automatisch opgeslagen binnen het gegevensbestand van de Campagne naast uw bestaande degenen. Deze doelgroepen kunnen zich dan richten op campagnes of op zelfstandige leveringen.

## Uw eerste publiek maken {#create}

Voer de volgende stappen uit om een publiek te maken:

1. Ga naar de **[!UICONTROL Audiences]** en klik op de knop **[!UICONTROL Create Audience]** in de rechterbovenhoek.
1. Geef een label voor uw publiek op.
1. Breid uit **[!UICONTROL Additional options]** om geavanceerde publieksparameters te configureren.

   Standaard worden soorten publiek gemaakt in de **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** verkenner-menu. U kunt de standaardopslaglocatie wijzigen met de **[!UICONTROL Folder]** veld.

   ![](assets/audiences-settings.png)

1. Als u de publieksinstellingen hebt geconfigureerd, klikt u op de knop **[!UICONTROL Create Audience]** knop. Er wordt een werkstroomcanvas weergegeven met twee standaardactiviteiten:

   * **[!UICONTROL Build audience]**: Dit is het beginpunt van uw workflow, zodat u een publiek kunt maken en dit kunt gebruiken als basis voor uw workflow.

   * **[!UICONTROL Save audience]**: Dit is de laatste stap in uw workflow, zodat u de workflowresultaten kunt opslaan als een nieuw publiek.

1. Open de **[!UICONTROL Build audience]** activiteit en gebruik de regelbouwer om de bevolking te bepalen om in uw publiek te omvatten door gegevens te filtreren in het gegevensbestand. [Leer hoe te om een het publieksactiviteit van de Bouwstijl te vormen](../workflows/activities/build-audience.md)

1. Als u aanvullende bewerkingen wilt uitvoeren op de doelpopulatie in de workflow, voegt u zoveel activiteiten toe als nodig zijn en verbindt u deze met elkaar. Voor meer informatie over hoe vormen de werkschemaactiviteiten, naar [werkstroomdocumentatie](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanaalactiviteiten zijn niet beschikbaar voor gebruik in publieksworkflows.

   ![](assets/audience-creation-canvas.png)

1. Vorm **[!UICONTROL Save audience]** activiteit om te specificeren hoe u de bevolking wilt bewaren die stroomopwaarts in het werkschema wordt berekend. [Leer hoe u een activiteit voor het opslaan van het publiek configureert](../workflows/activities/save-audience.md)

1. Wanneer uw workflow gereed is, klikt u op **[!UICONTROL Start]** om het uit te voeren.

De workflow wordt opgeslagen in het dialoogvenster **[!UICONTROL Workflows]** en de resulterende doelgroep(en) toegankelijk zijn in de **[!UICONTROL Audiences]** lijst.

## Voorbeeld van een publiek werkstroom {#example}

In het onderstaande voorbeeld ziet u een publieksworkflow die is geconfigureerd voor vrouwelijke klanten die in New York wonen en die twee nieuwe soorten publiek maakt, afhankelijk van hun laatste aankoop (Yoga of Running tandwieltje).

![](assets/audiences-example.png)

1. De **[!UICONTROL Build audience]** de activiteit is gericht op alle vrouwelijke profielen die in New York wonen.
1. De **[!UICONTROL Enrichment]** de activiteit verrijkt het publiek met informatie van de lijst van Aankopen om te identificeren welk type van product de klanten kochten.
1. De **[!UICONTROL Split]** de activiteit verdeelt het werkschema in twee wegen die op de recentste aankoop van klanten worden gebaseerd.
1. De **[!UICONTROL Save audience]** de activiteiten aan het eind van elk pad creëren twee nieuwe soorten publiek in de database , met inbegrip van de populatie die in elk pad is berekend .

## Het publiek bewaken en beheren {#monitor}

De lijst met publiek beschikbaar voor gebruik in het Web van de Campagne is toegankelijk van **[!UICONTROL Audiences]** -menu.

![](assets/audiences-list.png)

Het publiek kan uit veelvoudige bronnen voortkomen. De **[!UICONTROL Origin]** kolommen geven aan waar een bepaald publiek is gemaakt:

* **[!UICONTROL Adobe Campaign]**: Deze soorten publiek worden gemaakt in de Adobe Campaign V8-console. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/create-audiences/create-audiences.html){target="_blank"}.

* **[!UICONTROL Adobe Experience Platform:]** Dit publiek wordt gecreeerd binnen Adobe Experience Platform en is geïntegreerd in het Web van de Campagne gebruikend de Adobe Bronnen en de integratie van Doelen. Leer hoe u deze integratie instelt in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html)

* **[!UICONTROL Adobe Campaign WebUI]**: Deze doelgroepen worden gemaakt met de workflows voor het publiek van Campagne Web. [Leer hoe u een publiek kunt maken](create-audience.md)

Voor meer informatie over een publiek opent u deze vanuit de lijst. De publiekseigenschappen worden weergegeven, samen met het aantal profielen dat is opgenomen in het publiek. U kunt het aantal gebruikers op elk gewenst moment vernieuwen met de opdracht **[!UICONTROL Calculate]** knop.

De **[!UICONTROL Data]** kunt u de profielen die deel uitmaken van het publiek, vizualiseren. U kunt deze weergave aanpassen door meer kolommen toe te voegen of geavanceerde filters te gebruiken om de weergegeven gegevens te verfijnen.

![](assets/audiences-details.png)

Om een publiek te dupliceren of te schrappen, klik **[!UICONTROL More action]** in de lijst met soorten publiek naast de naam van het publiek of in het scherm met publieksdetails.
