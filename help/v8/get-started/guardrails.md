---
title: Hulplijnen en beperkingen in de gebruikersinterface van het web voor campagnes
description: Hulplijnen en beperkingen in de gebruikersinterface van het web voor campagnes
exl-id: 9c8c67ce-9823-4082-b0bd-5613f3feb6e3
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---

# Afvoerkanalen en beperkingen {#guardrails-limitations}

Wanneer het werken in het gebruikersinterface van het Web van de Campagne met werkschema&#39;s die in de cliëntconsole van de Campagne worden gecreeerd of worden gewijzigd, zijn de hieronder vermelde gidsen en beperkingen van toepassing.

Houd er rekening mee dat op deze pagina belangrijke overwegingen worden vermeld wanneer u werkt met workflows in de console en de webgebruikersinterface, maar dat deze pagina niet alle mogelijke oncompatibiliteit tussen de twee interfaces omvat.

## Workflowactiviteiten {#wkf-activities}

De activiteiten van het werkschema die nog niet in het Web van de Campagne worden gesteund zijn read-only en getoond als onverenigbare activiteiten. U kunt de workflow nog steeds uitvoeren, berichten verzenden, de logbestanden controleren, enz. De activiteiten van het werkschema die zowel in het Web van de Campagne als de cliëntconsole beschikbaar zijn zijn editable.

De activiteiten van het werkschema die nog niet in het gebruikersinterface van het Web van de Campagne worden gesteund zijn read-only en getoond als onverenigbare activiteiten. U kunt de workflow nog steeds uitvoeren, berichten verzenden, de logbestanden controleren, enz. De activiteiten van het werkschema die zowel in het gebruikersinterface van het Web van de Campagne als de de cliëntconsole van de Campagne beschikbaar zijn zijn editable.

| Console | Web |
| --- | --- |
| ![](assets/limitations-activities-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-activities-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

Wanneer een **Query** of een **Verrijking** De activiteit wordt gevormd met extra gegevens in de console, wordt de verrijkingsgegevens in het Web van de Campagne in aanmerking genomen en overgegaan in de uitgaande overgang, maar het kan niet worden uitgegeven.

| Console | Web |
| --- | --- |
| ![](assets/limitations-options-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-options-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

In de console, **Verrijking** deze activiteit kan zowel verzoening als verrijking tot stand brengen . Als u, in de cliëntconsole hebt bepaald, verzoeningsmontages in **Verrijking** activiteit, wordt deze weergegeven als een **Verzoening** activiteit in de gebruikersinterface van het Web van de Campagne.

| Console | Web |
| --- | --- |
| ![](assets/limitations-enrichment-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-enrichment-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

## Workflowcanvas {#wkf-canvas}

Wanneer het creëren van een nieuw werkschema in het gebruikersinterface van het Web van de Campagne, steunt het canvas slechts één ingangspunt. Nochtans, als u een werkstroom in de console met veelvoudige ingangspunten creeerde, kunt u het in het gebruikersinterface van het Web van de Campagne openen en uitgeven.

| Console | Web |
| --- | --- |
| ![](assets/limitations-multiple-console.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-multiple-web.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |

De positionering van de knooppunten wordt elke keer dat een activiteit wordt toegevoegd of verwijderd, vernieuwd. Als u een werkschema in de console creeert, wijzig het gebruikend het gebruikersinterface van het Web van de Campagne en open het in de console opnieuw, kunt u sommige minder belangrijke plaatsende onvolkomenheden opmerken. Dit heeft geen invloed op de processen en taken van de workflow.

| Beginworkflow | Positiewijziging |
| --- | --- |
| ![](assets/limitations-positioning1.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} | ![](assets/limitations-positioning2.png){zoomable=&quot;yes&quot;}{width="800px" align="left" zoomable="yes"} |
