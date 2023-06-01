---
audience: end-user
title: De workflowactiviteit voor het publiek van Build gebruiken
description: Leer hoe u de workflowactiviteit voor het publiek van Build gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: 9b639a533e75822570d6cc2b9752fc9380d069dd
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# publiek opbouwen {#build-audience}

Met deze activiteit kunt u een publiek definiëren. U kunt of een bestaand publiek selecteren of de regelbouwer gebruiken om uw eigen vraag te bepalen.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuratie

Voer de volgende stappen uit om de **publiek opbouwen** activiteit:

1. Voeg een de publieksactiviteit van de Bouwstijl toe.
1. Definieer een label.
1. Bepaal het publiekstype: **Maak uw eigen** of **Lees publiek**.

Voer de volgende extra stappen uit om uw eigen query te maken:

1. Selecteren **Uw eigen (query) maken**.
1. Kies de optie **Doeldimensie**. Met de doeldimensie kunt u de doelgroep voor de bewerking definiëren: ontvangers, begunstigden van contracten, exploitanten, abonnees, enz. Standaard is het doel geselecteerd bij de ontvangers. Zie de [v8-documentatie](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Klikken **Doorgaan**.
1. Gebruik de bouwer van de regel om uw vraag te bepalen, de zelfde manier u creeert een publiek wanneer het ontwerpen van een nieuwe e-mail. Zie dit [sectie](../../audience/segment-builder.md).

Voer de volgende stappen uit om een bestaand publiek te selecteren:

1. Selecteren **Lees publiek**.
1. Klikken **Doorgaan**.
1. Selecteer uw publiek, zoals u een publiek gebruikt bij het ontwerpen van een nieuwe e-mail. Zie dit [sectie](../../audience/add-audience.md).

## Voorbeeld

Hier is een voorbeeld van een worststroom met twee **publiek opbouwen** activiteiten. De eerste is gericht op het publiek van pokerspelers, gevolgd door een e-mailbezorging. De tweede is gericht op het publiek van VIP klanten, gevolgd door een SMS-levering.

![](../assets/workflow-audience-example.png)