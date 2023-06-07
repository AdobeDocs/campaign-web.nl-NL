---
audience: end-user
title: De workflowactiviteit Wachten gebruiken
description: Leer hoe u de workflowactiviteit Wacht gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 28%

---


# Wachten {#wait}

De **Wachten** activiteit is **Stroomregeling** activiteit. Het wordt gebruikt om een bepaalde hoeveelheid tijd toe te staan om tussen twee uit te voeren activiteiten over te gaan. Bijvoorbeeld als u een aantal dagen wilt wachten na een e-mailleveringsactiviteit om het aantal open- en klikacties tijdens die periode te analyseren voordat u follow-upbewerkingen gaat uitvoeren (herinneringsmail, doelgroep maken, enz.).

## Configuratie

Voer de volgende stappen uit om de **Wachten** activiteit:

1. Voeg een **Wachten** in uw workflow.

1. Geef de **Duur** van de wachttijd tussen de binnenkomende en uitgaande overgangen.

1. Selecteer de tijdeenheid in het dialoogvenster **Punten** veld: seconden, minuten, uren.

## Voorbeeld

In het volgende voorbeeld wordt het **Wachten** activiteit in een typisch geval van gebruik. U stuurt een e-mailuitnodiging voor een evenement. 24 uur nadat het is verzonden, wordt een SMS-verzending naar dezelfde populatie verzonden.

![](../assets/workflow-wait-example.png)
