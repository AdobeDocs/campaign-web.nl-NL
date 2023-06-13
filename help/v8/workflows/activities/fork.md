---
audience: end-user
title: De werkstroomactiviteit voor vork gebruiken
description: Leer hoe u de vorkworkflowactiviteit kunt gebruiken
badge: label="Alpha"
source-git-commit: fb6e389c25aebae8bfc17c4d88e33273aac427dd
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 18%

---


# Vertakking {#fork}

>[!CONTEXTUALHELP]
>id="acw_orchestration_fork_transitions"
>title="Vorkactiviteit"
>abstract="Met de activiteit Vertakking kunt u uitgaande overgangen maken om verschillende activiteiten tegelijk te starten."

## Configuratie

Voer de volgende stappen uit om de **Vork** activiteit:

1. Voeg een **Vork** activiteit aan uw werkschema.
1. Klikken **Overgang toevoegen** om een nieuwe uitgaande overgang toe te voegen. Standaard zijn twee overgangen gedefinieerd.
1. Voeg een label toe aan elk van uw overgangen.

## Voorbeeld

In het volgende voorbeeld gebruiken we twee **Vork** activiteiten:

* Eén voor de twee query&#39;s, om deze tegelijk uit te voeren.
* Eén na de doorsnede om een e-mail en een sms tegelijk naar de doelgroep te sturen.

![](../assets/workflow-fork-example.png)

