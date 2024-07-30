---
audience: end-user
title: Een overvulgroep gebruiken
hide: true
hidefromtoc: true
description: Leer hoe te om een valgroep voor uw levering in het gebruikersinterface van het Web van de Campagne te gebruiken
source-git-commit: 2feea0c5a1b021786e58bf6a69a2018ec37ea4b1
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 0%

---

# Een **[!UICONTROL trap group]** gebruiken {#trap-group}

Een **[!UICONTROL trap group]** (ook wel **[!UICONTROL Seed list]** genoemd) wordt gebruikt om specifieke adressen in uw leveringen op te nemen om het distributieproces te controleren en te verifiëren door zich te richten op profielen die niet aan de gedefinieerde doelcriteria voldoen. Op deze manier kunnen ontvangers die buiten het bereik van de levering vallen, de levering ontvangen, net als elke andere doelontvanger.
Een **[!UICONTROL trap group]** is een groep **[!UICONTROL seed addresses]** met de naam **[!UICONTROL Test profile]** in de interface van het AC-web.

## Waarom gebruiken **[!UICONTROL Trap group]**

U kunt **[!UICONTROL trap group]** gebruiken:

1. **als proef** : elk lid van **[!UICONTROL Trap group]** zal de levering ontvangen alsof zij deel van het publiek uitmaakten.


1. **om uw postingslijst** te beschermen: door te ontvangen wat het publiek zal ontvangen, zal elk **[!UICONTROL test profile]** van **[!UICONTROL Trap group]** worden opgemerkt als de postingslijst door een derde wordt gebruikt.

>[!NOTE]
>
>De groep van de val is verschillend van [ verzendende proeven tijdens de verwezenlijking van de levering ](../email/create-email.md#preview-test) en van [ controlegroep ](control-group.md).


## Informatie over **[!UICONTROL Trap group]**

De profielen van de test worden automatisch uitgesloten van rapporten over de volgende leveringsstatistieken: **klikt**, **opent**, **Abonnementen**. De verslagen gaan alleen over het echte publiek.

Voor een e-maillevering is alleen een e-mailadres nodig voor de **[!UICONTROL Trap group]** . Andere velden worden willekeurig door Campagne aangepast.

## Hoe te om a **[!UICONTROL Trap group]** in levering te plaatsen

Als u een **[!UICONTROL Trap group]** wilt instellen, gaat u naar de **[!UICONTROL Audience]** -instellingen van de levering. U hebt twee opties:
- [Testprofielen selecteren](#select-test-profile)
- [Voorwaarde maken](#create-condition)

![](assets/trap-group.png){zoomable="yes"}

### Testprofielen selecteren {#select-test-profiles}

Wanneer u &quot;Testprofielen selecteren&quot; kiest, wordt het venster weergegeven zoals hieronder aangegeven voor **[!UICONTROL Add test profile(s)]** :

![](assets/trap-no-test-profile.png){zoomable="yes"}

Wanneer u op de knop klikt, hebt u toegang tot de testprofielen die u aan **[!UICONTROL trap group]** kunt toevoegen. Controleer de bestanden die u wilt gebruiken.
U kunt nieuwe testprofielen maken. [Meer informatie](#create-seed)

![](assets/trap-select-test-profiles.png){zoomable="yes"}

Wanneer u uw testprofielen bevestigt, controleer dat u het correcte aantal onder **[!UICONTROL Trap group]** hebt.

![](assets/trap-check.png){zoomable="yes"}

### Voorwaarde maken {#create-condition}

Als u **[!UICONTROL Create condition]** kiest, krijgt u een nieuw venster waarin u een query kunt aanpassen om de testprofielen te definiëren die u wilt gebruiken:

![](assets/trap-create-condition.png){zoomable="yes"}

Uw query wordt weergegeven onder **[!UICONTROL Trap group]** .

![](assets/trap-custom.png){zoomable="yes"}

## Nieuwe methoden maken **[!UICONTROL Test profile]** {#create-seed}

U kunt een nieuwe **[!UICONTROL test profile]** maken in **[!UICONTROL Explorer]** > **[!UICONTROL Ressources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed members]**

![](assets/trap-create.png){zoomable="yes"}

U kunt alle details over uw **[!UICONTROL test profile]** voltooien alsof het een publieksprofiel was:

![](assets/trap-create-contact.png){zoomable="yes"}