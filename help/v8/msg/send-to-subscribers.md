---
audience: end-user
title: Berichten verzenden naar de abonnees van een service
description: Leer hoe te om berichten naar de abonnees van een dienst te verzenden
exl-id: f6e14db5-261c-4fa6-bd19-fd8bdc04aaf1
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Berichten verzenden naar de abonnees van een service {#send-to-subscribers}

U kunt abonnementsservices maken in Adobe Campaign en berichten verzenden naar uw abonnees. Leer hoe te om de abonnementsdiensten op [ tot stand te brengen deze pagina ](../audience//manage-services.md#create-service).

Als u berichten naar uw abonnees wilt verzenden, maakt u een specifiek publiek om de abonnees te identificeren en maakt u vervolgens de levering zoals hieronder beschreven.

1. Maak een publiek. Er wordt automatisch een nieuwe workflow gemaakt. [ leer meer over publiek ](../audience/create-audience.md).

1. Voor betere leesbaarheid, verander de naam van het werkschema op het gebied van het Etiket van de werkschemamontages ****. [ Leer hoe te om werkschemamontages ](../workflows/workflow-settings.md) te vormen.

1. Open de **[!UICONTROL Build audience]** -activiteit en selecteer **[!UICONTROL Create audience]** . [ Leer hoe te om een het publieksactiviteit van de Bouwstijl ](../workflows/activities/build-audience.md) te vormen.

   ![ Schermafbeelding die de configuratie van de het publieksactiviteit van de Bouwstijl in Adobe Campaign toont.](assets/service-create-audience.png){zoomable="yes"}

1. Selecteer in de stroom voor het maken van een publiek de volgende aangepaste voorwaarden: **[!UICONTROL Subscriptions]** bestaan, zoals **[!UICONTROL Service]** , is gelijk aan de service die u hebt gedefinieerd. In dit voorbeeld, selecteer uw **Luma yoga nieuwsbrief**.

   ![ het Schermafbeelding die de stroom van de publieksverwezenlijking met douanevoorwaarden voor abonnementen in Adobe Campaign toont.](assets/service-audience-subscribers.png){zoomable="yes"}

1. Selecteer **[!UICONTROL Confirm]** en klik op **[!UICONTROL Start]** om de workflow uit te voeren.

1. Een levering maken. De stappen om een levering tot stand te brengen zijn gedetailleerd op [ deze pagina ](../msg/gs-messages.md#create-delivery).

1. Blader naar uw leveringsmontages, en verander de standaarddoelafbeelding aan **Abonnementen (nms:abonnementen)**.

   ![ Schermafbeelding die de leveringsmontages met de doelafbeelding toont in Abonnementen in Adobe Campaign wordt veranderd.](assets/service-delivery-change-mapping.png){zoomable="yes"}

1. Selecteer in de hoofddoelsectie van de levering het publiek dat u hierboven hebt gemaakt.

   ![ Schermschot die de belangrijkste doelsectie van de levering met het geselecteerde publiek in Adobe Campaign tonen.](assets/service-delivery-targeting-subscribers.png){zoomable="yes"}

1. Creeer uw berichtinhoud, test het, en verzend de levering, zoals die in [ wordt gedetailleerd deze sectie ](../preview-test/preview-test.md).

   ![ Schermafbeelding die de levering toont klaar om in Adobe Campaign te worden verzonden.](assets/service-delivery-ready.png){zoomable="yes"}

Uw levering wordt alleen naar de abonnees van die service verzonden.