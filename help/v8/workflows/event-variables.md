---
audience: end-user
title: Workflowgebeurtenisvariabelen
description: Leer hoe u gebeurtenisvariabelen in uw workflows kunt gebruiken.
exl-id: 526dc98f-391d-4f3f-a687-c980bf60b93b
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Workflowgebeurtenisvariabelen {#event-variables}

Bij sommige workflowactiviteiten kunt u scripts in de expressie-editor bewerken om specifieke handelingen uit te voeren, zoals het ophalen van gegevens uit eerdere activiteiten, het bouwen van voorwaarden of het berekenen van bestandsnamen op basis van gebeurtenisvariabelen.

## Wat zijn gebeurtenisvariabelen {#scripting}

Scripts die worden uitgevoerd in de context van een workflow, openen een reeks aanvullende algemene scripts **objecten** zoals de workflow zelf die wordt uitgevoerd (`ìnstance`), de diverse taken (`task`) of de gebeurtenissen die een bepaalde taak hebben geactiveerd (`event`).

Naar elk type van **object** is gekoppeld aan een categorie **variabelen** die kunnen worden gebruikt in de expressie-editor wanneer scripts worden bewerkt in activiteiten zoals **[!UICONTROL JavaScript code]** of **[!UICONTROL Test]**.

* **Instantievariabelen** (`instance.vars.xxx`) zijn vergelijkbaar met algemene variabelen. Ze worden door alle activiteiten gedeeld.
* **Taakvariabelen** (`task.vars.xxx`) zijn vergelijkbaar met lokale variabelen. Ze worden alleen gebruikt door de huidige taak. Deze variabelen worden gebruikt door permanente activiteiten om gegevens te bewaren en worden soms gebruikt om gegevens tussen de verschillende manuscripten van een zelfde activiteit uit te wisselen.
* **Gebeurtenisvariabelen** (`vars.xxx`) de uitwisseling van gegevens mogelijk maken tussen de elementaire taken van een werkstroomproces. Deze variabelen worden doorgegeven door de taak die de actieve taak heeft geactiveerd. Deze worden vervolgens doorgegeven aan de volgende activiteiten. **Gebeurtenisvariabelen** Dit zijn de meest gebruikte variabelen en deze moeten bij voorkeur worden gebruikt in plaats van instantievariabelen.

>[!NOTE]
>
>Aanvullende informatie over scripts en de belichte objecten en variabelen in Adobe Campaign is beschikbaar in de Campagne v8 (clientconsole)-documentatie in [deze sectie](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-scripts-and-templates).
>
>Merk op dat terwijl deze bron waardevolle inzichten aanbiedt, er discrepanties kunnen bestaan aangezien het specifiek op de cliëntconsole eerder dan het Gebruikersinterface van het Web van de Campagne van toepassing is.

## Gebeurtenisvariabelen in de expressieeditor benutten {#expression-editor}

Vooraf gedefinieerde gebeurtenisvariabelen zijn beschikbaar voor gebruik in het linkerdeelvenster van de expressieeditor. U kunt ook nieuwe maken door een nieuwe variabele in uw code te initialiseren.

![](assets/event-variables.png)

Naast deze gebeurtenisvariabelen kunt u ook de functie **[!UICONTROL Conditions]** in het linkerdeelvenster om voorwaarden te maken en de **[!UICONTROL Add current date]** gebruiken voor functies die betrekking hebben op datumopmaak.
