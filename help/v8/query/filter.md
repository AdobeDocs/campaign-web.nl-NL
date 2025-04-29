---
audience: end-user
title: Filterlijsten
description: Leer hoe u Adobe Campaign Web-lijsten filtert met ingebouwde en aangepaste filters.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 485d8b4b715192cc5edb6442df0fa958e29d15ff
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Filterlijsten {#filter-lists}

Adobe Campaign Web verstrekt filters binnen elke lijst van voorwerpen, toelatend u om informatie te filtreren die op specifieke contextuele criteria wordt gebaseerd. U kunt leveringen bijvoorbeeld filteren op basis van hun status, kanaal, contactdatum of map. U kunt ook proefdrukken verbergen.

>[!IMPORTANT]
>
>Er is een gloednieuwe interface beschikbaar voor het Query-model. De Nieuwe regelbouwer staat u toe om uw vraag met meer gemak dankzij zijn vereenvoudigde interface te bouwen. Druk op de schakelknop in de rechterbovenhoek om naar deze ervaring over te schakelen. U kunt naar de klassieke modelleerling van de Vraag terugkeren wanneer u wilt door eenvoudig de knevel terug te duwen om de nieuwe interface onbruikbaar te maken. U kunt de zelfde principes toepassen zoals vraagmodeler in deze nieuwe interface.
>![Beeld die knevel voor de nieuwe interface van de regelbouwer tonen ](assets/query-modeler-toggle.png){zoomable="yes"}

## Filters toepassen {#apply}

Als u filters wilt toepassen op een lijst, klikt u op de knop **[!UICONTROL Show filters]** in de linkerbovenhoek van de lijst, naast de zoekbalk.

Het venster Filters wordt geopend en hierin worden de beschikbare filters voor de geselecteerde lijst weergegeven. U kunt bijvoorbeeld campagnes filteren op basis van hun status, begin- en einddatum of opslagmap, terwijl de lijst met abonnementsservices kan worden gefilterd op basis van hun kanaal- en opslagmap.

![ ruit van Filters die beschikbare filters voor lijsten tonen ](assets/filters-pane.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"}

Als u een lijst wilt filteren op basis van uw eigen criteria, maakt u een aangepast filter. Om dit te doen, doorblader aan de bodem van de filterruit en klik **voeg regels** knoop toe. [ Leer hoe te om douanefilters ](#custom) tot stand te brengen.

Wanneer filters op een lijst zijn toegepast, zijn ze zichtbaar onder de zoekbalk. U kunt een individuele filter op elk ogenblik verwijderen, of alle filters verwijderen door **te klikken ontruimen allen** knoop.

## Aangepaste filters maken {#custom}

Met aangepaste filters kunt u lijsten verfijnen op basis van uw eigen specifieke criteria. Zij worden ontworpen gebruikend de de vraagmodeler van de Campagne. Ga als volgt te werk om een aangepast filter te maken:

1. Open de filterruit, en klik **voeg regels** knoop toe die bij de bodem van de ruit wordt gevestigd.

1. De vraagmodeler opent. Definieer en combineer uw filtercriteria aan uw wensen. De gedetailleerde informatie over hoe te om de vraagmodelleur te gebruiken is beschikbaar in [ deze sectie ](../query/query-modeler-overview.md).

   In het onderstaande voorbeeld ziet u een aangepast filter dat is ontworpen om te worden weergegeven in de lijst met campagnes die worden uitgevoerd door operatoren van de afdelingen Running of Yoga.

   ![ het filtervoorbeeld van de Douane die campagnes van SMS tonen door afdeling ](assets/filters-sample.png){zoomable="yes"}{width="70%" align="left" zoomable="yes"} worden gefilterd

1. Wanneer uw aangepaste filter is geconfigureerd, klikt u op **[!UICONTROL Confirm]** om het toe te passen op de lijst.