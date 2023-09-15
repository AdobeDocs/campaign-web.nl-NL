---
audience: end-user
title: De workflowactiviteit Wachten gebruiken
description: Leer hoe u de workflowactiviteit Wacht gebruikt
badge: label="Beta"
source-git-commit: 74e64ded74db7aa69a059b785a8b29387c446648
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 25%

---


# Wachten {#wait}


>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Wachten"
>abstract="De **Wachten** activiteit is **Stroomregeling** activiteit. Het wordt gebruikt om een bepaalde hoeveelheid tijd toe te staan om tussen twee uit te voeren activiteiten over te gaan."


De **Wachten** activiteit is **Stroomregeling** activiteit. Het wordt gebruikt om een bepaalde hoeveelheid tijd toe te staan om tussen twee uit te voeren activiteiten over te gaan. Bijvoorbeeld als u een aantal dagen wilt wachten na een e-mailleveringsactiviteit om het aantal open- en klikacties tijdens die periode te analyseren voordat u follow-upbewerkingen gaat uitvoeren (herinneringsmail, doelgroep maken, enz.).

## Configuratie

Voer de volgende stappen uit om de **Wachten** activiteit:

1. Voeg een **Wachten** in uw workflow.

1. Geef de **Duur** van de wachttijd tussen de binnenkomende en uitgaande overgangen.

1. Selecteer de tijdeenheid in het dialoogvenster **Punten** veld: seconden, minuten, uren.

## Voorbeeld

In het volgende voorbeeld wordt het **Wachten** in een typisch geval. U stuurt een e-mailuitnodiging voor een evenement. 24 uur nadat het is verzonden, wordt een SMS-verzending naar dezelfde populatie verzonden.

![](../assets/workflow-wait-example.png)
