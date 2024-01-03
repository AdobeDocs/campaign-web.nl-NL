---
audience: end-user
title: Een publiek maken met de bouwer van de campagneregel
description: Leer hoe te met de regelbouwer te werken
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
badge: label="Beta"
source-git-commit: a53f33360f0dc7ca80b235bd5814fd3ccc0ff698
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Werken met de regelbouwer {#segment-builder}

De regelbouwer staat u toe om de bevolking te bepalen die door uw levering wordt gericht door gegevens te filtreren in het gegevensbestand. U kunt het gebruiken om een publiek of van een werkschema te bouwen gebruikend **[!UICONTROL Build audience]** of rechtstreeks wanneer u een levering maakt om een eenmalig publiek te maken.

* [Leer hoe u een publiek kunt maken](create-audience.md)
* [Leer hoe u een eenmalig publiek voor een levering kunt maken](one-time-audience.md)

## Het palet

Het palet aan de linkerkant bevat alle elementen waarop u kunt filteren om een publiek te maken. U kunt de zoekbalk gebruiken om snel naar elementen te zoeken. De tegels in het palet moeten naar het middelste canvas worden verplaatst om geconfigureerd en meegenomen te kunnen worden.

![](assets/segment-builder2.png){width="70%" align="left"}

Het palet bestaat uit twee tabbladen:

* **Attributen**: op dit tabblad hebt u toegang tot alle beschikbare velden via het schema. De lijst met velden is afhankelijk van het doelschema dat in de e-mailsjabloon is gedefinieerd.

* **Soorten publiek**: op dit tabblad kunt u filteren met een van de bestaande soorten publiek die zijn gedefinieerd in de Campaign Classic-console of vanuit Adobe Experience Platform. [Leer hoe u het publiek kunt bewaken en beheren](manage-audience.md)

  >[!NOTE]
  >
  >Om het publiek van Adobe Experience Platform te hefboomwerking, moet u de integratie met Doelen vormen. Zie de [Adobe Experience Platform-bestemmingsdocumentatie](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=nl){target="_blank"}.

## Het canvas

Het canvas is de centrale zone waarin u regels kunt configureren en combineren op basis van de elementen die vanuit het palet worden toegevoegd. Als u een nieuwe regel wilt toevoegen, sleept u een tegel uit het palet en zet u deze neer op het canvas. Vervolgens kunt u contextspecifieke opties weergeven, afhankelijk van het type gegevens dat wordt toegevoegd.

![](assets/segment-builder4.png){width="70%" align="left"}

## Het deelvenster Eigenschappen van regel

Aan de rechterkant **Eigenschappen van Rule** kunt u de hieronder vermelde handelingen uitvoeren.

![](assets/segment-builder5.png){width="70%" align="left"}

* **Resultaten weergeven:** geeft de lijst weer van ontvangers die het doelpubliek als doel heeft.
* **Codeweergave**: geeft een op code gebaseerde versie van het publiek in SQL weer.
* **Geavanceerde kenmerken weergeven**: controleer deze optie als u de volledige lijst met kenmerken in het linkerpalet wilt weergeven: knooppunten, groepen, 1-1 koppelingen, 1-N koppelingen.
* **Berekenen**: werkt bij en toont het aantal profielen die door uw vraag worden bedoeld.
* **Filter selecteren of opslaan**: gebruik een vooraf gedefinieerd filter om de query te filteren of sla de query op als een nieuw filter voor toekomstig hergebruik. [Leer hoe u met vooraf gedefinieerde filters werkt](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >In die versie van het product zijn sommige vooraf gedefinieerde filters niet beschikbaar in de gebruikersinterface. U kunt ze nog steeds gebruiken. [Meer informatie](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations)

* **Attributen**: geeft een beschrijving van het gemaakte publiek weer.

## Voorbeeld

In dit voorbeeld bouwen we een publiek dat gericht is op alle klanten die in Atlanta of Seattle wonen en na 1980 geboren zijn.

1. In de **Attributen** tabblad van het palet, zoekt u naar de **Geboortedatum** veld. Sleep de tegel naar het canvas.

   ![](assets/segment-builder6.png)

1. Kies op het canvas de optie **Na** en voert u de gewenste datum in.

   ![](assets/segment-builder7.png)

1. Zoek in het palet naar de **Plaats** en voeg het toe aan het canvas onder de eerste regel.

   ![](assets/segment-builder8.png)

1. Voer in het tekstveld de naam van de eerste plaats in en druk op Enter.

   ![](assets/segment-builder9.png)

1. Herhaal deze handeling voor de tweede plaatsnaam.

   ![](assets/segment-builder10.png)

1. Klikken **Resultaten weergeven** om de lijst en het aantal ontvangers te tonen die de vraag aanpassen. U kunt ook kolommen toevoegen om de gegevens te visualiseren en te controleren. Voeg in ons voorbeeld de opdracht **Plaats** kolom en zie Atlanta en Seattle.

   ![](assets/segment-builder11.png)

1. Klikken **Bevestigen**.