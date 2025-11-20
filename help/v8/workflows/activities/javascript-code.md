---
audience: end-user
title: Activiteit van de JavaScript-codewerkstroom gebruiken
description: Meer informatie over het gebruik van de JavaScript-workflowactiviteit voor code
exl-id: ca040ef8-5e0d-44e0-818d-08cfe99100be
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '946'
ht-degree: 0%

---

# JavaScript-code {#javascript-code}

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript-code"
>abstract="De **code van JavaScript** activiteit staat u toe om een manuscript van JavaScript in de context van een werkschema uit te voeren. Hierdoor kunt u handelingen uitvoeren of gegevens uit de database verzamelen. Gebruik **Eenvoudige** de codeactiviteiten van JavaScript om één codefragment tijdens werkschemauitvoering uit te voeren. **Geavanceerde** de codeactiviteiten van JavaScript staan u toe om complexere verrichtingen uit te voeren door twee verschillende codefragmenten opeenvolgend uit te voeren. De eerste keer dat de workflow start, wordt de eerste aanroep uitgevoerd. Telkens wanneer de werkstroom opnieuw loopt, wordt de code die in de tweede vraag wordt bepaald uitgevoerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript-fragment"
>abstract="Definieer het script dat moet worden uitgevoerd wanneer de activiteit wordt uitgevoerd. Als u een **Geavanceerde** activiteit van JavaScript vormt, geef twee codefragmenten uit: de eerste vraagcode om tijdens de eerste werkschemauitvoering uit te voeren, en de volgende vraagcode om tijdens verdere werkschemauitvoeringen uit te voeren."

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

De **code van JavaScript** activiteit is a **het beheer van Gegevens** activiteit. Gebruik deze activiteit om een JavaScript script uit te voeren in de context van een workflow. Op deze manier kunt u gegevens verzamelen uit de database of andere complexe bewerkingen uitvoeren.

## De JavaScript-codeactiviteit configureren {#javascript-code-configuration}

Volg deze stappen om de **code van JavaScript** activiteit te vormen:

1. Voeg de code van a **JavaScript** activiteit in uw werkschema toe.

1. Kies het type activiteit dat u wilt maken:

   * **Eenvoudig**: Voer één codefragment uit.
   * **Geavanceerd**: Voer geavanceerdere verrichtingen door twee verschillende codefragmenten uit te voeren. [&#x200B; Leer hoe te om een geavanceerde activiteit van JavaScript te vormen &#x200B;](#advanced)

   >[!NOTE]
   >
   >Met het Gebruikersinterface van het Web van de Campagne, zijn twee activiteiten geconsolideerd in door zowel **Eenvoudige** als **Geavanceerde** de codefunctionaliteit van JavaScript samen te voegen. Deze consolidatie heeft geen invloed op de functionaliteit van de activiteit.

1. Bevestig en klik op de knop **[!UICONTROL Edit code]** om de expressie-editor te openen. Het linkerdeelvenster bevat vooraf gedefinieerde syntaxis waarmee u code kunt maken, inclusief gebeurtenisvariabelen. [&#x200B; Leer hoe te met gebeurtenisvariabelen en de uitdrukkingsredacteur &#x200B;](../event-variables.md) te werken.

   ![&#x200B; de redacteurinterface van de Uitdrukking voor de codeactiviteit van JavaScript &#x200B;](../assets/javascript-editor.png)

1. Configureer in de sectie **[!UICONTROL Execution]** de vertraging om de activiteit na een uitvoeringsperiode te stoppen. Standaard kan de uitvoeringsfase niet langer duren dan 1 uur. Na deze vertraging wordt het proces afgebroken met een foutbericht en mislukt de uitvoering van de activiteit. Als u deze limiet wilt negeren, stelt u de waarde in op 0.

   ![&#x200B; interface van de Configuratie voor uitvoeringsvertraging &#x200B;](../assets/javascript-config.png)

1. Schakel de optie **[!UICONTROL Process errors]** in of uit om fouten te behouden die optreden tijdens de uitvoering van het script in een extra uitvoerovergang.

## Geavanceerde JavaScript-codeactiviteiten {#advanced}

Met geavanceerde JavaScript-activiteiten kunt u complexe bewerkingen uitvoeren. Met deze activiteiten kunt u:

* Twee verschillende codefragmenten uitvoeren. Het eerste codefragment wordt uitgevoerd de eerste keer dat de workflow start. Telkens wanneer de werkstroom opnieuw loopt, wordt het codefragment dat in de tweede vraag wordt bepaald uitgevoerd.
* Voeg meerdere uitvoerovergangen toe die u dynamisch kunt gebruiken met een script.

Voer de volgende stappen uit om een geavanceerde JavaScript-codeactiviteit te configureren:

1. Selecteer het **Geavanceerde** type, dan vorm de uit te voeren codefragmenten:

   * Klik **[!UICONTROL Edit first call code]** om het manuscript te bepalen dat tijdens de eerste vraag moet uitvoeren.
   * Klik op **[!UICONTROL Edit next call code]** om het script te definiëren dat moet worden uitgevoerd tijdens volgende aanroepen van de workflow. (optioneel)

1. Als u een of meerdere uitvoerovergangen wilt toevoegen, klikt u op de knop **[!UICONTROL Add transitions]** en geeft u een label en een interne naam voor elke overgang op.

   In dit voorbeeld worden twee overgangen geconfigureerd en geactiveerd door het script in het codefragment op basis van specifieke voorwaarden.

   ![&#x200B; Voorbeeld van gevormde overgangen &#x200B;](../assets/javascript-transitions.png)

1. Voltooi de activiteitenconfiguratie en begin het werkschema.

## Voorbeeld {#javascript-code-example}

### Variabelen initialiseren op basis van de binnenkomende populatie {#example1}

In dit voorbeeld ziet u hoe u een variabele initialiseert op basis van het aantal profielen dat wordt gebruikt door een workflow.

![&#x200B; Voorbeeld van veranderlijke initialisering die op profieltelling wordt gebaseerd &#x200B;](../assets/javascript-example1.png)

In dit voorbeeld worden VIP-profielen uit de database als doel ingesteld. Een variabele genoemd &quot;kanaal&quot;wordt gecreeerd met een waarde die van het aantal profielen afhangt die door de het publieksactiviteit van de Bouwstijl wordt gericht:

* Als u meer dan 1000 profielen als doel instelt, initialiseert u de variabele met de waarde &quot;email&quot;.
* Anders initialiseert u de code met de waarde &quot;sms&quot;.

Om dit te bereiken, volg deze stappen:

1. Voeg de code van a **JavaScript** activiteit met het type **Eenvoudige** na **toe bouwt publiek** activiteit.

1. Klik **uitgeven code** en vorm het codefragment zoals hieronder getoond:

   ```
   if (vars.recCount > 1000)
       vars.channel = "email";
   else
       vars.channel = "sms";
   ```

1. Start de workflow. De &quot;kanaal&quot;variabele wordt gecreeerd met de &quot;e-mail&quot;of &quot;sms&quot;waarde, afhankelijk van het aantal profielen die door **worden gericht bouwt publieksactiviteit**.

### Overgangen activeren op basis van de waarde van een variabele {#example2}

In dit voorbeeld wordt getoond hoe u een overgang activeert op basis van de waarde van een variabele.

![&#x200B; Voorbeeld van overgangen die door veranderlijke waarden &#x200B;](../assets/javascript-example2-transitions.png) worden teweeggebracht

In dit voorbeeld, begint het werkschema met een **Externe signaal** activiteit, waarin een variabele (`interest`) van een ander werkschema wordt overgegaan. De waarde van de variabele is ‘actief’ of ‘yoga’, afhankelijk van de filterbewerkingen die in de eerste workflow zijn uitgevoerd.

Verschillende overgangen in de workflow worden geactiveerd op basis van de waarde van de variabele.

Om dit te bereiken, volg deze stappen:

1. Voeg de code van a **JavaScript** activiteit na de Externe signaalactiviteit met het type **Geavanceerde** toe.

1. Voeg twee overgangen toe: één voor elke mogelijke variabelewaarde (&quot;lopend&quot;, &quot;yoga&quot;).

1. Klik **uitgeven eerste vraagcode** en vorm het codefragment zoals hieronder getoond:

   ```
   if (vars.interest == "running")
       task.postEvent(task.transitionByName("running"));
   else
       task.postEvent(task.transitionByName("yoga"));
   ```

1. Voltooi de configuratie van elke overgang aan uw behoeften, dan begin het werkschema. Één van de twee outputovergangen wordt geactiveerd gebaseerd op de waarde van de `interest` variabele die door de **Externe signaal** activiteit wordt overgegaan.