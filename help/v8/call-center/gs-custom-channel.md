---
audience: end-user
title: Aan de slag met aangepaste kanalen
description: Leer hoe u aangepaste kanaalleveringen maakt en verzendt met Adobe Campaign Web
exl-id: b4336a0a-d845-4024-a06b-400fce1316a4
source-git-commit: f772e19fd033b007680777f75b48775b6d7851b9
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 1%

---

# Aan de slag met aangepaste kanalen {#gs-custom-channel}

U kunt, direct van het Web UI van Adobe Campaign, leveringen organiseren en uitvoeren die op douanekanalen worden gebaseerd met derden worden geïntegreerd. De configuratie van het aangepaste kanaal wordt uitgevoerd in de clientconsole.

Er worden twee typen aangepaste kanalen ondersteund, extern en API. Met externe kanalen genereert de campagne aanpasbare exportbestanden met alle benodigde contact- en personalisatiegegevens. Met API-kanalen worden berichten verzonden naar de doelprofielen via de geconfigureerde API.

U kunt aangepaste kanaalleveringen toevoegen in workflows of deze alleen gebruiken als zelfstandige leveringen.

In de onderstaande stappen wordt de procedure voor een zelfstandige (one-shot) levering in detail beschreven. De meeste stappen zijn gelijkaardig om centrumleveringen te roepen. Voor meer details, verwijs naar deze [&#x200B; pagina &#x200B;](../call-center/create-call-center.md).

Ga als volgt te werk om een nieuwe, op zichzelf staande, aangepaste levering te verzenden:

1. Vorm het douanekanaal, [&#x200B; lees meer &#x200B;](#create-channel)
1. Creeer de levering, [&#x200B; lees meer &#x200B;](#create-delivery)
1. Bepaal het publiek, [&#x200B; lees meer &#x200B;](#select-audience)
1. Bewerk de inhoud, [&#x200B; lees meer &#x200B;](#edit-content)
1. De voorproef en verzendt de levering, [&#x200B; lees meer &#x200B;](#preview-send)

## Het aangepaste kanaal configureren{#create-channel}

Eerst, moet u het douanekanaal vormen. Hier volgen de belangrijkste stappen die in de clientconsole moeten worden uitgevoerd. Deze stappen worden gebruikt voor aangepaste externe en API-kanalen:

1. Vorm het schema om het nieuwe kanaal aan de lijst van beschikbare kanalen toe te voegen. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/other-channels/custom-channel.html#configure-schema){target="_blank"}
1. Creeer een nieuwe verpletterende externe rekening. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/other-channels/custom-channel.html#create-ext-account){target="_blank"}
1. Creeer een nieuw leveringsmalplaatje verbonden aan het nieuwe kanaal. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/other-channels/custom-channel.html#create-template){target="_blank"}

Aangepaste API-kanalen vereisen een extra configuratie. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/other-channels/custom-channel.html#api-additional){target="_blank"}

## De levering maken{#create-delivery}

Voer de volgende stappen uit om de levering te maken en de eigenschappen ervan te configureren:

1. Selecteer het menu **[!UICONTROL Deliveries]** en klik op de knop **[!UICONTROL Create delivery]** .

1. Kies het gewenste aangepaste kanaal, selecteer de bijbehorende sjabloon en klik op **[!UICONTROL Create delivery]** om te bevestigen.

   ![&#x200B; Schermafbeelding die de verwezenlijking van een douanelevering tonen &#x200B;](assets/cus-create.png){zoomable="yes"}

1. Voer onder **[!UICONTROL Properties]** een **[!UICONTROL Label]** in voor de levering.

   ![&#x200B; Screenshot die de eigenschappen configuratie voor een douanelevering tonen &#x200B;](assets/cus-properties.png){zoomable="yes"}

Voor meer details bij leveringsverwezenlijking, verwijs naar het vraagcentrum [&#x200B; documentatie &#x200B;](../call-center/create-call-center.md#create-delivery).

## De doelgroep definiëren{#select-audience}

Nu moet u het doelpubliek definiëren.

1. Klik in het gedeelte **[!UICONTROL Audience]** van het dashboard voor levering op **[!UICONTROL Select audience]** .

1. Kies een bestaand publiek of maak een eigen publiek.

   ![&#x200B; Schermschot die publieksselectie voor een douanelevering tonen &#x200B;](assets/cc-audience2.png){zoomable="yes"}

Voor meer details op publieksdefinitie, verwijs naar het vraagcentrum [&#x200B; documentatie &#x200B;](../call-center/create-call-center.md#select-audience).

## De inhoud bewerken{#edit-content}

Laten we nu de inhoud van de levering bewerken.

>[!BEGINTABS]

>[!TAB  Extern kanaal van de Douane ]

1. Klik op de knop **[!UICONTROL Edit content]** in het dashboard voor levering.

1. Geef een **[!UICONTROL File name]** op, selecteer een **[!UICONTROL File format]** en voeg zoveel kolommen toe als nodig zijn voor het extractiebestand.

   ![&#x200B; Screenshot die de opties van de attributenconfiguratie voor het extractiedossier toont.](assets/cc-content-attributes.png)

>[!TAB  het kanaal van Aangepast API ]

1. Klik op de knop **[!UICONTROL Edit content]** in het dashboard voor levering.

1. Vul de velden naar wens in. Leren hoe te opstelling dit scherm, naar deze [&#x200B; pagina &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/other-channels/custom-channel.html#api-additional-screen){target="_blank"} verwijzen.

   ![&#x200B; Screenshot die de opties van de attributenconfiguratie voor het API kanaal toont.](assets/cc-content-attributes-api.png)

>[!ENDTABS]

Voor meer details op inhoudsuitgave, verwijs naar het callcenter [&#x200B; documentatie &#x200B;](../call-center/create-call-center.md#edit-content).

## De levering voorvertonen en verzenden{#preview-send}

Als de inhoud klaar is voor levering, kunt u er een voorvertoning van weergeven met testprofielen. Vervolgens kunt u de levering verzenden om het extractiebestand te genereren of het bericht via de API te verzenden.

>[!BEGINTABS]

>[!TAB  Extern kanaal van de Douane ]

1. Klik op de knop **[!UICONTROL Edit content]** in het dashboard voor levering.

1. Klik op de pagina met inhoud voor levering op de knop **[!UICONTROL Simulate content]** en selecteer testprofielen.

   ![&#x200B; Schermafbeelding die de simulatie inhoudsoptie in de pagina van de leveringsinhoud tonen &#x200B;](assets/cus-simulate.png){zoomable="yes"}

>[!TAB  het kanaal van Aangepast API ]

1. Klik op de knop **[!UICONTROL Edit content]** in het dashboard voor levering.

1. Klik op de pagina met inhoud voor levering op de knop **[!UICONTROL Simulate content]** en selecteer testprofielen.

1. Op de rechterkant, klik **Open voorproef**. Dit vermogen moet worden gevormd gebruikend JSSP. Verwijs naar deze [&#x200B; pagina &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/other-channels/custom-channel.html#api-additional-preview){target="_blank"}.

   ![&#x200B; Schermafbeelding die de simulatie inhoudsoptie in de pagina van de leveringsinhoud voor API &#x200B;](assets/cus-simulate-api.png){zoomable="yes"} tonen

>[!ENDTABS]

Klik op het bezorgdashboard op **[!UICONTROL Review & send]** en klik op **[!UICONTROL Prepare]** . Dan, bevestig. Klik op **[!UICONTROL Send]** om door te gaan met het uiteindelijke verzendproces en bevestig het vervolgens.

![&#x200B; Schermafbeelding die de voor- optie en logboekenmenu toont &#x200B;](assets/cus-prepare.png){zoomable="yes"}

Voor meer details op voorproef en verzend, verwijs naar het vraagcentrum [&#x200B; documentatie &#x200B;](../call-center/create-call-center.md#preview-send).
