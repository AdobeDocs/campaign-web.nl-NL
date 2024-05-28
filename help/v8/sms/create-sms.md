---
audience: end-user
title: Een sms-levering maken
description: Meer informatie over het maken en verzenden van SMS met Adobe Campaign Web
exl-id: 54181498-8164-4600-8b3f-20892b77d5d7
source-git-commit: 35de060a73c17b304d63000656ff86bb4a80ab15
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 5%

---

# Een sms-levering maken {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Eigenschappen van SMS-berichten"
>abstract="De eigenschappen omvatten de gemeenschappelijke leveringsparameters die u in zowel het noemen als het classificeren van uw levering helpen. Als uw levering op een uitgebreid schema gebaseerd is, zijn de specifieke de optiesgebieden van de Douane beschikbaar."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Het SMS-publiek definiëren"
>abstract="U kunt een nieuw publiek maken of een bestaand publiek selecteren door op de knop **Doelgroep selecteren** knop. Voeg zo nodig een controlegroep toe om het effect van de levering te meten."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Een controlegroep instellen"

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Sjabloonselectie via SMS"
>abstract="Selecteer een vooraf gedefinieerde sjabloon om de SMS-levering te starten. Met leveringssjablonen kunt u eenvoudig aangepaste inhoud en instellingen hergebruiken in al uw campagnes en leveringen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Leveringssjablonen gebruiken"


U kunt een standalone levering van SMS tot stand brengen, of SMS in de context van een campagnewerkschema tot stand brengen. In de onderstaande stappen wordt de procedure beschreven voor een zelfstandige (one-shot) SMS-levering. Als u in de context van een campagnewerkstroom werkt, zijn de aanmaakstappen details in [deze sectie](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).


Ga als volgt te werk om een nieuwe, zelfstandige SMS-levering te maken:

1. Bladeren naar de **[!UICONTROL Deliveries]** op de linkerspoorstaaf en klik op  **[!UICONTROL Create delivery]** knop.

1. Onder de **[!UICONTROL Channel]** , kiest u SMS als het kanaal en selecteert u een sjabloon. [Meer informatie over sjablonen](../msg/delivery-template.md)

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.

   ![](assets/sms_create_1.png){zoomable="yes"}

1. Voer een **[!UICONTROL Label]** voor levering en toegang tot **[!UICONTROL Additional options]** vervolgkeuzelijst. Als uw levering op een uitgebreid schema wordt gebaseerd, specifiek **Aangepaste opties** zijn beschikbaar.

   +++Configureer de volgende instellingen op basis van uw vereisten.
   * **[!UICONTROL Internal name]**: Wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: Organiseer uw leveringen met uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: Geef een beschrijving voor de levering.
   * **[!UICONTROL Nature]**: Specificeer de aard van de levering voor classificatiedoeleinden.
+++

1. Klik op de knop **[!UICONTROL Select audience]** om een bestaand publiek als doel in te stellen of uw eigen publiek te maken. [Meer informatie over het publiek](../audience/about-recipients.md).

   ![](assets/sms_create_2.png){zoomable="yes"}

   Leer hoe u een bestaand publiek kunt selecteren in [deze pagina](../audience/add-audience.md)

   Leer hoe u een nieuw publiek kunt maken in [deze pagina](../audience/one-time-audience.md)

1. Schakel de **[!UICONTROL Enable control group]** om een controlegroep in te stellen om het effect van uw levering te meten. De berichten worden niet verzonden naar die controlegroep, zodat u het gedrag van de bevolking kunt vergelijken die het bericht met het gedrag van contacten ontving die niet. [Meer informatie](../audience/control-group.md)

1. Klikken **[!UICONTROL Edit content]** om de inhoud van je SMS-bericht te ontwerpen. [Meer informatie](content-sms.md)

   ![](assets/sms_create_4.png){zoomable="yes"}

   Vanuit dit scherm kunt u ook [simuleren, inhoud](../preview-test/preview-test.md) en [aanbiedingen instellen](../msg/offers.md).

1. Als u de levering wilt plannen op een bepaalde datum en tijd, schakelt u de optie **[!UICONTROL Enable scheduling]** -optie. Nadat u de levering in werking stelt, zal het bericht automatisch op de nauwkeurige datum en de tijd worden verzonden die u voor de ontvanger hebt bepaald. Meer informatie over de planning van de levering in [deze sectie](../msg/gs-deliveries.md#gs-schedule).

   >[!NOTE]
   >
   >Wanneer een levering in de context van een werkschema wordt verzonden, moet u gebruiken **Planner** activiteit. Meer informatie vindt u [op deze pagina](../workflows/activities/scheduler.md).

1. Klikken **[!UICONTROL Settings]** voor toegang tot geavanceerde opties met betrekking tot uw leveringsmalplaatje. [Meer informatie](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png){zoomable="yes"}
