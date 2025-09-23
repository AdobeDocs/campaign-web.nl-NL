---
title: Afmetingen gericht en filteren
description: Meer informatie over het opgeven en filteren van dimensies in de gebruikersinterface van Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 16fe04858870c58b2f0244f33f691f1606050e61
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Afmetingen gericht en filteren {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Doeldimensie selecteren"
>abstract="Met de doeldimensie kunt u de doelgroep voor de bewerking definiëren: ontvangers, begunstigden van contracten, operator, abonnees en nog veel meer. Standaard is het doel voor e-mails en SMS geselecteerd in de ingebouwde tabel Ontvangers. Voor pushberichten is de standaarddoeldimensie Subscriber-toepassingen."

De het richten dimensie, die ook als doelafbeelding wordt bekend, is het type van gegevens dat een verrichting behandelt. Het bepaalt de doelpopulatie, zoals profielen, contractbegunstigden, exploitanten, of abonnees. De het filtreren dimensie staat u toe om filters op de gerichte bevolking toe te passen door verwante criteria van verwijzingen te voorzien zonder de belangrijkste het richten dimensie te veranderen.

## Doelafmetingen {#targeting}

De doeldimensie van een workflow wordt gedefinieerd door de eerste **[!UICONTROL Build audience]** -activiteit en wordt gebruikt voor alle volgende activiteiten tot het einde van de workflow. Bijvoorbeeld, wanneer het vragen van profielen van het gegevensbestand, bevat de uitgaande overgang gegevens van type &quot;ontvanger&quot;, die aan de volgende activiteit wordt overgebracht.

Schakelaar richtend afmeting in een werkschema gebruikend de afmetingsactiviteit van de a [ Verandering ](../workflows/activities/change-dimension.md). Hierdoor kan de database worden opgevraagd in een specifieke tabel, zoals aankopen of abonnementen, en kan de doeldimensie worden gewijzigd in Ontvangers om leveringen naar de bijbehorende profielen te verzenden.

Wanneer het selecteren van een het richten dimensie (in de werkschemamontages of in activiteiten zoals **bouwt publiek**, **Verzoening**, of **dimensie van de Verandering**), wordt een lijst van algemeen gebruikte schema&#39;s getoond door gebrek. Als u alle beschikbare schema&#39;s wilt weergeven, schakelt u de knop **[!UICONTROL Show all schemas]** in of uit. De optie wordt voor elke gebruiker opgeslagen.

![ Screenshot die het richten afmetingsinterface met &quot;toont alle toegelaten schema&#39;s&quot;knoop toont.](assets/targeting-dimension-show-all.png){zoomable="yes"}

Standaard zijn de profielen voor e-mail- en sms-leveringssjablonen bedoeld. Hun doelafmeting gebruikt de gebieden van de **nms:recipient** lijst. Voor de Duw berichten, is de standaarddoelafmeting **toepassingen van de Abonnee nms:appSubscriptionRcp**, die met de lijst van ontvangers verbonden is.

Gebruik andere ingebouwde doeltoewijzingen in workflows en leveringen, zoals hieronder vermeld:

| Naam | Gebruiken om te leveren aan | Schema |
|-----------------------|-------------------------------------------------------|-------------------------|
| Ontvangers | Profielen/ontvangers (ingebouwde tabel voor ontvangers) | nms:recipient |
| Bezoekers | Bezoekers van wie de profielen via verwijzing werden verzameld (virale marketing voor ex) | mns:visitor |
| Lidmaatschappen | Profielen die zijn geabonneerd op een informatieservice zoals een nieuwsbrief | nms:subscription |
| Abonnementen van bezoekers | Bezoekers die zijn geabonneerd op een informatiedienst | nms:visitorSub |
| Operatoren | Adobe Campaign-operatoren | nms:operator |
| Extern bestand | Aflevering via een bestand dat alle vereiste informatie bevat | Geen gekoppeld schema, geen doel ingevoerd |
| Abonnementstoepassingen | Profielen die zijn geabonneerd op een toepassing | nms:appSubscriptionRcp |

Bovendien, creeer nieuwe doelafbeeldingen die op specifieke behoeften worden gebaseerd. Voer deze bewerking alleen uit vanaf de clientconsole. Leer meer in [ Campagne v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html?lang=nl-NL#new-mapping){target="_blank"}.

## Afmetingen filteren {#filtering}

Met de doeldimensie kunt u de doelgroep van de actie definiëren: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. Met de filterdimensie kunt u filters toepassen op deze populatie door naar verwante gegevens te verwijzen zonder de belangrijkste doeldimensie te wijzigen. U kunt bijvoorbeeld de populatie selecteren op basis van specifieke criteria, zoals contractanten of abonnees van nieuwsbrieven.

Het filtreren de afmetingen zijn beschikbaar slechts in **Bouwt de activiteit van het Publiek**.

Kies de volgende opties om klanten te selecteren die langer dan vijf jaar een levensverzekeringspolis hebben gehouden:

* Het richten dimensie: **Clients**
* Het filtreren afmeting: **de houder van het Contract**.

U kunt de het filtreren voorwaarden binnen **dan bepalen bouwt de activiteit van het Publiek**. Verwijs naar deze [ pagina ](../workflows/activities/build-audience.md).

Tijdens het richten van afmetingsselectie, slechts worden de compatibele het filtreren dimensies getoond in de interface. Deze twee dimensies moeten met elkaar in verband worden gebracht, zodat de inhoud van de filterdimensielijst afhankelijk is van de doeldimensie die in het eerste veld is geselecteerd.
