---
audience: end-user
title: Soorten publiek maken
description: Leer hoe u een publiek kunt maken op Adobe Campaign Web
exl-id: b6134c5d-9915-4a85-baca-54578a570ee4
source-git-commit: 362f657c689ce13c6c1fadc381d43e15c32d4d05
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# Soorten publiek maken {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Doelgroepen"
>abstract="Vanuit dit scherm hebt u toegang tot de lijst met alle soorten publiek die u kunt gebruiken voor workflows of zelfstandige leveringen. Klik **creëren** om een nieuw publiek in een visueel canvas tot stand te brengen.<br/><br/> verder vanaf kras om een eenvoudig publiek tot stand te brengen, kunt u hefboomwerkschemaactiviteiten ook gebruiken om uw publiek te verfijnen. U kunt bijvoorbeeld meerdere soorten publiek combineren tot één publiek, uw publiek verrijken met externe kenmerken of een publiek opsplitsen in meerdere soorten publiek op basis van uw eigen regels."

<!--
[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Audience settings"
>abstract="Enter the name of the audience and additional options, then click the **Create Audience** button."-->

Met Campagne Web kunt u nieuwe soorten publiek maken tot een visueel workflowcanvas. U kunt workflowactiviteiten niet alleen helemaal vanaf het begin gebruiken om een eenvoudig publiek te maken, maar ook om het publiek te verfijnen. U kunt bijvoorbeeld meerdere soorten publiek combineren tot één publiek, uw publiek verrijken met externe kenmerken of een publiek opsplitsen in meerdere soorten publiek op basis van uw eigen regels.

Zodra u uw werkschema hebt gecreeerd, worden de resulterende publiek automatisch opgeslagen binnen het gegevensbestand van de Campagne naast uw bestaande degenen. Deze doelgroepen kunnen dan worden gericht op workflows of op zelfstandige leveringen.

De kolommen **[!UICONTROL Origin]** geven de oorsprong van het publiek aan: **[!UICONTROL Adobe Campaign]** publiek is gemaakt met een Adobe Campaign v8-console of webgebruikersinterface, terwijl **[!UICONTROL Adobe Experience Platform:]** -publiek is gemaakt in Adobe Experience Platform en geïntegreerd in Campagne met behulp van de integratie Bronnen en doelen voor Adobe.

➡️ [ ontdekt deze eigenschap in video ](#video)

## Uw eerste publiek maken {#create}

Voer de volgende stappen uit om een publiek te maken:

1. Navigeer naar het menu **[!UICONTROL Audiences]** en klik op de knop **[!UICONTROL Create Audience]** in de rechterbovenhoek.

1. Er wordt automatisch een nieuwe workflow gemaakt, zodat u activiteiten kunt combineren om uw publiek te genereren. Standaard bevat het canvas twee hoofdactiviteiten:

   * De activiteit van de &quot;Vraag&quot; **[!UICONTROL Build audience]** is het uitgangspunt van uw werkschema, die u toestaat om een publiek tot stand te brengen en het als stichting voor uw werkschema te gebruiken.

   * De activiteit van het &quot;Nieuwe publiek&quot; **[!UICONTROL Save audience]** vertegenwoordigt de definitieve stap in uw werkschema, toelatend u om de resultaten als nieuw publiek te bewaren.

   ![](assets/create-audience-blank.png){zoomable="yes"}

   >[!IMPORTANT]
   >
   >De werkschema&#39;s van het publiek worden opgeslagen in het **Werkschema&#39;s** menu, naast uw andere werkschema&#39;s van de Campagne. Ze zijn specifiek ontworpen om een publiek te maken en kunnen worden herkend door hun verticale canvas.

1. Voor betere leesbaarheid, adviseren wij veranderend de naam van het werkschema op het gebied van het Etiket van de werkschemamontages ****. [ Leer hoe te om werkschemamontages ](../workflows/workflow-settings.md) te vormen

1. Open de **[!UICONTROL Build audience]** activiteit en gebruik vraagmodeler om de bevolking te bepalen om in uw publiek te omvatten door gegevens te filtreren in het gegevensbestand. [ leren hoe te om een het publieksactiviteit van de Bouwstijl te vormen ](../workflows/activities/build-audience.md)

1. Als u aanvullende bewerkingen wilt uitvoeren op de doelpopulatie in de workflow, voegt u zoveel activiteiten toe als nodig zijn en verbindt u deze met elkaar. Voor meer informatie over hoe vormen de werkschemaactiviteiten, verwijzen naar de [ documentatie van werkschema&#39;s ](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanaalactiviteiten zijn niet beschikbaar voor gebruik in publieksworkflows.

   ![](assets/audience-creation-canvas.png){zoomable="yes"}

1. Configureer de **[!UICONTROL Save audience]** -activiteit om op te geven hoe u de bevolking die stroomopwaarts in de workflow is berekend, wilt opslaan. [ Leer hoe te om sparen publieksactiviteit ](../workflows/activities/save-audience.md) te vormen

1. Wanneer uw werkstroom klaar is, klikt u op **[!UICONTROL Start]** om deze uit te voeren.

Het werkschema wordt bewaard in de **[!UICONTROL Workflows]** lijst, terwijl het resulterende publiek(en) in de **[!UICONTROL Audiences]** lijst met het etiket toegankelijk zijn dat in **wordt bepaald sparen publiek** activiteit. Leer hoe te om publiek in [ te controleren en te beheren deze sectie ](manage-audience.md)

U kunt dit publiek nu gebruiken als het hoofddoel van een levering. [Meer informatie](add-audience.md)

## Voorbeeld van een publiek werkstroom {#example}

In het onderstaande voorbeeld ziet u een publieksworkflow die is geconfigureerd voor vrouwelijke klanten die in New York wonen en die twee nieuwe soorten publiek maakt, afhankelijk van hun laatste aankoop (Yoga of Running tandwieltje).

![](assets/audiences-example.png){zoomable="yes"}

1. De **[!UICONTROL Build audience]** -activiteit is gericht op alle vrouwelijke profielen die in New York wonen.
1. De **[!UICONTROL Enrichment]** -activiteit verrijkt het publiek met informatie uit de tabel Aankopen om aan te geven welk type product de klanten hebben gekocht.
1. De **[!UICONTROL Split]** -activiteit verdeelt de workflow in twee paden op basis van de meest recente aankoop van klanten.
1. Met de **[!UICONTROL Save audience]** -activiteiten aan het einde van elk pad krijgt u twee nieuwe doelgroepen in de database, inclusief de populatie die in elk pad is berekend.

## Een publiek bewerken {#edit}

U kunt een publiek dat uit een werkstroom wordt geproduceerd wijzigen wanneer nodig door zijn overeenkomstige werkschema opnieuw uit te voeren. Hierdoor kunt u gemakkelijk de publieksgegevens vernieuwen of het publiek verfijnen door de query aan uw wensen aan te passen.

1. Navigeer aan het **Publiek** menu en open het publiek u wilt uitgeven.
1. In het **Overzicht** lusje, verstrekt de **Laatste werkschema** sectie een verbinding aan het werkschema wordt gebruikt om het publiek te produceren dat. Klik erop om tot het werkschema toegang te hebben.
1. Breng de gewenste veranderingen aan en klik de **knoop van het Begin** om het werkschema opnieuw uit te voeren. Na voltooiing wordt het publiek dat het resultaat is van de workflow automatisch bijgewerkt met de meest recente workflowresultaten.

Standaard wordt bij het opnieuw uitvoeren van een publieksworkflow de volledige inhoud van het publiek vervangen door nieuwe gegevens, waardoor eerdere gegevens verloren gaan.

Als u verkiest om de bestaande publieksresultaten niet te vervangen, vorm **sparen publiek** activiteiten om met uw vereisten te richten. Bijvoorbeeld, kunt u het **etiket van het Publiek** gebied veranderen om de nieuwe resultaten in een nieuw publiek op te slaan, of de nieuwe resultaten aan de bestaande publieksinhoud toe te voegen zonder vorige gegevens te wissen. [ Leer hoe te om sparen publieksactiviteit ](../workflows/activities/save-audience.md) te vormen

![](assets/edit-audience-save.png){zoomable="yes"}

## Hoe kan ik-video {#video}

Leer hoe te om publiek te bouwen en te beheren, hoe te om publiek voor een levering te selecteren, en controlegroepen te bepalen.

>[!VIDEO](https://video.tv.adobe.com/v/3425861?quality=12)
