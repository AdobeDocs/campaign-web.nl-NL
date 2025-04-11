---
audience: end-user
title: De workflowactiviteit van de planner gebruiken
description: Leer hoe u de workflowactiviteit van de planner gebruikt
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 2%

---

# Planner {#scheduler}

>[!CONTEXTUALHELP]
>
De **planner** activiteit is de controle **activiteit van de a** Stroom. Hiermee kunt u plannen wanneer de workflow wordt gestart. Deze activiteit moet worden beschouwd als een geplande start. Deze kan alleen worden gebruikt als de eerste activiteit van de workflow.

## Best practices {#scheduler-best-practices}

* Plan geen workflow die meer dan om de 15 minuten wordt uitgevoerd, aangezien dit de algehele systeemprestaties kan belemmeren en blokken in de database kan maken.
* Om één-schot levering in uw werkschema te verzenden, voeg een planneractiviteit toe en plaats het om **eens** in werking te stellen. Bepaal het **Programma** in de montages van de levering.
* Om een terugkomende levering in uw werkschema te verzenden, gebruik a **Planner** activiteit en plaats de uitvoeringsfrequentie. De terugkomende leveringsactiviteit staat u niet toe om een programma te bepalen.

## De planningsactiviteit configureren {#scheduler-configuration}

[!CONTEXTUALHELP]

[!CONTEXTUALHELP]

Volg deze stappen om de **Planner** activiteit te vormen:

![ interface van de de activiteitenconfiguratie van de Planner ](../assets/workflow-scheduler.png)

1. Voeg a **Planner** activiteit aan uw werkschema toe.

1. Vorm de **frequentie van de Uitvoering**:

   * **Eenmaal**: Het werkschema wordt uitgevoerd één keer.
   * **Dagelijks**: Het werkschema wordt uitgevoerd op een specifieke tijd, eens per dag.
   * **verscheidene tijden a dag**: Het werkschema wordt regelmatig uitgevoerd verscheidene keren per dag. De uitvoeringen van de opstelling op specifieke tijden of periodiek.
   * **Wekelijks**: Het werkschema wordt uitgevoerd op een gespecificeerd moment, eens of verscheidene tijden per week.
   * **Maandelijks**: Het werkschema wordt uitgevoerd op een gespecificeerd moment, eens of verscheidene tijden per maand. Selecteer maanden wanneer de workflow moet worden uitgevoerd. U kunt uitvoeringen ook instellen op bepaalde weekdagen van de maand, zoals de tweede dinsdag van de maand.

1. Definieer de details van de uitvoering op basis van de geselecteerde frequentie. De detailvelden kunnen variëren afhankelijk van de gebruikte frequentie (tijd, herhalingsfrequentie, opgegeven dagen en vergelijkbare opties).

1. Klik **de lanceringstijden van de Voorproef** om het programma van volgende tien uitvoeringen van uw werkschema te controleren.

1. Bepaal de geldigheidsperiode van de planner:

   * **Vaste (verloopt nooit)**: Het werkschema wordt uitgevoerd volgens de gespecificeerde frequentie, zonder enige grenzen aan het tijdkader of aantal herhalingen.
   * **periode van de Geldigheid**: Het werkschema wordt uitgevoerd volgens de gespecificeerde frequentie, tot een specifieke datum. Begin- en einddatum opgeven.

>[!NOTE]\
Als u het werkschema wilt onmiddellijk beginnen, **voert hangende taak** in de hoogste actiebar van de planner uit. Deze knop is alleen beschikbaar wanneer de workflow is gestart.

## Voorbeeld {#scheduler-example}

In het volgende voorbeeld is de activiteit zo geconfigureerd dat de workflow verschillende keren per dag om 9 en 12 uur wordt uitgevoerd, elke dag van de week van 1 oktober 2023 tot 1 januari 2024.

![ de configuratie van het de activiteitenvoorbeeld van de Planner ](../assets/workflow-scheduler2.png)