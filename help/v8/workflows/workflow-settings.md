---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: 806e465b7c1df6cd26d68103c45b175371d73485
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 2%

---

# Geavanceerde workflowinstellingen configureren {#workflow-settings}

Wanneer u workflowactiviteiten op het canvas ordent, hebt u toegang tot geavanceerde instellingen die betrekking hebben op de workflow. U kunt bijvoorbeeld een specifieke tijdzone voor de workflow instellen, beheren hoe de workflow zich moet gedragen als er een fout optreedt, of de vertraging beheren waarna de werkstroomgeschiedenis moet worden gewist.

Om dit te doen, klik **[!UICONTROL Workflow settings]** in de linkerbovenhoek van het canvas, naast het workflowlabel.

![](assets/workflow-settings.png)

## Workfloweigenschappen {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workfloweigenschappen"
>abstract="TBD"

De sectie met workfloweigenschappen biedt algemene eigenschappen die ook toegankelijk zijn wanneer u de workflow maakt.

* **[!UICONTROL Label]**: Het label van de workflow die in de lijst wordt weergegeven.
* **[!UICONTROL Internal name]**: De interne naam van de workflow.
* **[!UICONTROL Folder]**: De map waarin de workflow moet worden opgeslagen.
* **[!UICONTROL Linked campaign]**: Dit gebied toont als het werkschema binnen een campagne is gecreeerd. Hiermee kunt u de bijbehorende campagne openen.
* **[!UICONTROL Timezone]**: Definieer een specifieke tijdzone die standaard moet worden gebruikt in alle activiteiten van de workflow. Standaard is de tijdzone van de workflow de tijdzone die is gedefinieerd voor de huidige Campaign-operator.
* **[!UICONTROL Supervisor]**: Wanneer een workflow een fout bevat, worden de operatoren die tot de groep voor workflowtoezicht behoren, via e-mail op de hoogte gebracht, zolang hun e-mailadres in hun profiel wordt vermeld.
* **[!UICONTROL Description]**: Gebruik dit veld om een beschrijving van uw workflow te geven.

## Segmenteringsinstellingen

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinstellingen"
>abstract="TBD"

* **[!UICONTROL Targeting dimension]**: Selecteer de doeldimensie die u wilt gebruiken voor de doelprofielen: ontvangers, begunstigden van contracten, exploitanten, abonnees, enz.
* **[!UICONTROL Keep the result of interim populations between two executions]**: Standaard blijven alleen de werktabellen van de laatste uitvoering van de workflow behouden. De werklijsten van vorige uitvoeringen worden gezuiverd door een technische werkschema, die op een dagelijkse basis loopt.

   Als deze optie is ingeschakeld, worden werktabellen ook bewaard nadat de workflow is uitgevoerd. U kunt het voor testdoeleinden gebruiken en moet daarom alleen worden gebruikt in ontwikkelings- of testomgevingen. Het mag nooit worden gecontroleerd in een productiewerkstroom,

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
