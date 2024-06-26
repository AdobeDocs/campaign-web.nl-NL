---
title: Voorwaardelijke inhoud maken
description: Leer hoe u voorwaarden definieert om uw inhoud aan te passen aan uw wensen in Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: 101ad23b-7ea5-42c7-9249-7c14febe6eb7
source-git-commit: f6e3fc0da05ecc2fda158c970458cc702b27079c
workflow-type: tm+mt
source-wordcount: '923'
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

Als u voorwaardelijke inhoud wilt maken, moet u voorwaarden maken in het dialoogvenster **expressie-editor** specifieke hulpfuncties gebruiken. Deze methode is beschikbaar voor alle leveringskanalen, op om het even welk gebied waar u tot de uitdrukkingsredacteur, zoals de onderwerpregel, of e-mailverbindingen en tekst/knoop inhoudcomponenten kunt toegang hebben. [Leer hoe u toegang krijgt tot de expressie-editor](gs-personalization.md#access)

Naast de expressie-editor kunt u een speciale editor gebruiken **voorwaardelijk maken van inhoud** bij het ontwerpen van een e-mail waarmee u meerdere varianten voor een element van uw e-mailhoofdtekst kunt maken. [Meer informatie over het maken van voorwaardelijke inhoud in e-mails](#condition-condition-builder)

## Voorwaarden maken in de expressie-editor {#condition-perso-editor}

Voer de onderstaande stappen uit om voorwaardelijke inhoud voor een levering te definiëren met behulp van de expressieeditor. In dit voorbeeld willen we voorwaardelijke inhoud maken op basis van de taal van de ontvangers (Frans of Engels).

1. Open een levering en navigeer naar de sectie voor het bewerken van inhoud.

1. Zoek het veld waaraan u voorwaardelijke inhoud wilt toevoegen. U kunt bijvoorbeeld voorwaardelijke inhoud toevoegen aan een SMS-bericht.

1. Klik op de knop **[!UICONTROL Open personalization dialog]** pictogram naast het veld om de uitdrukkingseditor te openen.

   ![](assets/open-perso-editor-sms.png){zoomable=&quot;yes&quot;}

1. Blader in de verpersoonlijkingseditor naar de **[!UICONTROL Conditions]** links.

1. Als u wilt beginnen met het bouwen van uw voorwaarde, klikt u op het plusteken (+) naast de knop **Indien** functie. De volgende regel wordt toegevoegd aan het centrale scherm:`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Vervangen `<FIELD>` met een verpersoonlijkingsgebied, zoals de taal van de ontvanger: `recipient.language`.
   * Vervangen `<VALUE>` met de waarde waaraan moet worden voldaan. Bijvoorbeeld: `'French'`.
   * Vervangen `Ìnsert content here` met de inhoud die u wilt weergeven voor de profielen die aan de opgegeven voorwaarde voldoen.

     ![](assets/condition-sample1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. Geef de inhoud op die moet worden weergegeven als de ontvangers niet aan de voorwaarde voldoen. Om dit te doen gebruik **else** helperfunctie:

   1. Plaats de cursor vóór de afsluitingstag voor de expressie `%>` en klik op de knop `+` naast de **Else** functie.

   1. Vervangen `Ìnsert content here` met de inhoud die u wilt weergeven voor de profielen die niet voldoen aan de voorwaarde van de if-functie.

   ![](assets/condition-sample2.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   U kunt ook de opdracht **else if** de hulpfunctie om voorwaarden met veelvoudige inhoudvarianten te bouwen. De onderstaande expressie geeft bijvoorbeeld drie varianten van een bericht weer, afhankelijk van de taal van de ontvanger:

   ![](assets/condition-sample3.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

   >[!NOTE]
   >
   >Elke keer dat een hulpfunctie wordt toegevoegd, wordt het openen (`<%`) en sluiten (`%>`) automatisch worden toegevoegd voor en na de functie.
   >
   >Voorbeeld na het toevoegen van een hulpfunctie &quot;Else&quot; binnen een expressie: >
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
   >
   >Verwijder deze tags om syntaxisfouten te voorkomen. In dit voorbeeld wordt de gecorrigeerde expressie na het verwijderen van de **else** functietags zijn:
   >
   >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

1. Zodra uw voorwaarde klaar is, kunt u uw inhoud opslaan en de rendering ervan controleren door uw inhoud te simuleren.

## Voorwaardelijke inhoud maken in e-mails {#condition-condition-builder}

Voorwaardelijke inhoud in e-mails kan op twee manieren worden gemaakt:
* In de uitdrukkingsredacteur door een voorwaarde met helperfuncties te bouwen,
* In een speciale voorwaardelijke inhoudsontwikkelaar die toegankelijk is wanneer u een e-mail ontwerpt.

In de volgende sectie vindt u stapsgewijze instructies voor het maken van voorwaarden met de voorwaardelijke-inhoudmogelijkheden van e-mailontwerper. Gedetailleerde informatie over het maken van voorwaarden met de expressieeditor is beschikbaar [hier](#condition-perso-editor).

In dit voorbeeld willen we een e-mailbericht maken met meerdere varianten op basis van de taal van de ontvangers. Voer de volgende stappen uit:

1. Maak of open een e-maillevering, bewerk de inhoud en klik op de knop **[!UICONTROL Edit email body]** om de werkruimte voor het ontwerpen van e-mail te openen.

1. Selecteer een inhoudscomponent en klik op de knop **[!UICONTROL Enable conditional content]** pictogram.

   ![](assets/condition-email-enable.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. De **[!UICONTROL Conditional Content]** wordt aan de linkerkant van het scherm geopend. In dit deelvenster kunt u meerdere varianten van de geselecteerde inhoudscomponent maken aan de hand van voorwaarden.

1. Vorm uw eerste variant. Overslaan **[!UICONTROL Variant - 1]** in de **[!UICONTROL Conditional Content]** en klik op de knop **[!UICONTROL Add condition]** knop.

   ![](assets/condition-add-condition.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. De vraagmodeler opent. Het staat u toe om een voorwaarde te bouwen door de het profielgegevens van de ontvanger te filtreren. [Leer hoe te met vraagmodeler te werken](../query/query-modeler-overview.md).

   Zodra de voorwaarde voor de eerste variant van het bericht klaar is, klik **[!UICONTROL Confirm]**. In dit voorbeeld creëren we een regel die gericht is op ontvangers die &#39;Frans&#39; zijn.

   ![](assets/condition-example.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. De regel is nu gekoppeld aan de variant. Voor betere leesbaarheid raden we u aan de naam van de variant te wijzigen door op het ellipsmenu te klikken.

1. Vorm hoe de component zou moeten tonen als de regel wordt ontmoet wanneer het verzenden van het bericht. In dit voorbeeld willen we de tekst in het Frans weergeven als dit de voorkeurstaal van de ontvanger is.

   ![](assets/condition-email-variant1.png){zoomable=&quot;yes&quot;}{width="800" align="center"}

1. Voeg zoveel varianten toe als nodig zijn voor de inhoudscomponent. U kunt op elk gewenst moment schakelen tussen de varianten om te controleren hoe de inhoudscomponent wordt weergegeven op basis van hun voorwaardelijke regels.

   >[!NOTE]
   >Als aan geen van de regels in de varianten wordt bepaald wanneer het verzenden van het bericht wordt voldaan, zal de inhoudscomponent de inhoud tonen die in wordt bepaald **[!UICONTROL Default variant]** van de **[!UICONTROL Conditional Content]** venster.
