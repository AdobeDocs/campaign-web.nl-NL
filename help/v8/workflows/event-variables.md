---
audience: end-user
title: Workflowgebeurtenisvariabelen
description: Leer hoe u gebeurtenisvariabelen in uw workflows kunt gebruiken.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Workflowgebeurtenisvariabelen {#event-variables}

Bij sommige workflowactiviteiten kunt u scripts in de expressie-editor bewerken om specifieke handelingen uit te voeren, zoals het ophalen van gegevens uit eerdere activiteiten, het bouwen van voorwaarden of het berekenen van bestandsnamen op basis van gebeurtenisvariabelen.

## Wat zijn gebeurtenisvariabelen {#scripting}

De manuscripten die in de context van een werkschematoegang worden uitgevoerd tot een reeks extra globale **voorwerpen**, zoals het werkschema zelf dat (`instance`) wordt uitgevoerd, zijn diverse taken (`task`), of de gebeurtenissen die een bepaalde taak (`event`) activeerden.

Elk type van **voorwerp** wordt geassocieerd met een categorie van **variabelen** die in de uitdrukkingsredacteur kunnen worden gebruikt wanneer het uitgeven van manuscripten in activiteiten, zoals **[!UICONTROL JavaScript code]** of **[!UICONTROL Test]**.

* **de variabelen van de Instantie** (`instance.vars.xxx`) zijn vergelijkbaar met globale variabelen. Ze worden door alle activiteiten gedeeld.
* **de variabelen van de Taak** (`task.vars.xxx`) zijn vergelijkbaar met lokale variabelen. Ze worden alleen gebruikt door de huidige taak. Deze variabelen worden gebruikt door permanente activiteiten om gegevens te bewaren en worden soms gebruikt om gegevens tussen de verschillende manuscripten van de zelfde activiteit uit te wisselen.
* **de variabelen van de Gebeurtenis** (`vars.xxx`) laten de uitwisseling van gegevens tussen de elementaire taken van een werkschemaproces toe. Deze variabelen worden doorgegeven door de taak die de actieve taak heeft geactiveerd. Deze worden vervolgens doorgegeven aan de volgende activiteiten. **de variabelen van de Gebeurtenis** zijn de het meest algemeen gebruikte variabelen, en zij zouden in voorkeur aan instantievariabelen moeten worden gebruikt.

>[!NOTE]
>
>De extra informatie over scripting en de blootgestelde voorwerpen en de variabelen in Adobe Campaign is beschikbaar in de Campagne v8 (cliëntconsole) documentatie in [ deze sectie ](https://experienceleague.adobe.com/nl/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Merk op dat terwijl deze bron waardevolle inzichten aanbiedt, er discrepanties kunnen bestaan aangezien het specifiek op de cliëntconsole eerder dan het Gebruikersinterface van het Web van de Campagne van toepassing is.

## Gebeurtenisvariabelen in de expressieeditor benutten {#expression-editor}

De vooraf bepaalde gebeurtenisvariabelen zijn beschikbaar voor gebruik in de de linkerzijruit van de uitdrukkingsredacteur. U kunt ook nieuwe maken door een nieuwe variabele in uw code te initialiseren.

![ Schermafbeelding die vooraf bepaalde gebeurtenisvariabelen in de linkerzijruit van de uitdrukkingsredacteur toont ](assets/event-variables.png)

Naast deze gebeurtenisvariabelen kunt u ook het menu **[!UICONTROL Conditions]** in het linkerdeelvenster gebruiken om voorwaarden te maken en het menu **[!UICONTROL Add current date]** om functies toe te passen die betrekking hebben op datumopmaak.