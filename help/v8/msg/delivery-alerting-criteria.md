---
audience: end-user
title: Afleveringswaarschuwing
description: Leer hoe u werkt met waarschuwingsberichten voor leveringen.
exl-id: fc98d4e3-7986-42bb-82d5-b4f874aa71db
source-git-commit: 037b04475370b1a34ecec31ef2a774866278ce65
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 0%

---

# Beoordelingscriteria voor aflevering {#delivery-alerting-criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Dashboard voor leveringswaarschuwingscriteria"
>abstract="De gebruikersinterface van het Web van de campagne verstrekt vooraf bepaalde alarmerende criteria (leveringen met lage productie, leveranties de waarvan voorbereiding ontbrak...) die u aan uw dashboard kunt toevoegen. U kunt ook uw eigen criteria maken die aan uw behoeften voldoen."

De gebruikersinterface van het Web van de campagne verstrekt vooraf bepaalde alarmerende criteria, zoals leveringen met lage productie of leveringen de waarvan voorbereiding ontbrak, die u aan uw dashboard kunt toevoegen. U kunt ook uw eigen criteria maken die aan uw behoeften voldoen.

Het waarschuwen van criteria is toegankelijk van het **Alarm van de Levering** menu in de linkernavigatieruit, onder de **Criteria** tabel.

![&#x200B; Lijst van alarmerende criteria die in het het Alarm menu van de Levering worden getoond &#x200B;](assets/alerting-criteria-list.png)

## Vooraf gedefinieerde waarschuwingscriteria {#ootb-criteria}

Vooraf gedefinieerde waarschuwingscriteria zijn beschikbaar in de webgebruikersinterface van Campagne. Deze criteria bestrijken een reeks scenario&#39;s, die hieronder worden opgesomd:

* **Leveringen ontbrak**: Om het even welke levering die binnen een bepaalde waaier, met een verkeerde status wordt gepland.
* **Leveringen met ontbroken voorbereiding**: Om het even welke levering die binnen een bepaalde waaier wordt gewijzigd, waarvoor de voorbereidingsstap (doelberekening en inhoudsgeneratie) is ontbroken.
* **Levering met slechte foutenverhouding voor zachte stuiters**: Om het even welke levering die binnen een bepaalde waaier wordt gepland, met een status van minstens &quot;Bezig,&quot;en een zachte stuitfoutenverhouding groter dan een bepaald percentage.
* **Levering met slechte foutenverhouding voor harde stuiters**: Om het even welke levering die binnen een bepaalde waaier, met een status van minstens &quot;Bezig,&quot;en een harde stuitfoutenverhouding groter dan een bepaald percentage wordt gepland.
* **Leveringen met lange begin hangende**: Om het even welke levering die binnen een bepaalde waaier, met een &quot;Begin in behandeling&quot;status voor langer dan een bepaalde duur wordt gepland. De status &quot;In behandeling beginnen&quot; betekent dat de berichten nog niet door het systeem in aanmerking zijn genomen.
* **Leveringen met lage productie**: Om het even welke levering begon langer dan een bepaalde duur, met minder dan een bepaald percentage verwerkte berichten en een productie lager dan een bepaalde waarde.
* **Leveringen lopend**: Om het even welke levering die binnen een bepaalde waaier, met de &quot;Bezig&quot;status wordt gepland.

>[!NOTE]
>
>De standaardwaarden worden toegepast op alle parameters voor de bovenstaande criteria. Deze waarden kunnen in de **sectie van Parameters van Criteria** van de levering worden aangepast alarmerende dashboards waar zij worden gebruikt. [&#x200B; Leer hoe te met dashboards &#x200B;](../msg/delivery-alerting-dashboards.md) te werken

## Een waarschuwingscriterium maken {#criteria}

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Waarschuwingscriteria voor levering maken"
>abstract="Naast de vooraf gedefinieerde waarschuwingscriteria van Adobe Campaign kunt u zelf criteria maken die aan uw behoeften voldoen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicatoren die moeten worden toegevoegd aan signaleringen"
>abstract="Selecteer de indicatoren die u als kolommen wilt weergeven in de sectie &#39;Details&#39; van de e-mailwaarschuwingen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Type waarschuwing"
>abstract="Specificeer het **Type van Alarm** voor het criterium, betekenend het etiket en de kleur naast het leveringscriterium in de &quot;Samenvatting&quot;sectie van het alarm te tonen."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Criteriumfrequentie"
>abstract="De frequentie van waarschuwingen per dag controleren voor elke levering die aan het criterium voldoet."

Ga als volgt te werk om een nieuw criterium te maken:

1. Navigeer aan het **Waarschuwende van de Levering** menu in de linkernavigatieruit, en selecteer de **Criteria** tabel.
1. Klik **creeer levering alarmerende criteria** knoop.
1. Geef een label voor het criterium op. De interne naam wordt automatisch ingevuld en heeft het kenmerk Alleen-lezen.
1. Gebruik het **filter van de Levering dat door deze criteria** wordt toegepast om het werkingsgebied van het criterium te verfijnen door een vooraf bepaalde filter op het toe te passen.

   In het voorbeeld hieronder, is de **Geleveringen in uitvoering (critInProgressDeliveries)** filter geselecteerd, betekenend dat het criterium slechts rekening met leveringen met de &quot;Bezig&quot;status houdt.

   ![&#x200B; Voorbeeld van het waarschuwen van criteria eigenschappen met geselecteerde filter &#x200B;](assets/alerting-criteria-properties.png)

   >[!NOTE]
   >
   >Als geen van de vooraf bepaalde filters uw behoeften aanpassen, kunt u uw eigen degenen van het **Beheer van de Klant** tot stand brengen > **vooraf bepaald filters** menu. [Meer informatie](../get-started/predefined-filters.md)
   >
   >Deze bewerking mag alleen door gevorderde gebruikers worden uitgevoerd.

1. In de **Indicatoren om in alarm** sectie toe te voegen, verkies de indicatoren om als kolommen in de &quot;sectie van Details&quot;van het e-mailalarm te tonen.

1. Specificeer het **Type van Alarm** voor het criterium, betekenend het etiket en de kleur naast het leveringscriterium in de &quot;Samenvatting&quot;sectie van het alarm te tonen.

1. Gebruik de **sectie van de Frequentie van Criteria** om de frequentie van alarm per dag voor elke levering te controleren die aan het criterium voldoet:

   * **Dit leveringscriterium zal in elk bericht** worden herhaald: Toon een levering die aan het criterium in elke e-mailalarm van de dag voldoet.
   * **Dit leveringscriterium wordt verzonden slechts op het eerste voorkomen van de dag**: Toon een levering die aan het criterium in het eerste rapport van de dag voldoet slechts, zonder het in verdere e-mailalarm te herhalen.