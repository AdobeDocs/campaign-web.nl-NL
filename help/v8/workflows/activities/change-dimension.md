---
audience: end-user
title: De workflowactiviteit Change-dimensie gebruiken
description: Leer hoe u de workflowactiviteit Wijzigen kunt gebruiken
badge: label="Beta"
source-git-commit: 524d690ad5dbaa1d63c53cece05207eb0d745540
workflow-type: tm+mt
source-wordcount: '288'
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

De **Dimensie wijzigen** activiteit is **Targeting** activiteit. Met deze activiteit kunt u de doeldimensie wijzigen terwijl u uw workflow bouwt.
Deze activiteit verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie.

U kunt bijvoorbeeld de doeldimensie van een workflow veranderen van &quot;Ontvangers&quot; in &quot;toepassing Abonnees&quot; om pushberichten naar de beoogde ontvangers te verzenden.

## Vorm de de afmetingsactiviteit van de Verandering {#configure}

Voer de volgende stappen uit om de **Dimensie wijzigen** activiteit:

1. Voeg een **Dimensie wijzigen** activiteit aan uw werkschema.

   ![](../assets/workflow-change-dimension.png)

1. Definieer de **Nieuwe doeldimensie**. Tijdens het wijzigen van de afmetingen worden alle records bewaard. Andere opties zijn nog niet beschikbaar.

1. Voer de workflow uit om het resultaat weer te geven. Vergelijk de gegevens in de tabellen voor en na de activiteit voor de veranderingsdimensie en vergelijk de structuur van de workflowtabellen.

## Voorbeeld {#example}

In dit voorbeeld willen we een SMS-levering verzenden naar alle profielen die een aankoop hebben gedaan. Om dit te doen, gebruiken wij eerst **[!UICONTROL Build audience]** activiteit gekoppeld aan een aangepaste &#39;Aankoop&#39;-dimensie om alle aankopen die hebben plaatsgevonden te richten.

Daarna gebruiken we een **[!UICONTROL Change dimension]** activiteit om de werkschema het richten dimensie op &quot;Ontvangers&quot;te schakelen. Dit staat ons toe om de ontvangers te kunnen richten die de vraag aanpassen.

![](assets/workflow-change-dimension-example.png)
