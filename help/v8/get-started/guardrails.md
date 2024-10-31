---
title: Grafieken en beperkingen in de gebruikersinterfaceworkflows van Campaign Web
description: Grafieken en beperkingen bij het werken met workflows in de gebruikersinterface van Campaign Web
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: c156e4105cab5028249a2a3d5a1838205cac7d35
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# Grafieken en beperkingen voor workflows {#guardrails-limitations}

Wanneer u in de gebruikersinterface van het Web van Campaign werkt met workflows die in de clientconsole van Campaign worden gemaakt of aangepast, zijn de onderstaande beperkingen en beveiligingsinstructies van toepassing.

Houd er rekening mee dat op deze pagina belangrijke overwegingen worden vermeld wanneer u werkt met workflows in de console en de webgebruikersinterface, maar dat deze pagina niet alle mogelijke oncompatibiliteit tussen de twee interfaces omvat.

## Workflowactiviteiten {#wkf-activities}

>[!CONTEXTUALHELP]
>id="acw_orchestration_query_enrichment_noneditable"
>title="Activiteit niet bewerkbaar"
>abstract="Wanneer de a **Vraag** of een **Verrijkingsactiviteit** met extra gegevens in de console wordt gevormd, wordt de verrijkingsgegevens in het Web van de Campagne in de uitgaande overgang in aanmerking genomen en overgegaan, maar het kan niet worden uitgegeven."

Workflowactiviteiten die nog niet worden ondersteund in de gebruikersinterface van Campaign Web zijn alleen-lezen en worden weergegeven als incompatibele activiteiten. U kunt de workflow nog steeds uitvoeren, berichten verzenden, de logbestanden controleren, enzovoort. Workflowactiviteiten die beschikbaar zijn in de gebruikersinterface van Campaign Web en de Campaign-clientconsole zijn bewerkbaar.

| Console | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

Wanneer de a **Vraag** of een **Verrijkingsactiviteit** met extra gegevens in de console wordt gevormd, wordt de verrijkingsgegevens in het Web van de Campagne in de uitgaande overgang in aanmerking genomen en overgegaan, maar het kan niet worden uitgegeven.

| Console | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

In de console, kan de **Verrijking** activiteit zowel verzoening als verrijking uitvoeren. Als u, in de cliëntconsole, verzoeningsmontages in de **Verrijking** activiteit hebt bepaald, zal het als a **Verzoening** activiteit in het gebruikersinterface van het Web van de Campagne worden getoond.

| Console | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

## Workflowcanvas {#wkf-canvas}

Wanneer u een nieuwe workflow maakt in de gebruikersinterface van het Campaign Web, ondersteunt het canvas slechts één ingangspunt. Nochtans, als u een werkstroom in de console met veelvoudige ingangspunten creeerde, kunt u het in het gebruikersinterface van het Web van de Campagne openen en uitgeven.

| Console | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |

De positionering van de knooppunten wordt elke keer dat een activiteit wordt toegevoegd of verwijderd, vernieuwd. Als u een workflow in de console maakt, wijzigt u deze met de gebruikersinterface van Campaign Web en opent u deze opnieuw in de console, kan het zijn dat u onvolkomenheden met betrekking tot de positie opmerkt. Dit heeft geen invloed op de processen en taken van de workflow.

| Beginworkflow | Positiewijziging |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable="yes"}{width="800px" align="left" zoomable="yes"} |
