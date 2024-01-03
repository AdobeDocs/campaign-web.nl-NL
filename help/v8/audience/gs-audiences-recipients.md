---
title: Werken met ontvangers en publiek
description: Leer hoe u met ontvangers en publiek kunt werken in Campagne Web
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: 5183dd0045c7f13e79f65eca5b31dfd4cde2f31d
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Werken met ontvangers en publiek {#about-recipients}

## Ontvangers en publiek {#about}

In Adobe Campaign is de doelpopulatie van een levering een publiek. Een publiek is een groep personen die vergelijkbare gedragingen en/of kenmerken delen. Deze verzameling personen kan worden gegenereerd, geselecteerd of geladen [zoals hieronder beschreven](#audiences).

In de meeste gevallen bestaat het publiek uit profielen die worden opgeslagen als [ontvangers](#recipients) in Adobe Campaign. U kunt ook met andere doeltoewijzingen werken door de dimensie te wijzigen, zoals uitgelegd [in deze sectie](#targeting-dimensions).

## Doelafmetingen {#targeting-dimensions}

De gerichte dimensie, ook bekend als. target mapping, is het type gegevens dat een bewerking verwerkt. Hiermee kunt u de doelgroep definiëren: ontvangers, begunstigden van contracten, exploitanten, abonnees, enz.

De doeldimensie van een workflow wordt gedefinieerd door de eerste **[!UICONTROL Build audience]** en wordt gebruikt voor alle verdere activiteiten tot het einde van de werkstroom. Bijvoorbeeld, als u een vraag op de ontvangers van het gegevensbestand uitvoert, zal de uitgaande overgang gegevens van type ontvanger bevatten en het zal aan de volgende activiteit worden overgebracht.

Let op: u kunt de doeldimensie in een workflow wijzigen met een [Dimensieactiviteit wijzigen](../workflows/activities/change-dimension.md). Dit staat u toe, bijvoorbeeld, om het gegevensbestand op een specifieke lijst zoals aankopen of abonnementen te vragen, en dan de het richten dimensie aan Ontvangers te veranderen om leveringen naar de overeenkomstige ontvangers te verzenden.

Standaard wordt in sjablonen voor e-mail- en sms-verzending de doelstelling **[!UICONTROL Recipients]**. Hun doeldimensie gebruikt daarom de gebieden van **nms:ontvanger** tabel. Voor pushberichten is de standaarddoeldimensie: **Toepassingen voor abonnees nms:appSubscriptionRcp**, die is gekoppeld aan de tabel met ontvangers.

U kunt ook andere ingebouwde doeltoewijzingen gebruiken in uw workflows en leveringen die hieronder worden vermeld:

| Naam | Gebruiken voor | Schema |
|---|---|---|
| Ontvangers | Leveren aan ontvangers (ingebouwde ontvankelijke lijst) | nms:ontvanger |
| Bezoekers | Leveren aan bezoekers van wie de profielen via verwijzing (virale marketing) voor bv zijn verzameld. | mns:bezoeker |
| Lidmaatschappen | Leveren aan ontvangers die zijn geabonneerd op een informatiedienst zoals een nieuwsbrief | nms:abonnement |
| Abonnementen van bezoekers | Leveren aan bezoekers die zijn geabonneerd op een informatiedienst | nms:bezoekerSub |
| Operatoren | Leveren aan Adobe Campaign-operatoren | nms:operator |
| Extern bestand | Afleveren via een bestand dat alle benodigde informatie voor levering bevat | Geen gekoppeld schema, geen doel ingevoerd |
| Abonnementstoepassingen | Leveren aan ontvangers die zijn geabonneerd op een toepassing | nms:appSubscriptionRcp |

Bovendien kunt u een nieuwe doelafbeelding maken, afhankelijk van uw behoeften. Dit wordt uitgevoerd vanaf de clientconsole. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html#new-mapping){target="_blank"}.
