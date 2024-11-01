---
title: Voorwaardelijke inhoud maken
description: Leer hoe u voorwaarden definieert om uw inhoud aan te passen aan uw wensen in Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: f57e0f2de12780ff9f90c2c5f1933b0e9bffe493
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# Voorwaardelijke inhoud maken{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_conditional_content"
>title="Voorwaardelijke inhoud toevoegen"
>abstract="Configureer voorwaardelijke inhoudsvelden om geavanceerde dynamische personalisatie te maken op basis van de profielgegevens van de ontvanger. Tekstblokken, koppelingen, onderwerpregel en/of afbeeldingen worden vervangen in de inhoud van het bericht als aan een bepaalde voorwaarde is voldaan."

## Aan de slag met voorwaardelijke inhoud {#gs}

Voorwaardelijke inhoud is een krachtige functie waarmee u dynamische personalisatie kunt maken op basis van de profielgegevens van de ontvanger, waarbij tekstblokken en afbeeldingen automatisch worden vervangen wanneer aan bepaalde voorwaarden wordt voldaan. Met deze functie kunt u uw campagnes op een hoger niveau brengen en uw publiek een zeer doelgerichte, persoonlijke ervaring bieden.

Door voorwaardelijke inhoudsgebieden te vormen, kunt u geavanceerde dynamische verpersoonlijking tot stand brengen die op het profiel van de ontvanger bijvoorbeeld wordt gebaseerd. Tekstblokken, koppelingen, onderwerpregel en/of afbeeldingen worden vervangen in de inhoud van het bericht als aan een bepaalde voorwaarde is voldaan. U kunt bijvoorbeeld &#39;Mr&#39; of &#39;Mevrouw&#39; weergeven op basis van de waarde van het genderveld in de database van Adobe Campaign, of een andere link opnemen op basis van de voorkeurstaal van de ontvanger.

Om voorwaardelijke inhoud tot stand te brengen, moet u voorwaarden in de **uitdrukkingsredacteur** creëren gebruikend specifieke hulpfuncties. Deze methode is beschikbaar voor alle leveringskanalen, op om het even welk gebied waar u tot de uitdrukkingsredacteur, zoals de onderwerpregel, of e-mailverbindingen en tekst/knoop inhoudcomponenten kunt toegang hebben. [ Leer hoe te om tot de uitdrukkingsredacteur toegang te hebben ](gs-personalization.md#access)

Naast de uitdrukkingsredacteur, kunt u hefboomwerking een specifieke **voorwaardelijke inhoudsbouwer** wanneer het ontwerpen van een e-mail die u toestaat om veelvoudige varianten voor een element van uw e-maillichaam tot stand te brengen. [ Leer hoe te om voorwaardelijke inhoud in e-mails tot stand te brengen ](#condition-condition-builder)

## Voorwaarden maken in de expressie-editor {#condition-perso-editor}

Voer de onderstaande stappen uit om voorwaardelijke inhoud voor een levering te definiëren met behulp van de expressieeditor. In dit voorbeeld willen we voorwaardelijke inhoud maken op basis van de taal van de ontvangers (Frans of Engels).

1. Open een levering en navigeer naar de sectie voor het bewerken van inhoud.

1. Zoek het veld waaraan u voorwaardelijke inhoud wilt toevoegen. U kunt bijvoorbeeld voorwaardelijke inhoud toevoegen aan een SMS-bericht.

1. Klik op het pictogram **[!UICONTROL Open personalization dialog]** naast het veld om de expressie-editor te openen.

   ![](assets/open-perso-editor-sms.png){zoomable="yes"}

1. Blader in de verpersoonlijkingseditor naar het menu **[!UICONTROL Conditions]** aan de linkerkant.

1. Om uw voorwaarde te beginnen bouwen, klik &#39;+&#39; pictogram naast **als** functie. De volgende lijn wordt toegevoegd aan het centrale scherm:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Vervang `<FIELD>` door een verpersoonlijkingsveld, zoals de taal van de ontvanger: `recipient.language` .
   * Vervang `<VALUE>` door de waarde waaraan moet worden voldaan. Bijvoorbeeld `'French'` .
   * Vervang `Ìnsert content here` door de inhoud die u wilt weergeven door de profielen die aan de opgegeven voorwaarde voldoen.

     ![](assets/condition-sample1.png){zoomable="yes"}{width="800" align="center"}

1. Geef de inhoud op die moet worden weergegeven als de ontvangers niet aan de voorwaarde voldoen. Om dit te doen gebruik anders **** hulpfunctie:

   1. Plaats uw curseur vóór de uitdrukking die markering `%>` sluit en klik `+` naast de **anders** functie.

   1. Vervang `Ìnsert content here` door de inhoud die u wilt weergeven door de profielen die niet voldoen aan de voorwaarde van de if-functie.

   ![](assets/condition-sample2.png){zoomable="yes"}{width="800" align="center"}

   U kunt **anders ook gebruiken als** hulpfunctie om voorwaarden met veelvoudige inhoudsvarianten te bouwen. De onderstaande expressie geeft bijvoorbeeld drie varianten van een bericht weer, afhankelijk van de taal van de ontvanger:

   ![](assets/condition-sample3.png){zoomable="yes"}{width="800" align="center"}

   >[!NOTE]
   >
   >Telkens wanneer een hulpfunctie wordt toegevoegd, worden het openen (`<%`) en het sluiten (`%>`) markeringen automatisch toegevoegd vóór en na de functie.
   >
   >Voorbeeld na het toevoegen van een hulpfunctie &quot;Else&quot; binnen een expressie: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Verwijder deze tags om syntaxisfouten te voorkomen. In dit voorbeeld, is de gecorrigeerde uitdrukking na het verwijderen van **anders** functietags:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Zodra uw voorwaarde klaar is, kunt u uw inhoud opslaan en de rendering ervan controleren door uw inhoud te simuleren.

## Voorwaardelijke inhoud maken in e-mails {#condition-condition-builder}

Voorwaardelijke inhoud in e-mails kan op twee manieren worden gemaakt:
* In de uitdrukkingsredacteur door een voorwaarde met helperfuncties te bouwen,
* In een speciale voorwaardelijke inhoudsontwikkelaar die toegankelijk is wanneer u een e-mail ontwerpt.

In de volgende sectie vindt u stapsgewijze instructies voor het maken van voorwaarden met behulp van de voorwaardelijke inhoud van e-mail Designer. De gedetailleerde informatie over hoe te om voorwaarden tot stand te brengen gebruikend de uitdrukkingsredacteur is beschikbaar [ hier ](#condition-perso-editor).

In dit voorbeeld willen we een e-mailbericht maken met meerdere varianten op basis van de taal van de ontvangers. Voer de volgende stappen uit:

1. Maak of open een e-maillevering, bewerk de inhoud ervan en klik op de knop **[!UICONTROL Edit email body]** om de werkruimte voor het ontwerpen van e-mail te openen.

1. Selecteer een inhoudscomponent en klik op het pictogram **[!UICONTROL Enable conditional content]** .

   ![](assets/condition-email-enable.png){zoomable="yes"}{width="800" align="center"}

1. Het deelvenster **[!UICONTROL Conditional Content]** wordt aan de linkerkant van het scherm geopend. In dit deelvenster kunt u meerdere varianten van de geselecteerde inhoudscomponent maken aan de hand van voorwaarden.

1. Vorm uw eerste variant. Houd de cursor boven **[!UICONTROL Variant - 1]** in het deelvenster **[!UICONTROL Conditional Content]** en klik op de knop **[!UICONTROL Add condition]** .

   ![](assets/condition-add-condition.png){zoomable="yes"}{width="800" align="center"}

1. De vraagmodeler opent. Het staat u toe om een voorwaarde te bouwen door de het profielgegevens van de ontvanger te filtreren. [ Leer hoe te met de vraagmodelaar ](../query/query-modeler-overview.md) te werken.

   Klik op **[!UICONTROL Confirm]** als de voorwaarde voor de eerste variant van het bericht gereed is. In dit voorbeeld creëren we een regel die gericht is op ontvangers die &#39;Frans&#39; zijn.

   ![](assets/condition-example.png){zoomable="yes"}{width="800" align="center"}

1. De regel is nu gekoppeld aan de variant. Voor betere leesbaarheid raden we u aan de naam van de variant te wijzigen door op het ellipsmenu te klikken.

1. Vorm hoe de component zou moeten tonen als de regel wordt ontmoet wanneer het verzenden van het bericht. In dit voorbeeld willen we de tekst in het Frans weergeven als dit de voorkeurstaal van de ontvanger is.

   ![](assets/condition-email-variant1.png){zoomable="yes"}{width="800" align="center"}

1. Voeg zoveel varianten toe als nodig zijn voor de inhoudscomponent. U kunt op elk gewenst moment schakelen tussen de varianten om te controleren hoe de inhoudscomponent wordt weergegeven op basis van hun voorwaardelijke regels.

   >[!NOTE]
   >Als bij het verzenden van het bericht aan geen van de regels in de varianten wordt voldaan, wordt de inhoud die in het deelvenster **[!UICONTROL Default variant]** is gedefinieerd, weergegeven in de inhoudscomponent. **[!UICONTROL Conditional Content]**

## Variabelen gebruiken voor voorwaardelijke inhoud {#variables-conditional}

De variabelen kunnen voor voorwaardelijke inhoud in uw levering worden gebruikt.

Leer meer over [ toevoegend variabelen aan een levering ](../advanced-settings/delivery-settings.md#variables-delivery).

Kies het element waar u voorwaardelijke inhoud wilt plaatsen.

![](assets/variables-conditional.png){zoomable="yes"}

Om uw variabele te gebruiken, vorm de voorwaarde gebruikend de **[!UICONTROL Edit expression]** knoop, zoals hieronder getoond.
In dit voorbeeld wordt deze afbeelding weergegeven wanneer de waarde van de variabele `launch` is.

![](assets/variables-condition.png){zoomable="yes"}

U kunt ook een andere variant maken met de waarde `reminder` , bijvoorbeeld wanneer een andere afbeelding wordt weergegeven.
