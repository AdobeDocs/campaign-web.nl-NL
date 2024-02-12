---
audience: end-user
title: Filterlijsten
description: Leer hoe u Adobe Campaign Web-lijsten filtert met ingebouwde en aangepaste filters.
exl-id: 41c3c4c3-5991-4223-ad02-e2531d76fdda
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Filterlijsten {#filter-lists}

Adobe Campaign Web verstrekt filters binnen elke lijst van voorwerpen, toelatend u om informatie te filtreren die op specifieke contextuele criteria wordt gebaseerd. U kunt leveringen bijvoorbeeld filteren op de status, het kanaal, de contactdatum of de map. U kunt tests ook verbergen.

## Filters toepassen{#apply}

Als u filters wilt toepassen op een lijst, klikt u op de knop **[!UICONTROL Show filters]** in de linkerbovenhoek van de lijst, naast de zoekbalk.

Het venster Filters wordt geopend en hierin worden de beschikbare filters voor de geselecteerde lijst weergegeven. U kunt bijvoorbeeld campagnes filteren op hun status, begin- en einddatum of opslagmap, terwijl de lijst met abonnementenservices kan worden gefilterd op hun kanaal en opslagmap.

![](assets/filters-pane.png){zoomable=&quot;yes&quot;}{width="70%" align="left" zoomable="yes"}

Als u een lijst wilt filteren op basis van uw eigen criteria, maakt u een aangepast filter. Blader hiertoe naar de onderzijde van het venster Filters en klik op de knop **Regels toevoegen** knop. [Leer hoe u aangepaste filters kunt maken](#custom)

Wanneer filters op een lijst zijn toegepast, zijn ze zichtbaar onder de zoekbalk. U kunt een afzonderlijk filter op elk gewenst moment verwijderen of alle filters verwijderen door op het pictogram **Alles wissen** knop.

## Aangepaste filters maken {#custom}

Met aangepaste filters kunt u lijsten verfijnen op basis van uw eigen specifieke criteria. Zij worden ontworpen gebruikend de de vraagmodeler van de Campagne. Ga als volgt te werk om een aangepast filter te maken:

1. Open het venster Filters en klik op de knop **Regels toevoegen** onder aan het deelvenster.
1. De vraagmodeler opent. Definieer en combineer uw filtercriteria aan uw wensen. Gedetailleerde informatie over hoe te om vraagmodeler te gebruiken is beschikbaar in [deze sectie](../query/query-modeler-overview.md).

   In het onderstaande voorbeeld ziet u een aangepast filter dat is ontworpen om te worden weergegeven in de lijst met campagnes die worden uitgevoerd door exploitanten van de afdelingen Running of Yoga.

   ![](assets/filters-sample.png){zoomable=&quot;yes&quot;}{width="70%" align="left" zoomable="yes"}

1. Als uw aangepaste filter is geconfigureerd, klikt u op **[!UICONTROL Confirm]** om deze toe te passen op de lijst.
