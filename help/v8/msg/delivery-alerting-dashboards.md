---
audience: end-user
title: Afleveringswaarschuwing
description: Leer hoe u werkt met waarschuwingsberichten voor leveringen.
exl-id: b91ef82b-f3e9-4704-87a2-0e3f75104572
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 0%

---

# Waarschuwingsdashboards {#delivery-alerting-dashboards}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Dashboards voor leveringswaarschuwingen"
>abstract="De Alerting van de levering is een waakzaam beheersysteem dat groepen gebruikers toelaat om e-mailberichten met informatie over hun levering automatisch te ontvangen uitvoeren. Met de Dashboards voor leveringswaarschuwingen kunt u opgeven wie e-mailwaarschuwingen ontvangt, de waarschuwingscriteria voor het verzenden van deze waarschuwingen kiezen en configureren en de geschiedenis van alle verzonden berichten openen."

Met de Dashboards voor leveringswaarschuwingen kunt u opgeven wie e-mailwaarschuwingen ontvangt, de waarschuwingscriteria voor het verzenden van deze waarschuwingen kiezen en configureren en de geschiedenis van alle verzonden berichten openen. Zij zijn toegankelijk van het **Waarschuwende van de Levering** menu in de linkernavigatieruit, onder de **dashboards** tabel.

![](assets/alerting-dashboard-list.png)

## Een leveringsdashboard maken {#dashboards}

>[!CONTEXTUALHELP]
>id="acw_delery_alerting_dashboard_create"
>title="Waarschuwingsdashboard voor levering maken"
>abstract="Als u een dashboard voor bezorgingswaarschuwingen maakt, kunt u opgeven wie e-mailwaarschuwingen ontvangt, de waarschuwingscriteria kiezen en configureren die moeten worden gebruikt om deze waarschuwingen te verzenden en toegang krijgen tot de geschiedenis van alle verzonden meldingen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Algemene parameters voor leveringswaarschuwingen"
>abstract="Geef de algemene eigenschappen van het dashboard voor leveringswaarschuwingen op. In het **veld Waarschuwingsgroep** selecteren kunt u de **operatorgroep** opgeven die de waarschuwingen moet ontvangen die door dit dashboard worden verzonden."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Criteria voor waarschuwingen voor weergave"
>abstract="Voeg in deze sectie criteria toe die u wilt gebruiken om waarschuwingen vanuit dit dashboard te verzenden. Kies uit vooraf gedefinieerde criteria of creëer uw eigen criteria om af te stemmen op specifieke behoeften."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Criteria parameters"
>abstract="Criteria hebben standaardparameterwaarden die bepalen hoe ze moeten worden toegepast. U kunt deze waarden in dit gedeelte aanpassen aan uw behoeften."

Volg deze stappen om een bezorgingsdashboard te maken:

1. Navigeer naar het **menu Leveringswaarschuwingen** in het linkernavigatiedeelvenster en klik op **Bezorgingsdashboard** maken.

   ![](assets/alerting-dashboard.png)

1. Geef uw dashboard een naam in het **veld Label** . Het **Interne naamgebied** is automatisch bevolkt en read-only.

1. Op het **Uitgezochte waakzame groep** gebied, specificeer de **exploitantgroep** om het alarm te ontvangen dat door dit dashboard wordt verzonden. Alle leden van de geselecteerde operatorgroep ontvangen de waarschuwingen.

   Leer meer op toestemmingen en exploitantgroepen in [ Adobe Campaign v8 (console) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}

1. Voeg in de **sectie Waarschuwingscriteria** voor levering criteria toe die u wilt gebruiken om waarschuwingen te verzenden. Kies uit vooraf gedefinieerde criteria of creëer uw eigen criteria om af te stemmen op specifieke behoeften. [Leer werken met criteria](../msg/delivery-alerting-criteria.md)

1. De criteria hebben standaardparameterwaarden die bepalen hoe zij moeten worden toegepast. U kunt deze waarden veranderen om uw behoeften van de **sectie van de Parameters van Criteria** aan te passen.

   ![](assets/alerting-criteria-parameters.png)

   Bijvoorbeeld, door gebrek, wordt de **parameter van het 0} doel van de Levering minimumgrootte {aan 50 geplaatst, betekenend dat een levering in het alarm zal worden inbegrepen dat door dit dashboard wordt verzonden slechts als het minstens 50 profielen richt.** U kunt deze parameter wijzigen als u leveringen wilt opnemen die betrekking hebben op minder dan 50 profielen.

   Vouw de onderstaande sectie uit voor meer informatie over elke parameter criteria:

   +++Beschikbare parameters

   * **het doel minimumgrootte van de Levering**: Bijvoorbeeld, als u 100 op dit gebied ingaat, wordt een bericht verzonden slechts voor leveringen met een doel gelijk aan of groter dan 100 ontvangers. Deze parameter is van toepassing op alle criteria.
   * **Monitoringperiode voor en na de contactdatum (in uren):** Aantal uren voor en na de huidige tijd. Alleen de leveringen met een contactdatum in deze periode worden in aanmerking genomen. Deze parameter is van toepassing op alle criteria. Standaard is de waarde van dit veld ingesteld op 24 uur.
   * **Maximale verhouding van soft bounce-fouten**: Er wordt een melding verzonden voor alle leveringen met een soft bounce-foutratio die groter is dan de opgegeven waarde. Standaard is de waarde van dit veld ingesteld op 0,05 (5%).
   * **Maximale verhouding van harde bouncefouten**: Er wordt een melding verzonden voor alle leveringen met een harde bouncefout die groter is dan de opgegeven waarde. Standaard is de waarde van dit veld ingesteld op 0,05 (5%).
   * **Minimale tijdsdrempel voor levering in de status &#39;Start in behandeling&#39; (in minuten)**: Er wordt een melding verzonden voor alle leveringen met de status Start pending voor langer dan de duur die in dit veld is opgegeven, met de status Start pending betekent dat de berichten nog niet in aanmerking zijn genomen door het systeem.
   * **Minimale tijd die nodig is voor de berekening van de doorvoer (in minuten):** Alleen leveringen die langer dan de opgegeven duur zijn gestart (met de status In uitvoering) worden in aanmerking genomen voor het criterium Leveringen met een lage doorvoer.
   * **Maximaal percentage verwerkte berichten voor de berekening van de doorvoer**: Alleen leveringen met een percentage verwerkte berichten dat lager is dan het opgegeven percentage worden meegeteld voor het criterium Leveringen met lage doorvoer.
   * **Minimale verwachte debiet (in verzonden berichten per uur):** Alleen leveringen met een doorvoer lager dan de opgegeven waarde worden in aanmerking genomen voor het criterium Leveringen met een lage doorvoer.
   * **Minimale verwerkte ratio vereist voor het criterium** &#39;Leveringen in uitvoering&#39;: Alleen leveringen met een percentage verwerkte berichten dat hoger is dan het opgegeven percentage worden in aanmerking genomen.

+++

1. Standaard zijn waarschuwingsdashboards uitgeschakeld. Dit houdt in dat e-mailwaarschuwingen die aan dit dashboard zijn gekoppeld, niet worden verzonden. Om het dashboard toe te laten onmiddellijk, knevel **Toegelaten** optie in de **Algemene** sectie, naast het gebied van de waakzame groepsselectie.

   U kunt het dashboard ook opslaan en later inschakelen.

   ![](assets/alerting-dashboard-enable.png)

1. Als u het waarschuwingsdashboard wilt opslaan, klikt u op de **knop Opslaan** .

Het waarschuwingsdashboard wordt geopend met lege gegevens. Wanneer u klaar bent om het te activeren en meldingen te verzenden, klikt u op de **knop Instellingen** en schakelt u de **optie Ingeschakeld** in als u dit nog niet eerder hebt gedaan.

Telkens wanneer een levering voldoet aan de criteria die in dit dashboard zijn gedefinieerd, wordt een waarschuwingsbericht verzonden naar de opgegeven operatorgroep.

## Dashboards voor waarschuwingen beheren

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Bezorgingswaarschuwingen verzonden"
>abstract="In dit gedeelte kunt u informatie visualiseren met betrekking tot de meest recente verzonden waarschuwingen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Geschiedenis van bezorgingswaarschuwingen"
>abstract="Het **deelvenster Geschiedenis** bevat alle waarschuwingen die vanuit dit dashboard zijn verzonden. Klik op een item om toegang te krijgen tot de bijbehorende waarschuwingen die op dat specifieke moment zijn verzonden."

Alle gemaakte waarschuwingsdashboards zijn toegankelijk via het **menu Delivery Alerting** op het **tabblad Dashboards** .

![](assets/alerting-dashboard-list.png)

U kunt een dashboard dupliceren of verwijderen met behulp van de knop Meer acties **naast de** naam.

Om toegang te krijgen tot een gedetailleerde weergave van een dashboard, klikt u op de naam in de lijst. Vanuit dit scherm kunt u de laatst verzonden waarschuwing visualiseren. Alle verzonden waarschuwingen worden weergegeven in het linkerdeelvenster. Klik op een item om toegang te krijgen tot de bijbehorende waarschuwingen die op dat specifieke moment zijn verzonden.

![](assets/alerting-dashboard-details.png)

Om het dashboard uit te geven, klik de **knoop van Montages** in de hoger-juiste hoek en breng de gewenste veranderingen aan.
