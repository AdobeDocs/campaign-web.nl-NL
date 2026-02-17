---
title: Werken met aangepaste formulieren
description: Leer hoe u records in aangepaste schema's maakt, bewerkt en beheert met formulieren voor gegevensinvoer.
source-git-commit: be4876090ecaac853aaa88948505c444bef27ec2
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Werken met aangepaste formulieren {#custom-forms}

De vormen van de douane zijn interfaces van de gegevensingang die u toestaan om verslagen in douaneschema&#39;s direct van het Gebruikersinterface van het Web te beheren. Elk aangepast formulier komt overeen met een specifiek aangepast schema en biedt een lijstweergave voor het bladeren in records en een detailweergave voor het maken, bewerken en verwijderen van records.

Aangepaste formulieren zijn gebaseerd op de formulierdefinitie (schermdefinitie) van het schema, waarin wordt gedefinieerd welke velden worden weergegeven en hoe deze worden ingedeeld.

>[!NOTE]
>
>Aangepaste formulieren zijn alleen beschikbaar voor schema&#39;s waarvoor een formulierdefinitie is geconfigureerd.

## Aangepaste schema&#39;s maken en publiceren {#form-schema}

U moet eerst uw aangepaste schema&#39;s maken en publiceren. Voor gedetailleerde instructies, verwijs naar deze [ sectie ](schemas-create-publish.md).

Hier volgt het gegevensmodel dat voor dit voorbeeld wordt gebruikt:

* Een ontvanger koopt meerdere aankopen
* Een aankoop is gekoppeld aan een product
* Een product is gekoppeld aan een merk

Voor dit gebruik worden drie schema&#39;s gemaakt: de schema&#39;s Aankopen, Producten en Merk. Hier volgt een voorbeeld:

![ de vormen van de Douane ](assets/schemas-forms.png)

## Schermdefinitie configureren {#form-screen-schema}

Bepaal welke velden worden weergegeven en hoe deze worden ingedeeld. Voor gedetailleerde instructies, verwijs naar deze [ sectie ](schemas-browse-access.md#screen-def).

Hier is een voorbeeld voor het schema van het Merk waar de de douanelijst van Producten wordt toegevoegd. Het formulier bevat vervolgens een lijst met producten die aan het merk zijn gekoppeld.

![ de vormen van de Douane ](assets/schemas-forms2.png)

Voor het schema van Producten, voegen wij de Aankopen douanelijst toe. En voor het schema van Aankopen, de gebieden van het Product en van de Ontvanger.

## Navigatie-items maken {#form-screen-entries}

Maak mappen in de Verkenner voor toegang tot uw aangepaste formulier. Voor gedetailleerde instructies, verwijs naar deze [ sectie ](schemas-create-publish.md#navigation).

![ de vormen van de Douane ](assets/schemas-forms3.png)

In de lijstweergave worden alle records voor dat schema weergegeven. Als voor het schema een formulierdefinitie is geconfigureerd, is de lijst bewerkbaar en kunt u records maken, bewerken en verwijderen.
![ de vormen van de Douane ](assets/schemas-forms4.png)

U kunt dan:

* **Mening en geef verslagen** uit: klik op een verslag in de lijstmening om het in detail te openen mening en gebieden direct uit te geven.
* **creeer nieuwe verslagen**: klik de **[!UICONTROL Create]** knoop en vul de vereiste gebieden in. Voor gekoppelde velden gebruikt u het zoekpictogram om een keuze te maken uit beschikbare verwante records.
* **de verslagen van de Schrapping**: selecteer een verslag en gebruik de schrappingsactie beschikbaar in de verslagdetails of lijstmening.
* **Verwante gegevens van de Mening in lusjes**: toegang verwante verslagen door specifieke lusjes in de detailmening (bijvoorbeeld, bekijk alle producten verbonden aan een merk, of alle aankopen verbonden aan een product).
* **pas filters** toe: gebruik het filterpaneel om de lijstmening te verfijnen en specifieke verslagen te vinden die op om het even welk gebied in uw schema worden gebaseerd.
* **pas lijstkolommen** aan: vorm welke kolommen door gebrek in lijstmeningen door de het schermdefinitie worden getoond.
