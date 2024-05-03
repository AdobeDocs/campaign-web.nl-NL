---
audience: end-user
title: Soorten publiek maken
description: Leer hoe u een publiek kunt maken op Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 0%

---

# Soorten publiek maken {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Doelgroepen"
>abstract="Vanuit dit scherm hebt u toegang tot de lijst met alle soorten publiek die u kunt gebruiken voor workflows of zelfstandige leveringen. Klikken **Maken** om een nieuw publiek tot een visueel canvas te maken.<br/><br/>U kunt workflowactiviteiten niet alleen helemaal vanaf het begin gebruiken om een eenvoudig publiek te maken, maar ook om het publiek te verfijnen. U kunt bijvoorbeeld meerdere soorten publiek combineren tot één publiek, uw publiek verrijken met externe kenmerken of een publiek opsplitsen in meerdere soorten publiek op basis van uw eigen regels."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

Met Campagne Web kunt u nieuwe soorten publiek maken tot een visueel workflowcanvas. U kunt workflowactiviteiten niet alleen helemaal vanaf het begin gebruiken om een eenvoudig publiek te maken, maar ook om het publiek te verfijnen. U kunt bijvoorbeeld meerdere soorten publiek combineren tot één publiek, uw publiek verrijken met externe kenmerken of een publiek opsplitsen in meerdere soorten publiek op basis van uw eigen regels.

Zodra u uw werkschema hebt gecreeerd, worden de resulterende publiek automatisch opgeslagen binnen het gegevensbestand van de Campagne naast uw bestaande degenen. Deze doelgroepen kunnen dan worden gericht op workflows of op zelfstandige leveringen.

De **[!UICONTROL Origin]** kolommen geven de oorsprong van het publiek aan: **[!UICONTROL Adobe Campaign]** publiek is gemaakt met de Adobe Campaign v8-console of de Web User Interface, terwijl **[!UICONTROL Adobe Experience Platform:]** Het publiek is gecreëerd in Adobe Experience Platform en geïntegreerd in Campagne met behulp van de integratie van bronnen en doelen van de Adobe.

➡️ [Deze functie in video detecteren](#video)

## Uw eerste publiek maken {#create}

Voer de volgende stappen uit om een publiek te maken:

1. Ga naar de **[!UICONTROL Audiences]** en klik op de knop **[!UICONTROL Create Audience]** in de rechterbovenhoek.

1. Er wordt automatisch een nieuwe workflow gemaakt, zodat u activiteiten kunt combineren om uw publiek te genereren. Standaard bevat het canvas twee hoofdactiviteiten:

   * De &quot;query&quot; **[!UICONTROL Build audience]** activiteit is het uitgangspunt van uw werkschema, die u toestaat om een publiek tot stand te brengen en het als basis voor uw werkschema te gebruiken.

   * Het &quot;nieuwe publiek&quot; **[!UICONTROL Save audience]** activiteit vertegenwoordigt de definitieve stap in uw werkschema, toelatend u om de resultaten als nieuw publiek op te slaan.

   ![](assets/create-audience-blank.png){zoomable=&quot;yes&quot;}

   >[!IMPORTANT]
   >
   >De workflows van het publiek worden opgeslagen in de **Workflows** naast de andere workflows voor campagnes. Ze zijn specifiek ontworpen om een publiek te maken en kunnen worden herkend door hun verticale canvas.

1. Voor een betere leesbaarheid raden we u aan de naam van de workflow te wijzigen in de workflowinstellingen.&#39; **Label** veld. [Leer hoe u workflowinstellingen configureert](../workflows/workflow-settings.md)

1. Open de **[!UICONTROL Build audience]** activiteit en gebruik de vraagmodeler om de bevolking te bepalen om in uw publiek te omvatten door gegevens te filtreren in het gegevensbestand. [Leer hoe te om een het publieksactiviteit van de Bouwstijl te vormen](../workflows/activities/build-audience.md)

1. Als u aanvullende bewerkingen wilt uitvoeren op de doelpopulatie in de workflow, voegt u zoveel activiteiten toe als nodig zijn en verbindt u deze met elkaar. Voor meer informatie over hoe vormen de werkschemaactiviteiten, naar [werkstroomdocumentatie](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanaalactiviteiten zijn niet beschikbaar voor gebruik in publieksworkflows.

   ![](assets/audience-creation-canvas.png){zoomable=&quot;yes&quot;}

1. Vorm **[!UICONTROL Save audience]** activiteit om te specificeren hoe u de bevolking wilt bewaren die stroomopwaarts in het werkschema wordt berekend. [Leer hoe u een activiteit voor het opslaan van het publiek configureert](../workflows/activities/save-audience.md)

1. Wanneer uw workflow gereed is, klikt u op **[!UICONTROL Start]** om het uit te voeren.

De workflow wordt opgeslagen in het dialoogvenster **[!UICONTROL Workflows]** en de resulterende doelgroep(en) toegankelijk zijn in de **[!UICONTROL Audiences]** lijst met het label dat is gedefinieerd in het dialoogvenster **Adviezen opslaan** activiteit. Leer hoe u het publiek kunt controleren en beheren in [deze sectie](manage-audience.md)

U kunt dit publiek nu gebruiken als het hoofddoel van een levering. [Meer informatie](add-audience.md)

## Voorbeeld van een publiek werkstroom {#example}

In het onderstaande voorbeeld ziet u een publieksworkflow die is geconfigureerd voor vrouwelijke klanten die in New York wonen en die twee nieuwe soorten publiek maakt, afhankelijk van hun laatste aankoop (Yoga of Running tandwieltje).

![](assets/audiences-example.png){zoomable=&quot;yes&quot;}

1. De **[!UICONTROL Build audience]** de activiteit is gericht op alle vrouwelijke profielen die in New York wonen.
1. De **[!UICONTROL Enrichment]** de activiteit verrijkt het publiek met informatie van de lijst van Aankopen om te identificeren welk type van product de klanten kochten.
1. De **[!UICONTROL Split]** de activiteit verdeelt het werkschema in twee wegen die op de recentste aankoop van klanten worden gebaseerd.
1. De **[!UICONTROL Save audience]** de activiteiten aan het eind van elk pad creëren twee nieuwe soorten publiek in de database , met inbegrip van de populatie die in elk pad is berekend .

## Een publiek bewerken {#edit}

U kunt een publiek dat uit een werkstroom wordt geproduceerd wijzigen wanneer nodig door zijn overeenkomstige werkschema opnieuw uit te voeren. Hierdoor kunt u gemakkelijk de publieksgegevens vernieuwen of het publiek verfijnen door de query aan uw wensen aan te passen.

1. Ga naar de **Soorten publiek** en opent u het publiek dat u wilt bewerken.
1. In de **Overzicht** de **Laatste workflow** Deze sectie bevat een koppeling naar de workflow die wordt gebruikt om het publiek te genereren. Klik erop om tot het werkschema toegang te hebben.
1. Breng de gewenste wijzigingen aan en klik op **Start** om de workflow opnieuw uit te voeren. Na voltooiing wordt het publiek dat het resultaat is van de workflow automatisch bijgewerkt met de meest recente workflowresultaten.

Standaard wordt bij het opnieuw uitvoeren van een publieksworkflow de volledige inhoud van het publiek vervangen door nieuwe gegevens, waardoor eerdere gegevens verloren gaan.

Als u de bestaande publieksresultaten liever niet wilt vervangen, configureert u de **Adviezen opslaan** activiteiten om aan uw vereisten aan te sluiten. U kunt bijvoorbeeld de opdracht **Label publiek** om de nieuwe resultaten op te slaan in een nieuw publiek of om de nieuwe resultaten toe te voegen aan de bestaande publieksinhoud zonder eerdere gegevens te wissen. [Leer hoe u een publieksactiviteit voor opslaan configureert](../workflows/activities/save-audience.md)

![](assets/edit-audience-save.png){zoomable=&quot;yes&quot;}

## Hoe kan ik-video {#video}

Leer hoe te om publiek te bouwen en te beheren, hoe te om publiek voor een levering te selecteren, en controlegroepen te bepalen.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)
