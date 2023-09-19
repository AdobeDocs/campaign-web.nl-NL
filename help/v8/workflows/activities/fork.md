---
audience: end-user
title: De werkstroomactiviteit voor vork gebruiken
description: Leer hoe u de vorkworkflowactiviteit kunt gebruiken
badge: label="Beta"
source-git-commit: dfd3c62a8eeb6be3e5e63e7a1fdf352c280adbd0
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 1%

---


# Vertakking {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork"
>title="Vorkactiviteit"
>abstract="De **Vork** de activiteit staat u toe om uitgaande overgangen tot stand te brengen om verscheidene activiteiten tezelfdertijd te beginnen."


>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Overgangen naar vorkactiviteit"
>abstract="Standaard worden twee overgangen gemaakt met een **Vork** activiteit. Klik op de knop **Overgang toevoegen** om een extra uitgaande overgang te bepalen, en zijn etiket in te gaan."

De **Vork** activiteit is **Stroomregeling** activiteit. Het staat u toe om uitgaande overgangen tot stand te brengen om verscheidene activiteiten tezelfdertijd te beginnen.

## De vorkactiviteit configureren{#fork-configuration}

Voer de volgende stappen uit om de **Vork** activiteit:

![](../assets/workflow-fork.png)

1. Voeg een **Vork** activiteit aan uw werkschema.
1. Klikken **Overgang toevoegen** een nieuwe uitgaande overgang toevoegen. Standaard zijn twee overgangen gedefinieerd.
1. Voeg een label toe aan elk van uw overgangen.

## Voorbeeld{#fork-example}

In het volgende voorbeeld gebruiken we twee **Vork** activiteiten:

* Eén voor de twee query&#39;s, om deze tegelijk uit te voeren.
* Eén na de doorsnede om een e-mail en een sms tegelijk naar de doelgroep te sturen.

![](../assets/workflow-fork-example.png)

