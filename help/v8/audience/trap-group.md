---
audience: end-user
title: Een overvulgroep gebruiken
description: Leer hoe te om een valgroep voor uw levering in het gebruikersinterface van het Web van de Campagne te gebruiken
exl-id: 48c34581-8825-4798-b24e-c462303f7645
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---

# Een overvulgroep gebruiken {#trap-group}

Een **[!UICONTROL trap group]** (ook wel **[!UICONTROL Seed list]** genoemd) wordt gebruikt om specifieke adressen in uw leveringen op te nemen om het distributieproces te controleren en te verifiëren door zich te richten op profielen die niet aan de gedefinieerde doelcriteria voldoen. Op deze manier kunnen ontvangers die zich buiten het leveringsbereik bevinden, de levering ontvangen, net als elke andere doelontvanger.

Een **[!UICONTROL trap group]** is een groep **[!UICONTROL seed addresses]** met de naam **[!UICONTROL Test profile]** in de gebruikersinterface van het web van campagne.

## Waarom een overvulgroep gebruiken {#why-trap-group}

U kunt een **[!UICONTROL trap group]** gebruiken:

1. **als proef**: Elk lid van **[!UICONTROL trap group]** ontvangt de levering alsof zij deel van het publiek uitmaakten.

1. **om uw postingslijst** te beschermen: Door te ontvangen wat het publiek zal ontvangen, zal elk **[!UICONTROL Test profile]** van **[!UICONTROL Trap group]** worden opgemerkt als de postingslijst door een derde wordt gebruikt.

>[!NOTE]
>
>Naast [ verzendend proeven tijdens de verwezenlijking van de levering ](../email/create-email.md#preview-test) en van [ controlegroep ](control-group.md), is het toevoegen van een valgroep een goede manier om uw publiek te testen.

## Overvulgroepen {#about-trap-group}

De profielen van de test worden automatisch uitgesloten van rapporten over de volgende leveringsstatistieken: **klikt**, **opent**, **Abonnementen**. De verslagen zijn alleen gericht op het echte publiek.

Voor een e-maillevering is alleen het e-mailadres vereist voor de **[!UICONTROL Trap group]** . De personalisatie van andere gebieden wordt gevuld willekeurig door Campagne.

## Een overvulgroep toevoegen in een levering {#trap-group-in-delivery}

Als u een **[!UICONTROL Trap group]** wilt instellen, gaat u naar de **[!UICONTROL Audience]** -instellingen van de levering. U hebt twee opties:

* [Testprofielen selecteren](#select-test-profiles)
* [Voorwaarde maken](#create-condition)

[ het schermschot van de de de groepsmontages van de Vulling ](assets/trap-group.png){zoomable="yes"}

### Testprofielen selecteren {#select-test-profiles}

Wanneer u **Uitgezochte testprofielen** kiest, gebruik **testprofiel(en)** knoop zoals hieronder getoond:

[ voeg het screenshot van de de knoopknoop van het testprofiel toe ](assets/trap-no-test-profile.png){zoomable="yes"}

Wanneer u op de knop klikt, kunt u de testprofielen openen om deze aan uw **[!UICONTROL trap group]** toe te voegen. Selecteer de methoden die u wilt gebruiken.

U kunt ook nieuwe testprofielen maken. [Meer informatie](#create-seed)

[ Uitgezochte het schermschot van de het interfaceprofielen van de testprofielen ](assets/trap-select-test-profiles.png){zoomable="yes"}

Nadat u de testprofielen hebt bevestigd, controleert u of het juiste nummer onder **[!UICONTROL Trap group]** staat.

[ het schermschot van de de groepsbevestiging van de Vulling ](assets/trap-check.png){zoomable="yes"}

### Voorwaarde maken {#create-condition}

Maak met de optie **[!UICONTROL Create condition]** een query om de testprofielen te definiëren die u wilt gebruiken:

[ creeer het schermschot van de voorwaardeninterface ](assets/trap-create-condition.png){zoomable="yes"}

Uw query wordt weergegeven onder **[!UICONTROL Trap group]** .

[ het schermschot van de de vraagvertoning van de groep van de Vulling ](assets/trap-custom.png){zoomable="yes"}

## Een nieuw testprofiel maken {#create-seed}

U kunt een nieuwe **[!UICONTROL test profile]** maken in de map **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]** .

[ creeer het schermafbeelding van de het netwerknavigatie van het testprofiel ](assets/trap-create.png){zoomable="yes"}

Configureer alle instellingen voor uw **[!UICONTROL test profile]** op dezelfde manier als voor elk profiel:

[ het schermschot van de profielconfiguratie van de Test ](assets/trap-create-contact.png){zoomable="yes"}