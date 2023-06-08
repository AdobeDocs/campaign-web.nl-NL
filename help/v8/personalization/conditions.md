---
title: Voorwaardelijke content maken
description: Leer hoe u voorwaarden definieert voor het aanpassen van uw inhoud in de gebruikersinterface van Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positief"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 1dfd557b22de9888ab8d3a1f0479b45d59a86f93
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 1%

---

# Voorwaardelijke inhoud maken{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Voorwaardelijke content maken"
>abstract="Maak voorwaardelijke inhoud om dynamische personalisatie te definiëren op basis van het profiel van de ontvanger, waarbij tekstblokken en afbeeldingen automatisch worden vervangen wanneer aan bepaalde voorwaarden wordt voldaan. Met deze functie kunt u uw campagnes op een hoger niveau brengen en uw publiek een zeer doelgerichte, persoonlijke ervaring bieden."

Voorwaardelijke inhoud is een krachtige functie waarmee u een dynamische personalisatie kunt maken op basis van het profiel van de ontvanger, waarbij tekstblokken en afbeeldingen automatisch worden vervangen wanneer aan bepaalde voorwaarden wordt voldaan. Met deze functie kunt u uw campagnes op een hoger niveau brengen en uw publiek een zeer doelgerichte, persoonlijke ervaring bieden.

Door voorwaardelijke inhoudsgebieden te vormen, kunt u geavanceerde dynamische verpersoonlijking tot stand brengen die op het profiel van de ontvanger bijvoorbeeld wordt gebaseerd. Tekstblokken, koppelingen, onderwerpregel en/of afbeeldingen worden vervangen in de inhoud van het bericht als aan een bepaalde voorwaarde is voldaan. U kunt bijvoorbeeld &#39;Mr&#39; of &#39;Mevrouw&#39; weergeven op basis van de waarde van het genderveld in de database van Adobe Campaign, of een andere link opnemen op basis van de voorkeurstaal van de ontvanger.

## Voorwaardelijke inhoud maken

Als u voorwaardelijke inhoud wilt maken, moet u voorwaarden maken in de expressie-editor met een specifieke hulpfunctie. Deze methode is beschikbaar voor alle leveringskanalen, op om het even welk gebied waar u tot de uitdrukkingsredacteur, zoals het onderwerpregel gebied, of e-mailverbindingen en tekst/knoop inhoudcomponenten kunt toegang hebben. [Leer waar u dynamische inhoud wilt toevoegen](gs-personalization.md/#access)

Naast de expressie-editor kunt u een speciale, voorwaardelijke inhoudsontwikkelaar gebruiken bij het ontwerpen van een e-mail waarin u voorwaarden kunt maken met behulp van profielkenmerken.

## Voorwaarden maken in de expressie-editor {#condition-perso-editor}

Voer de onderstaande stappen uit om een voorwaardelijke inhoud voor een levering te definiëren. In dit voorbeeld willen we voorwaardelijke inhoud maken op basis van de taal van de ontvangers (Frans of Engels).

1. Open een levering en bewerk de inhoud.

1. Zoek het veld waaraan u voorwaardelijke inhoud wilt toevoegen en klik op de knop **[!UICONTROL Open personalization dialog]** pictogram om de uitdrukkingsredacteur te openen. In dit voorbeeld willen we voorwaardelijke inhoud toevoegen aan een SMS-bericht:

   ![](assets/open-perso-editor-sms.png)

1. Blader in de verpersoonlijkingseditor naar de **[!UICONTROL Helper functions]** links.

1. Klik op het pictogram ‘+’ naast het pictogram **Indien** om uw toestand te starten. De volgende regel wordt toegevoegd aan het centrale scherm:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`

   * Vervangen `<FIELD>` door een verpersoonlijkingsveld. Bijvoorbeeld de taal van de ontvanger: `recipient.language`.
   * Vervangen `<VALUE>` door de waarde waaraan moet worden voldaan. Bijvoorbeeld, `'French'`.
   * Vervangen `Ìnsert content here` door de inhoud die u wilt weergeven aan de profielen die aan de bovenstaande voorwaarde voldoen.

     ![](assets/condition-sample1.png)

1. Geef de inhoud op die moet worden weergegeven als de ontvangers niet aan de voorwaarde voldoen. Dit doet u als volgt:

   1. Een **else** helperfunctie: Plaats de cursor vóór de afsluitingstag voor de expressie `%>` en klik op de knop `+` naast de **Else** functie.

      >[!NOTE]
      >
      >Elke keer dat een hulpfunctie wordt toegevoegd, wordt het openen (`<%`) en sluiten (`%>`) automatisch worden toegevoegd voor en na de functie. Voorbeeld na het toevoegen van een hulpfunctie &quot;Else&quot; binnen een expressie:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } <% else { %> Insert content here<% } %>%>`
      >
      >Zorg ervoor dat u deze labels verwijdert om syntaxisfouten te voorkomen. In dit voorbeeld wordt de gecorrigeerde expressie na het verwijderen van de **Else** functietags zijn:
      >
      >`<% if (<FIELD>==<VALUE>) { %>Insert content here<% } else { %> Insert content here<% } %>`

   1. Vervangen `Ìnsert content here` door de inhoud die u wilt weergeven aan profielen die niet aan de voorwaarde voldoen.

      ![](assets/condition-sample2.png)

   U kunt ook de opdracht **else if** de hulpfunctie om voorwaarden met veelvoudige inhoudvarianten te bouwen. De onderstaande expressie geeft bijvoorbeeld drie varianten van een bericht weer, afhankelijk van de taal van de ontvanger:

   ![](assets/condition-sample3.png)

1. Zodra uw voorwaarde klaar is, kunt u uw inhoud opslaan en de rendering ervan controleren door uw inhoud te simuleren.

## Voorwaardelijke inhoud maken in e-mails  {#condition-condition-builder}

Voorwaardelijke inhoud in e-mails kan op twee manieren worden gemaakt:
* In de uitdrukkingsredacteur door een voorwaarde te bouwen gebruikend helperfuncties,
* In een speciale voorwaardelijke inhoudsontwikkelaar die toegankelijk is wanneer u een e-mail ontwerpt.

Gedetailleerde informatie over het maken van voorwaarden met de expressieeditor is beschikbaar [hier](#condition-perso-editor).

In de onderstaande sectie vindt u instructies voor het maken van voorwaarden met behulp van de voorwaardelijke inhoudsontwikkelaar van de e-mailontwerper. In dit voorbeeld maken we een e-mailbericht met meerdere varianten afhankelijk van de taal van de ontvangers. Ga als volgt te werk om dit te doen:

1. Maak of open een e-maillevering, bewerk de inhoud en klik op de knop **[!UICONTROL Edit email body]** om de werkruimte voor het ontwerpen van e-mail te openen.

1. Selecteer een inhoudscomponent en klik op **[!UICONTROL Enable conditional content]**.

   ![](assets/condition-email-enable.png)

1. De **[!UICONTROL Conditional Content]** wordt aan de linkerkant van het scherm geopend. In dit deelvenster kunt u meerdere varianten van de geselecteerde inhoudscomponent maken aan de hand van voorwaarden.

1. Vorm uw eerste variant. Houd de muisaanwijzer boven **[!UICONTROL Variant - 1]** in de **[!UICONTROL Conditional Content]** en klik op de knop **[!UICONTROL Add condition]** pictogram.

1. Er wordt een regelbouwer weergegeven. Gebruik de profielkenmerken om de voorwaarde voor de eerste variant van het bericht te maken en klik **[!UICONTROL Confirm]**. In dit voorbeeld creëren we een regel die gericht is op ontvangers die &#39;Frans&#39; zijn.

   ![](assets/condition-email-rule.png)

1. De regel is nu gekoppeld aan de variant. Voor betere leesbaarheid raden we u aan de naam van de variant te wijzigen door op het ovaalmenu te klikken.

   Vorm nu hoe de component zou moeten tonen als de regel wordt voldaan aan wanneer het verzenden van het bericht. In dit voorbeeld willen we de tekst in het Frans weergeven als dit de voorkeurstaal van de ontvanger is.

   ![](assets/condition-email-variant1.png)

1. Voeg zoveel varianten toe als nodig zijn voor de inhoudscomponent. U kunt op elk gewenst moment schakelen tussen de verschillende varianten om te controleren hoe de inhoudcomponent afhankelijk van de voorwaardelijke regels wordt weergegeven.

   >[!NOTE]
   >Als aan geen van de regels in de varianten wordt bepaald wanneer het verzenden van het bericht wordt voldaan, zal de inhoudscomponent de inhoud tonen die in wordt bepaald **[!UICONTROL Default variant]** van de **[!UICONTROL Conditional Content]** venster.
