---
audience: end-user
title: De workflowactiviteit Change-dimensie gebruiken
description: Leer hoe u de workflowactiviteit Wijzigen kunt gebruiken
badge: label="Beta"
source-git-commit: 9b945dcd4151e536e8a8be904100730c86e483b7
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 1%

---


# Dimensie wijzigen {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Een complement genereren"
>abstract="U kunt een extra uitgaande overgang met de resterende bevolking produceren, die als duplicaat werd uitgesloten. Om dit te doen, knevel op **Complement genereren** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Dimensieactiviteit wijzigen"
>abstract="Met deze activiteit kunt u de doeldimensie wijzigen terwijl u een publiek maakt. Het verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. U kunt bijvoorbeeld van de dimensie &quot;contracten&quot; naar de dimensie &quot;clients&quot; schakelen."

De **Dimensie wijzigen** activiteit is **Targeting** activiteit. Met deze activiteit kunt u de doeldimensie wijzigen terwijl u een publiek maakt. Deze activiteit verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. U kunt bijvoorbeeld van de dimensie &quot;contracten&quot; naar de dimensie &quot;clients&quot; schakelen.

## Configuratie

Voer de volgende stappen uit om de **Dimensie wijzigen** activiteit:

1. Voeg een **Dimensie wijzigen** activiteit aan uw werkschema.

   ![](../assets/workflow-change-dimension.png)

1. Definieer de **Nieuwe doeldimensie**. Tijdens het wijzigen van de afmetingen worden alle records bewaard. Andere opties zijn nog niet beschikbaar.

1. Voer de workflow uit om het resultaat weer te geven. Vergelijk de gegevens in de tabellen voor en na de activiteit voor de veranderingsdimensie en vergelijk de structuur van de workflowtabellen.



