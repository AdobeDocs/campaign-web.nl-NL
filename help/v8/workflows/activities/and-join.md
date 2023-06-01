---
audience: end-user
title: De activiteit van de AND-join-workflow gebruiken
description: Leer hoe u de workflowactiviteit AND-join gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: 6ed2c73a5348871348ec4cbdd89fc8119fdbc718
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 1%

---


# AND-join {#join}

De **En-join** Met activiteit kunt u meerdere uitvoertakken van een workflow synchroniseren.

De EN-toetreden activiteit teweegbrengt slechts zijn uitgaande overgang teweeg zodra alle binnenkomende overgangen, met andere woorden, worden geactiveerd zodra alle voorafgaande activiteiten hebben gebeëindigd.

## Configuratie

Voer de volgende stappen uit om de **AND-join** activiteit:

1. Meerdere activiteiten toevoegen, zoals **Combineren** activiteiten om ten minste twee verschillende uitvoerende bijkantoren te vormen.
1. Een **AND-join** activiteiten aan een van de bijkantoren.
1. In de **Samenvoegopties** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.
1. Selecteer **Primaire set** in de uitgaande overgang worden gehouden.

## Voorbeeld

In het volgende voorbeeld worden twee workflowvertakkingen getoond met een e-mail- en sms-levering. EN-toetreden zal teweegbrengen wanneer beide binnenkomende overgangen worden toegelaten. De pushberichten worden dan pas verzonden nadat beide leveringen zijn voltooid.

![](../assets/workflow-andjoin-example.png)