---
audience: end-user
title: Werken met mappen
description: Leer hoe u een map beheert in Adobe Campaign
exl-id: a4518a21-03cd-46ac-9c40-d181692e1b9b
source-git-commit: ed9a3a3ca3bbb5d2bd44c512643857d62b97393c
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Werken met mappen {#folders}

>[!CONTEXTUALHELP]
>id="acw_folder_properties"
>title="Eigenschappen van map"
>abstract="Eigenschappen van map"

>[!CONTEXTUALHELP]
>id="acw_folder_security"
>title="Mapbeveiliging"
>abstract="Mapbeveiliging"

>[!CONTEXTUALHELP]
>id="acw_folder_restrictions"
>title="Mapbeperkingen"
>abstract="Mapbeperkingen"

>[!CONTEXTUALHELP]
>id="acw_folder_schedule"
>title="Mapschema"
>abstract="Mapschema"

## Mappen {#about-folders}

Mappen zijn objecten in Adobe Campaign waarmee u uw componenten en gegevens kunt ordenen.

U kunt mappen in de navigatiestructuur maken, hernoemen, opnieuw ordenen en verplaatsen. U kunt ze ook verwijderen op basis van uw rechten.

![](assets/folders.png){zoomable="yes"}

U kunt een maptype instellen. Bijvoorbeeld: een map met leveringen.
Het pictogram van de map wordt gewijzigd op basis van dit type.

## Nieuwe map maken {#create-a-folder}

Ga als volgt te werk om een nieuwe map te maken in de gebruikersinterface van Adobe Campaign:

1. Ga in **[!UICONTROL Explorer]** naar de map waarin u de nieuwe map wilt maken.
Onder het menu **[!UICONTROL ...]** hebt u **[!UICONTROL Create new folder]**

![](assets/folder_create.png){zoomable="yes"}

Wanneer u een nieuwe map maakt, is het maptype standaard het type van de bovenliggende map. In ons voorbeeld maken we een map in de map **[!UICONTROL Deliveries]** .

![](assets/folder_new.png){zoomable="yes"}

1. Wijzig het type map door indien nodig op het pictogram Maptype te klikken en kies het type map in de weergegeven lijst, zoals hieronder:

![](assets/folder_type.png){zoomable="yes"}

Stel het maptype in door op de knop **[!UICONTROL Confirm]** te klikken.

Als u een map zonder specifiek type wilt maken, kiest u **[!UICONTROL Generic Folder]** type.

U kunt ook [ omslagen in de console van Adobe Campaign ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/folders-and-views) tot stand brengen en leiden.


## Mappen opnieuw ordenen {#reorder-folders}

U kunt de mappen naar wens opnieuw ordenen. Klik hiertoe op **[!UICONTROL Reorder folders]** zoals hieronder weergegeven.

In ons voorbeeld, de omslag **levert** 4 omslagen.

![](assets/folder-reorder.png){zoomable="yes"}

U kunt de orde van uw omslagen of door **slepen en laten vallen** veranderen, of door **op en neer pijlen** te gebruiken.

![](assets/folder-draganddrop.png){zoomable="yes"}


## Een map verwijderen {#delete-a-folder}

>[!CAUTION]
>
>Wanneer u een map verwijdert, worden ook alle in de map opgeslagen gegevens verwijderd.

Als u een map wilt verwijderen, selecteert u deze in de **[!UICONTROL Explorer]** -structuur en klikt u op het menu **[!UICONTROL ...]** .
Kies **[!UICONTROL Delete folder]** .

![](assets/folder_delete.png){zoomable="yes"}

## Verdeling van waarden in een map {#distribution-values-folder}

De verdeling van waarden helpt om het percentage van een waarde in een kolom binnen een lijst te kennen.

Ga als volgt te werk om de verdeling van waarden in een map te kennen:

Bijvoorbeeld, onder de leveringen, willen wij de distributie van waarden van de **kolom van het Kanaal** kennen.

Ga naar de map **[!UICONTROL Deliveries]** en klik op het pictogram **[!UICONTROL Configure columns]** om deze informatie op te halen.

Klik in het **[!UICONTROL Configure columns]** -venster op het **[!UICONTROL Information]** -pictogram van de kolom die u wilt kennen. Klik vervolgens op de knop **[!UICONTROL Distribution of values]** .

![](assets/values_deliveries.png){zoomable="yes"}

U krijgt het percentage van de waarden in de kolom **[!UICONTROL Channel]** .

![](assets/values_percentage.png){zoomable="yes"}

>[!NOTE]
>
> Voor kolommen met veel waarden worden alleen de eerste 20 waarden weergegeven. Een melding **[!UICONTROL Partial load]** waarschuwt u.

U kunt ook de verdeling van waarden van een koppeling hebben.

Klik in de lijst met kenmerken op de knop **+** naast de gewenste koppeling, zoals hieronder wordt weergegeven. Hiermee voegt u de koppeling toe aan **[!UICONTROL Output columns]** . U kunt nu het pictogram **[!UICONTROL Information]** gebruiken, zodat u de verdeling van de waarden kunt bekijken. Als u de koppeling niet in de **[!UICONTROL Output columns]** wilt behouden, klikt u op de knop **[!UICONTROL Cancel]** .

![](assets/values_link.png){zoomable="yes"}

Het is ook mogelijk om de distributie van waarden in een vraagmodeler te hebben. [ leer hier meer ](../query/build-query.md#distribution-of-values-in-a-query).

### De waarden filteren {#filter-values}

Door **[!UICONTROL Advanced filters]** in de distributie van waardenvenster te gebruiken, kunt u uw resultaten filtreren die op gespecificeerde voorwaarden worden gebaseerd.

In het voorbeeld van de leveringslijst hierboven, die de distributie per kanaal toont, kunt u, bijvoorbeeld, het filtreren om slechts de leveringen te tonen die status **wordt gebeëindigd**.

![](assets/values_filter.png){zoomable="yes"}
