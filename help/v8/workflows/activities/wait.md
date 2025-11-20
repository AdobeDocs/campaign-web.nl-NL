---
audience: end-user
title: De workflowactiviteit Wachten gebruiken
description: Leer hoe u de workflowactiviteit Wacht gebruikt
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 6%

---

# Wachten {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Wachtactiviteit"
>abstract="**wacht** activiteit wordt gebruikt om de overgang van één activiteit aan een andere te vertragen."

**wacht** activiteit is de controle **activiteit van de a** Stroom. Het biedt een zekere tijd om te wisselen tussen de uitvoering van twee activiteiten. Het kan bijvoorbeeld worden gebruikt om enkele dagen na een e-mailleveringsactiviteit te wachten en vervolgens de geopende berichten te analyseren en tijdens deze periode te klikken voordat u follow-upbewerkingen uitvoert, zoals het verzenden van een e-mail met een herinnering of het maken van een publiek.

## Configuratie {#wait-configuration}

Volg deze stappen om **te vormen wachten** activiteit:

1. Voeg a **toe wacht** activiteit in uw werkschema.

1. Specificeer de **Duur** van het wachten tussen de binnenkomende en uitgaande overgangen.

1. Selecteer de tijdeenheid op het **gebied van Punten**: seconden, notulen, uren, of dagen.

## Voorbeeld {#wait-example}

Het volgende voorbeeld illustreert **wacht** activiteit in een typisch gebruiksgeval. U stuurt een e-mailuitnodiging voor een evenement. Na 24 uur wordt een SMS-verzending naar dezelfde populatie verzonden.

![&#x200B; Voorbeeld van een werkschema dat de Wachtende activiteit gebruikt om SMS 24 uur na een e-mailuitnodiging te verzenden.](../assets/workflow-wait-example.png)