---
audience: end-user
title: Een pushmelding maken
description: Leer hoe u een pushmelding maakt met Adobe Campaign Web
exl-id: 49a3c05c-5806-4269-a98d-915eee216f90
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 1%

---

# Een pushmelding maken {#create-push}

>[!CONTEXTUALHELP]
>id="acw_push_notification_template"
>title="Sjabloon voor pushmelding"
>abstract="Selecteer een sjabloon voor pushmeldingen om de pushlevering te starten. Met leveringssjablonen kunt u eenvoudig aangepaste inhoud en instellingen hergebruiken in al uw campagnes en leveringen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/delivery-template.html" text="Leveringssjablonen gebruiken"


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_properties"
>title="Eigenschappen van push-levering"
>abstract="Definieer de eigenschappen voor het leveren van de push. Voer het label van de drukknop in en gebruik de **Aanvullende opties** om de interne naam, de leveringsomslag en de code te vormen. U kunt ook een aangepaste beschrijving invoeren."

U kunt een zelfstandige levering van pushberichten maken of een pushmelding maken in de context van een campagneworkflow. In de onderstaande stappen wordt de procedure beschreven voor een zelfstandige (one-shot) pushlevering. Als u in de context van een campagnewerkstroom werkt, zijn de aanmaakstappen details in [deze sectie](../workflows/activities/channels.md#create-a-delivery-in-a-campaign-workflow).

## Een pushbericht maken {#create-push-delivery}

Ga als volgt te werk om een nieuwe zelfstandige pushaanbieding te maken:

1. Bladeren naar de **[!UICONTROL Deliveries]** op de linkerspoorstaaf en klik op  **[!UICONTROL Create delivery]** knop.

1. Onder de **[!UICONTROL Channel]** sectie, kiest u **Pushmelding** als het kanaal en selecteer een sjabloon, afhankelijk van het gekozen besturingssysteem voor apparaatbewerking: Android of iOS. [Meer informatie over sjablonen](../msg/delivery-template.md)

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.

   ![](assets/push_create_1.png){zoomable=&quot;yes&quot;}

## De leveringsinstellingen configureren {#configure-push-settings}

Configureer uw leveringsinstellingen zoals hieronder beschreven:

1. Voer een **[!UICONTROL Label]** voor de levering. Standaard wordt het label ingesteld met het label van de geselecteerde sjabloon. Het moet worden bijgewerkt.

1. Bladeren in het dialoogvenster **[!UICONTROL Additional options]** , indien nodig, om de opties aan te passen. Als uw levering op een uitgebreid schema wordt gebaseerd, specifiek **Aangepaste opties** zijn beschikbaar.

   +++Configureer de volgende instellingen op basis van uw vereisten.
   * **[!UICONTROL Internal name]**: Wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: Organiseer uw leveringen met uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: Geef een beschrijving voor de levering.
   * **[!UICONTROL Nature]**: Geef de aard van de e-mail op voor classificatiedoeleinden.
+++


## Selecteer uw publiek voor pushlevering {#create-audience-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_audience"
>title="Het publiek voor pushmeldingen definiëren"
>abstract="Als u het publiek van uw bericht wilt definiëren, moet u eerst de app selecteren die aan de pushlevering is gekoppeld. Uw pushmelding wordt standaard naar alle abonnees van de toepassing verzonden. U kunt een bepaald publiek verfijnen door op de knop **Doelgroep selecteren** knop. Voeg zo nodig een controlegroep toe om het effect van de levering te meten."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Een controlegroep instellen"


U moet eerst de app selecteren en vervolgens het publiek voor pushmeldingen verfijnen, zoals hieronder wordt beschreven:

1. Van de **[!UICONTROL Audience]** selecteert u de toepassing die u voor deze levering wilt gebruiken. Uw pushmelding wordt standaard naar alle abonnees van de toepassing verzonden. U kunt een bepaald publiek verfijnen door op de knop **[!UICONTROL Select audience]** knop.

   ![](assets/push_create_2.png){zoomable=&quot;yes&quot;}

1. Selecteer een bestaand publiek of maak uw eigen publiek om de doelpopulatie voor uw pushlevering te verfijnen. Voor pushmeldingen wordt de standaardwaarde [doeldimensie](../audience/about-recipients.md#targeting-dimensions) is **Abonnementstoepassing** (nms:appSubscriptionRcp), die is gekoppeld aan de tabel met ontvangers.

   Leer hoe u een bestaand publiek kunt selecteren in [deze pagina](../audience/add-audience.md)

   Leer hoe u een nieuw publiek kunt maken in [deze pagina](../audience/one-time-audience.md)

1. Schakel de **[!UICONTROL Enable control group]** om een controlegroep in te stellen om het effect van uw levering te meten. De berichten worden niet verzonden naar die controlegroep, zodat u het gedrag van de bevolking kunt vergelijken die het bericht met het gedrag van contacten ontving die niet. [Meer informatie](../audience/control-group.md)

## De inhoud van het pushbericht definiëren {#create-content-push}

Klik op **[!UICONTROL Edit content]**. [Meer informatie](content-push.md)

![](assets/push_create_5.png){zoomable=&quot;yes&quot;}

Vanuit dit scherm kunt u ook [simuleren, inhoud](../preview-test/preview-test.md) en [aanbiedingen instellen](../msg/offers.md).

## Plaats de verzending van de levering {#schedule-push}

Wanneer een levering in de context van een werkschema wordt verzonden, moet u gebruiken **Planner** activiteit. Meer informatie in [deze pagina](../workflows/activities/scheduler.md). Onderstaande stappen zijn alleen van toepassing op zelfstandige leveringen.

Voer de volgende stappen uit om een zelfstandige pushlevering naar een bepaalde datum en tijd te plannen:

1. Bladeren naar de **[!UICONTROL Schedule]** van de leveringseigenschappen.

1. Gebruik de **[!UICONTROL Enable scheduling]** schakelen om het te activeren.

1. Stel de gewenste datum en tijd in voor het verzenden.

Nadat u de levering in werking stelt, wordt het bericht automatisch verzonden op de nauwkeurige datum en de tijd die u voor de ontvanger hebt bepaald.

![](assets/push_create_3.png){zoomable=&quot;yes&quot;}

Meer informatie over de planning van de levering in [deze sectie](../msg/gs-messages.md#gs-schedule)

## Geavanceerde instellingen voor levering {#adv-push}

Klikken **[!UICONTROL Configure delivery settings]** voor toegang tot geavanceerde opties met betrekking tot uw leveringsmalplaatje. [Meer informatie](../advanced-settings/delivery-settings.md)

![](assets/push_create_4.png){zoomable=&quot;yes&quot;}
