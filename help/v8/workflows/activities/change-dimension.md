---
audience: end-user
title: De workflowactiviteit Change-dimensie gebruiken
description: Leer hoe u de workflowactiviteit Wijzigen kunt gebruiken
exl-id: 08870946-91c6-4ab0-84de-4d9b968884b3
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# Dimensie wijzigen {#change-dimension}

>[!CONTEXTUALHELP]
>id="acw_orchestration_dimension_complement"
>title="Een complement genereren"
>abstract="U kunt een extra uitgaande overgang met de resterende bevolking produceren, die als duplicaat werd uitgesloten. Om dit te doen, op **van een knevel te voorzien produceert complement** optie."

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_dimension"
>title="Dimensieactiviteit wijzigen"
>abstract="Met deze activiteit kunt u de doeldimensie wijzigen terwijl u een publiek maakt. Het verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. U kunt bijvoorbeeld van de dimensie &#39;contracten&#39; overschakelen op de dimensie &#39;clients&#39;."

De **dimensie van de Verandering** activiteit is a **richtend** activiteit. Met deze activiteit kunt u de doeldimensie wijzigen terwijl u uw workflow bouwt. Het verschuift de as afhankelijk van het gegevensmalplaatje en de inputdimensie. [&#x200B; Leer meer over het richten van dimensies &#x200B;](../../audience/about-recipients.md#targeting-dimensions).

U kunt bijvoorbeeld de doeldimensie van een workflow veranderen van &quot;Ontvangers&quot; in &quot;Abonnees&quot; om pushberichten naar de beoogde ontvangers te verzenden.

>[!IMPORTANT]
>
>De activiteiten **[!UICONTROL Change Dimension]** en **[!UICONTROL Change Data source]** mogen niet in één rij worden toegevoegd. Als u beide activiteiten opeenvolgend wilt gebruiken, neemt u er een **[!UICONTROL Enrichment]** activiteit tussen op. Dit zorgt voor een correcte uitvoering en voorkomt mogelijke conflicten of fouten.

## Vorm de de afmetingsactiviteit van de Verandering {#configure}

Volg deze stappen om de **dimensie van de Verandering** activiteit te vormen:

1. Voeg de dimensie van de a **Verandering** activiteit aan uw werkschema toe.

   ![&#x200B; Schermafbeelding die de de afmetingsactiviteit van de Verandering tonen die aan een werkschema &#x200B;](../assets/workflow-change-dimension.png) wordt toegevoegd

1. Bepaal de **Nieuwe doelafmeting**. Tijdens het wijzigen van de afmetingen worden alle records bewaard. Andere opties zijn nog niet beschikbaar.

1. Voer de workflow uit om het resultaat weer te geven. Vergelijk de gegevens in de tabellen voor en na de activiteit Dimensie wijzigen en vergelijk de structuur van de workflowtabellen.

## Voorbeeld {#example}

In dit voorbeeld verzendt u een SMS-bericht naar alle profielen die een aankoop hebben gedaan. Gebruik eerst een **[!UICONTROL Build audience]** -activiteit die is gekoppeld aan een aangepaste &#39;Aankoop&#39;-doeldimensie om alle aankopen te activeren.

Gebruik vervolgens een **[!UICONTROL Change dimension]** -activiteit om de workflow voor het opgeven van dimensies te veranderen in &quot;Ontvangers&quot;. Dit staat het richten van de ontvangers toe die de vraag aanpassen.

![&#x200B; Schermafbeelding die een voorbeeld van de de afmetingsactiviteit van de Verandering toont die in een werkschema &#x200B;](../assets/workflow-change-dimension-example.png) wordt gebruikt