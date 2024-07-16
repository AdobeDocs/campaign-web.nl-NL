---
audience: end-user
title: De workflowactiviteit Wachten gebruiken
description: Leer hoe u de workflowactiviteit Wacht gebruikt
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 26%

---

# Wachten {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Wachtactiviteit"
>abstract="**wacht** activiteit wordt gebruikt om de overgang van een activiteit aan een andere te vertragen."

**wacht** activiteit is de controle **activiteit van de a** Stroom. Het wordt gebruikt om een bepaalde hoeveelheid tijd toe te staan om tussen twee uit te voeren activiteiten over te gaan. Bijvoorbeeld als u een aantal dagen wilt wachten na een e-mailleveringsactiviteit om het aantal open- en klikacties tijdens die periode te analyseren voordat u follow-upbewerkingen gaat uitvoeren (herinneringsmail, doelgroep maken, enz.).

## Configuratie{#wait-configuration}

Volg deze stappen om **te vormen wachten** activiteit:

1. Voeg a **toe wacht** activiteit in uw werkschema.

1. Specificeer de **Duur** van het wachten tussen de binnenkomende en uitgaande overgangen.

1. Selecteer de tijdeenheid op het **gebied van Punten**: seconden, notulen, uren, dagen.

## Voorbeeld{#wait-example}

Het volgende voorbeeld illustreert **wacht** activiteit in een typisch gebruiksgeval. U stuurt een e-mailuitnodiging voor een evenement. 24 uur nadat het is verzonden, wordt een SMS-verzending naar dezelfde populatie verzonden.

![](../assets/workflow-wait-example.png)
