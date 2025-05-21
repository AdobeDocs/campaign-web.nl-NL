---
audience: end-user
title: Alleen-lezen workflows
description: Ontdek waarom werkstromen alleen-lezen zijn
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 93a79b471c236e5bf67da0dbd0d76274598dcb0e
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Alleen-lezen workflows {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Deze workflow is alleen-lezen"
>abstract="U kunt deze workflow niet bewerken vanwege uw rechten of het type workflow."

Sommige workflows zijn alleen-lezen. Ingebouwde technische workflows zijn altijd alleen-lezen, maar deze beperking kan ook van toepassing zijn op andere typen workflows.

Campagnegebruikers hebben mogelijk beperkte toegang tot Adobe Campaign-gegevens. Een beheerder van de Campagne kan hen het recht verlenen om bepaalde eigenschappen te bekijken, maar niet om hen uit te geven of te wijzigen. Gebruikersmachtigingen voor gegevens zijn essentieel om de beveiliging van gegevens en processen te garanderen. Leer meer over toestemmingenbeheer in Campagne in [ deze sectie ](../get-started/permissions.md).

Wanneer een workflow alleen-lezen is:

* De vermelding **[!UICONTROL Read-only]** wordt weergegeven bij de knop **[!UICONTROL Settings]** .
* De actieknoppen zijn niet toegankelijk.

![ read-only werkschemainterface die de montagesknoop en gehandicapte actieknopen toont.](assets/readonly-workflow.png){zoomable="yes"}

Gebruikers kunnen niets in een alleen-lezen workflow bewerken. Ze mogen de instellingen van de activiteiten niet wijzigen.

![ de interface van de Planner op read-only wijze, tonend gehandicapte montagesopties.](assets/scheduler-readonly.png){zoomable="yes"}

Gebruikers kunnen de workflow niet verwijderen.

![ Interface die beperkte rechten voor het schrappen van werkschema&#39;s toont.](assets/readonly-rights.png){zoomable="yes"}

## Typen alleen-lezen workflows {#readonly-workflow-types}

Afhankelijk van het type workflow kan de alleen-lezen modus variëren.

### Workflows voor campagnes {#readonly-campaign-wf}

In een alleen-lezen campagneworkflow heeft de gebruiker geen toegang tot de knop Bewaking.

![ het werkschemainterface van de campagne op read-only wijze, die gehandicapte controleopties tonen.](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technische workflows {#readonly-tech-wf}

Ingebouwde technische workflows zijn alleen-lezen voor alle campagnegebruikers, inclusief beheerders. Nochtans, kunnen de gebruikers **pauzeren** of **hen ophouden** indien nodig. Dit zijn de enige toegestane acties.

![ Technische werkschemainterface op read-only wijze, die opties tonen om werkschema&#39;s te pauzeren of tegen te houden.](assets/readonly-technical-workflow.png){zoomable="yes"}

Leer meer over technische werkschema&#39;s in [ deze sectie ](https://experienceleague.adobe.com/nl/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows).