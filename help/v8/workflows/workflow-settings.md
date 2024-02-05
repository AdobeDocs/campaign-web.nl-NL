---
audience: end-user
title: Workflowinstellingen configureren
description: Leer hoe u workflowinstellingen configureert met Adobe Campaign Web
badge: label="Beperkte beschikbaarheid"
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: 1611278f759fb29d014b918e5d1e0f792a4b05a0
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 1%

---


# Workflowinstellingen configureren {#workflow-settings}

Wanneer u workflowactiviteiten op het canvas ordent, hebt u toegang tot geavanceerde instellingen die betrekking hebben op de workflow. U kunt bijvoorbeeld een specifieke tijdzone voor de workflow instellen, beheren hoe de workflow zich moet gedragen als er een fout optreedt, of de vertraging beheren waarna de werkstroomgeschiedenis moet worden gewist.

Deze instellingen zijn vooraf geconfigureerd in de sjabloon die is geselecteerd tijdens het maken van de workflow, maar kunnen zo nodig worden bewerkt voor deze specifieke workflow.

Om dit te doen, klik **[!UICONTROL Settings]** in de actiebalk boven het werkstroomcanvas beschikbaar.

![](assets/workflow-settings-button.png){width="70%" align="left"}

## Workfloweigenschappen {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workfloweigenschappen"
>abstract="Deze sectie biedt algemene workfloweigenschappen die ook toegankelijk zijn wanneer u de workflow maakt. U kunt de sjabloon kiezen die u wilt gebruiken om de workflow te maken en een label opgeven. Vouw de sectie Aanvullende opties uit om specifieke instellingen te configureren, zoals de workflow waarin de map of tijdzone wordt opgeslagen."

De **[!UICONTROL Properties]** biedt algemene instellingen die ook toegankelijk zijn wanneer u de workflow maakt.

![](assets/workflow-settings.png){width="70%" align="left"}


Deze eigenschappen zijn:

* De **[!UICONTROL Label]** van de workflow die in de lijst wordt weergegeven.
* De **[!UICONTROL Internal name]** van de workflow.
* De **[!UICONTROL Folder]** waar de workflow moet worden opgeslagen.
* De standaardwaarde **[!UICONTROL Timezone]** te gebruiken in alle activiteiten van de workflow. Standaard is de tijdzone van de workflow de tijdzone die is gedefinieerd voor de huidige Campagneoperator.
Mogelijke waarden zijn:
   * **Tijdzone van server** de tijdzone van de Adobe Campaign-toepassingsserver gebruiken
   * **Tijdzone van exploitant** om de tijdzone te gebruiken van de Adobe Campaign-operator die de workflow uitvoert, zoals gedefinieerd in het profiel van de operator, in de clientconsole
   * **Tijdzone van de database** om de tijdzone van de gegevensbestandserver te gebruiken
   * Een specifieke tijdzone
* Wanneer een workflow mislukt, worden de operatoren die tot de groep met operatoren behoren, geselecteerd in het dialoogvenster **[!UICONTROL Supervisor(s)]** veld wordt per e-mail op de hoogte gesteld.
* *U kunt ook een **[!UICONTROL Description]** van uw workflow.

Wanneer de workflow [gekoppeld aan een campagne](create-workflow.md), wordt deze weergegeven in het dialoogvenster **[!UICONTROL Linked campaign]** veld. U kunt de bijbehorende campagne vanuit dat veld openen.


## Segmenteringsinstellingen  {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinstellingen"
>abstract="In deze sectie kunt u de doeldimensie selecteren voor doelprofielen in de workflow en ervoor kiezen om de werkstroomresultaten tussen twee uitvoeringen te houden. Deze optie mag alleen voor testdoeleinden worden gebruikt en mag nooit in een productiewerkstroom worden ingeschakeld."

* **[!UICONTROL Targeting dimension]**: Selecteer de doeldimensie die u wilt gebruiken voor doelprofielen: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. [Meer informatie over doelgerichte dimensies](../audience/targeting-dimensions.md)

* **[!UICONTROL Keep the result of interim populations between two executions]**: Standaard blijven alleen de werktabellen van de laatste uitvoering van de workflow behouden. De werklijsten van vorige uitvoeringen worden gezuiverd door een technische werkschema, die op een dagelijkse basis loopt.

  Als deze optie is ingeschakeld, worden werktabellen ook bewaard nadat de workflow is uitgevoerd. U kunt het voor testdoeleinden gebruiken en daarom moet het worden gebruikt **alleen** op ontwikkelings- of staging-omgevingen. Deze mag nooit in een productiewerkstroom worden gecontroleerd.

## Instellingen voor uitvoering  {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Instellingen voor uitvoering"
>abstract="In deze sectie kunt u instellingen configureren die betrekking hebben op de uitvoering van de workflow, zoals het aantal dagen dat de werkstroomgeschiedenis wordt bijgehouden."

* **[!UICONTROL History in days]**: Geeft het aantal dagen aan waarna de historie moet worden gewist. De geschiedenis bevat elementen die verwant zijn aan de workflow: logboeken, taken, gebeurtenissen (technische objecten die zijn gekoppeld aan de workflowbewerking). De standaardwaarde is 30 dagen voor workflowsjablonen buiten de box. De geschiedenis wordt gewist door de technische workflow voor het opschonen van databases, die standaard dagelijks wordt uitgevoerd

  >[!IMPORTANT]
  >
  >Als de **[!UICONTROL History in days]** veld blanco gelaten, wordt de waarde ervan beschouwd als &quot;1&quot;, wat betekent dat de geschiedenis na 1 dag wordt gewist.

* **[!UICONTROL Default affinity]**: Als uw installatie meerdere workflowservers bevat, gebruikt u dit veld om de server op te geven waarop de workflow wordt uitgevoerd. Dit dwingt de uitvoering van die workflow op een bepaalde server. U kunt elke bestaande affiniteitsnaam kiezen, maar gebruik geen spaties of leestekens. Als u verschillende servers gebruikt, geeft u verschillende namen op, gescheiden door komma&#39;s.

  >[!IMPORTANT]
  >
  >Als de waarde die in dit veld wordt gedefinieerd, op geen enkele server bestaat, blijft de workflow in behandeling.


* **[!UICONTROL Save SQL queries in log]**: Schakel deze optie in om de SQL-query&#39;s uit de workflow op te slaan in de logbestanden. Deze functionaliteit is gereserveerd voor geavanceerde gebruikers. Het is van toepassing op werkstromen die gericht activiteiten zoals bevatten **[!UICONTROL Build audience]**. Als deze optie is ingeschakeld, worden de SQL-query&#39;s die tijdens de uitvoering van de workflow naar de database worden verzonden, weergegeven in de logbestanden van de workflow, zodat u ze kunt analyseren om query&#39;s te optimaliseren of problemen op te sporen.

## Instellingen voor foutbeheer  {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Instellingen voor foutbeheer"
>abstract="In deze sectie kunt u definiëren hoe fouten tijdens de uitvoering in de workflow moeten worden beheerd. U kunt ervoor kiezen het proces te pauzeren, een bepaald aantal fouten te negeren of de uitvoering van de workflow te stoppen."

* **[!UICONTROL Error management]**: In dit veld kunt u de handelingen definiëren die moeten worden uitgevoerd als een werkstroomtaak fouten bevat. Er zijn drie mogelijke opties:

   * **[!UICONTROL Suspend the process]**: De workflow wordt automatisch gepauzeerd en de status verandert in **[!UICONTROL Failed]**. Als het probleem is opgelost, hervat u de workflow met de **[!UICONTROL Resume]** knoppen.
   * **[!UICONTROL Ignore]**: De status van de taak die de fout heeft veroorzaakt, verandert in **[!UICONTROL Failed]**, maar de workflow houdt de **[!UICONTROL Started]** status. <!-- TO ADD ONCE SCHEUDLER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abord the process]**: De workflow wordt automatisch beëindigd en de status ervan verandert in **[!UICONTROL Failed]**. Als het probleem is opgelost, start u de workflow opnieuw met de **[!UICONTROL Start]** knoppen.

* **[!UICONTROL Consecutive errors]**: Dit veld is beschikbaar wanneer de **[!UICONTROL Ignore]** waarde is geselecteerd in het dialoogvenster **[!UICONTROL In case of errors]** veld. U kunt opgeven hoeveel fouten kunnen worden genegeerd voordat het proces wordt gestopt. Zodra dit aantal wordt bereikt, verandert de werkschemastatus in **[!UICONTROL Failed]**. Als de waarde van dit veld 0 is, wordt de workflow nooit gestopt, ongeacht het aantal fouten.
