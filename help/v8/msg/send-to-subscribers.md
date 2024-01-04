---
audience: end-user
title: Berichten verzenden naar de abonnees van een service
description: Leer hoe te om berichten naar de abonnees van een dienst te verzenden
badge: label="Beta"
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: cd7e2bb325b4e571018a8e04ffa0eaef74fe6768
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Berichten verzenden naar de abonnees van een service

U kunt abonnementsservices maken in Adobe Campaign en berichten verzenden naar abonnees. Leer hoe u abonnementenservices kunt maken in [deze pagina](../audience//manage-services.md#create-service).

Als u berichten naar uw abonnees wilt verzenden, maakt u een specifiek publiek om de abonnees te identificeren en maakt u vervolgens de levering zoals hieronder beschreven.

1. Maak een publiek. Meer informatie over publiek in [deze pagina](../audience/create-audience.md).

1. In de **[!UICONTROL Build audience]** activiteit, toon de geavanceerde attributen en selecteer **[!UICONTROL Recipient]** > **[!UICONTROL Subscriptions]** > **[!UICONTROL Service]**.

   In dit voorbeeld selecteert u de gebruikers die zijn geabonneerd op de service met de **Luma-nieuwsbrief** label.

   ![](assets/service-audience-subscribers.png)

1. Sla het publiek op.
1. Een levering maken. De stappen voor het maken van een levering worden beschreven in [deze pagina](../msg/gs-messages.md#create-delivery).
1. Blader naar uw leveringsinstellingen en wijzig de standaarddoeltoewijzing in **Abonnementen (nms:abonnementen)**.

   ![](assets/service-delivery-change-mapping.png)

1. Selecteer in de hoofddoelsectie van de levering het publiek dat u hierboven hebt gemaakt.

   ![](assets/service-delivery-targeting-subscribers.png)

1. Maak uw berichtinhoud, test en verzend de levering, zoals in [deze sectie](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png)

Uw levering wordt alleen naar de abonnees van die service verzonden.
