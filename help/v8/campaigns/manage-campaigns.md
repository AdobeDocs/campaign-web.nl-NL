---
audience: end-user
title: Aan de slag met campagnes
description: Leer hoe u begint met kanaalcampagnes
exl-id: 690229e7-73e1-4cc1-b69a-f3e5d8de58af
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 0%

---

# Toegang tot en beheer uw campagnes {#manage-campaigns}

>[!CONTEXTUALHELP]
>id="acw_campaign_schedule"
>title="Campagne"
>abstract="Plaats of wijzig uw campagneprogramma."

Als u uw campagnes wilt openen en beheren, klikt u op het menu **[!UICONTROL Campaigns]** links in de navigatie.

## Lijst met campagnes {#access-campaigns}

In de lijst met campagnes zijn twee tabbladen beschikbaar:

* Het **doorbladert** lusje maakt een lijst van alle bestaande campagnes. U kunt een campagne klikken om zijn dashboard te openen of een nieuwe campagne tot stand te brengen door **te klikken creeert campagneknoop**. Zie deze [ sectie ](create-campaigns.md#create-campaigns).

* Het **lusje van Malplaatjes** maakt een lijst van alle beschikbare campagnemalplaatjes. U kunt een bestaande sjabloon weergeven of een nieuwe sjabloon maken. [Meer informatie](#manage-campaign-templates).

![ Beschrijving: Het scherm van de campagnemijst dat de Browse en lusjes van Malplaatjes toont, samen met opties om campagnes tot stand te brengen of te bekijken ](assets/campaign-list.png)

Standaard geeft elke campagne in de lijst informatie weer over de huidige status, de begin- en einddatum, de aanmaakdatum, de laatste keer dat deze is gewijzigd, enzovoort.

U kunt de getoonde kolommen aanpassen door **te klikken vormt kolom voor een pictogram van de douanelay-out** dat in de hoger-juiste hoek van de lijst wordt gevestigd. Op deze manier kunt u kolommen toevoegen of verwijderen en gegevens opnieuw ordenen in de campagnemelijst.

Bovendien zijn er een zoekbalk en filters beschikbaar waarmee u gemakkelijk in de lijst kunt zoeken. [Meer informatie](../get-started/user-interface.md#list-screens).

U kunt bijvoorbeeld filteren op uw campagneprogramma. Open het filterpaneel en gebruik **Begin - de sectie van de Datum van het Eind**:

![ Beschrijving: Het filterpaneel dat opties toont om campagnes door begin en einddata te filtreren ](assets/campaign-filter-on-dates.png)

## Campagne-dashboard {#campaign-dashboard}

>[!CONTEXTUALHELP]
>id="acw_campaign_delivery_list"
>title="Lijst van leveringen in de campagne"
>abstract="Het **lusje van Leveringen** maakt een lijst van alle leveringen verbonden aan de huidige campagne. Klik op de naam van een levering om deze te bewerken. Met de knop Levering maken kunt u een nieuwe levering voor deze campagne toevoegen."

>[!CONTEXTUALHELP]
>id="acw_campaign_workflow_list"
>title="Workflowlijst in een campagne"
>abstract="Het **lusje van het Werkschema** maakt een lijst van al werkschema verbonden aan de huidige campagne."

In **doorbladert** lusje van de campagnemijst, klik een campagnenaam om zijn details te tonen.

![ Beschrijving: Het scherm van het campagnesdashboard dat de status, het programma, en de lusjes voor werkschema&#39;s en leveringen ](assets/campaign-dashboard.png) toont

De status en het schema van de campagne worden boven aan het scherm weergegeven. Gebruik de **knoop van Montages** om de eigenschappen van uw campagne, zoals zijn etiket, omslag, en beschrijving bij te werken. U kunt het programma van uw campagne van het montagescherm ook veranderen. Leer meer over campagneschema in [ deze sectie ](create-campaigns.md#campaign-schedule).

Van het campagnesdashboard, gebruik de **Logboeken** en **Rapporten** knopen om uw campagne te controleren. Leer meer in deze [ sectie ](create-campaigns.md#create-campaigns).

Voor elke campagne ziet u op het dashboard twee tabbladen: Workflows en Deliveries.

* Het **lusje van de Werkschema&#39;s** maakt een lijst van alle werkschema&#39;s verbonden aan de campagne. Op dit tabblad kunt u ook een nieuwe workflow in de campagne maken. Zie deze [ sectie ](create-campaigns.md#create-campaigns).

* Het **lusje van Leveringen** maakt een lijst van alle leveringen die in de huidige campagne worden gecreeerd. U kunt ook een nieuwe levering maken in de campagne. Zie deze [ sectie ](create-campaigns.md#create-campaigns).

>[!NOTE]
>
>Het **lusje van Leveringen** toont alle leveringen verbonden aan de campagne. Leveringen die in een workflow zijn gemaakt, kunnen daar echter niet van worden verwijderd. Als u een levering wilt verwijderen die in de context van een workflow is gemaakt, verwijdert u de leveringsactiviteit uit de workflow. [Meer informatie](../msg/gs-messages.md#delivery-delete).

## Een campagne verwijderen {#campaign-delete}

U kunt een campagne op twee manieren verwijderen:

* Van de lijst van campagnes, klik de elliptische knoop, dan uitgezochte **Schrapping**.

  ![ Beschrijving: Het scherm van de campagnemijst die de ellipselknoop en de optie van de Schrapping tonen ](assets/delete-a-campaign-from-list.png)

* Van de campagne zelf, klik **Meer** knoop, dan uitgezochte **Schrapping**.

  ![ Beschrijving: Het scherm van het campagnesdashboard dat de Meer knoop en de optie van de Schrapping toont ](assets/delete-a-campaign-from-dashboard.png)

## Een campagne dupliceren {#campaign-duplicate}

U kunt een campagne op twee manieren dupliceren:

* Van de lijst van campagnes, klik de elliptische knoop, dan selecteren **Dupliceert**.

* Van de campagne zelf, klik **Meer** knoop, dan selecteren **Dupliceer**.

In beide gevallen moet u de duplicatie van de nieuwe campagne bevestigen. Het etiket van de campagne is **Exemplaar van`<label of the initial campaign>`**. Blader naar de instellingen voor de campagne om dit label bij te werken.

## Werken met campagneresjablonen {#manage-campaign-templates}

Campagnemasjablonen bevatten vooraf geconfigureerde instellingen die opnieuw kunnen worden gebruikt voor het maken van nieuwe campagnes. Er is een set ingebouwde sjablonen beschikbaar om u te helpen aan de slag te gaan. U kunt uw campagnemalplaatjes tot stand brengen en vormen en dan campagnes van deze malplaatjes tot stand brengen.

Een campagnemalplaatje kan de volgende informatie opslaan:

* De campagne **Montages**
* Het campagne **Programma**
* Workflowsjablonen
* Afleveringssjablonen

Volg onderstaande stappen om een campagnemalplaatje te maken:

1. Klik het **[!UICONTROL Campaigns]** menu, doorblader aan het **lusje van Malplaatjes**, dan klik de **[!UICONTROL Create template]** knoop.
1. Selecteer het **Malplaatje** aan gebruik. Zo kunt u uw nieuwe sjabloon baseren op een eerder gemaakte sjabloon.
1. Geef een label voor de sjabloon op.
1. Indien nodig, verander de volgende **Extra opties**: interne naam, omslag, toegewezen, beschrijving, en aard.
1. Bepaal het **Programma** van uw campagne. Leer hoe te om uw campagneschema in [ te plaatsen deze sectie ](create-campaigns.md#campaign-schedule).
1. Klik **creëren**.
1. Workflows en leveringssjablonen toevoegen aan uw campagne.