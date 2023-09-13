---
audience: end-user
title: De workflowactiviteit van de planner gebruiken
description: Leer hoe u de workflowactiviteit van de planner gebruikt
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 30%

---


# Planner {#scheduler}

>[!CONTEXTUALHELP]
>id="acw_orchestration_schedule_options"
>title="Activiteit Planner"
>abstract="Met de planningsactiviteit kunt u..."

Met de activiteit Planner kunt u plannen wanneer een workflow of activiteit wordt gestart.

De activiteit van de Planner zou als een geplande aanvang moeten worden beschouwd. Deze activiteit kan slechts als eerste activiteit van het werkschema worden gebruikt.

## Beste praktijken

* Plan geen workflow die meer dan om de 15 minuten wordt uitgevoerd, aangezien dit de algehele systeemprestaties kan belemmeren en blokken in de database kan maken.

## Configuratie

Voer de volgende stappen uit om de **Planner** activiteit:

1. Voeg een **Planner** activiteit aan uw werkschema.

1. Vorm **Uitvoerfrequentie**:

   * Eenmaal: de workflow wordt één keer uitgevoerd.

   * Dagelijks: de workflow wordt op een bepaald tijdstip, eenmaal per dag, uitgevoerd.

   * Meerdere keren per dag: de workflow wordt regelmatig meerdere keren per dag uitgevoerd. U kunt uitvoeringen instellen op specifieke tijdstippen of periodiek.

   * Wekelijks: de workflow wordt uitgevoerd op een bepaald moment, één keer of meerdere keren per week.

   * Maandelijks: de workflow wordt uitgevoerd op een bepaald moment, één keer of meerdere keren per maand. U kunt aangeven in welke maanden u de workflow wilt uitvoeren. U kunt uitvoeringen ook instellen op de opgegeven weekdag van de maand, zoals de tweede dinsdag van de maand.
1. Definieer de details van de uitvoering op basis van de geselecteerde frequentie. De detailvelden variëren, afhankelijk van de gebruikte frequentie (tijd, herhalingsfrequentie, opgegeven dagen, enz.).

1. Klikken **Voorvertoning van opstartij** om het schema van de volgende tien uitvoeringen van uw werkschema te controleren.

1. Bepaal de geldigheidsperiode van de planner:

   * Permanent (nooit verloopt): de workflow zal worden uitgevoerd volgens de opgegeven frequentie, zonder beperkingen aan het tijdskader of het aantal herhalingen.

   * Geldigheidsperiode: de workflow wordt uitgevoerd volgens de opgegeven frequentie, tot een bepaalde datum. Hierbij moet dus de uitvoeringstermijn worden vastgesteld.

## Voorbeeld


