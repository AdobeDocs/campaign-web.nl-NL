---
audience: end-user
title: De workflowactiviteit Wachten gebruiken
description: Leer hoe u de workflowactiviteit Wacht gebruikt
badge: label="Beta"
exl-id: 970953a1-0091-477c-9f52-596af3a8857d
source-git-commit: f4ffb1e033dae3d631772ef602e48e336c8c0f16
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 27%

---

# Wachten {#wait}

>[!CONTEXTUALHELP]
>id="acw_orchestration_wait"
>title="Wachtactiviteit"
>abstract="De **Wachten** activiteit wordt gebruikt om de overgang van een activiteit aan een andere uit te stellen."

De **Wachten** activiteit is **Stroomregeling** activiteit. Het wordt gebruikt om een bepaalde hoeveelheid tijd toe te staan om tussen twee uit te voeren activiteiten over te gaan. Bijvoorbeeld als u een aantal dagen wilt wachten na een e-mailleveringsactiviteit om het aantal open- en klikacties tijdens die periode te analyseren voordat u follow-upbewerkingen gaat uitvoeren (herinneringsmail, doelgroep maken, enz.).

## Configuratie{#wait-configuration}

Voer de volgende stappen uit om de **Wachten** activiteit:

1. Voeg een **Wachten** in uw workflow.

1. Geef de **Duur** van de wachttijd tussen de binnenkomende en uitgaande overgangen.

1. Selecteer de tijdeenheid in het dialoogvenster **Punten** veld: seconden, minuten, uren.

## Voorbeeld{#wait-example}

In het volgende voorbeeld wordt het **Wachten** in een typisch geval. U stuurt een e-mailuitnodiging voor een evenement. 24 uur nadat het is verzonden, wordt een SMS-verzending naar dezelfde populatie verzonden.

![](../assets/workflow-wait-example.png)
