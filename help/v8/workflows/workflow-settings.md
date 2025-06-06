---
audience: end-user
title: Workflowinstellingen configureren
description: Leer hoe u workflowinstellingen configureert met Adobe Campaign Web
exl-id: 3aef912b-086b-4aa4-9556-c09396112313
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 1%

---

# Workflowinstellingen configureren {#workflow-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workfloweigenschappen"
>abstract="Kies in dit scherm de sjabloon die u wilt gebruiken om de workflow te maken en geef een label op. Vouw de **Extra opties** sectie uit om meer montages, zoals de werkschemainterne naam, zijn omslag, timezone, en supervisorgroep te vormen. Het wordt hoogst geadviseerd om een supervisorgroep te selecteren zodat de exploitanten worden gealarmeerd als een fout voorkomt."

Als u een workflow maakt of workflowactiviteiten op het canvas ordent, hebt u toegang tot geavanceerde instellingen voor de workflow. Stel bijvoorbeeld een specifieke tijdzone in voor de workflow, beheer hoe de workflow zich moet gedragen in het geval van een fout, of beheer de vertraging waarna de werkstroomgeschiedenis wordt gewist.

Deze instellingen zijn vooraf geconfigureerd in de sjabloon die is geselecteerd tijdens het maken van de workflow, maar kunnen zo nodig worden bewerkt voor deze specifieke workflow.

![ de montages van het Werkschema knoopinterface ](assets/workflow-settings-button.png){zoomable="yes"}{width="70%" align="left"}

## Workfloweigenschappen {#properties}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_properties"
>title="Workfloweigenschappen"
>abstract="Deze sectie biedt algemene workfloweigenschappen die ook toegankelijk zijn wanneer u de workflow maakt. U kunt de sjabloon kiezen die u wilt gebruiken om de workflow te maken en een label opgeven. Vouw de sectie Aanvullende opties uit om specifieke instellingen te configureren, zoals de workflow waarin de map of tijdzone wordt opgeslagen."

De sectie **[!UICONTROL Properties]** biedt algemene instellingen die kunnen worden geconfigureerd wanneer u een workflow maakt. Als u de eigenschappen van een bestaande workflow wilt openen, klikt u op de knop **[!UICONTROL Settings]** in de actiebalk boven het werkstroomcanvas.

![ interface van de montages van het Werkschema ](assets/workflow-settings.png){zoomable="yes"}{width="70%" align="left"}

Deze eigenschappen zijn:

* De **[!UICONTROL Label]** van de workflow die in de lijst wordt weergegeven.
* De **[!UICONTROL Internal name]** van de workflow.
* De **[!UICONTROL Folder]** waar de workflow moet worden opgeslagen.
* De standaardinstelling **[!UICONTROL Timezone]** die moet worden gebruikt in alle activiteiten van de workflow. Standaard is de tijdzone van de workflow de tijdzone die is gedefinieerd voor de huidige Campagneoperator.
Mogelijke waarden zijn:
   * **timezone van de Server** om timezone van de de toepassingsserver van Adobe Campaign te gebruiken.
   * **timezone van de Exploitant** om timezone van de exploitant van Adobe Campaign te gebruiken die het werkschema uitvoert, zoals die in het profiel van de exploitant in de cliëntconsole wordt bepaald.
   * **Tijdzone van het gegevensbestand** om timezone van de gegevensbestandserver te gebruiken.
   * Een specifieke tijdzone.
* Wanneer een workflow mislukt, worden de operatoren die tot de groep met operatoren behoren die in het veld **[!UICONTROL Supervisor(s)]** is geselecteerd, via e-mail op de hoogte gebracht.
* Voer een **[!UICONTROL Description]** van uw workflow in.

Wanneer het werkschema [ met een campagne ](create-workflow.md) wordt geassocieerd, wordt het getoond op het **[!UICONTROL Linked campaign]** gebied. Open de bijbehorende campagne vanuit dat veld.

## Segmenteringsinstellingen {#segmentation-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_segmentation"
>title="Segmenteringsinstellingen"
>abstract="In deze sectie kunt u de doeldimensie selecteren voor doelprofielen in de workflow en ervoor kiezen de workflowresultaten tussen twee uitvoeringen te houden. Deze optie mag alleen voor testdoeleinden worden gebruikt en mag nooit in een productiewerkstroom worden ingeschakeld."

* **[!UICONTROL Targeting dimension]**: selecteer de doeldimensie die u wilt gebruiken voor doelprofielen, zoals ontvangers, begunstigden van contracten, operators, abonnees en andere. [ Leer meer over het richten van dimensies ](../audience/targeting-dimensions.md).

* **[!UICONTROL Keep the result of interim populations between two executions]**: Standaard blijven alleen de werktabellen van de laatste uitvoering van de workflow behouden. De werklijsten van vorige uitvoeringen worden gezuiverd door een technische werkschema, die dagelijks loopt.

  Als deze optie is ingeschakeld, worden werktabellen ook bewaard nadat de workflow is uitgevoerd. Gebruik het voor testende doeleinden, en zorg ervoor het **slechts** op ontwikkeling of het opvoeren milieu&#39;s wordt gebruikt. Deze mag nooit in een productiewerkstroom worden gecontroleerd.

## Instellingen voor uitvoering {#exec-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution"
>title="Instellingen voor uitvoering"
>abstract="In deze sectie kunt u instellingen configureren die betrekking hebben op de uitvoering van de workflow, zoals het aantal dagen dat de werkstroomgeschiedenis wordt bijgehouden."

* **[!UICONTROL History in days]** - Geeft het aantal dagen aan waarna de historie moet worden gewist. De geschiedenis bevat elementen die verwant zijn aan de werkstroom, zoals logboeken, taken, en gebeurtenissen (technische voorwerpen verbonden aan de werkschemaverrichting). De standaardwaarde is 30 dagen voor out-of-the-box werkstroomsjablonen. De geschiedenis wordt gewist door het technische werkschema van de Opschoonmaakbeurt van het Gegevensbestand, dat dagelijks wordt uitgevoerd.

  >[!IMPORTANT]
  >
  >Als het veld **[!UICONTROL History in days]** leeg blijft, wordt de waarde ervan beschouwd als &quot;1&quot;. Dit betekent dat de historie na 1 dag wordt gewist.

* **[!UICONTROL Default affinity]**: Als uw installatie meerdere workflowservers bevat, gebruikt u dit veld om de server op te geven waarop de workflow wordt uitgevoerd. Dit dwingt de uitvoering van die workflow op een bepaalde server. Kies een bestaande affiniteitsnaam, maar gebruik geen spaties of leestekens. Als u verschillende servers gebruikt, geeft u verschillende namen op, gescheiden door komma&#39;s.

  >[!IMPORTANT]
  >
  >Als de waarde die in dit veld wordt gedefinieerd, op geen enkele server bestaat, blijft de workflow in behandeling.

* **[!UICONTROL Save SQL queries in log]**: Schakel deze optie in om de SQL-query&#39;s uit de workflow op te slaan in de logbestanden. Deze functionaliteit is gereserveerd voor geavanceerde gebruikers. De klasse is van toepassing op workflows die doelactiviteiten bevatten, zoals **[!UICONTROL Build audience]** . Als deze optie is ingeschakeld, worden de SQL-query&#39;s die tijdens de uitvoering van de workflow naar de database worden verzonden, weergegeven in de logbestanden van de workflow, zodat u ze kunt analyseren om query&#39;s te optimaliseren of problemen op te sporen.

## Instellingen voor foutbeheer {#error-settings}

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_error"
>title="Instellingen voor foutbeheer"
>abstract="In deze sectie kunt u definiëren hoe fouten tijdens de uitvoering in de workflow moeten worden beheerd. U kunt ervoor kiezen het proces te pauzeren, een bepaald aantal fouten te negeren of de uitvoering van de workflow te stoppen."

* **[!UICONTROL Error management]**: In dit veld kunt u de acties definiëren die moeten worden uitgevoerd als een werkstroomtaak fouten bevat. Er zijn drie mogelijke opties:

   * **[!UICONTROL Suspend the process]**: De werkstroom wordt automatisch gepauzeerd en de status verandert in **[!UICONTROL Failed]** . Zodra het probleem is opgelost, hervat u de workflow met de knoppen **[!UICONTROL Resume]** .
   * **[!UICONTROL Ignore]**: De status van de taak die de fout heeft veroorzaakt, verandert in **[!UICONTROL Failed]** , maar de workflow behoudt de status **[!UICONTROL Started]** . <!-- TO ADD ONCE SCHEDULER IS AVAILABLE This configuration is relevant for recurring tasks: if the branch includes a scheduler, it will start normally next time the workflow is executed.-->
   * **[!UICONTROL Abort the process]**: De werkstroom wordt automatisch gestopt en de status verandert in **[!UICONTROL Failed]** . Zodra het probleem is opgelost, start u de workflow opnieuw met de knoppen **[!UICONTROL Start]** .

* **[!UICONTROL Consecutive errors]**: Dit veld wordt beschikbaar wanneer de **[!UICONTROL Ignore]** -waarde wordt geselecteerd in het **[!UICONTROL In case of errors]** -veld. Geef het aantal fouten op dat kan worden genegeerd voordat het proces wordt gestopt. Zodra dit aantal wordt bereikt, verandert de werkschemastatus in **[!UICONTROL Failed]**. Als de waarde van dit veld 0 is, wordt de workflow nooit gestopt, ongeacht het aantal fouten.

## Initialisatiescript {#initialization-script}

Het **manuscript van de Initialisatie** laat u variabelen initialiseren of activiteiteneigenschappen wijzigen. Klik **geef code** knoop uit en typ het fragment van uit te voeren code. Het script wordt aangeroepen wanneer de workflow wordt uitgevoerd. Verwijs naar de sectie met betrekking tot [ gebeurtenisvariabelen ](../workflows/event-variables.md).