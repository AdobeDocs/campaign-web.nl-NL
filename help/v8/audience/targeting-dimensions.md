---
title: Doelafmetingen
description: Meer informatie over doelgerichte dimensies vindt u op Adobe Campaign Web
exl-id: b910649a-7300-4f99-8f40-3a8965572ee9
source-git-commit: 395109aeb603ecce53eda89adff70a9ef36fde17
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Doelafmetingen {#targeting-dimensions}

>[!CONTEXTUALHELP]
>id="acw_orchestration_build_audience_dimension"
>title="Doeldimensie selecteren"
>abstract="Met de doeldimensie kunt u de doelgroep van de actie definiëren: ontvangers, begunstigden van contracten, exploitant, abonnees, enz. Standaard is het doel voor e-mails en SMS geselecteerd in de ingebouwde tabel Ontvangers. Voor pushberichten is de standaarddoeldimensie Subscriber-toepassingen."

De gerichte dimensie, ook bekend als. target mapping, is het type gegevens dat een bewerking verwerkt. Hiermee kunt u de doelgroep definiëren: profielen, begunstigden van contracten, exploitanten, abonnees, enz.

## Doeldimensies van workflows {#workflow}

De doeldimensie van een workflow wordt gedefinieerd door de eerste **[!UICONTROL Build audience]** -activiteit en wordt gebruikt voor alle verdere activiteiten tot het einde van de workflow. Bijvoorbeeld, als u een vraag op de profielen van het gegevensbestand uitvoert, zal de uitgaande overgang gegevens van type &quot;ontvanger&quot;bevatten en het zal aan de volgende activiteit worden overgebracht.

Merk op dat u het richten afmeting in een werkschema kunt schakelen gebruikend de afmetingsactiviteit van de a [ Verandering ](../workflows/activities/change-dimension.md). Hierdoor kunt u bijvoorbeeld de database opvragen in een specifieke tabel, zoals aankopen of abonnementen, en vervolgens de dimensie voor het opgeven van doelen wijzigen in Ontvangers om leveringen naar de bijbehorende profielen te verzenden.

Wanneer het selecteren van een het richten afmeting (in de werkschemamontages, of in activiteiten zoals **bouwt publiek**, **Afstemming** of **afmeting van de Verandering**), wordt een selectie van algemeen gebruikte schema&#39;s getoond door gebrek in de lijst. Schakel de knop **[!UICONTROL Show all schemas]** in om alle beschikbare schema&#39;s weer te geven. De optie wordt voor elke gebruiker opgeslagen.

![](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Doelafmetingen {#list}

Standaard zijn de profielen voor e-mail- en sms-leveringssjablonen bedoeld. Hun doelafmeting gebruikt daarom de gebieden van **nms:ontvankelijke** lijst. Voor de Duw berichten, is de standaarddoelafmeting **toepassingen van de Abonnee nms:appSubscriptionRcp**, die met de lijst van ontvangers verbonden is.

U kunt ook andere ingebouwde doeltoewijzingen gebruiken in uw workflows en leveringen die hieronder worden vermeld:

| Naam | Gebruiken voor | Schema |
|---|---|---|
| Ontvangers | Leveren aan profielen/ontvangers (ingebouwde tabel voor ontvangers) | nms:ontvanger |
| Bezoekers | Leveren aan bezoekers van wie de profielen via verwijzing (virale marketing) voor bv zijn verzameld. | mns:bezoeker |
| Lidmaatschappen | Leveren aan profielen die zijn geabonneerd op een informatiedienst zoals een nieuwsbrief | nms:abonnement |
| Abonnementen van bezoekers | Leveren aan bezoekers die zijn geabonneerd op een informatiedienst | nms:bezoekerSub |
| Operatoren | Leveren aan Adobe Campaign-operatoren | nms:operator |
| Extern bestand | Afleveren via een bestand dat alle benodigde informatie voor levering bevat | Geen gekoppeld schema, geen doel ingevoerd |
| Abonnementstoepassingen | Leveren aan profielen die zijn geabonneerd op een toepassing | nms:appSubscriptionRcp |

Bovendien kunt u een nieuwe doelafbeelding maken, afhankelijk van uw behoeften. Deze bewerking wordt alleen vanaf de clientconsole uitgevoerd. Leer meer in [ Campagne v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping) {target="_blank"}.
