---
audience: end-user
title: De workflowactiviteit Change-dimensie gebruiken
description: Leer hoe u de workflowactiviteit Wijzigen kunt gebruiken
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: 52b129be88e48dd70c0f55b404fd3bbe699dbebb
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Dimensie wijzigen {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Een complement genereren"
>abstract="U kunt een extra uitgaande overgang met de resterende bevolking produceren, die als duplicaat werd uitgesloten. Om dit te doen, op **van een knevel voorzien produceer complement** optie"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Dimensieactiviteit wijzigen"
>abstract="Met deze activiteit kunt u de doeldimensie wijzigen terwijl u een publiek maakt. Het verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. U kunt bijvoorbeeld van de dimensie &quot;contracten&quot; naar de dimensie &quot;clients&quot; schakelen."

De **dimensie van de Verandering** activiteit is a **richtend** activiteit. Met deze activiteit kunt u de doeldimensie wijzigen terwijl u uw workflow bouwt. Het verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. [ leer meer bij het richten van dimensies ](../../audience/about-recipients.md#targeting-dimensions)

U kunt bijvoorbeeld de doeldimensie van een workflow veranderen van &quot;Ontvangers&quot; in &quot;Abonnees&quot; om pushberichten naar de beoogde ontvangers te verzenden.

>[!IMPORTANT]
>
>De activiteiten **[!UICONTROL Change Dimension]** en **[!UICONTROL Change Data source]** mogen niet in één rij worden toegevoegd. Als u beide activiteiten opeenvolgend moet gebruiken, zorg ervoor u een **[!UICONTROL Enrichement]** activiteit binnen tussen hen omvat. Dit zorgt voor een correcte uitvoering en voorkomt mogelijke conflicten of fouten.

## Vorm de de afmetingsactiviteit van de Verandering {#configure}

Volg deze stappen om de **dimensie van de Verandering** activiteit te vormen:

1. Voeg de dimensie van de a **Verandering** activiteit aan uw werkschema toe.

   ![](../assets/workflow-change-dimension.png)

1. Bepaal de **Nieuwe doelafmeting**. Tijdens het wijzigen van de afmetingen worden alle records bewaard. Andere opties zijn nog niet beschikbaar.

1. Voer de workflow uit om het resultaat weer te geven. Vergelijk de gegevens in de tabellen voor en na de activiteit voor de veranderingsdimensie en vergelijk de structuur van de workflowtabellen.

## Voorbeeld {#example}

In dit voorbeeld willen we een SMS-levering verzenden naar alle profielen die een aankoop hebben gedaan. Hiervoor gebruiken we eerst een **[!UICONTROL Build audience]** -activiteit die gekoppeld is aan een aangepaste &#39;Aankoop&#39;-doeldimensie om alle aankopen te activeren.

Vervolgens gebruiken we een **[!UICONTROL Change dimension]** -activiteit om de workflow voor het opgeven van de dimensie te veranderen in &quot;Ontvangers&quot;. Dit staat ons toe om de ontvangers te kunnen richten die de vraag aanpassen.

![](../assets/workflow-change-dimension-example.png)
