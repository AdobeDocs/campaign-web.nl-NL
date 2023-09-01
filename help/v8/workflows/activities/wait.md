---
audience: end-user
title: De workflowactiviteit Wachten gebruiken
description: Leer hoe u de workflowactiviteit Wacht gebruikt
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 29%

---


# Wachten {#wait}

De **Wachten** activiteit is **Stroomregeling** activiteit. Het wordt gebruikt om een bepaalde hoeveelheid tijd toe te staan om tussen twee uit te voeren activiteiten over te gaan. Bijvoorbeeld als u een aantal dagen wilt wachten na een e-mailleveringsactiviteit om het aantal open- en klikacties tijdens die periode te analyseren voordat u follow-upbewerkingen gaat uitvoeren (herinneringsmail, doelgroep maken, enz.).

## Configuratie

Voer de volgende stappen uit om de **Wachten** activiteit:

1. Voeg een **Wachten** in uw workflow.

1. Geef de **Duur** van de wachttijd tussen de binnenkomende en uitgaande overgangen.

1. Selecteer de tijdeenheid in het dialoogvenster **Punten** veld: seconden, minuten, uren.

## Voorbeeld

In het volgende voorbeeld wordt het **Wachten** in een typisch geval. U stuurt een e-mailuitnodiging voor een evenement. 24 uur nadat het is verzonden, wordt een SMS-verzending naar dezelfde populatie verzonden.

![](../assets/workflow-wait-example.png)
