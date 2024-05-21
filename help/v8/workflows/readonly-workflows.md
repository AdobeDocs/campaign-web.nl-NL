---
audience: end-user
title: Alleen-lezen workflows
description: Ontdek waarom werkstromen alleen-lezen zijn
source-git-commit: 6985e8cb11f12ab7818cc71441a4d3b41f1a0493
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---

# Alleen-lezen workflows {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Deze workflow is alleen-lezen"
>abstract="U kunt deze workflow niet bewerken vanwege uw rechten of het type workflow."

Sommige workflows zijn mogelijk in de modus Alleen-lezen. Je kunt het zien met:

- De vermelding **[!UICONTROL ** Alleen-lezen **]**  nabij de **[!UICONTROL Settings]** knop
- De actieknoppen zijn niet toegankelijk

![](assets/readonly-workflow.png){zoomable="yes"}

U kunt niets in een read-only werkschema uitgeven. U mag de instellingen van de activiteiten niet wijzigen.


![](assets/scheduler-readonly.png){zoomable="yes"}


U hebt niet de rechten om de workflow ook te verwijderen.

![](assets/readonly-rights.png){zoomable="yes"}

## Waarom alleen-lezen workflows

De modus Alleen-lezen is bedoeld voor gebruikers die geen machtigingen en toegangsrechten hebben om deze workflows te bewerken. [Meer informatie hier](../get-started/permissions.md)

Een campagnegebruiker kan beperkingen hebben in de gegevens waartoe hij toegang heeft in Adobe Campaign. De beheerder kan hem de mogelijkheid geven om sommige eigenschappen te bekijken maar niet om aan hen te werken.

## Typen alleen-lezen workflows

Afhankelijk van het type workflow kan de alleen-lezen modus verschillen.

### Workflows voor campagnes

In het geval van een alleen-lezen campagneworkflow heeft de gebruiker geen toegang tot de knop Bewaking.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technische workflows

De technische werkschema&#39;s zijn op read-only wijze voor campagnegebruikers.
De ingebouwde technische werkschema&#39;s zijn op read-only wijze voor allen, zelfs voor de beheerdergebruikers. Maar de gebruiker kan **pauzeren** of **stoppen** indien nodig. Dat zijn de enige toegestane acties. [Meer informatie hier](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)

![](assets/readonly-technical-workflow.png){zoomable="yes"}