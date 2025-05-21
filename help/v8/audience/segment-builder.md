---
audience: end-user
title: Een publiek maken met de bouwer van de campagneregel
description: Leer hoe te met de regelbouwer te werken
exl-id: 167ad4ce-3760-413c-9949-9649245766e3
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# Werken met de regelbouwer {#segment-builder}

De regelbouwer laat u de bevolking bepalen die door uw levering wordt gericht door gegevens te filtreren in het gegevensbestand. Met deze methode kunt u een publiek maken op basis van een workflow met een **[!UICONTROL Build audience]** -activiteit of rechtstreeks wanneer u een levering maakt om een eenmalig publiek te maken.

* [Leer hoe u een publiek kunt maken en opslaan](create-audience.md)
* [Leer hoe u een eenmalig publiek voor een levering kunt maken](one-time-audience.md)

## Het palet

Het palet, dat zich aan de linkerkant bevindt, bevat alle elementen waarop u kunt filteren om een publiek te maken. Gebruik de zoekbalk om snel elementen te zoeken. Verplaats de tegels in het palet naar het middelste canvas om ze te configureren en er rekening mee te houden.

![ de paletinterface die het filtreren opties en lusjes toont ](assets/segment-builder2.png){zoomable="yes"}{width="70%" align="left"}

Het palet bestaat uit twee tabbladen:

* **Attributen**: Dit lusje verleent toegang tot alle beschikbare gebieden van het schema. De lijst met velden is afhankelijk van het doelschema dat in de e-mailsjabloon is gedefinieerd.

* **Soorten publiek**: Dit lusje laat u filtreren gebruikend één van het bestaande publiek dat in de console van Campaign Classic of van Adobe Experience Platform wordt bepaald. Leer hoe te om publiek in [ te controleren en te beheren deze sectie ](manage-audience.md).

  >[!NOTE]
  >
  >Om het publiek van Adobe Experience Platform te gebruiken, vorm de integratie met Doelen. Verwijs naar de [ documentatie van de Doelen van Adobe Experience Platform ](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html?lang=nl){target="_blank"}.

## Het canvas

Het canvas is de centrale zone waar u regels kunt configureren en combineren op basis van de elementen die vanuit het palet worden toegevoegd. Als u een nieuwe regel wilt toevoegen, sleept u een tegel uit het palet en zet u deze neer op het canvas. Contextspecifieke opties worden weergegeven op basis van het type gegevens dat wordt toegevoegd.

![ de interface van het canvas die opties van de regelconfiguratie toont ](assets/segment-builder4.png){zoomable="yes"}{width="70%" align="left"}

## Het deelvenster Eigenschappen van regel

Aan de rechterkant, laat de **eigenschappen van de Regel** ruit u de hieronder vermelde acties uitvoeren.

![ de ruit van regeleigenschappen die beschikbare acties ](assets/segment-builder5.png){zoomable="yes"}{width="70%" align="left"} tonen

* **resultaten van de Mening:** toont de lijst van profielen die door het publiek worden gericht.
* **mening van de Code**: Toont een op code-gebaseerde versie van het publiek in SQL.
* **Geavanceerde attributen van de Vertoning**: Controle deze optie om de volledige lijst van attributen in het linkerpalet, met inbegrip van knopen, groeperingen, 1-1 verbindingen, en 1-N verbindingen te bekijken.
* **berekent**: Updates en toont het aantal profielen die door uw vraag worden gericht.
* **Uitgezocht of sparen filter**: Gebruik een vooraf bepaald filter om uw vraag te filtreren, of sparen uw vraag als nieuw filter voor toekomstig hergebruik. [ Leer hoe te met vooraf bepaalde filters ](../get-started/predefined-filters.md) te werken.

  >[!IMPORTANT]
  >
  >In deze versie van het product zijn sommige vooraf gedefinieerde filters niet beschikbaar in de gebruikersinterface. U kunt ze nog steeds gebruiken. [Meer informatie](../get-started/guardrails.md#predefined-filters-filters-guardrails-limitations).

* **Attributen**: Toont een beschrijving van het gecreeerde publiek.

## Voorbeeld

In dit voorbeeld is een publiek gebouwd dat gericht is op alle klanten die in Atlanta of Seattle wonen en na 1980 geboren zijn.

1. In het **lusje van Attributen** van het palet, onderzoek naar de **Datum van geboorte** gebied. Sleep de tegel naar het canvas.

   ![ Toevoegend de Datum van geboortegebied aan het canvas ](assets/segment-builder6.png){zoomable="yes"}

1. In het canvas, kies **na** exploitant en ga de gewenste datum in.

   ![ Vormend de Na exploitant voor de Datum van geboortegebied ](assets/segment-builder7.png){zoomable="yes"}

1. In het palet, onderzoek naar het **gebied van de Stad** en voeg het aan het canvas onder de eerste regel toe.

   ![ Toevoegend het gebied van de Stad aan het canvas ](assets/segment-builder8.png){zoomable="yes"}

1. Voer in het tekstveld de naam van de eerste plaats in en druk op Enter.

   ![ die de eerste plaatsnaam op het gebied van de Stad ingaan ](assets/segment-builder9.png){zoomable="yes"}

1. Herhaal deze handeling voor de tweede plaatsnaam.

   ![ die de tweede plaatsnaam op het gebied van de Stad ingaan ](assets/segment-builder10.png){zoomable="yes"}

1. Klik **resultaten van de Mening** om de lijst en het aantal ontvangers te tonen die de vraag aanpassen. Voeg kolommen toe om de gegevens te visualiseren en te controleren. In dit voorbeeld, voeg de **kolom van de Stad** toe om Atlanta en Seattle te zien.

   ![ het Bekijken resultaten met de toegevoegde kolom van de Stad ](assets/segment-builder11.png){zoomable="yes"}

1. Klik **bevestigen**.