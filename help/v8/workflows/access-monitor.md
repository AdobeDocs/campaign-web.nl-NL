---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 0%

---

# Workflows openen en beheren {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Workflows"
>abstract="In dit scherm, kunt u tot de volledige lijst van standalone en campagnewerkschema&#39;s toegang hebben, hun huidige status, laatste/volgende uitvoeringsdata controleren, en een nieuw werkschema creëren. Blader naar het tabblad &#39;Sjablonen&#39; voor toegang tot beschikbare werkstroomsjablonen."

De **[!UICONTROL Workflows]** kunt u de volledige lijst met workflows openen. Deze lijst bevat beide **zelfstandige workflows** die op basis van dit scherm zijn gemaakt, en **campagneworkflows**, die in een campagne zijn gemaakt.

![](assets/workflow-list.png){zoomable=&quot;yes&quot;}

Elke werkstroom in de lijst bevat informatie over de huidige [status](#status), de laatste keer dat deze werd uitgevoerd of gewijzigd, en de volgende geplande uitvoeringsdatum en -tijd.

U kunt de weergegeven kolommen aanpassen door op de knop **[!UICONTROL Configure column for a custom layout]** in de rechterbovenhoek van de lijst. Op deze manier kunt u aanvullende informatie aan de lijst toevoegen, zoals de laatste foutactiviteit voor elke werkstroom of de toegepaste doeldimensie.

Bovendien zijn er een zoekbalk en filters beschikbaar waarmee u gemakkelijk in de lijst kunt zoeken. U kunt de workflows bijvoorbeeld filteren om alleen de workflows weer te geven die bij een campagne horen of de workflows die tijdens een specifiek datumbereik worden verwerkt.

Als u een workflow wilt dupliceren of verwijderen, klikt u op de knop voor ovaal en selecteert u **[!UICONTROL Duplicate]** of **[!UICONTROL Delete]**.

>[!NOTE]
>
>U kunt een actieve workflow dupliceren, maar u kunt deze niet verwijderen.

## Status van workflows {#status}

Workflows kunnen meerdere statussen hebben:

* **[!UICONTROL Draft]**: De workflow is gemaakt en opgeslagen.
* **[!UICONTROL In progress]**: De workflow wordt momenteel uitgevoerd.
* **[!UICONTROL Finished]**: De uitvoering van de workflow is voltooid.
* **[!UICONTROL Paused]**: De werkstroom is gepauzeerd.
* **[!UICONTROL Erroneous]**: Er is een fout opgetreden in de workflow. Open de workflow en open de logboeken en taken om de fout te identificeren en op te lossen. [Leer hoe u logbestanden en taken kunt controleren](start-monitor-workflows.md#logs-tasks)

Gedetailleerde informatie over het starten en controleren van de uitvoering van de workflow is beschikbaar in [deze pagina](start-monitor-workflows.md).

## Workflowsjablonen {#templates}

De **[!UICONTROL Templates]** worden alle beschikbare werkstroomsjablonen weergegeven.

De malplaatjes van het werkschema bevatten pre-gevormde activiteiten en algemene bezitsconfiguraties die voor het creëren van nieuwe werkschema&#39;s kunnen worden opnieuw gebruikt.

U kunt werkstroomsjablonen maken op basis van een bestaande workflow of helemaal zelf. [Leer hoe u werkstroomsjablonen maakt](create-workflow.md#workflow-templates)
