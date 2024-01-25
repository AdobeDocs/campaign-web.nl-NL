---
title: Werken met vooraf gedefinieerde filters
description: Leer hoe u vooraf gedefinieerde filters maakt en beheert in Adobe Campaign Web
badge: label="Beperkte beschikbaarheid"
exl-id: f6b73792-063d-4371-93e1-efa2aa02ee28
source-git-commit: cbfd821173466c51e9073f01e8792cbdc069c6a2
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

# Werken met vooraf gedefinieerde filters {#predefined-filters}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card4"
>title="Vooraf gedefinieerd filterbeheer"
>abstract="Campagne Web biedt u nu een gebruikersvriendelijke interface om vooraf gedefinieerde filters moeiteloos te beheren en aan te passen aan uw specifieke behoeften. Maak één keer en sla dit op voor toekomstig gebruik."


<!--TO REMOVE BELOW-->
>[!CONTEXTUALHELP]
>id="acw_homepage_card4"
>title="Vooraf gedefinieerd filterbeheer"
>abstract="Campagne Web biedt u nu een gebruikersvriendelijke interface om vooraf gedefinieerde filters moeiteloos te beheren en aan te passen aan uw specifieke behoeften. Maak één keer en sla dit op voor toekomstig gebruik."

<!--TO REMOVE ABOVE-->


>[!CONTEXTUALHELP]
>id="acw_predefined-filters-dashboard"
>title="Vooraf gedefinieerde filters"
>abstract="Campagne Web biedt u nu een gebruikersvriendelijke interface om vooraf gedefinieerde filters moeiteloos te beheren en aan te passen aan uw specifieke behoeften. Maak één keer en sla dit op voor toekomstig gebruik."

Vooraf gedefinieerde filters zijn aangepaste filters die worden gemaakt en opgeslagen om in de toekomst beschikbaar te zijn. Zij kunnen als kortere weg tijdens om het even welke het filtreren verrichtingen met de vraagmodeller, bijvoorbeeld worden gebruikt wanneer het filtreren van een lijst van gegevens, of het creëren van het publiek van een levering.

U kunt bestaande ingebouwde filters gebruiken om toegang te krijgen tot een specifieke subset van uw gegevens, of uw eigen vooraf gedefinieerde filters maken en deze opslaan.

![](assets/predefined-filters-menu.png)

>[!IMPORTANT]
>
>In die versie van het product, wanneer het bouwen van regels, het selecteren van het publiek van een levering, of wanneer het bouwen van een publiek in een werkschema, zijn sommige vooraf bepaalde filters niet beschikbaar in het gebruikersinterface. U kunt ze nog steeds gebruiken. [Meer informatie](guardrails.md#predefined-filters-filters-guardrails-limitations)


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

U kunt een aangepast filter opslaan in het dialoogvenster [querymodel](../query/query-modeler-overview.md) om het voor toekomstig gebruik beschikbaar te hebben. Voer de volgende stappen uit:

1. Open de vraagmodeler en bepaal uw het filtreren voorwaarden. In het onderstaande voorbeeld filtert u ontvangers die in Madrid wonen en zich op een nieuwsbrief hebben geabonneerd.
1. Klik op de knop **Filter selecteren of opslaan** en selecteert u **Opslaan als filter**.

   ![](assets/predefined-filters-save.png)

1. Selecteren **Een nieuw filter maken** en voert u een naam en een beschrijving voor dat filter in.

   ![](assets/predefined-filters-save-filter.png)

   U kunt het filter indien nodig opslaan als favoriet. Meer informatie in [deze sectie](#fav-filter).

1. Klikken **Bevestigen** om uw wijzigingen op te slaan.

Uw aangepaste filter is nu beschikbaar in het dialoogvenster **Vooraf gedefinieerde filters** en toegankelijk voor alle campagnegebruikers.


### Een filter maken in de filterlijst {#create-filter-from-list}

U kunt een filter maken op basis van het **Vooraf gedefinieerde filters** in het linkermenu. Volg onderstaande stappen om dit te doen:

1. Bladeren in het dialoogvenster **Vooraf gedefinieerde filters** in het linkermenu.
1. Klik op de knop **Filter maken** knop.
1. Voer de filternaam in en typ **Documenttype** selecteert u het schema waarop het van toepassing is. Het standaardschema is `Recipients(nms)`.


1. Definieer de regel voor het filter. Profielen die ouder zijn dan 30.

   ![](assets/filter-30+.png)


1. Sla uw wijzigingen op.

   ![](assets/new-filter.png)


Het filter wordt toegevoegd aan de vooraf gedefinieerde filterlijst. U kunt het filter indien nodig opslaan als favoriet. Meer informatie in [deze sectie](#fav-filter).


## Filter opslaan als favoriet {#fav-filter}

Wanneer u een vooraf gedefinieerd filter maakt, kunt u **Opslaan als favoriet** als u dit vooraf gedefinieerde filter wilt zien in uw favorieten.


Wanneer een filter als favoriet wordt opgeslagen, is het beschikbaar voor alle gebruikers in **Favoriete filters** sectie van de lijst van de filterverwezenlijking, zoals hieronder getoond:

![](assets/predefined-filters-favorite.png){width="30%" align="left"}

## Een vooraf gedefinieerd filter gebruiken {#use-predefined-filter}

Vooraf gedefinieerde filters zijn beschikbaar wanneer u regeleigenschappen definieert. Als u toegang wilt tot vooraf gedefinieerde filters, kiest u **Aangepast filter selecteren** in de drop-down van vraagmodeler.

Vervolgens hebt u toegang tot de volledige lijst met vooraf gedefinieerde filters die beschikbaar zijn voor de huidige context.

U kunt ook de filtersneltoetsen gebruiken die beschikbaar zijn in het dialoogvenster **Favoriete filters** van de vervolgkeuzelijst. Meer informatie over favorieten vindt u in [deze sectie](#fav-filter).

Als u bijvoorbeeld een publiek wilt maken op basis van een vooraf gedefinieerd filter, voert u de volgende stappen uit:

1. Bladeren in het dialoogvenster **Soorten publiek** in het linkermenu.
1. Klik op de knop **Publiek maken** knop.
1. Voer de naam van het publiek in en klik op **Publiek maken** knop.
1. Selecteer de **Query** activiteit, en, van de juiste ruit, klik **publiek maken** knop.

   ![](assets/build-audience-from-filter.png)

1. Van de **Filterknop selecteren of opslaan**, kiest u de **Aangepast filter selecteren** -optie.

   ![](assets/build-audience-select-custom-filter.png)

1. Blader naar het vooraf gedefinieerde filter dat u wilt gebruiken om het publiek te maken, selecteer het en bevestig het.

   ![](assets/build-audience-filter-list.png)

1. Controleer de regeleigenschappen voor dit filter en bevestig.

   Het filter wordt nu gebruikt als een query in het dialoogvenster **Query** activiteit.

   ![](assets/build-audience-confirm.png)

1. Sla uw wijzigingen op en klik op de knop **Start** om het publiek te maken en beschikbaar te maken in de lijst met doelgroepen.

## Uw vooraf gedefinieerde filters beheren {#manage-predefined-filter}

Vooraf gedefinieerde filters worden allemaal gegroepeerd in de toegewezen vermelding van het navigatiemenu links.

![](assets/list-of-filters.png)

In deze lijst kunt u een nieuw filter maken, zoals hierboven beschreven, en:

* een bestaand filter bewerken en de regels en eigenschappen ervan wijzigen
* Een vooraf gedefinieerd filter dupliceren
* een vooraf gedefinieerd filter verwijderen

U kunt een vooraf gedefinieerd filter als favoriet voor een snelle toegang toevoegen wanneer het bouwen van uw publiek. Meer informatie in [deze sectie](#fav-filter).

<!--
## Built-in predefined filters {#ootb-predefined-filter}

Campaign comes with a set of predefined filters, built from the client console. These filters can be used to define your audiences, and rules. They must not be modified.
-->
