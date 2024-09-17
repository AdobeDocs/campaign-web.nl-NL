---
audience: end-user
title: Berichten verzenden naar de abonnees van een service
description: Leer hoe te om berichten naar de abonnees van een dienst te verzenden
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Berichten verzenden naar de abonnees van een service {#send-to-subscribers}

U kunt abonnementsservices maken in Adobe Campaign en berichten verzenden naar abonnees. Leer hoe te om de abonnementendiensten op [ tot stand te brengen deze pagina ](../audience//manage-services.md#create-service).

Als u berichten naar uw abonnees wilt verzenden, maakt u een specifiek publiek om de abonnees te identificeren en maakt u vervolgens de levering zoals hieronder beschreven.

1. Maak een publiek. Er wordt automatisch een nieuwe workflow gemaakt. [ leer meer over publiek ](../audience/create-audience.md)

1. Voor betere leesbaarheid, verander de naam van het werkschema op het gebied van het Etiket van de werkschemamontages ****. [ Leer hoe te om werkschemamontages ](../workflows/workflow-settings.md) te vormen

1. Open de **[!UICONTROL Build audience]** -activiteit en selecteer **[!UICONTROL Create audience]** . [ leren hoe te om een het publieksactiviteit van de Bouwstijl te vormen ](../workflows/activities/build-audience.md)

   ![](assets/service-create-audience.png){zoomable="yes"}

1. Selecteer de volgende aangepaste voorwaarden in de stroom voor het maken van een publiek: **[!UICONTROL Susbscriptions]** bestaan, zoals **[!UICONTROL Service]** , is gelijk aan de service die u hebt gedefinieerd. In dit voorbeeld, selecteer uw **Luma yoga nieuwsbrief**.

   ![](assets/service-audience-subscribers.png){zoomable="yes"}

1. Selecteer **[!UICONTROL Confirm]** en klik op **[!UICONTROL Start]** om de workflow uit te voeren.

1. Een levering maken. De stappen om een levering tot stand te brengen zijn gedetailleerd in [ deze pagina ](../msg/gs-messages.md#create-delivery).
1. Blader naar uw leveringsmontages, verander de standaarddoelafbeelding in **Abonnementen (nms:abonnementen)**.

   ![](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. Selecteer in de hoofddoelsectie van de levering het publiek dat u hierboven hebt gemaakt.

   ![](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Creeer uw berichtinhoud, test en verzend de levering, zoals die in [ wordt gedetailleerd deze sectie ](../preview-test/preview-test.md).

   ![](assets/service-delivery-ready.png){zoomable="yes"}

Uw levering wordt alleen naar de abonnees van die service verzonden.
