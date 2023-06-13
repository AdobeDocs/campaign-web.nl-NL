---
audience: end-user
title: De workflowactiviteit voor het publiek van Build gebruiken
description: Leer hoe u de workflowactiviteit voor het publiek van Build gebruikt
badge: label="Alpha" type="Positief"
source-git-commit: bbebd9dc462a189618cbf6e71467bb0935e1317a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---


# publiek opbouwen {#build-audience}

De **publiek opbouwen** activiteit is **Doelstelling** activiteit. Met deze activiteit kunt u het publiek definiëren dat de workflow zal betreden. Wanneer het verzenden van berichten in de context van een campagnewerkschema, wordt het berichtpubliek niet bepaald in de kanaalactiviteit, maar in **publiek opbouwen** activiteit.

Om de publieksbevolking te bepalen, kunt u:

* Selecteer een bestaand publiek dat als een lijst in de cliëntconsole wordt gecreeerd.
* Selecteer een Adobe Experience Platform-publiek.
* Bouw een nieuw publiek met de regelbouwer door het filtreren criteria te bepalen en te combineren.

>[!NOTE]
>
>In deze context kunt u geen publiek uit een bestand laden. Hiervoor moet u een zelfstandige levering maken. [Meer informatie](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Configuratie

Voer de volgende stappen uit om de **publiek opbouwen** activiteit:

1. Voeg een **publiek opbouwen** activiteit.
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

Hier is een voorbeeld van een workflow met twee **publiek opbouwen** activiteiten. De eerste is gericht op het publiek van pokerspelers, gevolgd door een e-mailbezorging. De tweede is gericht op het publiek van VIP klanten, gevolgd door een SMS-levering.

![](../assets/workflow-audience-example.png)