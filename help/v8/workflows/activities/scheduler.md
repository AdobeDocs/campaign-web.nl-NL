---
audience: end-user
title: De workflowactiviteit van de planner gebruiken
description: Leer hoe u de workflowactiviteit van de planner gebruikt
exl-id: 84142fbe-fd8a-4329-88a5-cf7a8f4e8b8f
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '525'
ht-degree: 9%

---

# Planner {#scheduler}


>[!CONTEXTUALHELP]
>id="acw_orchestration_scheduler"
>title="Planningsactiviteit"
>abstract="De **Planner** activiteit staat u toe om te plannen wanneer het werkschema begonnen wordt. Deze activiteit moet worden beschouwd als een geplande start. Deze kan alleen worden gebruikt als de eerste activiteit van de workflow."


De **planner** activiteit is de controle **activiteit van de a** Stroom. Hiermee kunt u plannen wanneer de workflow wordt gestart. Deze activiteit moet worden beschouwd als een geplande start. Deze kan alleen worden gebruikt als de eerste activiteit van de workflow.

## Best practices{#scheduler-best-practices}

* Plan geen workflow die meer dan om de 15 minuten wordt uitgevoerd, aangezien dit de algehele systeemprestaties kan belemmeren en blokken in de database kan maken.
* Als u één-schot levering in uw werkschema wilt verzenden, kunt u een planneractiviteit toevoegen en het plaatsen om **eens** in werking te stellen. U kunt het **Programma** in de montages van de levering ook bepalen.
* Als u een terugkomende levering in uw werkschema wilt verzenden, moet u a **Planner** activiteit gebruiken en de uitvoeringsfrequentie plaatsen. De terugkomende leveringsactiviteit staat u niet toe om een programma te bepalen.

## De planningsactiviteit configureren {#scheduler-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_validity"
>title="Geldigheid van planner"
>abstract="U kunt een geldigheidsperiode voor de planner bepalen. Deze kan permanent zijn (standaard) of geldig zijn tot een bepaalde datum."


>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Planningsopties"
>abstract="Bepaal de frequentie van de planner. Het kan op een specifiek moment, één keer of verscheidene keren per dag, week of maand worden uitgevoerd."

Volg deze stappen om de **Planner** activiteit te vormen:

![](../assets/workflow-scheduler.png)

1. Voeg a **Planner** activiteit aan uw werkschema toe.

1. Vorm de **frequentie van de Uitvoering**:

   * **Eenmaal**: het werkschema wordt uitgevoerd één keer.

   * **Dagelijks**: het werkschema wordt uitgevoerd op een specifieke tijd, eens per dag.

   * **verscheidene tijden per dag:** het werkschema wordt regelmatig uitgevoerd verscheidene keren per dag. U kunt uitvoeringen instellen op specifieke tijdstippen of periodiek.

   * **Wekelijks**: het werkschema wordt uitgevoerd op een gespecificeerd moment, eens of verscheidene tijden per week.

   * **Maandelijks**: het werkschema wordt uitgevoerd op een gespecificeerd moment, eens of verscheidene tijden per maand. U kunt aangeven in welke maanden u de workflow wilt uitvoeren. U kunt uitvoeringen ook instellen op bepaalde weekdagen van de maand, zoals de tweede dinsdag van de maand.

1. Definieer de details van de uitvoering op basis van de geselecteerde frequentie. De detailvelden variëren, afhankelijk van de gebruikte frequentie (tijd, herhalingsfrequentie, opgegeven dagen, enz.).

1. Klik **de lanceringstijden van de Voorproef** om het programma van volgende tien uitvoeringen van uw werkschema te controleren.

1. Bepaal de geldigheidsperiode van de planner:

   * **Vaste (verloopt nooit)**: het werkschema wordt uitgevoerd, volgens de gespecificeerde frequentie, zonder enige grenzen aan het tijdkader of aantal herhalingen.

   * **periode van de Geldigheid**: het werkschema wordt uitgevoerd volgens de gespecificeerde frequentie, tot een specifieke datum. U moet begin- en einddatums opgeven.

>[!NOTE]
>
>Als u het werkschema wilt onmiddellijk beginnen, kunt u **klikken voert hangende taak** in de hoogste actiebar van de planner uit. Deze knop is alleen beschikbaar wanneer u de workflow hebt gestart.

## Voorbeeld{#scheduler-example}

In het volgende voorbeeld, wordt de activiteit gevormd zodat het werkschema verscheidene keren per dag om 9 en 12 AM, elke dag van de week van 1 Oktober, 2023 tot 1 Januari, 2024 loopt.

![](../assets/workflow-scheduler2.png)
