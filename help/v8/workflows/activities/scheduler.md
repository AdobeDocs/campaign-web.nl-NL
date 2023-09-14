---
audience: end-user
title: De workflowactiviteit van de planner gebruiken
description: Leer hoe u de workflowactiviteit van de planner gebruikt
badge: label="Beta"
source-git-commit: bbb22de6ff1398dbb1431f51a55350d206b4690a
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 15%

---


# Planner {#scheduler}

<!--
>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Scheduler activity"
>abstract="The Scheduler activity allows you..."
-->

De **Planner** activiteit is **Stroomregeling** activiteit. Hiermee kunt u plannen wanneer de workflow wordt gestart. Deze activiteit moet worden beschouwd als een geplande start. Deze kan alleen worden gebruikt als de eerste activiteit van de workflow.

## Beste praktijken

Plan geen workflow die meer dan om de 15 minuten wordt uitgevoerd, aangezien dit de algehele systeemprestaties kan belemmeren en blokken in de database kan maken.

## Configuratie

Voer de volgende stappen uit om de **Planner** activiteit:

1. Voeg een **Planner** activiteit aan uw werkschema.

   ![](../assets/workflow-scheduler.png)

1. Vorm **Uitvoerfrequentie**:

   * **Eenmaal**: de workflow wordt één keer uitgevoerd.

   * **Dagelijks**: de workflow wordt op een bepaald tijdstip, eenmaal per dag, uitgevoerd.

   * **Meerdere keren per dag:** de workflow wordt regelmatig verscheidene keren per dag uitgevoerd . U kunt uitvoeringen instellen op specifieke tijdstippen of periodiek.

   * **Wekelijks**: de workflow wordt op een bepaald moment, één keer of meerdere keren per week uitgevoerd.

   * **Maandelijks**: de workflow wordt uitgevoerd op een bepaald moment, één keer of meerdere keren per maand. U kunt aangeven in welke maanden u de workflow wilt uitvoeren. U kunt uitvoeringen ook instellen op bepaalde weekdagen van de maand, zoals de tweede dinsdag van de maand.

1. Definieer de details van de uitvoering op basis van de geselecteerde frequentie. De detailvelden variëren, afhankelijk van de gebruikte frequentie (tijd, herhalingsfrequentie, opgegeven dagen, enz.).

1. Klikken **Voorvertoning van opstartij** om het schema van de volgende tien uitvoeringen van uw werkschema te controleren.

1. Bepaal de geldigheidsperiode van de planner:

   * **Permanent (nooit verlopen)**: de werkstroom wordt uitgevoerd volgens de opgegeven frequentie, zonder enige beperking van het tijdkader of het aantal herhalingen.

   * **Geldigheidsperiode**: de workflow wordt uitgevoerd volgens de opgegeven frequentie, tot een bepaalde datum. U moet begin- en einddatums opgeven.

## Voorbeeld

In het volgende voorbeeld, wordt de activiteit gevormd zodat het werkschema verscheidene keren per dag om 9 en 12 AM, elke dag van de week van 1 Oktober, 2023 tot 1 Januari, 2024 begint.

![](../assets/workflow-scheduler2.png)



