---
audience: end-user
title: Een Adobe Experience Platform-publiek gebruiken
description: Leer hoe u een publiek van Adobe Experience Platform kunt gebruiken
badge: label="Beta"
exl-id: beb73107-3d27-40ac-afef-ac2b66ae8d34
source-git-commit: 97e2d37d0a91e50b516f2fa0b6d5559f89b6c096
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 2%

---

# Een Adobe Experience Platform-publiek gebruiken{#aep-audience}

Met de Adobe Campaign Managed Cloud Service Destination and Source-connectors kunt u Adobe Campaign en Adobe Experience Platform naadloos integreren.

Zodra u een publiek van Adobe Experience Platform hebt gecreeerd en het in de cliëntconsole beschikbaar is, kunt u het op de zelfde manier gebruiken zoals u voor een publiek van de Campagne zou personaliseren en berichten verzenden.

>[!NOTE]
>
>Om het publiek van Adobe Experience Platform in Campaign te gebruiken, moet u de integratie met de Bronnen en Doelen van de Adobe vormen. Zie [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

Als u het publiek van een levering wilt selecteren, kunt u ook:

* Maak een nieuw publiek. [Meer informatie](../query/query-modeler-overview.md)
* Laad een publiek vanuit een extern bestand. [Meer informatie](file-audience.md)
* Gebruik een bestaand publiek van de Campagne. [Meer informatie](add-audience.md).

Volg onderstaande stappen om een Adobe Experience Platform-publiek voor uw levering te selecteren:

1. Van de **Publiek** sectie van de medewerker van de leveringsverwezenlijking, klik **[!UICONTROL Select audience]** knop.

   ![](assets/create-audience.png)

1. Kies **[!UICONTROL Select audience]** om een bestaand publiek te gebruiken. Als u een nieuw publiek wilt maken dat in deze e-mail wordt gebruikt, kiest u **Maak uw eigen**. Zie dit [sectie](../query/query-modeler-overview.md).

   In dit scherm worden alle bestaande soorten publiek weergegeven die zijn gedefinieerd in de Adobe Campaign-clientconsole, voor de huidige map. Blader naar de `AEP Audiences folder` in het filtergedeelte van het scherm.

   ![](assets/select-audience-folder.png)

   U kunt ook een regel definiëren om op de oorsprong van het publiek te filteren, zoals hieronder:

   ![](assets/filter-on-aep-audience.png)

1. Kies een publiek en klik op **Selecteren**.

1. Klikken **Regels bewerken** als u uw publiek wilt verfijnen.

   ![](assets/refine-audience.png)

1. Met behulp van de querymodelfunctie kunt u het publiek verrijken met extra filters of door verschillende soorten publiek te combineren. Zie dit [sectie](../query/query-modeler-overview.md).

1. Klikken **Opslaan**.
