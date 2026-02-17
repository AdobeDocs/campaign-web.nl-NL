---
title: Bladeren en toegang krijgen tot schema's
description: Leer hoe te om en toegangsschema's in de interface te doorbladeren.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Toegang tot en vorm schema&#39;s {#access}

Schema&#39;s zijn toegankelijk via het menu **[!UICONTROL Administration]** > **[!UICONTROL Schemas]** .

![ het lijstscherm van Schema&#39;s die beschikbare schema&#39;s en filters tonen ](assets/schemas-list.png)

Vanuit dit scherm kunt u alle bestaande schema&#39;s weergeven. Er zijn filters beschikbaar waarmee u de lijst kunt verfijnen, zoals alleen bewerkbare schema&#39;s weergeven.

Als u een schema wilt openen, selecteert u de naam ervan. Er wordt een gedetailleerde schemaweergave weergegeven.

![ het detailscherm van het Schema die schemaeigenschappen en inhoud tonen ](assets/schema-details.png)

## Overzicht van schema {#overview}

Het tabblad **[!UICONTROL Overview]** biedt een algemene weergave van het schema:

* In de sectie **[!UICONTROL Properties]** worden belangrijke gegevens weergegeven, zoals de naam van het schema, de naamruimte en de bijbehorende tabelnaam.

* In de sectie **[!UICONTROL Schema definition]** worden details weergegeven over de schemadefinitie, waaronder de primaire sleutel die wordt gebruikt voor het afstemmen van gegevens en de koppelingen naar andere tabellen.

  Klik op de knop **[!UICONTROL Schema preview]** om de verschillende velden en koppelingen waaruit het schema bestaat, weer te geven. Hierdoor kunt u de volledige structuur van een schema controleren. Als het schema is uitgebreid met aangepaste velden, kunt u alle extensies visualiseren.

* In de sectie **[!UICONTROL Content]** wordt de XML-inhoud van het schema weergegeven, zodat u kunt schakelen tussen de bron en de gegenereerde syntaxis.

## Schema-gegevens {#data}

Het tabblad **[!UICONTROL Data]** bevat informatie over de schemagegevens.

![ de gegevenslusje van het Schema die gegevensstructuur en attributen tonen ](assets/schemas-data.png)

## Schermweergave aanpassen {#screen-def}

Met de schermdefinitie kunt u configureren hoe schemavelden worden weergegeven en bewerkt in de interface. U kunt standaardkolommen configureren voor lijstweergaven, aanpassen welke aangepaste velden worden weergegeven in detailschermen, verzamelingslijsten toevoegen om verwante gegevens weer te geven en velden indelen in secties met scheidingstekens en zichtbaarheidscriteria.

De schermdefinitie openen:

1. Blader naar het menu **[!UICONTROL Schemas]** en zoek bewerkbare schema&#39;s met de filters.

   ![ het lijstscherm van Schema&#39;s die beschikbare schema&#39;s en filters tonen ](assets/schemas-list2.png)

1. Selecteer de schemanaam in de lijst om het te openen en de **[!UICONTROL Screen edition]** knoop in de mening van schemadetails te klikken om tot de het schermdefinitie toegang te hebben.

   ![ het lijstscherm van Schema&#39;s die beschikbare schema&#39;s en filters tonen ](assets/schemas-list3.png)

   Met de verschillende lijsten kunt u elementen opnieuw ordenen met de pictogrammen Pijl-omhoog en Pijl-omlaag of door ze te slepen en neer te zetten. Als u items wilt verwijderen, klikt u op het prullenbakpictogram op een bepaalde rij of selecteert u **[!UICONTROL Delete all]** in het ellipspictogram.

   ![ de definitie van het Scherm Algemene sectie ](assets/schemas-general.png)

Vanuit de schermdefinitie kunt u:

* [ vorm standaardlijstkolommen ](schemas-list-columns.md) - vorm welke kolommen door gebrek in lijstmeningen worden getoond.
* [ geef douanegebieden ](schemas-custom-fields.md) uit - vorm welke douanegebieden op detailschermen worden getoond en organiseer hen in secties.
* [ voeg inzamelingslijsten ](schemas-collection-lists.md) toe - voeg inzamelingslijsten toe om verwante gegevens in profielschermen te tonen.
