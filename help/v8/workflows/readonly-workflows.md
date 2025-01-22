---
audience: end-user
title: Alleen-lezen workflows
description: Ontdek waarom werkstromen alleen-lezen zijn
exl-id: 5eaffe2c-7a9c-4508-8dd1-495cfcf99c59
source-git-commit: 58f25a6b41c89e97c0f721f4437b5245d16b3757
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# Alleen-lezen workflows {#readonly-workflows}

>[!CONTEXTUALHELP]
>id="acw_wf_read_only_canvas"
>title="Deze workflow is alleen-lezen"
>abstract="U kunt deze workflow niet bewerken vanwege uw rechten of het type workflow."

Sommige workflows zijn alleen-lezen. Ingebouwde technische workflows zijn altijd alleen-lezen, maar deze reconstructie kan ook op andere typen werkstromen worden geactiveerd.

Campagnegebruikers hebben mogelijk beperkte toegang tot de Adobe Campaign-gegevens. Een beheerder van de Campagne kan hen het recht verlenen om sommige eigenschappen te bekijken, maar niet om hen uit te geven of te wijzigen. Gebruikersmachtigingen voor gegevens zijn van wezenlijk belang voor de beveiliging van gegevens en processen. Leer meer over toestemmingenbeheer in Campagne in [ deze sectie ](../get-started/permissions.md)

Wanneer een workflow alleen-lezen is:

* De vermelding **[!UICONTROL Read-only]** bij de knop **[!UICONTROL Settings]**
* De actieknoppen zijn niet toegankelijk

![](assets/readonly-workflow.png){zoomable="yes"}

Gebruikers kunnen niets in een alleen-lezen workflow bewerken. zij mogen de instellingen van de activiteiten niet wijzigen .

![](assets/scheduler-readonly.png){zoomable="yes"}

Gebruikers kunnen de workflow niet verwijderen.

![](assets/readonly-rights.png){zoomable="yes"}


## Typen alleen-lezen workflows {#readonly-workflow-types}

Afhankelijk van het type workflow kan de alleen-lezen modus verschillen.

### Workflows voor campagnes {#readonly-campaign-wf}

In het geval van een alleen-lezen campagneworkflow heeft de gebruiker geen toegang tot de knop Bewaking.

![](assets/readonly-campaign-workflow.png){zoomable="yes"}

### Technische workflows {#readonly-tech-wf}

De ingebouwde technische werkschema&#39;s zijn read-only voor alle campagnegebruikers, zelfs voor de beheerder. Nochtans, kunnen de gebruikers **pauzeren** of **hen ophouden** indien nodig. Dat zijn de enige toegestane acties.

![](assets/readonly-technical-workflow.png){zoomable="yes"}

Leer meer over technische werkschema&#39;s in [ deze sectie ](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/introduction/wf-type/technical-workflows)
