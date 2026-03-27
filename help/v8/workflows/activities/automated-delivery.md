---
audience: end-user
title: Activiteit geautomatiseerde leveringswerkstroom
description: Meer informatie over het gebruik van de workflowactiviteit voor geautomatiseerde levering
exl-id: a9c485f1-0369-414d-9e43-bedb0390a2f5
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Geautomatiseerde levering {#automated-delivery}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Geautomatiseerde leveringsactiviteit"
>abstract="De activiteit van de geautomatiseerde leveringswerkstroom is nu beschikbaar in het werkschemapalet. U kunt het gebruiken om leveringsacties (voorbereidingen treffen, een proef verzenden, voorbereidingen treffen en beginnen, enz.) direct binnen uw werkschema tot stand te brengen of uit te voeren."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"

>[!CONTEXTUALHELP]
>id="acw_orchestration_automated-delivery"
>title="Geautomatiseerde leveringsactiviteit"
>abstract="De **Geautomatiseerde levering** activiteit wordt gebruikt voor automatisering: creeer of hergebruik een levering in uw werkschema, dan kies de actie om uit te voeren (voorbereidingen treffen, voorbereidingen treffen en beginnen, verzendt proef, enz.). U kunt een bestaande expliciete levering selecteren die buiten het werkschema wordt gecreeerd, of een nieuwe levering van een malplaatje creëren telkens als de activiteit loopt."

De **Geautomatiseerde levering** activiteit laat u, leveringsacties direct binnen uw werkschema creëren vormen en uitvoeren. Gebruik het wanneer u een vooraf bepaalde levering op een programma of als deel van een geautomatiseerde stroom wilt in werking stellen, of wanneer u een nieuwe levering van een malplaatje wilt produceren telkens als de activiteit loopt.

<!--
**[Continuous delivery](continuous-delivery.md)** always uses a template. The first run creates one delivery; later runs send to new recipients through that same delivery. **Automated delivery** is different: you either reuse one existing delivery every run, or you create a new delivery from a template each time—so each run can be its own delivery if you want. -->

Voer de volgende stappen uit om deze activiteit te configureren:

1. Bepaal de leveringsmontages, [ lees meer ](#delivery-settings)
1. Selecteer de uit te voeren actie, [ lees meer ](#action-to-execute)
1. Opstelling de overgang, [ lees meer ](#transition-to-execute)
1. Bepaal een wijzigingsmanuscript, [ lees meer ](#script)

## De leveringsinstellingen definiëren {#delivery-settings}

Wanneer u de activiteit vormt, kiest u waar de levering uit komt. In deze sectie zijn twee opties beschikbaar:

![ Screenshot die de geautomatiseerde levering ](../assets/automated-delivery.png){zoomable="yes"} tonen

* Selecteer **Expliciete levering** wanneer u op een bestaande levering, bijvoorbeeld een stand-alone levering of een levering wilt handelen die van een campagne wordt gecreeerd. Kies de levering gebruikend **Uitgezochte levering** knoop. Telkens als de werkschemalooppas en deze activiteit bereikt, handelt het op **de zelfde** levering. Er wordt geen nieuwe levering gemaakt per uitvoering. De activiteit gebruikt dezelfde levering opnieuw. Dit is nuttig wanneer u één enkele levering hebt die u wilt voorbereiden of herhaaldelijk verzenden, bijvoorbeeld op een programma of na een goedkeuringsstap.

<!-- by default, the list shows unfinished deliveries in the Deliveries folder. You can browse other folders to select a delivery from another campaign. You choose the action to perform (prepare, prepare and start, send a proof, and so on).-->

* Selecteer **Nieuw, die van een malplaatje** wordt gecreeerd wanneer u a **nieuwe** levering wilt worden gecreeerd telkens als de activiteitenlooppas. Kies het leveringsmalplaatje gebruikend het **Uitgezochte malplaatje** knoop. Elke uitvoering genereert een nieuwe levering op basis van die sjabloon. Gebruik dit wanneer elke uitvoering van de workflow een eigen, afzonderlijke levering moet opleveren (bijvoorbeeld één e-mail per uitvoering).

<!-- Unlike the Continuous delivery activity, there is no “append” to a previous execution—each run produces a separate delivery. -->

>[!NOTE]
>
>**specificeerde in de overgang** en **die door manuscript** opties wordt verwerkt, voor geavanceerde gebruiksgevallen wordt gebruikt, kan slechts in de Console van de Cliënt worden gevormd. Zie de [ documentatie van de Campagne v8 ](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/wf-activities/action-activities/delivery){target="_blank"}.

## Selecteer de uit te voeren actie {#action-to-execute}

Kies in deze sectie wat de activiteit doet met de levering. De volgende opties zijn beschikbaar:

![ Schermschot die de acties tonen in de geautomatiseerde levering uit te voeren ](../assets/automated-delivery2.png){zoomable="yes"}

* **sparen**: Creeert en bewaart de levering zonder het te analyseren of te verzenden.
* **Schatting het doel**: Berekent het leveringsdoel om zijn potentieel (eerste analysefase) te beoordelen.
* **voorbereidt**: Lanceert de volledige analyse (doelberekening en inhoudsvoorbereiding). De levering wordt niet verzonden.
* **verzend een proef**: Verzendt een bewijs van de levering.
* **voorbereidingen treffen en beginnen**: Lanceert de volledige analyse (doelberekening en inhoudsvoorbereiding) en verzendt de levering.

## De overgang instellen {#transition-to-execute}

In deze sectie kunt u kiezen of u na de activiteit overgangen wilt genereren. De volgende opties zijn beschikbaar:

![ Schermafbeelding die de overgangen in de geautomatiseerde levering tonen ](../assets/automated-delivery3.png){zoomable="yes"}

* **produceer een uitgaande overgang**: Produceert een uitgaande overgang wanneer de activiteit eindigt.
* **etiket van de Overgang**: Staat u toe om het etiket aan te passen dat op de overgang in het canvas wordt getoond.
* **de fouten van het Proces**: Voegt een extra overgang voor de behandeling van fouten toe.

## Een wijzigingsscript definiëren {#script}

U kunt een manuscript gebruiken om het gedrag van de activiteit, bijvoorbeeld, leveringsparameters zoals het activiteitenetiket te veranderen. Gebruik deze optie wanneer u aangepaste logica voor deze activiteit nodig hebt.

Klik **creeer manuscript** en schrijf uw wijzigingslogica in de redacteur.

## Verwante onderwerpen {#related}

* [Workflowactiviteiten](about-activities.md)
* [Doorlopende levering](continuous-delivery.md)
* [Activiteiten op het gebied van e-mail, sms, pushberichten, direct mail](channels.md)
* [Afleveringssjablonen](../../msg/delivery-template.md)
