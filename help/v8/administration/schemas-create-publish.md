---
title: Schema's maken en publiceren
description: Leer hoe u schema's maakt, uitbreidt en publiceert.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Schema&#39;s maken en publiceren {#create-publish}

## Schema&#39;s maken en beheren {#create-schemas}

U kunt nieuwe schema&#39;s tot stand brengen, bestaande schema&#39;s uitbreiden, en tot externe gegevensbestanden toegang hebben.

### Een schema maken of uitbreiden {#create-new}

Een schema maken of uitbreiden:

1. Ga naar **[!UICONTROL Administration]** > **[!UICONTROL Schemas]**.
1. Klik op **[!UICONTROL Create schema]**.

   ![ de aanmaakdialoog van het Schema ](assets/schemas-create1.png)

1. Voer een naamruimte in voor uw schema (bijvoorbeeld `cus` voor aangepaste schema&#39;s).
1. Voer een unieke naam en een uniek label in en kies of u een nieuw schema wilt maken of een bestaand schema wilt uitbreiden.

1. Klik op **[!UICONTROL Create]**.
   ![ de aanmaakdialoog van het Schema ](assets/schemas-create2.png)

Het schema wordt gecreeerd en de geproduceerde schemastructuur wordt getoond.

Het schema is standaard leeg. U moet nu de gebieden toevoegen u in uw schema wilt omvatten gebruikend de schemaredacteur:

1. Klik op het potloodpictogram in de sectie **[!UICONTROL Content]** van het scherm Schema-details.
2. Voeg de benodigde elementen toe en sla deze op. Hier volgt een voorbeeld van een aangepaste schemastructuur:

   ![ de aanmaakdialoog van het Schema ](assets/schemas-create3.png)

Het systeem valideert automatisch de XML-structuur en genereert het schema.

### Schermeditie definiëren {#define-attributes}

Nadat u het schema hebt gemaakt, moet u de schermeditie definiëren.

Voor meer informatie over het scherm van de het schermdefinitie en hoe te om tot het toegang te hebben, verwijs naar [ toegang tot de sectie van de het schermdefinitie ](schemas-browse-access.md#screen-def).

In ons voorbeeld voegen we gewoon twee aangepaste velden toe:

1. Klik op de knop **[!UICONTROL Screen edition]** in de weergave Schema-details om de schermdefinitie te openen.

1. Klik op het pictogram van de ovaal boven de tabel **[!UICONTROL List of custom fields]** en kies **[!UICONTROL Select attributes]** .
1. Selecteer de aangepaste velden die u wilt toevoegen en bevestigen.

   ![ de aanmaakdialoog van het Schema ](assets/schemas-create4.png)

## Schema&#39;s publiceren en synchroniseren {#publish}

Na het creëren van of het wijzigen van een schema, moet u het publiceren om het logische schema met de fysieke gegevensbestandstructuur te synchroniseren.

### Schema-wijzigingen publiceren {#publish-changes}

>[!CAUTION]
>
>Als u schemawijzigingen publiceert, wordt de databasestructuur gewijzigd. Zorg ervoor dat u de gevolgen van deze wijzigingen begrijpt voordat u de publicatie bevestigt.

Uw schemawijzigingen publiceren:

1. Navigeer naar **[!UICONTROL Administration]** > **[!UICONTROL Schemas]** om het schema te openen.
1. Klik op **[!UICONTROL Publishing]** en bevestig het.

   ![ de publicatiedialoog die van het Schema veranderingen toont om worden toegepast ](assets/schemas-publish1.png)

1. Selecteer in de lijst het schema dat u wilt synchroniseren.

   ![ de publicatiedialoog die van het Schema veranderingen toont om worden toegepast ](assets/schemas-publish2.png)

1. Controleer het SQL-script dat wordt uitgevoerd om de databasestructuur bij te werken.
1. Klik op **[!UICONTROL Publish]** en bevestig om door te gaan met de publicatie.

>[!NOTE]
>
>Het proces kan enige tijd duren, afhankelijk van de grootte van uw database en de complexiteit van de wijzigingen.

### Een navigatie-item maken {#navigation}

Na het publiceren van een douaneschema, kunt u een navigatieingang in de Ontdekkingsreiziger tot stand brengen om tot uw douanegegevens toegang te hebben:

1. Navigeer naar het menu **[!UICONTROL Explorer]** en selecteer een map waarin u het aangepaste schema wilt plaatsen.
1. Klik op het pictogram voor de ovaal en klik op **[!UICONTROL Create new folder]** .
   ![ de ingangsverwezenlijking van de Navigatie voor douaneschema ](assets/schemas-publish3.png)
1. Voeg een label toe en kies uw schema in het **[!UICONTROL Folder type]** gebied.
   ![ de ingangsverwezenlijking van de Navigatie voor douaneschema ](assets/schemas-publish5.png)
1. Het aangepaste schema is nu toegankelijk vanuit de weergave **[!UICONTROL Explorer]** .

Vanuit de nieuwe map kunt u:

* Bekijk de lijst met records in uw aangepaste schema.
* Nieuwe records maken.
* Bestaande records bewerken en verwijderen.
* Pas aan welke kolommen standaard worden weergegeven in de lijstweergave.
