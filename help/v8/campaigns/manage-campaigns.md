---
audience: end-user
title: Aan de slag met campagnes
description: Leer hoe u begint met kanaalcampagnes
badge: label="Beta"
source-git-commit: 9b945dcd4151e536e8a8be904100730c86e483b7
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 1%

---


# Toegang tot en beheer uw campagnes{#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Campagne"
>abstract="Plaats of wijzig uw campagneprogramma."

Als u een nieuwe campagne wilt maken of bestaande campagnes wilt beheren, klikt u op de knop **[!UICONTROL Campaigns]** op de linkernavigatie.

## Lijst met campagnes {#access-campaigns}


In de lijst met campagnes zijn twee tabbladen beschikbaar:

* De **Bladeren** worden alle bestaande campagnes weergegeven. U kunt op een campagne klikken om het dashboard te openen of een nieuwe campagne te maken door op de knop **Campagne maken** knop. Zie dit [sectie](create-campaigns.md#create-campaigns).

* De **Sjablonen** worden alle beschikbare campagnemalplaatjes vermeld. U kunt een bestaande sjabloon weergeven of een nieuwe sjabloon maken. [Meer informatie](manage-campaign-templates.md).

![Lijst met campagnes](assets/campaign-list.png)

Standaard geeft elke campagne in de lijst informatie weer over de huidige status, de aanmaakdatum, de laatste keer dat de campagne is gewijzigd, enzovoort.

U kunt de weergegeven kolommen aanpassen door op de knop **Kolom voor een aangepaste indeling configureren** in de rechterbovenhoek van de lijst. Op deze manier kunt u aanvullende informatie aan de lijst toevoegen. Bovendien zijn er een zoekbalk en filters beschikbaar waarmee u gemakkelijk in de lijst kunt zoeken. [Meer informatie](../get-started/user-interface.md#list-screens).

U kunt bijvoorbeeld filteren op uw campagneprogramma. Open het filterdeelvenster en gebruik de knop **Begin - Einddatum** sectie:

![Campagne, filter](assets/campaign-filter-on-dates.png)

## Campagne-dashboard{#campaign-dashboard}


>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Lijst van leveringen in de campagne"
>abstract="De **Leveringen** worden alle leveringen weergegeven die aan de huidige campagne zijn gekoppeld. Klik op de naam van een levering om deze te bewerken. Met de knop Levering maken kunt u een nieuwe levering voor deze campagne toevoegen."

In de **Bladeren** klikt u op een campagne om de details ervan weer te geven.

![Campagne-dashboard](assets/campaign-dashboard.png)

De status en het schema van de campagne worden boven aan het scherm weergegeven. U kunt de **Campagne-instellingen configureren** pictogram om de eigenschappen van de campagne te wijzigen die tijdens het maken van de campagne zijn gedefinieerd. Er zijn drie knoppen beschikbaar waarmee u logbestanden kunt weergeven, rapporteren, dupliceren of verwijderen van de campagne. Zie dit [sectie](create-campaigns.md#create-campaigns)

Er zijn twee tabbladen beschikbaar:

* De **Workflows** worden alle workflows weergegeven die aan de campagne zijn gekoppeld. Op dit tabblad kunt u ook een nieuwe workflow in de campagne maken. Zie dit [sectie](create-campaigns.md#create-campaigns).

* De **Leveringen** worden alle leveringen weergegeven die aan de huidige campagne zijn gekoppeld. U kunt ook een nieuwe levering maken in de campagne. Zie dit [sectie](create-campaigns.md#create-campaigns).

## Een campagne dupliceren en verwijderen

U kunt een campagne dupliceren of verwijderen:

* in de lijst met campagnes klikt u op de knop voor ovaal en selecteert u **Dupliceren** of **Verwijderen**.
* Klik in de campagne zelf op de knop **Meer** dan selecteert u **Dupliceren** of **Verwijderen**.

>[!NOTE]
>
>De **Leveringen** worden alle leveringen weergegeven die aan de campagne zijn gekoppeld. Leveringen die in een workflow zijn gemaakt, kunnen daar echter niet van worden verwijderd. Als u een levering wilt verwijderen die in de context van een workflow is gemaakt, moet u de leveringsactiviteit uit de workflow verwijderen. [Meer informatie](../msg/gs-messages.md#delivery-delete).

## Werken met campagneresjablonen{#manage-campaign-templates}

Campagnemasjablonen bevatten vooraf geconfigureerde instellingen die opnieuw kunnen worden gebruikt voor het maken van nieuwe workflows. Er is een set ingebouwde sjablonen beschikbaar om u te helpen aan de slag te gaan. U kunt uw campagnemalplaatjes tot stand brengen en vormen en dan campagnes van deze malplaatjes tot stand brengen.

Een campagnemalplaatje kan de volgende informatie opslaan:

* de campagne **Eigenschappen** en **Schema** instellingen
* werkstroomsjablonen
* leveringssjablonen

Volg onderstaande stappen om een campagnemalplaatje te maken:

1. Klik op de knop **[!UICONTROL Campaigns]** , bladert u naar de **Sjablonen** en klikt u op de knop **[!UICONTROL Create template]** knop.
1. Selecteer de **Sjabloon** een label voor de campagne te gebruiken en te verstrekken. Zo kunt u de nieuwe sjabloon baseren op een sjabloon die al is gemaakt.
1. Indien nodig kunt u het volgende wijzigen **Aanvullende opties**: interne naam, map, ontvanger, beschrijving en aard.
1. Definieer de **Schema** van uw campagne. Meer informatie over het instellen van uw campagneschema in [deze sectie](create-campaigns.md#campaign-schedule)
1. Klikken **Maken**.
1. Workflows en leveringssjablonen toevoegen aan uw campagne.
