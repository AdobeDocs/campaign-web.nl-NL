---
audience: end-user
title: Een overvulgroep gebruiken
hide: true
hidefromtoc: true
description: Leer hoe te om een valgroep voor uw levering in het gebruikersinterface van het Web van de Campagne te gebruiken
source-git-commit: 15d8ea478a234136dc654683798957d6c7026327
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Een **[!UICONTROL trap group]** {#trap-group}

A **[!UICONTROL trap group]** wordt gebruikt om ontvangers aan te wijzen die niet aan de bepaalde doelcriteria voldoen. Op deze manier kunnen ontvangers die buiten het bereik van de levering vallen, de levering ontvangen, net als elke andere doelontvanger.
A **[!UICONTROL trap group]** is een groep **[!UICONTROL seed addresses]**.

## Waarom gebruiken **[!UICONTROL trap group]**

U kunt **[!UICONTROL trap group]** :

1. **Als bewijs** : elk lid van de **[!UICONTROL Trap group]** zal de levering ontvangen alsof ze deel uitmaken van het publiek.


1. **Je mailinglijst beveiligen** : door te ontvangen wat het publiek zal ontvangen, elk **[!UICONTROL seed address]** van de **[!UICONTROL Trap group]** wordt opgemerkt als de mailinglijst door een derde wordt gebruikt.

## Informatie over **[!UICONTROL Trap group]**

Zaadadressen worden automatisch uitgesloten van rapporten over de volgende leveringsstatistieken: **Klikken**, **Openen**, **Abonnementen**. De verslagen gaan alleen over het echte publiek.

Voor een e-maillevering is alleen een e-mailadres nodig voor de **[!UICONTROL Trap group]**, wordt de personalisatie van andere gebieden willekeurig ingevuld door Campagne.

## Hoe kan ik een **[!UICONTROL Trap group]** in de levering

Als u een **[!UICONTROL Trap group]**, ga naar de **[!UICONTROL Audience]** instellingen van uw levering. U hebt twee opties:
- [Testprofielen selecteren](#select-test-profile)
- [Voorwaarde maken](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Testprofielen selecteren {#select-test-profiles}

Als u &quot;Testprofielen selecteren&quot; kiest, wordt het venster weergegeven zoals hieronder. Hieronder ziet u **[!UICONTROL Add test profile(s)]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Wanneer u op de knoop klikt, zult u toegang tot de zaadadressen hebben u kunt toevoegen **[!UICONTROL trap group]**. Controleer de bestanden die u wilt gebruiken.
U kunt nieuwe zaadadressen tot stand brengen. [Meer informatie](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Wanneer u uw overvuladressen bevestigt, controleer dan of u het juiste nummer onder hebt **[!UICONTROL Trap group]**.

![](assets/trap-check.png){zoomable="yes"}

### Voorwaarde maken {#create-condition}

Met de **[!UICONTROL Create condition]** u kunt kiezen, zult u een nieuw venster krijgen waar u een vraag kunt aanpassen om de zaadadressen te bepalen u wilt gebruiken:

![](assets/trap-create-condition.png){zoomable="yes"}

Uw query wordt weergegeven onder **[!UICONTROL Trap group]**.

![](assets/trap-custom.png){zoomable="yes"}

## Een nieuwe **[!UICONTROL seed address]** {#create-seed}

U kunt een nieuwe **[!UICONTROL seed address]** in **[!UICONTROL Explorer]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]**

![](assets/trap-create.png){zoomable="yes"}

U kunt alle details over uw zaadlid voltooien alsof het een publieksprofiel was:

![](assets/trap-create-contact.png){zoomable="yes"}