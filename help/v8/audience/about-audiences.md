---
audience: end-user
title: Aan de slag met het publiek
description: Leer hoe te om publiek in het Web UI van de Campagne te gebruiken
badge: label="Beta"
exl-id: 21bb5082-82ce-47d6-a4d4-becf44490f13
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 4%

---


# Aan de slag met het publiek {#about-audiences}

<!--
Audience only created for the delivery, not available later-->


<!--
Three ways:
* existing audience

Campaign or AEP Audiences

* create new on the fly

query like AEP segment builder (same component with campaign data)

* import from file

show use case with a new audience creation (or import from file?)

control groups like acc: exract, random, based on attribute
-->


Het publiek is het belangrijkste doel van uw levering: de ontvangers die de berichten ontvangen. Het type publiek hangt van de doelafbeelding af die in het leveringsmalplaatje wordt bepaald. Meer weten over een leveringssjabloon [in deze sectie](../msg/delivery-template.md).

Om de publieksbevolking te bepalen, kunt u:

* Selecteer een bestaand publiek dat als een lijst in de cliëntconsole wordt gecreeerd. [Meer informatie](add-audience.md)
* Selecteer een Adobe Experience Platform-publiek. [Meer informatie](aep-audience.md)
* Bouw een nieuw publiek met de regelbouwer door het filtreren criteria te bepalen en te combineren. [Meer informatie](segment-builder.md)
* Gebruik een publiek uit een extern bestand: deze optie is alleen beschikbaar voor zelfstandige e-mailleveringen en kan niet worden gebruikt in campagneleveringen. [Meer informatie](file-audience.md)

Wanneer het verzenden van berichten in de context van een campagnewerkschema, wordt het publiek bepaald in een specifiek **Lees publiek** workflowactiviteit. In deze context kunt u geen publiek uit een bestand laden voor e-maillevering en wordt het publiek alleen gedefinieerd in deze toegewijde activiteit. Leer hoe u het publiek van uw levering kunt definiëren in een campagneworkflow [in deze sectie](../workflows/orchestrate-activities.md).

Bovendien kunt u controlegroepen bepalen vermijden verzendend berichten naar een gedeelte van uw publiek, en de invloed van uw campagnes meten. [Meer informatie](control-group.md)

![](assets/about-audience.png)

