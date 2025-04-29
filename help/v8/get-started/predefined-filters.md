---
title: Werken met vooraf gedefinieerde filters
description: Leer hoe u vooraf gedefinieerde filters maakt en beheert in Adobe Campaign Web
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: 1a751aed6d5185e700dafb1de2afd88300dfcd79
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 2%

---

# Werken met vooraf gedefinieerde filters {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="Vooraf gedefinieerd filterbeheer"
>abstract="De gebruikersinterface van het Web van de campagne biedt een gebruikersvriendelijke interface aan moeiteloos beheren en vooraf bepaalde filters aanpassen om aan uw specifieke behoeften te voldoen. Maak één keer en sla dit op voor toekomstig gebruik."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Vooraf gedefinieerde filters"
>abstract="De gebruikersinterface van het Web van de campagne biedt een gebruikersvriendelijke interface aan moeiteloos beheren en vooraf bepaalde filters aanpassen om aan uw specifieke behoeften te voldoen. Maak één keer en sla dit op voor toekomstig gebruik."

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Een waarschuwingscriterium maken"
>abstract="U kunt uw eigen leveringsfilters van het Beheer van de Klant > het Vooraf bepaalde menu van filters tot stand brengen."

Vooraf gedefinieerde filters zijn aangepaste filters die zijn gemaakt en opgeslagen voor toekomstig gebruik. Zij doen dienst als kortere weg tijdens het filtreren verrichtingen met de vraagmodeller. Ze kunnen bijvoorbeeld worden gebruikt wanneer een gegevenslijst wordt gefilterd of wanneer het publiek van een levering wordt gemaakt.

U kunt bestaande ingebouwde filters gebruiken om tot een specifieke ondergroep van uw gegevens toegang te hebben of uw eigen vooraf bepaalde filters tot stand te brengen en hen te bewaren.

![ Vooraf bepaalde interface van het filtermenu ](assets/predefined-filters-menu.png){zoomable="yes"}

## Een vooraf gedefinieerd filter maken {#create-predefined-filter}

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-creation"
>title="Een vooraf gedefinieerd filter maken"
>abstract="Voer een label in voor het vooraf gedefinieerde filter en selecteer de tabel waarop het van toepassing is. Open de aanvullende opties om een beschrijving toe te voegen en stel dit filter in als favoriet. Vervolgens gebruikt u de knop &#39;Regel maken&#39; om de filtervoorwaarden te definiëren."

>[!CONTEXTUALHELP]
>id="acw_predefined-filters-rules"
>title="Vooraf gedefinieerde filterregels maken"
>abstract="Als u de filtervoorwaarden van het aangepaste filter wilt definiëren, klikt u op de knop Regel maken."

### Een filter maken op basis van de querymodelfunctie {#create-from-rule-builder}

Sparen een douanefilter van [ vraagmodeler ](../query/query-modeler-overview.md) om het voor toekomstig gebruik beschikbaar te maken. Voer de volgende stappen uit:

1. Open de vraagmodeler en bepaal uw het filtreren voorwaarden. In het onderstaande voorbeeld worden ontvangers die in Madrid wonen en zich op een nieuwsbrief abonneren, gefilterd.
1. Klik **Uitgezocht of sparen filter** knoop, en uitgezocht **sparen als filter**.

   ![ sparen vooraf bepaalde filterinterface ](assets/predefined-filters-save.png){zoomable="yes"}

1. Selecteer **creeer een nieuwe filter**, en ga een naam en een beschrijving voor die filter in.

   ![ sparen interface van filterdetails ](assets/predefined-filters-save-filter.png){zoomable="yes"}

   U kunt het filter indien nodig opslaan als favoriet. Lees meer in [deze sectie](#fav-filter).

1. Klik **bevestigen** om uw veranderingen te bewaren.

Uw douanefilter is nu beschikbaar in de **Vooraf bepaalde lijst van Filters** en toegankelijk voor alle gebruikers van de Campagne.

### Een filter maken in de filterlijst {#create-filter-from-list}

Creeer een filter van de **Vooraf bepaalde filters** ingang in het linkermenu. Voer de volgende stappen uit:

1. Blader aan de **Vooraf bepaalde filters** ingang in het linkermenu.
1. Klik **creeer filterknoop**.
1. Ga de filternaam in en, van het **type van Document** gebied, selecteer het schema het op van toepassing is. Het standaardschema is `Recipients(nms)` .

1. Definieer de regel voor het filter. Profielen die ouder zijn dan 30.

   ![ regel van de Filter voor profielen ouder dan 30 ](assets/filter-30+.png){zoomable="yes"}

1. Sla uw wijzigingen op.

   ![ Nieuwe filter bewaarde interface ](assets/new-filter.png){zoomable="yes"}

Het filter wordt toegevoegd aan de vooraf gedefinieerde filterlijst. U kunt het filter indien nodig opslaan als favoriet. Lees meer in [deze sectie](#fav-filter).

## Filter opslaan als favoriet {#fav-filter}

Wanneer het creëren van een vooraf bepaald filter, laat **sparen als favoriete** optie toe om dit vooraf bepaalde filter in uw favorieten te zien.

Wanneer een filter als favoriet wordt bewaard, is het beschikbaar aan alle gebruikers in de **favoriete filters** sectie van de lijst van de filterverwezenlijking, zoals hieronder getoond:

![ Favoriete filterssectie ](assets/predefined-filters-favorite.png){zoomable="yes"}{width="30%" align="left"}

## Een vooraf gedefinieerd filter gebruiken {#use-predefined-filter}

Vooraf gedefinieerde filters zijn beschikbaar wanneer u regeleigenschappen definieert. Om tot vooraf bepaalde filters toegang te hebben, verkies de **Uitgezochte optie van de douanefilter** in de drop-down van de vraagmodelleur.

Heb toegang tot de volledige lijst van vooraf bepaalde filters beschikbaar voor de huidige context, en gebruikskortere weg in de **Favoriete filters** sectie van de drop-down. Leer meer over favorieten in [ deze sectie ](#fav-filter).

Als u bijvoorbeeld een publiek wilt maken op basis van een vooraf gedefinieerd filter, voert u de volgende stappen uit:

1. Blader aan de **ingang van het Soorten publiek** in het linkermenu en klik **creëren de knoop van het Publiek** in de upper-left hoek van de lijst van soorten publiek.
1. Ga de publieksnaam in, en klik **creëren de knoop van het Publiek**.
1. Selecteer de **activiteit van de Vraag**, en, van de juiste ruit, klik **creëren publiek** knoop.

   ![ creeer publieksinterface ](assets/build-audience-from-filter.png){zoomable="yes"}

1. Van **Uitgezocht of sparen filter** knoop, kies de **Uitgezochte optie van de douanefilter**.

   ![ Uitgezochte optie van de douanefilter ](assets/build-audience-select-custom-filter.png){zoomable="yes"}

1. Blader naar het vooraf gedefinieerde filter dat u wilt gebruiken om het publiek te maken, selecteer het en bevestig het.

   ![ Vooraf bepaalde interface van de filterlijst ](assets/build-audience-filter-list.png){zoomable="yes"}

1. Controleer de regeleigenschappen voor dit filter en bevestig.

   Het filter wordt nu gebruikt als vraag in de **activiteit van de Vraag**.

   ![ de activiteit van de Vraag met vooraf bepaalde filter ](assets/build-audience-confirm.png){zoomable="yes"}

1. Sparen uw veranderingen en klik de **knoop van het Begin** om het publiek te bouwen en het beschikbaar te maken in de publiekslijst.

## Uw vooraf gedefinieerde filters beheren {#manage-predefined-filter}

Alle vooraf gedefinieerde filters worden gegroepeerd in de specifieke vermelding van het navigatiemenu links.

![ Lijst van vooraf bepaalde filters ](assets/list-of-filters.png){zoomable="yes"}

In deze lijst kunt u een nieuw filter maken zoals hierboven beschreven en de onderstaande handelingen uitvoeren:

* Bewerk een bestaand filter en wijzig de regels en eigenschappen ervan.
* Een vooraf gedefinieerd filter dupliceren.
* Verwijder een vooraf gedefinieerd filter.

U kunt ook een vooraf gedefinieerd filter toevoegen als een favoriet voor snelle toegang bij het maken van uw publiek. Lees meer in [deze sectie](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->