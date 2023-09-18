---
audience: end-user
title: De workflowactiviteit voor het publiek van Build gebruiken
description: Leer hoe u de workflowactiviteit voor het publiek van Build gebruikt
badge: label="Beta"
source-git-commit: ff3e93a6c8e66c8160f132772ea1a8bfd769ec5b
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---


# publiek opbouwen {#build-audience}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience"
>title="Activiteit voor publiek opbouwen"
>abstract="De **publiek opbouwen** Met deze activiteit kunt u het publiek definiëren dat de workflow zal betreden. Wanneer het verzenden van berichten in de context van een werkschema, wordt het berichtpubliek niet bepaald in de kanaalactiviteit, maar in **publiek opbouwen** activiteit."


De **publiek opbouwen** activiteit is **Targeting** activiteit. Met deze activiteit kunt u het publiek definiëren dat de workflow zal betreden. Wanneer het verzenden van berichten in de context van een werkschema, wordt het berichtpubliek niet bepaald in de kanaalactiviteit, maar in **publiek opbouwen** activiteit.

Om de publieksbevolking te bepalen, kunt u:

* Selecteer een bestaand publiek dat als een lijst in de cliëntconsole wordt gecreeerd.
* Selecteer een Adobe Experience Platform-publiek.
* Bouw een nieuw publiek met de regelbouwer door het filtreren criteria te bepalen en te combineren.

>[!NOTE]
>
>In deze context kunt u geen publiek uit een bestand laden. Hiervoor moet u een zelfstandige e-maillevering maken. [Meer informatie](../../audience/about-audiences.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Vorm de het publieksactiviteit van de Bouwstijl

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Doeldimensie selecteren"
>abstract="Met de doeldimensie kunt u de doelgroep van de actie definiëren: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. Standaard is het doel geselecteerd bij de ontvangers."


Voer de volgende stappen uit om de **publiek opbouwen** activiteit:

1. Voeg een **publiek opbouwen** activiteit.
1. Definieer een label.
1. Bepaal het publiekstype: **Maak uw eigen** of **Lees publiek**.

Voer de volgende extra stappen uit om uw eigen query te maken:

1. Selecteren **Uw eigen bestand maken (query)**.
1. Kies de optie **Doeldimensie**. Met de doeldimensie kunt u de doelgroep van de actie definiëren: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. Standaard is het doel geselecteerd bij de ontvangers. Zie de [v8-documentatie](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Klikken **Doorgaan**.
1. Gebruik de bouwer van de regel om uw vraag te bepalen, de zelfde manier u creeert een publiek wanneer het ontwerpen van een nieuwe e-mail. Zie dit [sectie](../../audience/segment-builder.md).

Voer de volgende stappen uit om een bestaand publiek te selecteren:

1. Selecteren **Lees publiek**.
1. Klikken **Doorgaan**.
1. Selecteer uw publiek, zoals u een publiek gebruikt bij het ontwerpen van een nieuwe e-mail. Zie dit [sectie](../../audience/add-audience.md).

>[!IMPORTANT]
>
>Als u meerdere **[!UICONTROL Build audience]** activiteiten in een werkstroom, waaronder een publiek in een Experience Platform, moet u een **[!UICONTROL Change dimension]** activiteiten daarna, om ervoor te zorgen dat alle doelgroepen behoren tot de doeldimensie &quot;Ontvanger&quot;. Onder aan deze pagina vindt u een voorbeeld van de workflow.

## Voorbeelden

Hier is een voorbeeld van een workflow met twee **publiek opbouwen** activiteiten. De eerste is gericht op het publiek van pokerspelers, gevolgd door een e-mailbezorging. De tweede is gericht op het publiek van VIP klanten, gevolgd door een SMS-levering.

![](../assets/workflow-audience-example.png)

Hier is nog een voorbeeld van een combinatie van een Adobe Experience Platform-publiek met een Adobe Campaign-publiek. Om deze doelgroepen te kunnen combineren, moet u **[Dimensie iUICONTROL-wijziging]** activiteit met de &quot;Ontvanger&quot;het richten dimensie wordt toegevoegd na het publiek van Adobe Experience Platform.

![](../assets/workflow-audience-aep.png)
