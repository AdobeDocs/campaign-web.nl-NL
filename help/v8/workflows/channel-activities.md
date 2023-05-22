---
audience: end-user
title: Werken met workflowkanaalactiviteiten
description: Leer hoe u kanaalactiviteiten kunt gebruiken in Adobe Campaign Web-workflows
badge: label="Alpha" type="Positief"
exl-id: 6f9be348-6138-470c-8c40-750dc0311424
source-git-commit: dd006d1e161dec49d9a1a6bcb8cb67503178479b
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---

# Kanaalactiviteiten {#channel}

Met Adobe Campaign Web kunt u marketingcampagnes automatiseren en uitvoeren op meerdere kanalen, zoals e-mail, SMS of push. Met Adobe Campaign-workflows kunt u kanaalactiviteiten combineren tot het canvas om kanaalworkflows te maken die acties op basis van klantgedrag kunnen activeren.

U kunt bijvoorbeeld een welkomstcampagne voor e-mail maken met een reeks berichten via verschillende kanalen, zoals e-mail, SMS en push. U kunt ook een e-mail verzenden nadat een klant een aankoop heeft voltooid of een gepersonaliseerd verjaardagsbericht via SMS naar een klant sturen.

Door kanaalactiviteiten te gebruiken, kunt u uitvoerige, gepersonaliseerde campagnes tot stand brengen die klanten over veelvoudige touchpoints en aandrijvingsomzettingen in dienst nemen.

Kanaalactiviteiten zijn beschikbaar in het palet, links op het scherm, in de sectie Kanalen.

## Email {#email}

beschrijving, die het geval gebruikt u kunt uitvoeren (gemeenschappelijke andere activiteiten die u voor van na de activiteit kunt verbinden)

hoe te om de activiteit toe te voegen en te vormen

voorbeeld van een geconfigureerde activiteit binnen een workflow


Met de activiteit E-mail verzenden kunt u het verzenden van een e-mail configureren in een workflow.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

E-mailontvangers worden vóór de activiteit in dezelfde workflow gedefinieerd via een doelactiviteit voor het publiek.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->