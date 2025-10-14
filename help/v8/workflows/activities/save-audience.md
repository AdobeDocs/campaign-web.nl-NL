---
audience: end-user
title: De workflowactiviteit voor het publiek opslaan gebruiken
description: Leer hoe u de vorkworkflowactiviteit kunt gebruiken
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Doelgroep opslaan {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Een publiek opslaan"
>abstract="Gebruik deze activiteit om een bestaand publiek bij te werken of een nieuw publiek van de bevolking te creëren die stroomopwaarts in het werkschema wordt berekend. Het gecreeerde publiek wordt toegevoegd aan de lijst van publiek, en beschikbaar via het **Publiek** menu."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Uitgaande overgang genereren"
>abstract="Gebruik deze optie als u een overgang na **wilt toevoegen sparen publiek** activiteit."

**sparen publiek** activiteit is a **richtend** activiteit. Met deze activiteit kunt u een bestaand publiek bijwerken of een nieuw publiek maken van de populatie die stroomopwaarts in een workflow is berekend. Het gecreeerde publiek wordt toegevoegd aan de lijst van toepassingspubliek, en beschikbaar gemaakt via het **publiek** menu.

Deze activiteit wordt hoofdzakelijk gebruikt om populatiegroepen te behouden die in het zelfde werkschema worden berekend door hen in herbruikbaar publiek om te zetten. Verbind het met andere het richten activiteiten zoals a **bouwt publiek** of a **combineer** activiteit.

## Vorm sparen publieksactiviteit {#save-audience-configuration}

Volg deze stappen om **te vormen sparen publiek** activiteit:

![&#x200B; Beschrijving: De configuratie van het werkschema voor sparen publieksactiviteit &#x200B;](../assets/workflow-save-audience.png)

1. Voeg a **sparen publiek** activiteit aan uw werkschema toe.

1. Op de **drop-down Wijze**, selecteer de actie u wilt uitvoeren:

   * **creeer of werk een bestaand publiek** bij: Bepaal een **etiket van het Publiek**. Als het publiek reeds bestaat, wordt het bijgewerkt; anders, wordt een nieuw publiek gecreeerd.

   * **werk een bestaand publiek** bij: Kies het **Publiek** u van de lijst van bestaand publiek wilt bijwerken.

1. Selecteer de **wijze van de Update** die op bestaand publiek van toepassing is:

   * **vervang publieksinhoud met nieuwe gegevens**: Alle publieksinhoud wordt vervangen, en het oude gegeven wordt verloren. Slechts worden de gegevens van de binnenkomende overgang van **sparen publiek** activiteit behouden. Met deze optie wist u het publiekstype en de doeldimensie van het bijgewerkte publiek.

   * **Volledig publiek met nieuwe gegevens**: De oude publieksinhoud wordt behouden, en de gegevens van de binnenkomende overgang van **sparen publiek** activiteit wordt toegevoegd aan het.

1. Controle **produceert een uitgaande overgang** optie als u een overgang na **wilt toevoegen sparen publiek** activiteit.

De inhoud van het bewaarde publiek is dan beschikbaar in de detailmening van het publiek, dat van het **Publiek** menu kan worden betreden. De kolommen beschikbaar in deze mening beantwoorden aan de kolommen van de binnenkomende overgang van het werkschema **sparen publiek** activiteit.

## Voorbeeld {#save-audience-example}

In het volgende voorbeeld ziet u hoe u een eenvoudige publieksupdate maakt. Een planner stelt het werkschema eens per maand in werking. Met een query worden alle profielen opgehaald die zijn geabonneerd op de verschillende beschikbare toepassingen. **sparen publiek** activiteit werkt het publiek door profielen uit te verwijderen die van de dienst sinds de laatste werkschemauitvoering hebben afgemeld en onlangs ingetekende profielen toevoegen.