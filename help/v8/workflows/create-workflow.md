---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: c842829915784654b7130563d36dea188e84ff3d
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---


# Een workflow maken {#create}

>[!CONTEXTUALHELP]
>id="acw_workflow_creation_properties"
>title="Workfloweigenschappen"
>abstract="TBD"

## De workflow maken {#create-workflow}

De eerste stap om uw werkschema in Campagne v8 Web tot stand te brengen is het of als standalone werkschema of direct binnen een campagne te creëren en zijn algemene eigenschappen te bepalen. Voer hiertoe de volgende stappen uit:

1. Begin door te beslissen of u een standalone werkschema wilt tot stand brengen of het direct binnen een campagne integreren:

   * **Zelfstandige workflow**: Navigeer naar het menu Worklows en klik op de knop Create workflow in de rechterbovenhoek.
   * **Workflow voor campagnes:** Navigeer naar het menu Campagnes en open de campagne waar u een nieuwe workflow wilt maken. Klik op de knop Workflow maken in de rechterbovenhoek van het tabblad Workflows.

   Het dialoogvenster Eigenschappen van workflow wordt geopend.

   ![](assets/workflow-create.png)

1. Selecteer de sjabloon die u wilt gebruiken om de workflow te maken en geef een label voor de workflow op.

   De malplaatjes van het werkschema bevatten pre-gevormde activiteiten en algemene bezitsconfiguraties die voor het creëren van nieuwe werkschema&#39;s kunnen worden opnieuw gebruikt. Zij worden gecreeerd van de cliëntconsole. [Leer hoe u met sjablonen werkt](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/build-a-workflow.html#workflow-templates)

1. Vouw de sectie Aanvullende opties uit als u specifieke instellingen voor de workflow wilt configureren, zoals de opslagmap en de tijdzone. [Leer hoe u werkstroomeigenschappen configureert](workflow-settings.md)

1. Klik op de knop Workflow maken om te bevestigen dat u een workflow maakt.

Als uw workflow is gemaakt, kunt u nu beginnen met het orchestreren van de verschillende taken die worden uitgevoerd met een speciaal visueel canvas. [Leer hoe u workflowactiviteiten kunt ordenen](#build)

## Workflowactiviteiten ordenen {#build}

Zodra u [een workflow hebben gemaakt](create-workflow.md)Of u nu het workflowmenu of een campagne gebruikt, u kunt de verschillende taken die het uitvoert gaan ordenen. Hiervoor wordt een visueel canvas verschaft, zodat u een workflowdiagram kunt maken. Binnen dit diagram, kunt u diverse activiteiten toevoegen en hen in een opeenvolgende orde verbinden.

In dit stadium van de configuratie, wordt het diagram getoond met een beginpictogram, dat het begin van uw werkschema vertegenwoordigt. Als u de eerste activiteit wilt toevoegen, klikt u op de knop + die is verbonden met het startpictogram.

Er wordt een lijst met activiteiten weergegeven die aan het diagram kunnen worden toegevoegd. De beschikbare activiteiten zijn afhankelijk van uw positie binnen het werkstroomdiagram. Wanneer u bijvoorbeeld uw eerste activiteit toevoegt, kunt u de workflow starten door zich te richten op een publiek, het workflowpad te splitsen of een wachtactiviteit in te stellen om de uitvoering van de workflow uit te stellen. Anderzijds, na een het publieksactiviteit van de Bouwstijl, kunt u uw doel met het richten van activiteiten verfijnen, een levering naar uw publiek met kanaalactiviteiten verzenden, of het werkschemaproces met debietcontroleactiviteiten organiseren.

![](assets/workflow-start.png)

Zodra een activiteit aan het diagram is toegevoegd, verschijnt een juiste ruit, toestaand u om de onlangs toegevoegde activiteit met specifieke montages te vormen. Gedetailleerde informatie over hoe te om elke activiteit te vormen is beschikbaar in [deze sectie](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

Herhaal dit proces om zoveel activiteiten toe te voegen als u wilt afhankelijk van de taken die u de workflow wilt uitvoeren. U kunt ook een nieuwe activiteit invoegen tussen twee activiteiten. Om dit te doen, klik + knoop op de overgang tussen de activiteiten, selecteer de gewenste activiteit en vorm het in de juiste ruit.

Als u een activiteit wilt verwijderen, selecteert u deze op het canvas en klikt u op het pictogram Verwijderen in de activiteitseigenschappen.

>[!TIP]
>
>U kunt de naam van de overgangen tussen elke activiteit aanpassen. U doet dit door de overgang te selecteren en het label ervan te wijzigen in het rechterdeelvenster.

Nadat u de workflow hebt voltooid, voegt u de activiteit &#39;en End&#39; aan het einde van het diagram toe. Met deze activiteit kunt u visueel het einde van een werkstroom markeren en heeft dit geen invloed op de functionaliteit.

Nadat u het werkstroomdiagram hebt ontworpen, kunt u de werkstroom uitvoeren en de voortgang van de verschillende taken volgen. [Leer hoe u een workflow kunt starten en de uitvoering ervan kunt controleren](start-monitor-workflows.md)
