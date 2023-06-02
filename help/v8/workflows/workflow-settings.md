---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
exl-id: 7ac8eedf-c141-4a61-b4d3-d81f99247c6d
source-git-commit: eed308685edc00c61d59f1529f363ac9b57d25cf
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 2%

---

# Workflowinstellingen configureren {#workflow-settings}

Wanneer u workflowactiviteiten op het canvas ordent, hebt u toegang tot geavanceerde instellingen die betrekking hebben op de workflow. U kunt bijvoorbeeld een specifieke tijdzone voor de workflow instellen, beheren hoe de workflow zich moet gedragen als er een fout optreedt, of de vertraging beheren waarna de werkstroomgeschiedenis moet worden gewist.

Deze instellingen zijn vooraf geconfigureerd in de sjabloon die is geselecteerd tijdens het maken van de workflow, maar kunnen zo nodig worden bewerkt voor deze specifieke workflow.

Om dit te doen, klik **[!UICONTROL Workflow settings]** in de linkerbovenhoek van het canvas, naast het workflowlabel.

![](assets/workflow-settings.png)

## Workfloweigenschappen {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workfloweigenschappen"
>abstract="Deze sectie biedt algemene workfloweigenschappen die ook toegankelijk zijn wanneer u de workflow maakt. U kunt de sjabloon kiezen die u wilt gebruiken om de workflow te maken en een label opgeven. Vouw de sectie Aanvullende opties uit om specifieke instellingen te configureren, zoals de workflow waarin de map of tijdzone wordt opgeslagen."

De **[!UICONTROL Properties]** biedt algemene instellingen die ook toegankelijk zijn wanneer u de workflow maakt.

* **[!UICONTROL Label]**: Het label van de workflow die in de lijst wordt weergegeven.
* **[!UICONTROL Name]**: De interne naam van de workflow.
* **[!UICONTROL Folder]**: De map waarin de workflow moet worden opgeslagen.
* **[!UICONTROL Linked campaign]**: Dit gebied toont als het werkschema binnen een campagne is gecreeerd. Hiermee kunt u de bijbehorende campagne openen.
* **[!UICONTROL Timezone]**: Definieer een specifieke tijdzone die standaard moet worden gebruikt in alle activiteiten van de workflow. Standaard is de tijdzone van de workflow de tijdzone die is gedefinieerd voor de huidige Campaign-operator.
* **[!UICONTROL Supervisor(s)]**: Wanneer een workflow een fout bevat, worden de operatoren die tot de groep voor workflowtoezicht behoren, via e-mail op de hoogte gebracht, zolang hun e-mailadres in hun profiel wordt vermeld.
* **[!UICONTROL Description]**: Gebruik dit veld om een beschrijving van uw workflow te geven.

## Segmenteringsinstellingen

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinstellingen"
>abstract="In deze sectie kunt u de doeldimensie selecteren voor doelprofielen in de workflow en ervoor kiezen om de werkstroomresultaten tussen twee uitvoeringen te houden. Deze optie mag alleen voor testdoeleinden worden gebruikt en mag nooit in een productiewerkstroom worden ingeschakeld."

* **[!UICONTROL Targeting dimension]**: Selecteer de doeldimensie die u wilt gebruiken voor de doelprofielen: ontvangers, begunstigden van contracten, exploitanten, abonnees, enz.
* **[!UICONTROL Keep the result of interim populations between two executions]**: Standaard blijven alleen de werktabellen van de laatste uitvoering van de workflow behouden. De werklijsten van vorige uitvoeringen worden gezuiverd door een technische werkschema, die op een dagelijkse basis loopt.

   Als deze optie is ingeschakeld, worden werktabellen ook bewaard nadat de workflow is uitgevoerd. U kunt het voor testdoeleinden gebruiken en moet daarom alleen worden gebruikt in ontwikkelings- of testomgevingen. Deze mag nooit in een productiewerkstroom worden gecontroleerd.

## Instellingen voor uitvoering

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Instellingen voor uitvoering"
>abstract="In deze sectie kunt u instellingen configureren die betrekking hebben op de uitvoering van de workflow, zoals het aantal dagen dat de werkstroomgeschiedenis wordt bewaard."

* **[!UICONTROL History in days]**: Hier geeft u het aantal dagen op waarna de historie moet worden gewist. De geschiedenis bevat elementen die gerelateerd zijn aan de workflow: logbestanden, taken, gebeurtenissen (technische objecten die zijn gekoppeld aan de workflowbewerking). De standaardwaarde is 30 dagen voor workflowsjablonen buiten de box. De geschiedenis wordt gewist door de technische workflow voor het opschonen van databases, die standaard dagelijks wordt uitgevoerd

   >[!IMPORTANT]
   >
   >Als de **[!UICONTROL History in days]** veld blanco gelaten, wordt de waarde ervan beschouwd als &quot;1&quot;, wat betekent dat de geschiedenis na 1 dag wordt gewist.

* **[!UICONTROL Default affinity]**: Als uw installatie meerdere workflowservers bevat, gebruikt u dit veld om de computer te kiezen waarop de workflow wordt uitgevoerd. Als de waarde die in dit veld wordt gedefinieerd, op geen enkele server bestaat, blijft de workflow in behandeling.

* **[!UICONTROL Save SQL queries in log]**: Hiermee kunt u de SQL-query&#39;s uit de workflow opslaan in de logbestanden. Deze functionaliteit is gereserveerd voor geavanceerde gebruikers. Het is van toepassing op werkstromen die gericht activiteiten zoals bevatten **[!UICONTROL Build audience]**. Als deze optie is ingeschakeld, worden de SQL-query&#39;s die tijdens de uitvoering van de workflow naar de database worden verzonden, weergegeven in de logbestanden van de workflow, zodat u ze kunt analyseren om query&#39;s te optimaliseren of problemen op te sporen.

## Instellingen voor foutbeheer

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Instellingen voor foutbeheer"
>abstract="In deze sectie kunt u beheren hoe de workflow moet werken wanneer een fout optreedt tijdens de uitvoering (het pauzeren/stoppen of negeren van fouten)."

* **[!UICONTROL Error management]**: In dit veld kunt u de acties definiëren die moeten worden uitgevoerd als een workflowtaak fouten bevat. Er zijn twee mogelijke opties:

   * **[!UICONTROL Suspend the process]**: De werkstroom wordt automatisch onderbroken en de status wordt gewijzigd in **[!UICONTROL Failed]**. Als het probleem is opgelost, hervat u de workflow met de **[!UICONTROL Resume]** knoppen.
   * **[!UICONTROL Ignore]**: De status van de taak die de fout heeft veroorzaakt, verandert in **[!UICONTROL Failed]**, maar de workflow houdt de **[!UICONTROL Started]** status. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abord the process]**: De workflow wordt automatisch beëindigd en de status ervan verandert in **[!UICONTROL Failed]**. Als het probleem is opgelost, start u de workflow opnieuw met de **[!UICONTROL Start]** knoppen.

* **[!UICONTROL Consecutive errors]**: Dit veld is beschikbaar wanneer de **[!UICONTROL Ignore]** waarde is geselecteerd in het dialoogvenster **[!UICONTROL In case of errors]** veld. U kunt opgeven hoeveel fouten kunnen worden genegeerd voordat het proces wordt gestopt. Zodra dit aantal wordt bereikt, verandert de werkschemastatus in **[!UICONTROL Failed]**. Als de waarde van dit veld 0 is, wordt de workflow nooit gestopt, ongeacht het aantal fouten.
