---
audience: end-user
title: Een sms-levering maken
description: Meer informatie over het maken en verzenden van SMS met Adobe Campaign Web
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 7f7063572b95df9c289e614cb217239f579ddb27
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 5%

---

# Een sms-levering maken {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Eigenschappen van SMS-berichten"
>abstract="De eigenschappen omvatten de gemeenschappelijke leveringsparameters die u helpen uw levering noemen en classificeren. Als voor de levering een uitgebreid schema wordt gebruikt, zijn specifieke velden voor aangepaste opties beschikbaar."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Het SMS-publiek definiëren"
>abstract="Creeer een nieuw publiek of selecteer bestaande door de **Uitgezochte publiek** knoop te klikken. Voeg zo nodig een controlegroep toe om het effect van de levering te meten."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=nl-NL" text="Een controlegroep instellen"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Sjabloonselectie via SMS"
>abstract="Selecteer een vooraf gedefinieerde sjabloon om de SMS-levering te starten. Met leveringssjablonen kunt u aangepaste inhoud en instellingen opnieuw gebruiken voor al uw campagnes en leveringen."
>additional-url="https://experienceleague.adobe.com/nl/docs/campaign-web/v8/start/delivery-template" text="Leveringssjablonen gebruiken"

U kunt een standalone levering van SMS tot stand brengen, of SMS in de context van een campagnewerkschema tot stand brengen. De stappen verklaren hieronder de procedure voor een standalone (one-shot) levering van SMS. Als u in de context van een campagnewerkschema werkt, worden de aanmaakstappen verklaard in [&#x200B; deze sectie &#x200B;](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

Ga als volgt te werk om een nieuwe, zelfstandige SMS-levering te maken:

1. Blader naar het menu **[!UICONTROL Deliveries]** op de linkertrack en klik op de knop **[!UICONTROL Create delivery]** .

1. Kies onder de sectie **[!UICONTROL Channel]** SMS als kanaal en selecteer een sjabloon. [&#x200B; Leer meer over malplaatjes &#x200B;](../msg/delivery-template.md)

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.

   ![&#x200B; Schermafbeelding die de Create leveringsknoop en de het kanaalselectie van SMS tonen &#x200B;](assets/sms_create_1.png){zoomable="yes"}

1. Voer een **[!UICONTROL Label]** in voor levering en open de vervolgkeuzelijst **[!UICONTROL Additional options]** . Als uw levering een uitgebreid schema gebruikt, zijn de specifieke **opties van de Douane** gebieden beschikbaar.

   +++Configureer de volgende instellingen op basis van uw vereisten.
   * **[!UICONTROL Internal name]**: wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: organiseer uw leveringen met behulp van uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: geef een beschrijving voor de levering.
   * **[!UICONTROL Nature]**: geef de aard van de levering op voor classificatiedoeleinden.
   +++

1. Klik op de knop **[!UICONTROL Select audience]** om een bestaand publiek als doel in te stellen of uw eigen publiek te maken. [&#x200B; leer meer over publiek &#x200B;](../audience/about-recipients.md).

   ![&#x200B; Schermafbeelding die de Uitgezochte publieksknoop toont &#x200B;](assets/sms_create_2.png){zoomable="yes"}

   Leer hoe te om een bestaand publiek in [&#x200B; te selecteren deze pagina &#x200B;](../audience/add-audience.md).

   Leer hoe te om een nieuw publiek in [&#x200B; tot stand te brengen deze pagina &#x200B;](../audience/one-time-audience.md).

1. Schakel de optie **[!UICONTROL Enable control group]** in om een besturingsgroep in te stellen om de impact van de levering te meten. De berichten worden niet verzonden naar die controlegroep, zodat kunt u het gedrag van de bevolking vergelijken die het bericht met het gedrag van contacten ontving die niet. [Meer informatie](../audience/control-group.md)

1. U kunt uw levering van SMS als meertalige levering vormen om berichten te verzenden die op de aangewezen taal van een profiel worden gebaseerd. [Meer informatie](../msg/multilingual.md).

1. Klik op **[!UICONTROL Edit content]** om de inhoud van uw SMS-bericht te ontwerpen. [Meer informatie](content-sms.md)

   ![&#x200B; Schermafbeelding die de Edit inhoudsknoop tonen &#x200B;](assets/sms_create_4.png){zoomable="yes"}

   Van dit scherm, kunt u ook [&#x200B; uw inhoud &#x200B;](../preview-test/preview-test.md) simuleren en [&#x200B; opstellingsaanbiedingen &#x200B;](../msg/offers.md).

1. Schakel de optie **[!UICONTROL Enable scheduling]** in om de levering naar een bepaalde datum en tijd te plannen. Nadat u de levering in werking stelt, wordt het bericht automatisch verzonden op de nauwkeurige datum en de tijd die u voor de ontvanger bepaalt. Leer meer over levering het plannen in [&#x200B; deze sectie &#x200B;](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Wanneer een levering in de context van een werkschema wordt verzonden, gebruik de **Planner** activiteit. Meer informatie vindt u [op deze pagina](../workflows/activities/scheduler.md).

1. Klik op **[!UICONTROL Settings]** voor toegang tot geavanceerde opties met betrekking tot de leveringssjabloon. [Meer informatie](../advanced-settings/delivery-settings.md)

   ![&#x200B; Schermafbeelding die de knoop van Montages toont &#x200B;](assets/sms_create_3.png){zoomable="yes"}