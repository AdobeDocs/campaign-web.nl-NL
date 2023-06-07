---
audience: end-user
title: De werkstroomactiviteit voor vork gebruiken
description: Leer hoe u de vorkworkflowactiviteit kunt gebruiken
badge: label="Alpha" type="Positief"
source-git-commit: 55a5d09dcd8d98f7a848b2e4ace388e54f6f896e
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 2%

---


# Vertakking {#fork}

De **Vork** activiteit is **Stroomregeling** activiteit. Het staat u toe om uitgaande overgangen tot stand te brengen om verscheidene activiteiten tezelfdertijd te beginnen.

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

