---
audience: end-user
title: Activiteit van de JavaScript-codewerkstroom gebruiken
description: Meer informatie over het gebruik van de JavaScript-workflowactiviteit voor code
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '951'
ht-degree: 1%

---

# JavaScript-code {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript-code"
>abstract="De **JavaScript-code** Met activiteit kunt u een JavaScript-script uitvoeren in de context van een workflow. Op deze manier kunt u handelingen uitvoeren of gegevens uit de database verzamelen. Gebruiken **eenvoudig** JavaScript-codeactiviteiten om één codefragment uit te voeren bij de uitvoering van de workflow. **Geavanceerd** Met JavaScript-codeactiviteiten kunt u complexere bewerkingen uitvoeren door twee verschillende codefragmenten in een opeenvolgende volgorde uit te voeren. De eerste keer wordt het werkschema begonnen, wordt de eerste vraag uitgevoerd. Telkens wanneer de werkstroom opnieuw loopt, wordt de code die in de tweede vraag wordt bepaald uitgevoerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript-fragment"
>abstract="Definieer het script dat moet worden uitgevoerd wanneer de activiteit wordt uitgevoerd. Als u een **Geavanceerd** JavaScript-activiteit, moet u twee codefragmenten bewerken: de eerste aanroepcode die wordt uitgevoerd bij de eerste uitvoering van de workflow en de volgende aanroepcode die wordt uitgevoerd bij de volgende aanroepen van de workflow."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript Execution"
>abstract="Vorm de uitvoeringsvertraging om de activiteit na een periode van uitvoering te stoppen. Standaard kan de uitvoeringsfase niet langer duren dan 1 uur. Na deze vertraging wordt het proces afgebroken met een foutbericht en mislukt de uitvoering van de activiteit. Als u deze limiet wilt negeren, stelt u de waarde in op 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript-overgang"
>abstract="Als u meerdere uitvoerovergangen wilt toevoegen, klikt u op de knop **[!UICONTROL Add transitions]** knop. Zo kunt u bijvoorbeeld een specifieke overgang activeren op basis van een specifieke voorwaarde die is gedefinieerd in de JavaScript-codeactiviteit. Deze optie is beschikbaar voor **Geavanceerd** Alleen JavaScript-codeactiviteiten."

De **JavaScript-code** activiteit is **Gegevensbeheer** activiteit. Gebruik deze activiteit om een JavaScript script uit te voeren in de context van een workflow. Op deze manier kunt u gegevens van de database verzamelen of andere complexe bewerkingen uitvoeren.

## De JavaScript-codeactiviteit configureren {#javascript-code-configuration}

Voer de volgende stappen uit om de **JavaScript-code** activiteit:

1. Voeg een **JavaScript-code** in uw workflow.

1. Kies welk type activiteit u wilt maken:

   * **eenvoudig**: Eén codefragment uitvoeren.
   * **Geavanceerd**: Met deze optie kunt u geavanceerdere bewerkingen uitvoeren door twee verschillende codefragmenten uit te voeren. [Leer hoe u een geavanceerde JavaScript-activiteit configureert](#advanced)

   >[!NOTE]
   >
   >Met het Web-gebruikersinterface van de Campagne, hebben wij twee activiteiten in één geconsolideerd door allebei samen te voegen **eenvoudig** en **Geavanceerd** JavaScript-codefuncties. Deze consolidatie heeft op geen enkele wijze invloed op de functionaliteit van de activiteit.

1. Bevestig en klik op **[!UICONTROL Edit code]** om de uitdrukkingsredacteur te openen. Het linkerdeelvenster bevat vooraf gedefinieerde syntaxis waarmee u code kunt samenstellen, inclusief gebeurtenisvariabelen. [Leer hoe u met gebeurtenisvariabelen en de expressie-editor werkt](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. In de **[!UICONTROL Execution]** , configureert u de vertraging om de activiteit na een uitvoeringsperiode te stoppen. Standaard kan de uitvoeringsfase niet langer duren dan 1 uur. Na deze vertraging wordt het proces afgebroken met een foutbericht en mislukt de uitvoering van de activiteit. Als u deze limiet wilt negeren, stelt u de waarde in op 0.

   ![](../assets/javascript-config.png)

1. In-/uitschakelen **[!UICONTROL Process errors]** om fouten die optreden tijdens de uitvoering van het script, in een extra uitvoerovergang te houden.

## Geavanceerde JavaScript-codeactiviteiten {#advanced}

Met geavanceerde JavaScript-activiteiten kunt u complexe bewerkingen uitvoeren. Zo kunt u:

* Twee verschillende codefragmenten uitvoeren. Het eerste codefragment wordt uitgevoerd de eerste keer dat de workflow wordt gestart. Telkens wanneer de werkstroom opnieuw loopt, wordt het codefragment dat in de tweede vraag wordt bepaald uitgevoerd.
* Voeg meerdere uitvoerovergangen toe die u dynamisch kunt gebruiken met een script.

Voer de volgende stappen uit om een geavanceerde JavaScript-codeactiviteit te configureren:

1. Selecteer de **Geavanceerd** het type, vormt dan de uit te voeren codefragmenten:

   * Klikken **[!UICONTROL Edit first call code]** om het manuscript te bepalen dat tijdens de eerste vraag moet uitvoeren.
   * Klikken **[!UICONTROL Edit next call code]** om het manuscript te bepalen dat tijdens de volgende vraag van het werkschema moet uitvoeren. (optioneel)

1. Als u een of meerdere uitvoerovergangen wilt toevoegen, klikt u op de knop **[!UICONTROL Add transitions]** en geeft u voor elke overgang een label en een interne naam op.

   In dit voorbeeld hebben we twee overgangen geconfigureerd die door het script in het codefragment worden geactiveerd op basis van specifieke voorwaarden.

   ![](../assets/javascript-transitions.png)

1. Voltooi de configuratie van de activiteit en start de workflow.

## Voorbeeld {#javascript-code-example}

### Variabelen initialiseren op basis van de binnenkomende populatie {#example1}

In dit voorbeeld ziet u hoe u een variabele initialiseert op basis van het aantal profielen dat wordt gebruikt door een workflow.

![](../assets/javascript-example1.png)

Hier richten we ons op VIP profielen uit onze database. Wij willen een variabele tot stand brengen genoemd &quot;kanaal&quot;met een waarde die van het aantal profielen afhangt dat door de het publieksactiviteit van de Bouwstijl wordt gericht:

* Als u meer dan 1000 profielen als doel instelt, initialiseert u de variabele met de waarde &quot;email&quot;.
* Anders initialiseert u de code met de waarde &quot;sms&quot;.

Ga als volgt te werk om dit te doen:

1. Voeg een **JavaScript-code** activiteit met het type **eenvoudig** na de **publiek opbouwen** activiteit.

1. Klikken **Code bewerken** en configureer het codefragment als volgt:

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. Start de workflow. De variabele &quot;channel&quot; wordt gemaakt met de waarde &quot;email&quot; of &quot;sms&quot;, afhankelijk van het aantal profielen dat wordt gebruikt door de **publiek opbouwen** activiteit.

### Overgangen activeren op basis van de waarde van een variabele {#example2}

In dit voorbeeld wordt getoond hoe u een overgang activeert op basis van de waarde van een variabele.

![](../assets/javascript-example2-transitions.png)

Hier begint de workflow met een **Extern signaal** activiteit waarin een variabele (`interest`) wordt doorgegeven vanuit een andere workflow. De waarde van de variabele is ‘actief’ of ‘yoga’, afhankelijk van de filterbewerkingen die in de eerste workflow zijn uitgevoerd.

We willen verschillende overgangen in de workflow activeren op basis van de waarde van de variabele.

Ga als volgt te werk om dit te doen:

1. Voeg een **JavaScript-code** activiteit na de Externe signaalactiviteit met het type **Geavanceerd**.

1. Voeg twee overgangen toe: één voor elke mogelijke variabelewaarde (&quot;lopend&quot;, &quot;yoga&quot;).

1. Klikken **Eerste aanroepcode bewerken** en configureer het codefragment als volgt:

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Voltooi de configuratie van elke overgang aan uw behoeften dan begin het werkschema. Een van de twee uitvoerovergangen wordt geactiveerd op basis van de waarde van de optie `interest` variabele die door **Extern signaal** activiteit.
