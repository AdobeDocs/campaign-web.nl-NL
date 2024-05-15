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
>abstract="U kunt een extra uitgaande overgang met de resterende bevolking produceren, die als duplicaat werd uitgesloten. Om dit te doen, knevel op **Complement genereren** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Dimensieactiviteit wijzigen"
>abstract="Met deze activiteit kunt u de doeldimensie wijzigen terwijl u een publiek maakt. Het verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. U kunt bijvoorbeeld van de dimensie &quot;contracten&quot; naar de dimensie &quot;clients&quot; schakelen."

De **Dimensie wijzigen** activiteit is **Targeting** activiteit. Met deze activiteit kunt u de doeldimensie wijzigen terwijl u uw workflow bouwt. Het verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. [Meer informatie over doelgerichte dimensies](../../audience/about-recipients.md#targeting-dimensions)

U kunt bijvoorbeeld de doeldimensie van een workflow veranderen van &quot;Ontvangers&quot; in &quot;Abonnees&quot; om pushberichten naar de beoogde ontvangers te verzenden.

>[!IMPORTANT]
>
>Houd er rekening mee dat de **[!UICONTROL Change Dimension]** en **[!UICONTROL Change Data source]** activiteiten mogen niet in één rij worden toegevoegd. Als u beide activiteiten opeenvolgend moet gebruiken, zorg ervoor u omvat **[!UICONTROL Enrichement]** tussen hen. Dit zorgt voor een correcte uitvoering en voorkomt mogelijke conflicten of fouten.

## Vorm de de afmetingsactiviteit van de Verandering {#configure}

Voer de volgende stappen uit om de **Dimensie wijzigen** activiteit:

1. Voeg een **Dimensie wijzigen** activiteit aan uw werkschema.

   ![](../assets/workflow-change-dimension.png)

1. Definieer de **Nieuwe doeldimensie**. Tijdens het wijzigen van de afmetingen worden alle records bewaard. Andere opties zijn nog niet beschikbaar.

1. Voer de workflow uit om het resultaat weer te geven. Vergelijk de gegevens in de tabellen voor en na de activiteit voor de veranderingsdimensie en vergelijk de structuur van de workflowtabellen.

## Voorbeeld {#example}

In dit voorbeeld willen we een SMS-levering verzenden naar alle profielen die een aankoop hebben gedaan. Om dit te doen, gebruiken wij eerst **[!UICONTROL Build audience]** activiteit gekoppeld aan een aangepaste &#39;Aankoop&#39;-dimensie om alle aankopen te richten die hebben plaatsgevonden.

Daarna gebruiken we een **[!UICONTROL Change dimension]** activiteit om de werkschema het richten dimensie op &quot;Ontvangers&quot;te schakelen. Dit staat ons toe om de ontvangers te kunnen richten die de vraag aanpassen.

![](../assets/workflow-change-dimension-example.png)
