---
audience: end-user
title: Activiteit van de JavaScript-codewerkstroom gebruiken
description: Meer informatie over het gebruik van de JavaScript-workflowactiviteit voor code
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: 1f5bd502527d0ba285e82fdda7b3f8dc86ac2c76
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 1%

---

# JavaScript-code {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript-code"
>abstract="De **code van JavaScript** activiteit staat u toe om een manuscript van JavaScript in de context van een werkschema uit te voeren. Op deze manier kunt u handelingen uitvoeren of gegevens uit de database verzamelen. Gebruik **Eenvoudige** de codeactiviteiten van JavaScript om één codefragment bij werkschemauitvoering uit te voeren. **Geavanceerde** Javascript codeactiviteiten staat u toe om complexere verrichting uit te voeren door twee verschillende codefragmenten in een opeenvolgende orde uit te voeren. De eerste keer wordt het werkschema begonnen, wordt de eerste vraag uitgevoerd. Telkens wanneer de werkstroom opnieuw loopt, wordt de code die in de tweede vraag wordt bepaald uitgevoerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript-fragment"
>abstract="Definieer het script dat moet worden uitgevoerd wanneer de activiteit wordt uitgevoerd. Als u een **Geavanceerde** activiteit van JavaScript vormt, moet u twee codefragmenten uitgeven: de eerste vraagcode om bij de eerste uitvoering van het werkschema uit te voeren, en de volgende vraagcode om bij de volgende vraag van het werkschema uit te voeren."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript Execution"
>abstract="Vorm de uitvoeringsvertraging om de activiteit na een periode van uitvoering te stoppen. Standaard kan de uitvoeringsfase niet langer duren dan 1 uur. Na deze vertraging wordt het proces afgebroken met een foutbericht en mislukt de uitvoering van de activiteit. Als u deze limiet wilt negeren, stelt u de waarde in op 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="JavaScript-overgang"
>abstract="Als u een of meerdere uitvoerovergangen wilt toevoegen, klikt u op de knop **[!UICONTROL Add transitions]** en geeft u een label en een interne naam voor elke overgang op."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_processerrors"
>title="Procesfouten"
>abstract="Schakel de optie **[!UICONTROL Process errors]** in of uit om fouten te behouden die optreden tijdens de uitvoering van het script in een extra uitvoerovergang."

De **code van JavaScript** activiteit is a **het beheer van Gegevens** activiteit. Gebruik deze activiteit om een JavaScript script uit te voeren in de context van een workflow. Op deze manier kunt u gegevens van de database verzamelen of andere complexe bewerkingen uitvoeren.

## De JavaScript-codeactiviteit configureren {#javascript-code-configuration}

Volg deze stappen om de **code van JavaScript** activiteit te vormen:

1. Voeg de code van a **JavaScript** activiteit in uw werkschema toe.

1. Kies welk type activiteit u wilt maken:

   * **Eenvoudig**: Voer één codefragment uit.
   * **Geavanceerd**: Deze optie staat u toe om geavanceerdere verrichtingen uit te voeren door twee verschillende codefragmenten uit te voeren. [ Leer hoe te om een geavanceerde activiteit van JavaScript te vormen ](#advanced)

   >[!NOTE]
   >
   >Met het Gebruikersinterface van het Web van de Campagne, hebben wij twee activiteiten in één geconsolideerd door zowel **Eenvoudige** als **Geavanceerde** de codefunctionaliteit van JavaScript samen te voegen. Deze consolidatie heeft op geen enkele wijze invloed op de functionaliteit van de activiteit.

1. Bevestig vervolgens de expressie-editor door op de knop **[!UICONTROL Edit code]** te klikken. Het linkerdeelvenster bevat vooraf gedefinieerde syntaxis waarmee u code kunt samenstellen, inclusief gebeurtenisvariabelen. [ Leer hoe te met gebeurtenisvariabelen en de uitdrukkingsredacteur te werken ](../event-variables.md)

   ![](../assets/javascript-editor.png)

1. Configureer in de sectie **[!UICONTROL Execution]** de vertraging om de activiteit na een uitvoeringsperiode te stoppen. Standaard kan de uitvoeringsfase niet langer duren dan 1 uur. Na deze vertraging wordt het proces afgebroken met een foutbericht en mislukt de uitvoering van de activiteit. Als u deze limiet wilt negeren, stelt u de waarde in op 0.

   ![](../assets/javascript-config.png)

1. Schakel de optie **[!UICONTROL Process errors]** in of uit om fouten te behouden die optreden tijdens de uitvoering van het script in een extra uitvoerovergang.

## Geavanceerde JavaScript-codeactiviteiten {#advanced}

Met geavanceerde JavaScript-activiteiten kunt u complexe bewerkingen uitvoeren. Zo kunt u:

* Twee verschillende codefragmenten uitvoeren. Het eerste codefragment wordt uitgevoerd de eerste keer dat de workflow wordt gestart. Telkens wanneer de werkstroom opnieuw loopt, wordt het codefragment dat in de tweede vraag wordt bepaald uitgevoerd.
* Voeg meerdere uitvoerovergangen toe die u dynamisch kunt gebruiken met een script.

Voer de volgende stappen uit om een geavanceerde JavaScript-codeactiviteit te configureren:

1. Selecteer het **Geavanceerde** type, dan vorm de uit te voeren codefragment(en):

   * Klik **[!UICONTROL Edit first call code]** om het manuscript te bepalen dat tijdens de eerste vraag moet uitvoeren.
   * Klik op **[!UICONTROL Edit next call code]** om het script te definiëren dat moet worden uitgevoerd tijdens de volgende aanroepen van de workflow. (optioneel)

1. Als u een of meerdere uitvoerovergangen wilt toevoegen, klikt u op de knop **[!UICONTROL Add transitions]** en geeft u een label en een interne naam voor elke overgang op.

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

1. Voeg de code van a **JavaScript** activiteit met het type **Eenvoudige** na **toe bouwt publiek** activiteit.

1. Klik **uitgeven code** en vorm het codefragment zoals hieronder:

   ```
   if (vars.recCount > 1000)
       vars.channel ="email"
   else
       vars.channel = "sms"
   ```

1. Start de workflow. De &quot;kanaal&quot;variabele wordt gecreeerd met de &quot;e-mail&quot;of &quot;sms&quot;waarde, afhankelijk van het aantal profielen die door **worden gericht bouwt publieksactiviteit**.

### Overgangen activeren op basis van de waarde van een variabele {#example2}

In dit voorbeeld wordt getoond hoe u een overgang activeert op basis van de waarde van een variabele.

![](../assets/javascript-example2-transitions.png)

Hier, begint het werkschema met een **Externe signaal** activiteit, waarin een variabele (`interest`) van een ander werkschema wordt overgegaan. De waarde van de variabele is ‘actief’ of ‘yoga’, afhankelijk van de filterbewerkingen die in de eerste workflow zijn uitgevoerd.

We willen verschillende overgangen in de workflow activeren op basis van de waarde van de variabele.

Ga als volgt te werk om dit te doen:

1. Voeg de code van a **JavaScript** activiteit na de Externe signaalactiviteit met het type **Geavanceerde** toe.

1. Voeg twee overgangen toe: één voor elke mogelijke variabelewaarde (&quot;lopend&quot;, &quot;yoga&quot;).

1. Klik **uitgeven eerste vraagcode** en vorm het codefragment zoals hieronder:

   ```
   if (vars.interest=="running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Voltooi de configuratie van elke overgang aan uw behoeften dan begin het werkschema. Één van de twee outputovergangen wordt geactiveerd, gebaseerd op de waarde van de `interest` variabele die door de **Externe signaal** activiteit is overgegaan.
