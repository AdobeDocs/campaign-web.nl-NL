---
audience: end-user
title: Aan de slag met campagnes
description: Leer hoe u begint met kanaalcampagnes
badge: label="Beperkte beschikbaarheid"
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
source-git-commit: 80e9937fcac0f1e66c317d3d31efab0d5f6ae2d8
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 1%

---

# Toegang tot en beheer uw campagnes{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Campagne"
>abstract="Plaats of wijzig uw campagneprogramma."

Als u uw campagnes wilt openen en beheren, klikt u op **[!UICONTROL Campaigns]** op de linkernavigatie.

## Lijst met campagnes {#access-campaigns}

In de lijst met campagnes zijn twee tabbladen beschikbaar:

* De **Bladeren** worden alle bestaande campagnes weergegeven. U kunt op een campagne klikken om het dashboard te openen of een nieuwe campagne te maken door op de knop **Campagne maken** knop. Zie dit [sectie](create-campaigns.md#create-campaigns).

* De **Sjablonen** worden alle beschikbare campagnemalplaatjes vermeld. U kunt een bestaande sjabloon weergeven of een nieuwe sjabloon maken. [Meer informatie](#manage-campaign-templates).

![Lijst met campagnes](assets/campaign-list.png)

Standaard geeft elke campagne in de lijst informatie weer over de huidige status, de begin- en einddatum, de aanmaakdatum, de laatste keer dat deze is gewijzigd, enzovoort.

U kunt de weergegeven kolommen aanpassen door op de knop **Kolom voor een aangepaste indeling configureren** in de rechterbovenhoek van de lijst. Op deze manier kunt u kolommen toevoegen of verwijderen en gegevens opnieuw ordenen in de campagnemelijst.

Bovendien zijn er een zoekbalk en filters beschikbaar waarmee u gemakkelijk in de lijst kunt zoeken. [Meer informatie](../get-started/user-interface.md#list-screens).

U kunt bijvoorbeeld filteren op uw campagneprogramma. Open het filterdeelvenster en gebruik de knop **Begin - Einddatum** sectie:

![Campagne, filter](assets/campaign-filter-on-dates.png)

## Campagne-dashboard {#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Lijst van leveringen in de campagne"
>abstract="De **Leveringen** worden alle leveringen weergegeven die aan de huidige campagne zijn gekoppeld. Klik op de naam van een levering om deze te bewerken. Met de knop Levering maken kunt u een nieuwe levering voor deze campagne toevoegen."

In de **Bladeren** klikt u op de naam van een campagne om de details weer te geven.

![Campagne-dashboard](assets/campaign-dashboard.png)

De status en het schema van de campagne worden boven aan het scherm weergegeven. U kunt de **Instellingen** om de eigenschappen van uw campagne bij te werken, zoals het label, de map en de beschrijving ervan. U kunt het programma van uw campagne van het montagescherm ook veranderen. Meer informatie over het campagnereschema vindt u in [deze sectie](create-campaigns.md#campaign-schedule).

Gebruik vanuit het campagnemdashboard de **Logboeken** en **Rapporten** knoppen om uw campagne te controleren. Meer informatie in deze [sectie](create-campaigns.md#create-campaigns)

Voor elke campagne ziet u op het dashboard twee tabbladen: Workflows en Deliveries.

* De **Workflows** worden alle workflows weergegeven die aan de campagne zijn gekoppeld. Op dit tabblad kunt u ook een nieuwe workflow in de campagne maken. Zie dit [sectie](create-campaigns.md#create-campaigns).

* De **Leveringen** bevat alle leveringen die in de huidige campagne zijn gemaakt. U kunt ook een nieuwe levering maken in de campagne. Zie dit [sectie](create-campaigns.md#create-campaigns).

>[!NOTE]
>
>De **Leveringen** worden alle leveringen weergegeven die aan de campagne zijn gekoppeld. Leveringen die in een workflow zijn gemaakt, kunnen daar echter niet van worden verwijderd. Als u een levering wilt verwijderen die in de context van een workflow is gemaakt, moet u de leveringsactiviteit uit de workflow verwijderen. [Meer informatie](../msg/gs-messages.md#delivery-delete).


## Een campagne verwijderen {#campaign-delete}

U kunt een campagne op twee manieren verwijderen:

* in de lijst met campagnes klikt u op de knop voor ovaal en selecteert u **Verwijderen**

  ![Een campagne verwijderen uit de lijst met campagnes](assets/delete-a-campaign-from-list.png)

* Klik in de campagne zelf op de knop **Meer** dan selecteert u **Verwijderen**

  ![Een campagne verwijderen van het campagnedashboard](assets/delete-a-campaign-from-dashboard.png)


## Een campagne dupliceren {#campaign-duplicate}

U kunt een campagne op twee manieren dupliceren:

* in de lijst met campagnes klikt u op de knop voor ovaal en selecteert u **Dupliceren**

* Klik in de campagne zelf op de knop **Meer** dan selecteert u **Dupliceren**

In beide gevallen moet u de duplicatie van de nieuwe campagne bevestigen. Het etiket van de campagne **Kopie van`<label of the initial campaign`**. Blader naar de instellingen voor de campagne om dit label bij te werken.


## Werken met campagneresjablonen{#manage-campaign-templates}

Campagnemasjablonen bevatten vooraf geconfigureerde instellingen die opnieuw kunnen worden gebruikt voor het maken van nieuwe campagnes. Er is een set ingebouwde sjablonen beschikbaar om u te helpen aan de slag te gaan. U kunt uw campagnemalplaatjes tot stand brengen en vormen en dan campagnes van deze malplaatjes tot stand brengen.

Een campagnemalplaatje kan de volgende informatie opslaan:

* de campagne **Instellingen**
* de campagne  **Schema**
* werkstroomsjablonen
* leveringssjablonen

Volg onderstaande stappen om een campagnemalplaatje te maken:

1. Klik op de knop **[!UICONTROL Campaigns]** , bladert u naar de **Sjablonen** en klikt u op de knop **[!UICONTROL Create template]** knop.
1. Selecteer de **Sjabloon** te gebruiken. Zo kunt u uw nieuwe sjabloon baseren op een eerder gemaakte sjabloon.
1. Geef een label voor de sjabloon op.
1. Indien nodig kunt u het volgende wijzigen **Aanvullende opties**: interne naam, map, ontvanger, beschrijving en aard.
1. Definieer de **Schema** van uw campagne. Meer informatie over het instellen van uw campagneschema in [deze sectie](create-campaigns.md#campaign-schedule)
1. Klikken **Maken**.
1. Workflows en leveringssjablonen toevoegen aan uw campagne.
