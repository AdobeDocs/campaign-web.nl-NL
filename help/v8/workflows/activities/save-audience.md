---
audience: end-user
title: De workflowactiviteit voor het publiek opslaan gebruiken
description: Leer hoe u de vorkworkflowactiviteit kunt gebruiken
exl-id: 0f7cbc34-0536-493e-bb3b-0b1ac93d1232
source-git-commit: 75c612d50d2d4a675829a412e2c4f55ed1cb817c
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 1%

---

# Doelgroep opslaan {#save-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_save_audience"
>title="Een publiek opslaan"
>abstract="Gebruik deze activiteit om een bestaand publiek bij te werken of een nieuw publiek van de bevolking te creëren die stroomopwaarts in het werkschema wordt berekend. Het publiek dat wordt gemaakt, wordt toegevoegd aan de lijst met doelgroepen en is beschikbaar via de **Soorten publiek** -menu."

>[!CONTEXTUALHELP]
>id="acw_orchestration_saveaudience_outbound"
>title="Uitgaande overgang genereren"
>abstract="Gebruik deze optie als u een overgang wilt toevoegen na het dialoogvenster **Adviezen opslaan** activiteit."

De **Adviezen opslaan** activiteit is **Targeting** activiteit. Met deze activiteit kunt u een bestaand publiek bijwerken of een nieuw publiek maken van de populatie die stroomopwaarts in een workflow is berekend. Het publiek dat wordt gemaakt, wordt toegevoegd aan de lijst met doelgroepen van toepassingen en wordt beschikbaar gesteld via de **Soorten publiek** -menu.

Deze activiteit wordt hoofdzakelijk gebruikt om populatiegroepen in de zelfde werkschema gegevens te bewaren, door hen in herbruikbaar publiek om te zetten. Verbind het met andere gerichte activiteiten zoals **publiek opbouwen** of **Combineren** activiteit.

## Vorm sparen publieksactiviteit{#save-audience-configuration}

Voer de volgende stappen uit om de **Adviezen opslaan** activiteit:

![](../assets/workflow-save-audience.png)

1. Voeg een **Adviezen opslaan** activiteit aan uw werkschema.

1. In de **Modus** selecteert u de actie die u wilt uitvoeren:

   * **Een bestaand publiek maken of bijwerken**: definieer een **Label publiek**. Als het publiek reeds bestaat, zal het worden bijgewerkt, anders zal een nieuw publiek worden gecreeerd.

   * **Een bestaand publiek bijwerken**: kies de optie **Publiek** U wilt een update uitvoeren in de lijst met bestaande doelgroepen.

1. Selecteer de **Modus Bijwerken** die van toepassing zijn op bestaande doelgroepen:

   * **De inhoud van het publiek vervangen door nieuwe gegevens**: alle publieksinhoud wordt vervangen. De oude data gaan verloren. Alleen de gegevens van de binnenkomende overgang van de activiteit voor het opslaan van het publiek blijven behouden. Met deze optie wist u het publiekstype en de doeldimensie van het bijgewerkte publiek.

   * **Volledige doelgroep met nieuwe gegevens**: de oude publieksinhoud wordt bewaard en de gegevens van de binnenkomende overgang van de activiteit van het sparen publiek worden toegevoegd aan het.

1. Controleer de **Een uitgaande overgang genereren** als u een overgang wilt toevoegen na de **Adviezen opslaan** activiteit.

De inhoud van het opgeslagen publiek is dan beschikbaar in de gedetailleerde weergave van het publiek, die toegankelijk is vanuit het **Soorten publiek** -menu. De kolommen beschikbaar van deze mening beantwoorden aan de kolommen van de binnenkomende overgang van het werkschema **Adviezen opslaan** activiteit.


## Voorbeeld{#save-audience-example}

In het volgende voorbeeld ziet u hoe u een eenvoudige publieksupdate maakt. Een planner wordt toegevoegd om het werkschema eens per maand in werking te stellen. Met een query worden alle profielen hersteld die zijn geabonneerd op de verschillende beschikbare toepassingen. De **Adviezen opslaan** de activiteit werkt het publiek door profielen te schrappen die van de dienst sinds de laatste werkschemauitvoering hebben losgemaakt en door de onlangs geabonneerde profielen toe te voegen.
