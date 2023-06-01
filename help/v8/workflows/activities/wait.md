---
audience: end-user
title: De workflowactiviteit Wachten gebruiken
description: Leer hoe u de workflowactiviteit Wacht gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: 9be56c3c9c7a339e1f348ac9c74d425b501c317d
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 37%

---


# Wachten {#wait}

De **Wachten** activiteit onderbreekt tijdelijk het uitvoeren van een deel van een werkstroom. De uitgaande overgang wordt na een vertraging (van een paar seconden tot meerdere maanden) weer geactiveerd, zodat de later geplaatste activiteiten worden uitgevoerd.

De **Wachten** de activiteit wordt gebruikt om een bepaalde hoeveelheid tijd tussen twee uit te voeren activiteiten toe te staan. Bijvoorbeeld als u een aantal dagen wilt wachten na een e-mailleveringsactiviteit om het aantal open- en klikacties tijdens die periode te analyseren voordat u follow-upbewerkingen gaat uitvoeren (herinneringsmail, doelgroep maken, enz.).

## Configuratie

Voer de volgende stappen uit om de **Wachten** activiteit:

1. Voeg een **Wachten** in uw workflow.

1. Geef de **Duur** van de wachttijd tussen wanneer de binnenkomende en uitgaande overgangen van de activiteit worden geactiveerd.

1. De tijdeenheid selecteren **Periode**: seconden, minuten, uren.

## Voorbeeld

In het volgende voorbeeld wordt het **Wachten** activiteit in een typisch geval van gebruik. U stuurt een e-mailuitnodiging voor een evenement. 24 uur nadat het is verzonden, wordt een SMS-verzending naar dezelfde populatie verzonden.

![](../assets/workflow-wait-example.png)
