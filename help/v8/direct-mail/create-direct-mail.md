---
audience: end-user
title: Een levering voor direct mail maken
description: Meer informatie over het maken van een directe-maillevering via Adobe Campaign Web
exl-id: 9b5172b2-1880-4768-a33b-8a20ec5a30ab
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 5%

---

# Een levering voor direct mail maken {#create-direct-mail}

U kunt een standalone directe postlevering tot stand brengen, of een directe postlevering in de context van een campagnewerkschema tot stand brengen. In de onderstaande stappen wordt de procedure beschreven voor een zelfstandige (one-shot) direct-maillevering. Als u in de context van een campagnewerkstroom werkt, worden de aanmaakstappen beschreven in [deze sectie](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Voer de volgende stappen uit om een nieuwe, zelfstandige levering via e-mail te maken:

1. Bladeren naar de **[!UICONTROL Deliveries]** op de linkerspoorstaaf en klik op  **[!UICONTROL Create delivery]** knop.

1. Onder de **[!UICONTROL Channel]** sectie, kiest u **[!UICONTROL Direct mail]** als het kanaal en selecteer een sjabloon. [Meer informatie over sjablonen](../msg/delivery-template.md)

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.

   ![](assets/dm-create.png){zoomable="yes"}

1. Voer een **[!UICONTROL Label]** voor levering en toegang tot **[!UICONTROL Additional options]** vervolgkeuzelijst. Als uw levering op een uitgebreid schema wordt gebaseerd, specifiek **Aangepaste opties** zijn beschikbaar.

   ![](assets/dm-properties.png){zoomable="yes"}

   +++Configureer de volgende instellingen op basis van uw vereisten.
   * **[!UICONTROL Internal name]**: Wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: Organiseer uw leveringen met uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: Geef een beschrijving voor de levering.
   * **[!UICONTROL Nature]**: Specificeer de aard van de levering voor classificatiedoeleinden.
+++

1. Klik op de knop **[!UICONTROL Select audience]** om een bestaand publiek als doel in te stellen of uw eigen publiek te maken.

   * [Leer hoe u een bestaand publiek kunt selecteren](../audience/add-audience.md)
   * [Leer hoe u een nieuw publiek kunt maken](../audience/one-time-audience.md)

   ![](assets/dm-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >Ontvangers van direct mail moeten ten minste hun naam en postadres bevatten. Een adres wordt als volledig beschouwd als de naam, het gebied van de code van ZIP/Postal, en stad/stad gebieden niet leeg zijn. Ontvangers met onvolledige adressen worden uitgesloten van directe mailleveringen.

1. Schakel de **[!UICONTROL Enable control group]** om een controlegroep in te stellen om het effect van uw levering te meten. De berichten worden niet verzonden naar die controlegroep, zodat u het gedrag van de bevolking kunt vergelijken die het bericht met het gedrag van contacten ontving die niet. [Leer hoe u met besturingsgroepen werkt](../audience/control-group.md)

1. Klikken **[!UICONTROL Edit content]** om de informatie (kolommen) te definiëren die naar het extractiebestand moet worden geëxporteerd. [Meer informatie](content-direct-mail.md)

   ![](assets/dm-content.png){zoomable="yes"}

1. Als u de levering wilt plannen op een bepaalde datum en tijd, schakelt u de optie **[!UICONTROL Enable scheduling]** -optie. Nadat u de levering hebt gestart, wordt het extractiebestand automatisch gegenereerd op de exacte datum en tijd die u hebt gedefinieerd. [Leer hoe u leveringen kunt plannen](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Wanneer een levering in de context van een werkschema wordt verzonden, moet u gebruiken **Planner** activiteit. Meer informatie vindt u [op deze pagina](../workflows/activities/scheduler.md).

1. Klikken **[!UICONTROL Settings]** voor toegang tot geavanceerde opties met betrekking tot uw leveringsmalplaatje. [Meer informatie](../advanced-settings/delivery-settings.md)

   ![](assets/dm-settings.png){zoomable="yes"}

1. Klik op de knop **[!UICONTROL Review and send]** om uw levering te valideren en te verzenden en het extractiebestand te genereren. [Leer hoe u een directe verzending per e-mail kunt voorvertonen en verzenden](send-direct-mail.md)
