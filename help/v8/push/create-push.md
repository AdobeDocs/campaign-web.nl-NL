---
audience: end-user
title: Een pushmelding maken
description: Leer hoe u een pushmelding maakt met Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: eb18e2cfc97c13bb0cffac0f8a5bcfa5b18ceabb
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 1%

---

# Een pushmelding maken {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Sjabloon voor pushmelding"
>abstract="Selecteer een sjabloon voor pushmeldingen om de pushlevering te starten. Met leveringssjablonen kunt u eenvoudig aangepaste inhoud en instellingen hergebruiken in al uw campagnes en leveringen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Eigenschappen van push-levering"
>abstract="Definieer de eigenschappen voor het leveren van de push. Ga het etiket van de duw in en gebruik **Extra Opties** om de interne naam, de leveringsomslag, en de code te vormen. U kunt ook een aangepaste beschrijving invoeren."

U kunt een zelfstandige levering van pushberichten maken of een pushmelding maken in de context van een campagneworkflow. In de onderstaande stappen wordt de procedure beschreven voor een zelfstandige (one-shot) pushlevering. Als u in de context van een campagnewerkschema werkt, zijn de aanmaakstappen gedetailleerd in [&#x200B; deze sectie &#x200B;](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Een pushbericht maken {#create-push-delivery}

Ga als volgt te werk om een nieuwe zelfstandige pushaanbieding te maken:

1. Blader naar het menu **[!UICONTROL Deliveries]** op de linkertrack en klik op de knop **[!UICONTROL Create delivery]** .

1. Onder de **[!UICONTROL Channel]** sectie, kies **Push bericht** als kanaal, en selecteer een malplaatje, afhankelijk van het gekozen apparaat werkende systeem: Android of iOS. [&#x200B; Leer meer over malplaatjes &#x200B;](../msg/delivery-template.md)

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.

   ![&#x200B; Screenshot die de verwezenlijking van een duw levering &#x200B;](assets/push_create_1.png){zoomable="yes"} tonen

## De leveringsinstellingen configureren {#configure-push-settings}

Configureer uw leveringsinstellingen zoals hieronder beschreven:

1. Voer een **[!UICONTROL Label]** in voor de levering. Standaard wordt het label ingesteld met het label van de geselecteerde sjabloon. Het moet worden bijgewerkt.

1. Blader naar de vervolgkeuzelijst **[!UICONTROL Additional options]** om de opties indien nodig aan te passen. Als uw levering op een uitgebreid schema gebaseerd is, zijn de specifieke **opties van de Douane** gebieden beschikbaar.

   +++Configureer de volgende instellingen op basis van uw vereisten.
   * **[!UICONTROL Internal name]**: wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: organiseer uw leveringen met behulp van uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: geef een beschrijving voor de levering.
   * **[!UICONTROL Nature]**: geef de aard van de levering op voor classificatiedoeleinden.
   +++

1. U kunt uw pushmelding configureren als een meertalige levering om berichten te verzenden op basis van de voorkeurstaal van een profiel. [Meer informatie](../msg/multilingual.md).

## Selecteer uw publiek voor pushlevering {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Het publiek voor pushmeldingen definiëren"
>abstract="Als u het publiek van uw bericht wilt definiëren, moet u eerst de app selecteren die aan de pushlevering is gekoppeld. Uw pushmelding wordt standaard naar alle abonnees van de toepassing verzonden. U kunt tot een specifiek publiek verfijnen door de **Uitgezochte publiek** knoop te klikken. Voeg zo nodig een controlegroep toe om het effect van de levering te meten."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Een controlegroep instellen"

U moet eerst de app selecteren en vervolgens het publiek voor pushmeldingen verfijnen, zoals hieronder wordt beschreven:

1. Selecteer in de sectie **[!UICONTROL Audience]** de toepassing die u voor deze levering wilt gebruiken. Uw pushmelding wordt standaard naar alle abonnees van de toepassing verzonden. U kunt een bepaald publiek verfijnen door op de knop **[!UICONTROL Select audience]** te klikken.

   ![&#x200B; Schermafbeelding die publieksenselectie voor duwlevering tonen &#x200B;](assets/push_create_2.png){zoomable="yes"}

1. Selecteer een bestaand publiek of maak uw eigen publiek om de doelpopulatie voor uw pushlevering te verfijnen. Voor het pushbericht, is de standaard [&#x200B; doelafmeting &#x200B;](../audience/about-recipients.md#targeting-dimensions) **toepassing van de Abonnee** (nms :appSubscriptionRcp), die met de lijst van ontvangers wordt verbonden.

   Leer hoe te om een bestaand publiek in [&#x200B; te selecteren deze pagina &#x200B;](../audience/add-audience.md).

   Leer hoe te om een nieuw publiek in [&#x200B; tot stand te brengen deze pagina &#x200B;](../audience/one-time-audience.md).

1. Schakel de optie **[!UICONTROL Enable control group]** in om een besturingsgroep in te stellen om de impact van de levering te meten. De berichten worden niet verzonden naar die controlegroep, zodat kunt u het gedrag van de bevolking vergelijken die het bericht met het gedrag van contacten ontving die niet. [Meer informatie](../audience/control-group.md).

## De inhoud van het pushbericht definiëren {#create-content-push}

Klik op **[!UICONTROL Edit content]** om de inhoud van uw melding te definiëren. [Meer informatie](content-push.md).

![&#x200B; Schermafbeelding die inhoud het uitgeven voor duplevering &#x200B;](assets/push_create_5.png){zoomable="yes"} tonen

Van dit scherm, kunt u ook [&#x200B; uw inhoud &#x200B;](../preview-test/preview-test.md) simuleren en [&#x200B; opstellingsaanbiedingen &#x200B;](../msg/offers.md).

## Plaats de verzending van de levering {#schedule-push}

Wanneer een levering in de context van een werkschema wordt verzonden, moet u de **Planner** activiteit gebruiken. Leer meer in [&#x200B; deze pagina &#x200B;](../workflows/activities/scheduler.md). Onderstaande stappen zijn alleen van toepassing op zelfstandige leveringen.

Voer de volgende stappen uit om een zelfstandige pushlevering naar een bepaalde datum en tijd te plannen:

1. Blader naar de sectie **[!UICONTROL Schedule]** van de leveringseigenschappen.

1. Activeer de schakeloptie **[!UICONTROL Enable scheduling]** .

1. Stel de gewenste datum en tijd in voor het verzenden.

Nadat u de levering in werking stelt, wordt het bericht automatisch verzonden op de nauwkeurige datum en de tijd die u voor de ontvanger hebt bepaald.

![&#x200B; Schermafbeelding die het plannen opties voor duplevering toont &#x200B;](assets/push_create_3.png){zoomable="yes"}

Leer meer over levering het plannen in [&#x200B; deze sectie &#x200B;](../msg/gs-deliveries.md#gs-schedule).

## Geavanceerde instellingen voor levering {#adv-push}

Klik op **[!UICONTROL Configure delivery settings]** voor toegang tot geavanceerde opties met betrekking tot de leveringssjabloon. [Meer informatie](../advanced-settings/delivery-settings.md).

![&#x200B; Schermafbeelding die geavanceerde montages voor duwlevering toont &#x200B;](assets/push_create_4.png){zoomable="yes"}