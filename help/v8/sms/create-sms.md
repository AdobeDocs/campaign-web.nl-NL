---
audience: end-user
title: Een sms-levering maken
description: Meer informatie over het maken en verzenden van SMS met Adobe Campaign Web
badge: label="Alpha"
exl-id: 89c9da76-1e04-41cd-9636-0d3b957875b6
source-git-commit: 4f7cedc4197a983d4d13294744e30836a0263d3a
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 7%

---

# Een sms-levering maken {#create-sms}

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_properties"
>title="Eigenschappen van SMS-berichten"
>abstract="De eigenschappen omvatten de gemeenschappelijke leveringsparameters die u in zowel het noemen als het classificeren van uw levering helpen. Als uw levering op een uitgebreid schema gebaseerd is, zijn de specifieke de optiesgebieden van de Douane beschikbaar."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_audience"
>title="Het SMS-publiek definiëren"
>abstract="Selecteer het beste publiek voor uw SMS-bericht."

>[!CONTEXTUALHELP]
>id="acw_deliveries_sms_template_selection"
>title="Sjabloonselectie via SMS"
>abstract="Selecteer een vooraf gedefinieerde sjabloon om de SMS-levering te starten."

1. Van de **[!UICONTROL Deliveries]** homepage, klik **[!UICONTROL Create delivery]**.

1. Onder de **[!UICONTROL Channel]** , kiest u SMS als het kanaal en selecteert u een sjabloon. [Meer informatie over sjablonen](../msg/delivery-template.md)

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.

   ![](assets/sms_create_1.png)

1. Voer een **[!UICONTROL Label]** voor levering en toegang tot **[!UICONTROL Additional options]** vervolgkeuzelijst.

   +++Configureer de volgende instellingen op basis van uw vereisten.
   * **[!UICONTROL Internal name]**: Wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: Organiseer uw leveringen met behulp van uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: Geef een beschrijving voor de levering.
   * **[!UICONTROL Nature]**: Geef de aard van de e-mail op voor classificatiedoeleinden.
+++

1. Klik op de knop **[!UICONTROL Select audience]** om een bestaand publiek als doel in te stellen of uw eigen publiek te maken. [Meer informatie](../audience/about-audiences.md).

   ![](assets/sms_create_2.png)

1. Schakel de **[!UICONTROL Enable control]** groepoptie om een controlegroep te plaatsen om het effect van uw levering te meten toelatend u om het gedrag van de bevolking te vergelijken die het bericht met het gedrag van contacten ontving die niet. [Meer informatie](../audience/control-group.md)

1. Klikken **[!UICONTROL Edit content]** om de inhoud van je SMS-bericht te ontwerpen. [Meer informatie](content-sms.md)

   ![](assets/sms_create_4.png)

   Vanuit dit scherm kunt u ook [simuleren, inhoud](../preview-test/preview-test.md) en [aanbiedingen instellen](../content/offers.md).

1. Als u de levering wilt plannen op een bepaalde datum en tijd, schakelt u de optie **[!UICONTROL Enable scheduling]** optie. Nadat u de levering in werking stelt, zal het bericht automatisch op de nauwkeurige datum en de tijd worden verzonden die u voor de ontvanger hebt bepaald.

1. Klikken **[!UICONTROL Configure delivery settings]** voor toegang tot geavanceerde opties met betrekking tot uw leveringsmalplaatje. [Meer informatie](../advanced-settings/delivery-settings.md)

   ![](assets/sms_create_3.png)
