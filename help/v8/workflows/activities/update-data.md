---
audience: end-user
title: De activiteit van de gegevenswerkstroom bijwerken gebruiken
description: Leer hoe u de activiteit van de gegevenswerkstroom bijwerken gebruikt
source-git-commit: 347f8f84a8eda60538366eb3dc49f8d7e06379c3
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 12%

---

# Gegevens bijwerken {#update-data}

De **Gegevens bijwerken** activiteit is **Gegevensbeheer** activiteit. Hiermee kunt u een massale update uitvoeren op velden in de database. Met verschillende opties kunt u de gegevensupdate aanpassen.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update (it if it has already been added). You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or direct use of reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section let you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example if there is a duplicate). The update generally marks the end of a targeting workflow and therefore the option is not activated by default.
-->

## De updategegevensactiviteit configureren{#update-data-configuration}

Om te vormen **Gegevens bijwerken** activiteit, begin door de activiteit aan uw werkschema toe te voegen en een etiket te bepalen.

![](../assets/workflow-update-data.png)

### Type bewerking

De **Type bewerking** kunt u het proces kiezen dat op de gegevens in de database moet worden uitgevoerd:

* **Invoegen of bijwerken**: voeg gegevens in of werk deze bij als de records al in de database bestaan.
* **Invoegen**: alleen gegevens invoegen. De al bestaande records worden niet bijgewerkt. Als er afstemmingscriteria worden gedefinieerd, worden alleen de niet-afgestemde records toegevoegd.
* **Bijwerken**: werk alleen de gegevens bij van de records die al in de database bestaan.
* **Verwijderen**: gegevens verwijderen.

De **Batchgrootte** in dit veld kunt u het aantal inkomende overgangselementen selecteren dat moet worden bijgewerkt. Als u bijvoorbeeld 500 opgeeft, worden de eerste 500 records die worden afgehandeld, bijgewerkt.

### Registeridentificatie

In deze sectie kunt u opgeven hoe de records in de database moeten worden geïdentificeerd:

* Als gegevensinvoer betrekking heeft op een bestaande doeldimensie, selecteert u de optie **De doeldimensie gebruiken** en selecteert u deze in het dialoogvenster **Dimensie die moet worden bijgewerkt** veld.
* U kunt ook de optie **Aangepaste koppelingen gebruiken** en een of meer koppelingen specificeren die identificatie van de gegevens in de database mogelijk maken
* Als het geselecteerde bewerkingstype een update vereist, moet u de opdracht **Afstemmingsregels gebruiken** -optie.

### Bij te werken velden

In de **Bij te werken velden** voegt u de velden toe waarop de update wordt toegepast en voegt u, indien nodig, voorwaarden toe zodat deze update wordt uitgevoerd. Om dit te doen, gebruik **Wordt in aanmerking genomen indien** veld. De voorwaarden worden een na een toegepast in de volgorde van de lijst. Gebruik de pijlen aan de rechterkant om de volgorde van de updates te wijzigen. U kunt hetzelfde bestemmingsveld meerdere keren gebruiken.

U kunt velden automatisch koppelen met de **Automatisch toewijzen** knop. Door automatische koppeling worden velden met dezelfde naam gedetecteerd.

Tijdens een **Invoegen of bijwerken** Bij het type bewerking kunt u de bewerking die u voor elk veld wilt toepassen, afzonderlijk selecteren. Selecteer hiertoe de gewenste waarde in het dialoogvenster **Type bewerking** veld.

### Geavanceerde opties

De **Geavanceerde opties** Hiermee kunt u aanvullende opties opgeven voor het bijwerken van gegevens en het beheren van duplicaten.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Met de laatste twee opties kunt u specifieke handelingen uitvoeren:

* **Een uitgaande overgang genereren**: maakt een uitgaande overgang die aan het einde van de uitvoering wordt geactiveerd. Bij het bijwerken wordt doorgaans het einde van een doelworkflow aangegeven en wordt de optie daarom niet standaard geactiveerd.

* **Een uitgaande overgang genereren voor de afwijzing**: maakt een uitgaande overgang die records bevat die niet correct zijn verwerkt na de update (bijvoorbeeld als er een duplicaat is). De update markeert doorgaans het einde van een doelworkflow en daarom wordt de optie niet standaard geactiveerd.
