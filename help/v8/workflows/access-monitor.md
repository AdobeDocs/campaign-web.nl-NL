---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
exl-id: 2a9b7e52-2b8b-4293-9b4d-a228ba95bed3
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Workflows openen en beheren {#access-monitor}

>[!CONTEXTUALHELP]
>id="acw_targeting_workflow_list"
>title="Workflows"
>abstract="In dit scherm, kunt u tot de volledige lijst van standalone en campagnewerkschema&#39;s toegang hebben, hun huidige status, laatste/volgende uitvoeringsdata controleren, en een nieuw werkschema creëren. Blader naar het tabblad &#39;Sjablonen&#39; voor toegang tot beschikbare werkstroomsjablonen."

Het menu **[!UICONTROL Workflows]** biedt toegang tot de volledige lijst met workflows. Deze lijst omvat zowel **standalone werkschema&#39;s**, die van dit scherm worden gecreeerd, en **campagnewerkschema&#39;s**, binnen een campagne worden gecreeerd.

{het lijstscherm van het 0} Werkschema dat standalone en campagnewerkschema&#39;s toont ![](assets/workflow-list.png){zoomable="yes"}

Elk werkschema in de lijst toont informatie over zijn huidige [ status ](#status), de laatste tijd het werd uitgevoerd of, en de volgende geplande uitvoeringsdatum en tijd gewijzigd.

Pas de weergegeven kolommen aan door op het pictogram **[!UICONTROL Configure column for a custom layout]** in de rechterbovenhoek van de lijst te klikken. Hierdoor kunt u aanvullende informatie aan de lijst toevoegen, zoals de laatste foutactiviteit voor elke werkstroom of de toegepaste doeldimensie.

Bovendien zijn er een zoekbalk en filters beschikbaar om het zoeken in de lijst te vereenvoudigen. U kunt workflows bijvoorbeeld filteren om alleen workflows weer te geven die tot een campagne behoren of die welke gedurende een bepaald datumbereik zijn verwerkt.

Als u een workflow wilt dupliceren of verwijderen, klikt u op de knop Ovaal en selecteert u **[!UICONTROL Duplicate]** of **[!UICONTROL Delete]** .

>[!NOTE]
>
>U kunt een actieve workflow dupliceren, maar u kunt deze niet verwijderen.

## Status van workflows {#status}

Workflows kunnen meerdere statussen hebben:

* **[!UICONTROL Draft]**: De workflow is gemaakt en opgeslagen.
* **[!UICONTROL In progress]**: De workflow wordt momenteel uitgevoerd.
* **[!UICONTROL Finished]**: De uitvoering van de workflow is voltooid.
* **[!UICONTROL Paused]**: de workflow is gepauzeerd.
* **[!UICONTROL Erroneous]**: Er is een fout opgetreden in de workflow. Open de workflow en open de logboeken en taken om de fout te identificeren en op te lossen. [ leer hoe te om logboeken en taken te controleren ](start-monitor-workflows.md#logs-tasks)

De gedetailleerde informatie over hoe te om werkschemauitvoering te beginnen en te controleren is beschikbaar op [ deze pagina ](start-monitor-workflows.md).

## Workflowsjablonen {#templates}

Op het tabblad **[!UICONTROL Templates]** worden alle beschikbare werkstroomsjablonen weergegeven.

De malplaatjes van het werkschema bevatten pre-gevormde activiteiten en algemene bezitsconfiguraties die voor het creëren van nieuwe werkschema&#39;s kunnen worden opnieuw gebruikt.

Workflowsjablonen maken op basis van een bestaande workflow of helemaal opnieuw. [ Leer hoe te om werkschemamalplaatjes ](create-workflow.md#workflow-templates) tot stand te brengen