---
audience: end-user
title: De workflowactiviteit voor het publiek van Build gebruiken
description: Leer hoe u de workflowactiviteit voor het publiek van Build gebruikt
badge: label="Beperkte beschikbaarheid"
exl-id: c07bb025-51b7-428e-ba00-cd552f0db9d4
source-git-commit: fb72b943b324990f6dd82a4a05bfd28e5452480a
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 1%

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
* Bouw een nieuw publiek met de bouwer van de vraagmodelleur door het filtreren criteria te bepalen en te combineren.

>[!NOTE]
>
>In deze context kunt u geen publiek uit een bestand laden. Hiervoor moet u een zelfstandige e-maillevering maken. [Meer informatie](../../audience/about-recipients.md)

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

## Vorm de het publieksactiviteit van de Bouwstijl{#build-audience-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Doeldimensie selecteren"
>abstract="Met de doeldimensie kunt u de doelgroep van de actie definiëren: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. Standaard is het doel geselecteerd bij de ontvangers."

Voer de volgende stappen uit om de **publiek opbouwen** activiteit:

![](../assets/workflow-audience.png)

1. Voeg een **publiek opbouwen** activiteit.
1. Definieer een label.
1. Bepaal het publiekstype: **Maak uw eigen** of **Lees publiek**.
1. Configureer uw publiek door de stappen uit te voeren die in de onderstaande tabbladen worden beschreven.

>[!BEGINTABS]

>[!TAB Uw eigen bestand maken (query)]

Voer de volgende stappen uit om uw eigen query te maken:

1. Selecteren **Uw eigen bestand maken (query)**.
1. Kies de optie **Doeldimensie**. Met de doeldimensie kunt u de doelgroep van de actie definiëren: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. Standaard is het doel geselecteerd bij de ontvangers. [Meer informatie over doelgerichte dimensies](../../audience/about-recipients.md#targeting-dimensions)
1. Klikken **Doorgaan**.
1. Gebruik de vraagmodeler om uw vraag te bepalen, de zelfde manier u creeert een publiek wanneer het ontwerpen van een nieuwe e-mail. [Leer hoe te met vraagmodeler te werken](../../audience/../query/query-modeler-overview.md)

>[!TAB Doelgroep lezen]

Voer de volgende stappen uit om een bestaand publiek te selecteren:

1. Selecteren **Lees publiek**.
1. Klikken **Doorgaan**.
1. Selecteer uw publiek, de zelfde manier u een publiek gebruikt wanneer het ontwerpen van een nieuwe levering. Zie dit [sectie](../../audience/add-audience.md).

>[!IMPORTANT]
>
>Als u een **[!UICONTROL Build audience]** activiteit gericht op een publiek van het Experience Platform, moet u toevoegen **[!UICONTROL Change dimension]** activiteit daarna, om ervoor te zorgen dat de doelgerichte dimensie van het publiek aan &quot;Ontvanger&quot;wordt geplaatst. Onder aan deze pagina vindt u een voorbeeld van de workflow.

>[!ENDTABS]

## Voorbeelden{#build-audience-examples}

Hier is een voorbeeld van een workflow met twee **publiek opbouwen** activiteiten. De eerste is gericht op het publiek van pokerspelers, gevolgd door een e-mailbezorging. De tweede is gericht op het publiek van VIP klanten, gevolgd door een SMS-levering.

![](../assets/workflow-audience-example.png)

Hier is nog een voorbeeld van een workflow waarbij een Adobe Experience Platform-publiek wordt gecombineerd met een Adobe Campaign-publiek. Om deze doelgroepen te kunnen combineren, moet u **[!UICONTROL Change dimension]** activiteit met de &quot;Ontvanger&quot;het richten dimensie wordt toegevoegd na het publiek van Adobe Experience Platform. [Leer hoe te om een de dimensie van de Verandering activiteit te vormen](change-dimension.md)

![](../assets/workflow-audience-aep.png)
