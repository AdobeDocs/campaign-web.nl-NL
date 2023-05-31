---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 696fa6192c16f8fd1d2dd77ad533203277f8a2dd
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 2%

---

# Workflowinstellingen configureren {#workflow-settings}

inhoud-TBD

instellingen definiëren die beschikbaar zijn via de knop in het werkstroomcanvas
<!--à reformuler-->

## Workfloweigenschappen {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workfloweigenschappen"
>abstract="TBD"

(= hetzelfde als bij het maken van de workflow? te controleren)

* Label
* Aanvullende opties
* Interne naam
* Map
* Gekoppelde campagne > kan deze wijzigen. Als dat het geval is, verdwijnt de workflow uit de huidige campagne en wordt deze weergegeven in de nieuwe gekoppelde campagne

   Wanneer u een workflow binnen een campagne maakt, vindt u een extra veld Campagne waarmee u de campagne die aan de workflow is gekoppeld gemakkelijk kunt identificeren en openen.

* Tijdzone: een specifieke tijdzone definiëren die standaard in alle activiteiten van de workflow moet worden gebruikt. Standaard is de tijdzone van de workflow de tijdzone die is gedefinieerd voor de huidige Campaign-operator.
* Supervisor: Wanneer een workflow een fout bevat, worden de operatoren die tot de groep voor workflowtoezicht behoren, via e-mail op de hoogte gebracht, zolang hun e-mailadres in hun profiel wordt vermeld. Deze groep is geselecteerd in het dialoogvenster **[!UICONTROL Supervisor(s)]** veld van de workfloweigenschappen.
* beschrijving

## Segmenteringsinstellingen

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinstellingen"
>abstract="TBD"

* doelgerichtheid:

   Tijdens de verrichtingen van de gegevenssegmentatie, wordt de het richten sleutel in kaart gebracht aan een het filtreren dimensie. Met de doeldimensie kunt u de doelgroep voor de bewerking definiëren: ontvangers, begunstigden van contracten, exploitanten, abonnees, enz. Met de filterdimensie kunt u de populatie selecteren op basis van bepaalde criteria: contractanten, abonnees van nieuwsbrieven enz.

* resultaten behouden: De **Behoud het resultaat van tussentijdse populaties tussen twee executies** houdt tijdelijke lijsten tussen twee uitvoeringen van een werkschema.  Het is beschikbaar in de eigenschappen van de workflow. **[!UICONTROL General]** en kan worden gebruikt voor ontwikkelings- en testdoeleinden om gegevens te controleren en de resultaten te controleren. U kunt deze optie in ontwikkelomgevingen gebruiken, maar nooit in productieomgevingen. Het houden van tijdelijke lijsten zou in de grootte van het gegevensbestand kunnen resulteren die beduidend en uiteindelijk de groottegrens wordt bereikt. Bovendien zal het de back-up vertragen.

   Alleen de werktabellen van de laatste uitvoering van de workflow worden bewaard. Werktabellen van eerdere uitvoeringen worden door de **[!UICONTROL cleanup]** werkschema, dat dagelijks loopt.

   >[!CAUTION]
   >
   >Deze optie moet **nooit** worden gecontroleerd in een **productie** workflow. Deze optie wordt gebruikt om de resultaten te analyseren en is alleen ontworpen voor testdoeleinden en moet daarom alleen worden gebruikt in ontwikkelings- of testomgevingen.

## Instellingen voor workflowuitvoering

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Instellingen voor uitvoering"
>abstract="TBD"

* Geschiedenis in dagen: De het werklijsten van het gegevensbestand houden een geschiedenis van uitvoeringen (taken, gebeurtenissen, logboek). Hier kunt u het aantal dagen definiëren dat voor deze workflow moet worden gearchiveerd: het schoonmaakproces zal de oudste archieven eenmaal per dag verwijderen . Als de waarde in dit veld nul is, wordt het archief nooit verwijderd.

   geeft het aantal dagen aan waarna de historie moet worden gewist. De geschiedenis bevat elementen die gerelateerd zijn aan de workflow: logbestanden, taken, gebeurtenissen (technische objecten die zijn gekoppeld aan de workflowbewerking) en bestanden die zijn gedownload door de **[!UICONTROL Transfer file]** activiteit. De standaardwaarde is 30 dagen voor workflowsjablonen buiten de box.

   De geschiedenis wordt gewist door de technische workflow voor het opschonen van databases, die standaard dagelijks wordt uitgevoerd

   >[!IMPORTANT]
   >
   >Als de **[!UICONTROL History in days]** veld blanco gelaten, wordt de waarde ervan beschouwd als &quot;1&quot;, wat betekent dat de geschiedenis na 1 dag wordt gewist.

* standaardaffiniteit: in dit veld kunt u ervoor zorgen dat een workflow of een werkstroomactiviteit op een bepaalde computer wordt uitgevoerd.   Als uw installatie meerdere workflowservers bevat, gebruikt u dit veld om de computer te kiezen waarop de workflow wordt uitgevoerd. Als de waarde die in dit veld wordt gedefinieerd, op geen enkele server bestaat, blijft de workflow in behandeling.

* sql queriesi opslaan in logboek: Hiermee kunt u de SQL-query&#39;s uit de workflow opslaan in de logbestanden. (waar kunt u SQL-logbestanden openen?)

   Deze functionaliteit is gereserveerd voor geavanceerde gebruikers. Het heeft betrekking op werkstromen die gericht activiteiten (vraag, vereniging, doorsnede, enz.) bevatten. Als deze optie is ingeschakeld, worden de SQL-query&#39;s die tijdens de uitvoering van de workflow naar de database worden verzonden, weergegeven in Adobe Campaign: dit betekent dat u ze kunt analyseren om query&#39;s te optimaliseren of problemen te diagnosticeren.

   Vragen worden weergegeven in een **[!UICONTROL SQL logs]** tabblad dat wordt toegevoegd aan de workflow (behalve workflows voor campagnes) en de **[!UICONTROL Properties]** activiteit wanneer de optie wordt toegelaten. De **[!UICONTROL Audit]** bevat ook SQL-query&#39;s.

## Instellingen voor foutbeheer

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Instellingen voor foutbeheer"
>abstract="TBD"

* In dit veld kunt u de acties definiëren die moeten worden uitgevoerd als een workflowtaak fouten bevat. Er zijn twee mogelijke opties:

   Stop het proces: de workflow wordt automatisch gepauzeerd. de workflowstatus verandert in Failed. Zodra het probleem is opgelost, start u de workflow opnieuw met de knoppen Start of Opnieuw starten.

   Negeren: De status van de taak die de fout heeft veroorzaakt, verandert in Mislukt, maar de werkstroom behoudt de status Gestart. Deze configuratie is relevant voor terugkerende taken: als de tak een planner omvat, zal het normaal beginnen volgende tijd het werkschema wordt uitgevoerd.

* Opeenvolgende fouten: Dit veld wordt beschikbaar wanneer de waarde Negeren is geselecteerd in het veld Bij fouten. U kunt opgeven hoeveel fouten kunnen worden genegeerd voordat het proces wordt gestopt. Zodra dit aantal wordt bereikt, verandert de werkschemastatus in Ontbroken. Als de waarde van dit veld 0 is, wordt de workflow nooit gestopt, ongeacht het aantal fouten.
