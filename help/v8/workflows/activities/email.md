---
audience: end-user
title: De e-mailworkflowactiviteit gebruiken
description: Leer hoe u de e-mailworkflowactiviteit gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: 3df57348b82b4efc871166a5b5a6163f3a950b44
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 2%

---


# E-mail, SMS, Push {#email}

Met Adobe Campaign Web kunt u marketingcampagnes automatiseren en uitvoeren op meerdere kanalen, zoals e-mail, SMS of push. U kunt kanaalactiviteiten in het canvas combineren om kanaalworkflows te maken die acties op basis van klantgedrag kunnen activeren.

U kunt bijvoorbeeld een welkomstcampagne voor e-mail maken met een reeks berichten via verschillende kanalen, zoals e-mail, SMS en push. U kunt ook een e-mail verzenden nadat een klant een aankoop heeft voltooid of een gepersonaliseerd verjaardagsbericht via SMS naar een klant sturen.

Door kanaalactiviteiten te gebruiken, kunt u uitvoerige en gepersonaliseerde campagnes tot stand brengen die klanten over veelvoudige touchpoints en aandrijvingsomzettingen in dienst nemen.

Hier volgen de stappen om een **Kanaal** activiteit in een werkstroom:

1. Controleer of u een **publiek opbouwen** activiteit. Het publiek is het belangrijkste doel van uw levering: de ontvangers die de berichten ontvangen. Wanneer het verzenden van berichten in de context van een campagnewerkschema, wordt het berichtpubliek niet bepaald in de kanaalactiviteit, maar in **publiek opbouwen** activiteit. Zie [deze sectie](build-audience.md).

   ![](../../msg/assets/add-delivery-in-wf.png)

1. Selecteer een leveringsactiviteit: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]** of **[!UICONTROL Push notification (iOS)]**.

1. Selecteer een **Sjabloon**. Sjablonen zijn vooraf geconfigureerde leveringsinstellingen die zijn opgeslagen voor toekomstig gebruik. [Meer informatie](../../msg/delivery-template.md)

1. Klikken **Levering maken** en definieer uw bericht op dezelfde manier als wanneer u een zelfstandige levering maakt. [Meer informatie](../../msg/gs-messages.md)


1. Start de workflow en controleer logbestanden.

<!--
description, which use case you can perform (common other activities that you can link before of after the activity)

how to add and configure the activity

example of a configured activity within a workflow
The Email delivery activity allows you to configure the sending an email in a workflow. 

-->



<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

E-mailontvangers worden vóór de activiteit in dezelfde workflow gedefinieerd via een doelactiviteit voor het publiek.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->
