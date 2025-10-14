---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u een workflow maakt met Adobe Campaign Web
exl-id: 26e7360e-cce7-4240-bb29-1dc8613f55ca
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '787'
ht-degree: 2%

---

# De workflow maken {#create-first-workflow}

>[!CONTEXTUALHELP]
>id="acw_campaign_creation_workflow"
>title="Lijst met workflows in de campagne"
>abstract="Het **lusje van de Werkschema&#39;s** maakt een lijst van alle werkschema&#39;s verbonden aan de huidige campagne. Klik op de naam van een workflow om deze te bewerken. Gebruik **creeer werkschemaknoop** om een nieuw werkschema voor deze campagne toe te voegen."

U kunt zelfstandige workflows of workflows in een campagne maken. De eerste stap bestaat uit het selecteren van een sjabloon en het definiëren van de algemene eigenschappen ervan. Vervolgens configureert u zo nodig aanvullende instellingen.

Voer hiertoe de volgende stappen uit:

1. Om a **standalone werkschema** tot stand te brengen, doorblader aan het **&#x200B;**&#x200B;menu van Werkschema&#39;s. Om het werkschema van de a **Campagne** tot stand te brengen, doorblader aan het **menu van Campagnes**, en open de campagne waarvoor u een nieuw werkschema wilt creëren.

1. Klik op de knop **[!UICONTROL Create workflow]** in de rechterbovenhoek van het scherm.

   ![&#x200B; Schermschot die de Create werkschemaknoop in de hoger-juiste hoek van het scherm tonen.](assets/workflow-create.png){zoomable="yes"}

1. In het werkschema{**dialoog 0} Eigenschappen, selecteer het malplaatje om het werkschema tot stand te brengen (u kunt het gebrek ingebouwde malplaatje ook gebruiken).** [&#x200B; Leer meer over werkschemamalplaatjes &#x200B;](#workflow-templates).

1. Voer een label in voor de workflow. Voeg bovendien een beschrijving toe aan uw workflow in het specifieke veld van de sectie **[!UICONTROL Additional options]** van het scherm.

1. Vouw de sectie **[!UICONTROL Additional options]** uit om aanvullende instellingen voor de workflow te configureren. Leer hoe te om de werkschemaeigenschappen in [&#x200B; te vormen deze pagina &#x200B;](workflow-settings.md#properties).

   ![&#x200B; Schermafbeelding die de Extra optiessectie voor het vormen van werkschemamontages toont.](assets/workflow-additional-options.png){zoomable="yes"}

1. Klik op de knop **[!UICONTROL Create workflow]** om het maken van uw workflow te bevestigen.

Uw workflow wordt nu gemaakt en beschikbaar in de lijst met workflows. U kunt tot zijn visueel canvas toegang hebben en beginnen toevoegend, vormend, en de taken te ordenen het zal uitvoeren. [&#x200B; Leer hoe te om werkschemaactiviteiten &#x200B;](orchestrate-activities.md) te ordenen.

## Werken met workflowsjablonen {#workflow-templates}

>[!CONTEXTUALHELP]
>id="acw_workflow_template_for_campaign"
>title="Workflowsjablonen"
>abstract="Workflowsjablonen bevatten vooraf geconfigureerde instellingen en activiteiten die opnieuw kunnen worden gebruikt voor het maken van nieuwe workflows."

>[!CONTEXTUALHELP]
>id="acw_workflow_template_creation_properties"
>title="Workfloweigenschappen"
>abstract="Workflowsjablonen bevatten vooraf geconfigureerde instellingen en activiteiten die opnieuw kunnen worden gebruikt voor het maken van nieuwe workflows. In dit scherm, ga het etiket van het werkschemamalplaatje in en vorm zijn montages zoals zijn interne naam, omslag en uitvoeringsomslagen, timezone, en supervisorgroep."

Workflowsjablonen bevatten vooraf geconfigureerde instellingen en activiteiten die opnieuw kunnen worden gebruikt voor het maken van nieuwe workflows. U selecteert de sjabloon van uw workflow in de workfloweigenschappen wanneer u een workflow maakt. Er wordt standaard een lege sjabloon weergegeven.

U kunt een sjabloon maken op basis van een bestaande workflow of een geheel nieuwe sjabloon maken. Beide methoden worden hieronder beschreven.

>[!BEGINTABS]

>[!TAB  creeer een malplaatje van een bestaand werkschema ]

Voer de volgende stappen uit om een werkstroomsjabloon te maken op basis van een bestaande workflow:

1. Open het **menu van Werkschema&#39;s** en doorblader aan het werkschema om als malplaatje te bewaren.
1. Klik de drie punten op het recht van de naam van het werkschema, en kies **Exemplaar als malplaatje**.

   ![&#x200B; Screenshot die het Exemplaar als malplaatjeoptie in het werkschemamenu toont.](assets/wf-copy-as-template.png){zoomable="yes"}

1. Bevestig het maken van de sjabloon in het pop-upvenster.
1. In het canvas van het werkschemamalplaatje, controleer, voeg, en vorm de activiteiten toe zoals nodig.
1. Blader naar de montages, van de **knoop van Montages**, om de naam van het werkschemamalplaatje te veranderen, en een beschrijving in te gaan.
1. Selecteer de **omslag** en **uitvoeringsomslag** van het malplaatje. De map is de locatie waar het werkstroomsjabloon wordt opgeslagen. De uitvoeringsmap is de map waarin workflows worden opgeslagen die op basis van deze sjabloon zijn gemaakt.

   ![&#x200B; Schermafbeelding die de montages voor omslag en uitvoeringsomslag in het werkschemamalplaatje toont.](assets/wf-settings-template.png){zoomable="yes"}

   De andere eigenschappen komen veel voor in workflows. Meer informatie vindt u [op deze pagina](workflow-settings.md#properties).

1. Sla uw wijzigingen op.

Het werkstroomsjabloon is nu beschikbaar in de sjabloonlijst. U kunt een workflow maken op basis van deze sjabloon. Deze workflow wordt vooraf geconfigureerd met de instellingen en activiteiten die in de sjabloon zijn gedefinieerd.

>[!TAB  creeer een malplaatje van kras ]

Ga als volgt te werk om een werkstroomsjabloon helemaal zelf te maken:

1. Open het **menu van Werkschema&#39;s** en doorblader aan de **Malplaatjes** tabel. U kunt de lijst met beschikbare werkstroomsjablonen bekijken.
1. Klik op de knop **[!UICONTROL Create template]** in de rechterbovenhoek van het scherm.
1. Voer het label in en open de aanvullende opties om een beschrijving van de werkstroomsjabloon in te voeren.
1. Selecteer de map en de uitvoeringsmap van de sjabloon. De map is de locatie waar het werkstroomsjabloon wordt opgeslagen. De uitvoeringsmap is de map waarin workflows worden opgeslagen die op basis van deze sjabloon zijn gemaakt.

   ![&#x200B; Scherenshot die de verwezenlijking van een nieuw werkschemamalplaatje met omslag en uitvoeringsomslagmontages toont.](assets/new-wf-template.png){zoomable="yes"}

   De andere eigenschappen komen veel voor in workflows. Meer informatie vindt u [op deze pagina](workflow-settings.md#properties).

1. Klik **creeer** knoop om uw montages te bevestigen.
1. In het canvas van het werkschemamalplaatje, voeg en vorm de activiteiten toe zoals nodig.

   ![&#x200B; Schermschot die het canvas van het werkschemamalplaatje voor het toevoegen van en het vormen van activiteiten tonen.](assets/wf-template-activities.png){zoomable="yes"}

1. Sla uw wijzigingen op.

Het werkstroomsjabloon is nu beschikbaar in de sjabloonlijst. U kunt een workflow maken op basis van deze sjabloon. Deze workflow wordt vooraf geconfigureerd met de instellingen en activiteiten die in de sjabloon zijn gedefinieerd.

>[!ENDTABS]