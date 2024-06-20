---
audience: end-user
title: Afleveringswaarschuwing
description: Leer hoe u werkt met waarschuwingsberichten voor leveringen.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: bbfee1479593ff6ae3f77ef5bfd760d63e640c76
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# Beoordelingscriteria voor aflevering {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Dashboard voor leveringswaarschuwingscriteria"
>abstract="De gebruikersinterface van het Web van de campagne verstrekt vooraf bepaalde alarmerende criteria (leveringen met lage productie, leveranties de waarvan voorbereiding ontbrak...) die u aan uw dashboard kunt toevoegen. U kunt ook uw eigen criteria maken die aan uw behoeften voldoen."

De gebruikersinterface van het Web van de campagne verstrekt vooraf bepaalde alarmerende criteria (leveringen met lage productie, leveranties de waarvan voorbereiding ontbrak...) die u aan uw dashboard kunt toevoegen. U kunt ook uw eigen criteria maken die aan uw behoeften voldoen.

Waarschuwingscriteria zijn toegankelijk via de **Leveringswaarschuwing** menu in het linkernavigatievenster, onder **Criteria** tab.

![](assets/alerting-criteria-list.png)

## Vooraf gedefinieerde waarschuwingscriteria {#ootb-criteria}

Vooraf gedefinieerde waarschuwingscriteria zijn beschikbaar in de webgebruikersinterface van Campagne. Deze criteria bestrijken een reeks scenario&#39;s, die hieronder worden opgesomd:

* **Leveringen mislukt**: Elke levering die binnen een bepaald bereik is gepland, met een onjuiste status.
* **Leveringen met voorbereiding mislukt**: Elke levering die binnen een bepaald bereik is gewijzigd en waarvoor de bereidingsstap (berekening van het doel en genereren van de inhoud) is mislukt.
* **Aflevering met slechte foutverhouding voor zachte stuiteringen**: Elke levering die binnen een bepaald bereik wordt gepland, met een status die ten minste bezig is, met een soft bounce error ratio die groter is dan een bepaald percentage.
* **Aflevering met slechte foutenverhouding voor harde grenzen**: Elke levering die binnen een bepaald bereik wordt gepland, met een status die ten minste bezig is, met een harde stuiterfout-verhouding die groter is dan een bepaald percentage.
* **Leveringen met lange start in behandeling**: Elke levering die binnen een bepaald bereik is gepland, met een status in behandeling voor een periode die langer is dan een bepaalde duur, Beginnen in afwachting van status. Dit houdt in dat de berichten nog niet in aanmerking zijn genomen door het systeem.
* **Levert met lage doorvoer**: Elke levering die langer dan een bepaalde duur is gestart, met minder dan een bepaald percentage verwerkte berichten, met een doorvoer die lager is dan een gedefinieerde waarde.
* **Leveringen in uitvoering**: Elke levering die binnen een bepaald bereik is gepland, met de status In uitvoering.

>[!NOTE]
>
>De standaardwaarden worden toegepast op alle parameters voor de bovenstaande criteria. Deze waarden kunnen worden aangepast in het dialoogvenster **Criteria** sectie van de leveringsalarmerende dashboards waar zij worden gebruikt. [Leer hoe u met dashboards werkt](../msg/delivery-alerting-dashboards.md)

## Een waarschuwingscriterium maken {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Waarschuwingscriteria voor levering maken"
>abstract="Naast de vooraf gedefinieerde waarschuwingscriteria van Adobe Campaign kunt u zelf criteria maken die aan uw behoeften voldoen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicatoren die moeten worden toegevoegd aan signaleringen"
>abstract="Selecteer de indicatoren die u als kolommen wilt weergeven in de sectie &quot;Details&quot; van de e-mailwaarschuwingen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Type waarschuwing"
>abstract="Geef de **Type waarschuwing** voor het criterium: het etiket en de kleur die naast het leveringscriterium moeten worden weergegeven in de rubriek &quot;Samenvatting&quot; van de waarschuwingen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Criteriumfrequentie"
>abstract="De frequentie van waarschuwingen per dag controleren voor elke levering die aan het criterium voldoet."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Een waarschuwingscriterium maken"
>abstract="Als u uw eigen leveringsfilters wilt maken, maakt u een nieuw, vooraf gedefinieerd filter in de Campagne v8-console via de **Administratie** > **Configuratie** > **Vooraf gedefinieerde filters** knooppunt."

Ga als volgt te werk om een nieuw criterium te maken:

1. Ga naar de **Aflevering is vereist** in het linkernavigatievenster en selecteer de optie **Criteria** tab.
1. Klik op de knop **Waarschuwingscriteria voor levering maken** knop.
1. Geef een label voor het criterium op. De interne naam wordt automatisch ingevuld en heeft het kenmerk Alleen-lezen.
1. De **Het door deze criteria toegepaste filter van de levering** kunt u het bereik van het criterium verfijnen door er een vooraf gedefinieerd filter op toe te passen.

   In het onderstaande voorbeeld wordt **Bezig met levering (critInProgressDeliveries)** is geselecteerd, wat betekent dat het criterium alleen leveringen met de status &quot;In uitvoering&quot; in aanmerking neemt.

   ![](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Als geen van de vooraf gedefinieerde filters aan uw behoeften voldoet, kunt u contact opnemen met de beheerder om uw eigen filter te maken.  Gedetailleerde informatie over het maken van vooraf gedefinieerde filters in de Campagne-console is beschikbaar in het dialoogvenster [Adobe Campaign v8 (console)-documentatie](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/create-audiences/create-filters){target="_blank"}
   >
   >Deze bewerking mag alleen door gevorderde gebruikers worden uitgevoerd.

1. In de **Indicatoren die moeten worden toegevoegd aan signaleringen** in de sectie &quot;Details&quot; van de e-mailwaarschuwingen kiest u de indicatoren die u als kolommen wilt weergeven.

1. Geef de **Type waarschuwing** voor het criterium: het etiket en de kleur die naast het leveringscriterium moeten worden weergegeven in de rubriek &quot;Samenvatting&quot; van de waarschuwingen.

1. De **Frequentie criteria** kunt u de frequentie van waarschuwingen per dag controleren voor elke levering die aan het criterium voldoet:

   * **Dit leveringscriterium wordt in elke kennisgeving herhaald**: Geef in elke e-mailwaarschuwing van de dag een levering weer die aan het criterium voldoet.
   * **Dit leveringscriterium wordt alleen op het eerste tijdstip van de dag verzonden**: Geef alleen in het eerste rapport van de dag een levering weer die voldoet aan het criterium en niet in volgende e-mailwaarschuwingen.
