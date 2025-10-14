---
audience: end-user
title: De activiteit van de gegevenswerkstroom bijwerken gebruiken
description: Leer hoe u de activiteit van de gegevenswerkstroom bijwerken gebruikt
exl-id: db978482-43f6-48a7-8d8d-4b921eb610b2
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 9%

---

# Gegevens bijwerken {#update-data}

De **gegevens van de Update** activiteit is a **het Beheer van Gegevens** activiteit. Hiermee kunt u een massa-update uitvoeren op velden in de database. U kunt de gegevensupdate op verschillende manieren aanpassen.

<!--
The **Operation type** field lets you choose the process to be carried out on the data in the database. Select the first option to add data or update it if it has already been added. You can also only add data, only update data, or delete data. Select the **Update and merge collections** to select a primary record to link duplicates to, and delete those duplicates safely.

Specify how to identify the records in the database: if data relate to an existing targeting dimension, select the **Using the targeting dimension** option and select the targeting dimension and fields to update. Otherwise, specify one or more custom links to identify the data in the database, or directly use reconciliation keys.

Select the fields to update and reconciliation settings. You can use the **Auto-mapping** option to automatically identify the fields to be updated.

The **Advanced options** section lets you specify additional settings to manage data and duplicates.

Toggle the **Generate an outbound transition** option to add an outbound transition that will be activated at the end of the execution of the **Update data** activity. The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.

Toggle the **Generate an outbound transition for rejects** option to add an outbound transition containing records that have not been correctly processed after the update (for example, if there is a duplicate). The update generally marks the end of a targeting workflow, and therefore the option is not activated by default.
-->

## De updategegevensactiviteit configureren {#update-data-configuration}

Om de **gegevens van de Update** activiteit te vormen, voeg de activiteit aan uw werkschema toe en bepaal een etiket.

![&#x200B; Activiteit van de Gegevens van de Update van het Werkschema &#x200B;](../assets/workflow-update-data.png)

### Type bewerking

Het **type van Verrichting** gebied laat u het proces kiezen dat op de gegevens in het gegevensbestand moet worden uitgevoerd:

* **Tussenvoegsel of update**: De gegevens van het tussenvoegsel of werkt het bij als de verslagen reeds in het gegevensbestand bestaan.
* **Tussenvoegsel**: De gegevens van het Tussenvoegsel slechts. Records die al bestaan, worden niet bijgewerkt. Als er afstemmingscriteria worden gedefinieerd, worden alleen de niet-afgestemde records toegevoegd.
* **Update**: De gegevens van de update van de verslagen die reeds in het gegevensbestand slechts bestaan.
* **Schrapping**: Schrap gegevens.

Het **gebied van de Partij** laat u het aantal binnenkomende overgangselementen selecteren die moeten worden bijgewerkt. Als u bijvoorbeeld 500 opgeeft, worden de eerste 500 verwerkte records bijgewerkt.

### Registeridentificatie

In deze sectie kunt u opgeven hoe de records in de database moeten worden geïdentificeerd:

* Als de gegevensingangen op bestaand richten afmeting betrekking hebben, selecteer **Gebruikend de het richten afmeting** optie, en kies het op **het richten afmeting om** gebied bij te werken.
* U kunt **ook selecteren Gebruikend douaneverbindingen** en één of meerdere verbindingen specificeren die identificatie van de gegevens in het gegevensbestand zullen toelaten.
* Als het geselecteerde verrichtingstype een update vereist, gebruik **Gebruikend verzoeningsregels** optie.

### Bij te werken velden

In de **Gebieden om** sectie bij te werken, voeg de gebieden toe waarop de update zal worden toegepast. Voeg zo nodig voorwaarden toe om deze update uit te voeren. Gebruik **in aanmerking genomen als** gebied om voorwaarden te bepalen. De voorwaarden worden opeenvolgend toegepast in lijstorde. Gebruik de pijlen aan de rechterkant om de volgorde van de updates te wijzigen. U kunt hetzelfde bestemmingsveld meerdere keren gebruiken.

Verbind automatisch gebieden gebruikend de **auto-afbeelding** knoop. Door automatische koppeling worden velden met dezelfde naam gedetecteerd.

Tijdens **Tussenvoegsel of werk** verrichtingstype bij, selecteer individueel de verrichting om voor elk gebied van toepassing te zijn. Gebruik het **het type van Verrichting** gebied om de gewenste waarde te specificeren.

### Geavanceerde opties

De **Geavanceerde opties** sectie laat u extra opties specificeren om het bijwerken van gegevens te behandelen en duplicaten te beheren.

<!--
* **Disable automatic key management**
* **Disable audit**
* **Empty the destination value if the source value is empty**
* **Update all columns with matching names**
* **Ignore records which concern the same target**: only the first in the list of expressions will be considered
-->

Met de laatste twee opties kunt u specifieke handelingen uitvoeren:

* **produceer een uitgaande overgang**: Creeert een uitgaande overgang die aan het eind van uitvoering zal worden geactiveerd. Bij het bijwerken wordt doorgaans het einde van een doelworkflow aangegeven en wordt de optie daarom niet standaard geactiveerd.

* **produceer een uitgaande overgang voor verwerpt**: Creeert een uitgaande overgang die verslagen bevat die niet correct na de update (bijvoorbeeld, als er een dubbel is) zijn verwerkt. De update markeert doorgaans het einde van een doelworkflow en de optie wordt niet standaard geactiveerd.