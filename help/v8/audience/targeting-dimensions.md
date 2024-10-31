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
>abstract="Met de targetingdimensie kun je de doelgroep van de actie definiëren: ontvangers, contractontvangers, operator, abonnees, enz. Voor e-mails en sms is het doel standaard geselecteerd in de ingebouwde tabel Ontvangers. Voor pushmeldingen is de standaarddoeldimensie Subscriber-toepassingen."

The targeting dimension, ook bekend als. doeltoewijzing is het type gegevens dat door een bewerking wordt verwerkt. Hiermee kunt u de doelgroep definiëren: profielen, begunstigden van contracten, operators, abonnees, enz.

## Targetingdimensies van workflows {#workflow}

De targetingdimensie van een workflow wordt gedefinieerd door de eerste **[!UICONTROL Build audience]** -activiteit en wordt gebruikt voor alle verdere activiteiten tot het einde van de workflow. Als u bijvoorbeeld een query uitvoert op de profielen uit de database, bevat de uitgaande overgang gegevens van het type &#39;ontvanger&#39; en wordt deze overgebracht naar de volgende activiteit.

Merk op dat u het richten afmeting in een werkschema kunt schakelen gebruikend de afmetingsactiviteit van de a [ Verandering ](../workflows/activities/change-dimension.md). Hierdoor kunt u bijvoorbeeld de database opvragen in een specifieke tabel, zoals aankopen of abonnementen, en vervolgens de dimensie voor het opgeven van doelen wijzigen in Ontvangers om leveringen naar de bijbehorende profielen te verzenden.

Wanneer het selecteren van een het richten afmeting (in de werkschemamontages, of in activiteiten zoals **bouwt publiek**, **Afstemming** of **afmeting van de Verandering**), wordt een selectie van algemeen gebruikte schema&#39;s getoond door gebrek in de lijst. Schakel de knop **[!UICONTROL Show all schemas]** in om alle beschikbare schema&#39;s weer te geven. De optie wordt voor elke gebruiker opgeslagen.

![](assets/targeting-dimension-show-all.png){zoomable="yes"}

## Doelafmetingen {#list}

Standaard zijn e-mail- en sms-leveringssjablonen bedoeld voor profielen. Hun doelafmeting gebruikt daarom de gebieden van **nms:ontvankelijke** lijst. Voor Push berichten, is de standaarddoelafmeting **de toepassingen van de Abonnee nms:appSubscriptionRcp**, die met de lijst van ontvangers verbonden is.

U kunt ook andere ingebouwde doeltoewijzingen gebruiken in uw workflows en leveringen die hieronder worden vermeld:

| Naam | Gebruiken voor | Schema |
|---|---|---|
| Ontvangers | Leveren aan profielen/ontvangers (ingebouwde tabel voor ontvangers) | nms:ontvanger |
| Bezoekers | Leveren aan bezoekers van wie de profielen via verwijzing (virale marketing) voor bv zijn verzameld. | mns:bezoeker |
| Lidmaatschappen | Leveren aan profielen die zijn geabonneerd op een informatieservice zoals een nieuwsbrief | nms:abonnement |
| Abonnementen van bezoekers | Leveren aan bezoekers die zijn geabonneerd op een informatiedienst | nms:bezoekerSub |
| Operatoren | Leveren aan Adobe Campaign-operatoren | nms:operator |
| Extern bestand | Via een bestand leveren dat alle informatie bevat die nodig is voor levering | Geen gekoppeld schema, geen doel ingevoerd |
| Abonnementtoepassingen | Leveren aan profielen die zijn geabonneerd op een toepassing | nms:appSubscriptionRcp |

Bovendien kunt u een nieuwe doelafbeelding maken, afhankelijk van uw behoeften. Deze bewerking wordt alleen uitgevoerd vanaf de clientconsole. Leer meer in [ Campagne v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping) {target="_blank"}.
