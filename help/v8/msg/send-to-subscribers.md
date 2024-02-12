---
audience: end-user
title: Berichten verzenden naar de abonnees van een service
description: Leer hoe te om berichten naar de abonnees van een dienst te verzenden
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Berichten verzenden naar de abonnees van een service {#send-to-subscribers}

U kunt abonnementsservices maken in Adobe Campaign en berichten verzenden naar abonnees. Leer hoe u abonnementenservices kunt maken op [deze pagina](../audience//manage-services.md#create-service).

Als u berichten naar uw abonnees wilt verzenden, maakt u een specifiek publiek om de abonnees te identificeren en maakt u vervolgens de levering zoals hieronder beschreven.

1. Maak een publiek. Er wordt automatisch een nieuwe workflow gemaakt. [Meer informatie over het publiek](../audience/create-audience.md)

1. Voor een betere leesbaarheid wijzigt u de naam van de workflow in de workflowinstellingen.&#39; **Label** veld. [Leer hoe u workflowinstellingen configureert](../workflows/workflow-settings.md)

1. Open de **[!UICONTROL Build audience]** activiteit, en selecteer **[!UICONTROL Create audience]**. [Leer hoe te om een het publieksactiviteit van de Bouwstijl te vormen](../workflows/activities/build-audience.md)

   ![](assets/service-create-audience.png){zoomable=&quot;yes&quot;}

1. Selecteer de volgende aangepaste voorwaarden in de aanmaakstroom voor het publiek: **[!UICONTROL Susbscriptions]** bestaan **[!UICONTROL Service]** is gelijk aan de dienst u bepaalde. Selecteer in dit voorbeeld de optie **Luma-yoga nieuwsbrief**.

   ![](assets/service-audience-subscribers.png){zoomable=&quot;yes&quot;}

1. Selecteren **[!UICONTROL Confirm]** en klik op **[!UICONTROL Start]** om de workflow uit te voeren.

1. Een levering maken. De stappen voor het maken van een levering worden beschreven in [deze pagina](../msg/gs-messages.md#create-delivery).
1. Blader naar uw leveringsinstellingen en wijzig de standaarddoeltoewijzing in **Abonnementen (nms:abonnementen)**.

   ![](assets/service-delivery-change-mapping.png){zoomable=&quot;yes&quot;}

1. Selecteer in de hoofddoelsectie van de levering het publiek dat u hierboven hebt gemaakt.

   ![](assets/service-delivery-targeting-subscribers.png){zoomable=&quot;yes&quot;}

1. Maak uw berichtinhoud, test en verzend de levering, zoals in [deze sectie](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png){zoomable=&quot;yes&quot;}

Uw levering wordt alleen naar de abonnees van die service verzonden.
