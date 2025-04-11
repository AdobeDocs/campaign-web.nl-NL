---
audience: end-user
title: De activiteit van de testworkflow gebruiken
description: Leer hoe u de activiteit van de testworkflow kunt gebruiken
exl-id: 1bb25ad4-2cab-4656-85bd-4ed018e8477b
source-git-commit: eccd1ce6f95682d3dcfc224061f747f7da0b6681
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---


# Testen {#test}

>[!CONTEXTUALHELP]
>id="acw_orchestration_test"
>title="Testactiviteit"
>abstract="De **activiteit van de Test** is de controle **activiteit van de a** Stroom. Hiermee kunt u overgangen inschakelen op basis van opgegeven voorwaarden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_test_conditions"
>title="Voorwaarden"
>abstract="De **activiteit van de Test** kan veelvoudige uitvoerovergangen hebben. Tijdens de uitvoering van de workflow wordt elke voorwaarde opeenvolgend getest totdat aan een van deze voorwaarden is voldaan. Als aan geen van de voorwaarden wordt voldaan, gaat de workflow verder langs het pad van de **[!UICONTROL Default condition]** . Als geen standaardvoorwaarde wordt geactiveerd, stopt de werkstroom op dit punt."

De **activiteit van de Test** is de controle **activiteit van de a** Stroom. Hiermee kunt u overgangen inschakelen op basis van opgegeven voorwaarden.

## De testactiviteit configureren {#test-configuration}

Volg deze stappen om de **Test** activiteit te vormen:

1. Voeg de activiteit van de a **Test** aan uw werkschema toe.

1. De **[!UICONTROL Test]** -activiteit geeft standaard een eenvoudige booleaanse test weer. Als aan de voorwaarde in de overgang &quot;Waar&quot; wordt bepaald, wordt deze overgang geactiveerd. Anders wordt de standaardovergang &quot;False&quot; geactiveerd.

1. Klik op het pictogram **[!UICONTROL Open personalization dialog]** om de voorwaarde te configureren die aan een overgang is gekoppeld. Gebruik de uitdrukkingsredacteur om de regels te bepalen die worden vereist om deze overgang te activeren. U kunt ook gebeurtenisvariabelen, voorwaarden en datum-/tijdfuncties gebruiken. [ Leer hoe te met gebeurtenisvariabelen en de uitdrukkingsredacteur ](../event-variables.md) te werken.

   Pas bovendien het veld **[!UICONTROL Label]** aan om de naam van de overgang aan te passen op het werkstroomcanvas.

   ![ Standaardconfiguratie van de activiteit van de Test ](../assets/workflow-test-default.png)

1. Voeg meerdere uitvoerovergangen toe aan een **[!UICONTROL Test]** -activiteit. Klik hiertoe op de knop **[!UICONTROL Add condition]** en configureer het label en de bijbehorende voorwaarde voor elke overgang.

1. Tijdens de uitvoering van de workflow wordt elke voorwaarde opeenvolgend getest totdat aan een van deze voorwaarden is voldaan. Als aan geen van de voorwaarden wordt voldaan, gaat de workflow verder langs het pad van de **[!UICONTROL Default condition]** . Als geen standaardvoorwaarde wordt geactiveerd, stopt de werkstroom op dit punt.

## Voorbeeld {#example}

In dit voorbeeld worden verschillende overgangen geactiveerd op basis van het aantal profielen waarop een **[!UICONTROL Build audience]** -activiteit is gericht:
* Als er meer dan 10.000 profielen zijn bedoeld, wordt een e-mailbericht verzonden.
* Voor 1.000 tot 10.000 profielen, wordt SMS verzonden.
* Als de doelprofielen lager zijn dan 1.000, worden ze omgeleid naar een overgang &quot;neem geen contact op&quot;.

![ Voorbeeld van de overgangen van de activiteit van de Test ](../assets/workflow-test-example.png)

Hiertoe wordt de gebeurtenisvariabele `vars.recCount` in de voorwaarden &quot;email&quot; en &quot;sms&quot; gebruikt om het aantal doelprofielen te tellen en de juiste overgang te activeren.

![ Configuratie van het de activiteitenvoorbeeld van de Test ](../assets/workflow-test-example-config.png)
