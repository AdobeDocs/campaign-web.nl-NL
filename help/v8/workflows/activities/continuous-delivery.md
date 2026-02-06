---
audience: end-user
title: Activiteit van de doorlopende leveringsworkflow gebruiken
description: Leer hoe u de activiteit van de workflow voor continue levering gebruikt
exl-id: 659bddcb-280c-4623-8115-6f975515d1a2
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Doorlopende levering {#continuous-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Continue leveringsactiviteit"
>abstract="U kunt nu nieuwe ontvangers toevoegen aan een bestaande levering. Dit leveringstype vermijdt het moeten een nieuwe levering tot stand brengen telkens als, die het voor laagvolumealarm of berichten efficiënter maakt die worden verzonden zoals nodig."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=nl-NL" text="Zie opmerkingen bij releases"

De **Ononderbroken levering** activiteit staat u toe om nieuwe ontvangers aan een bestaande levering toe te voegen. Dit leveringstype vermijdt het moeten een nieuwe levering tot stand brengen telkens als, die het voor laagvolumealarm of berichten efficiënter maakt die worden verzonden zoals nodig.

Een ononderbroken levering leidt tot één enkele leveringsinstantie. Alle leveringslogbestanden (wideLog) en trackinglogboeken verwijzen naar deze ene levering, waardoor de bewaking en rapportage worden vereenvoudigd.

## Vorm de Ononderbroken leveringsactiviteit {#configure}

1. Voeg a **Ononderbroken levering** activiteit aan uw werkschemacanvas toe.

   ![&#x200B; Schermafbeelding die de Ononderbroken leveringsactiviteit &#x200B;](../assets/continuous-delivery.png){zoomable="yes"} tonen

1. Voer een aangepaste waarde **[!UICONTROL Label]** in voor de activiteit (optioneel). Standaard krijgt deze het label &quot;Continue levering&quot;.

1. Klik naast het veld **[!UICONTROL Template]** op het zoekpictogram om een leveringssjabloon te selecteren. Alleen sjablonen (geen standaardleveringen) zijn beschikbaar voor selectie. De sjabloon definieert het leveringskanaal, de inhoud en de configuratie.

1. Kies in de **[!UICONTROL Targeting options]** hoe de doelpopulatie wordt gedefinieerd:

   * **[!UICONTROL Specified by the inbound events]**: het doel komt uit de binnenkomende overgang (van upstream activiteiten zoals het publiek van de Bouwstijl of Incrementele query). Dit is de meest voorkomende optie.

   * **[!UICONTROL Specified in the delivery template]**: Het doel wordt gedefinieerd in de sjabloon zelf.

   * **[!UICONTROL File specified in the input event]**: Het doel wordt opgegeven via een bestand dat door de workflow wordt doorgegeven.

De ononderbroken leveringsactiviteit produceert automatisch een uitgaande overgang om uw werkschema voort te zetten.

## Verwante onderwerpen {#related}

* [Workflowactiviteiten](about-activities.md)
* [Activiteiten op het gebied van e-mail, sms, pushberichten, direct mail](channels.md)
* [Afleveringssjablonen](../../msg/delivery-template.md)
