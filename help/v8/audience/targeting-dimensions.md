---
title: Doelafmetingen
description: Meer informatie over doelgerichte dimensies vindt u op Adobe Campaign Web
badge: label="Beperkte beschikbaarheid"
source-git-commit: 9fd523a04ac4bfb2d760202b1f7e9bd9e7097dfe
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 1%

---

# Doelafmetingen {#targeting-dimensions}

De gerichte dimensie, ook bekend als. target mapping, is het type gegevens dat een bewerking verwerkt. Hiermee kunt u de doelgroep definiëren: profielen, begunstigden van contracten, exploitanten, abonnees, enz.

De doeldimensie van een workflow wordt gedefinieerd door de eerste **[!UICONTROL Build audience]** en wordt gebruikt voor alle verdere activiteiten tot het einde van de werkstroom. Bijvoorbeeld, als u een vraag op de profielen van het gegevensbestand uitvoert, zal de uitgaande overgang gegevens van type &quot;ontvanger&quot;bevatten en het zal aan de volgende activiteit worden overgebracht.

Let op: u kunt de doeldimensie in een workflow wijzigen met een [Dimensieactiviteit wijzigen](../workflows/activities/change-dimension.md). Hierdoor kunt u bijvoorbeeld de database opvragen in een specifieke tabel, zoals aankopen of abonnementen, en vervolgens de dimensie voor het opgeven van doelen wijzigen in Ontvangers om leveringen naar de bijbehorende profielen te verzenden.

Standaard zijn de profielen voor e-mail- en sms-leveringssjablonen bedoeld. Hun doeldimensie gebruikt daarom de gebieden van **nms:ontvanger** tabel. Voor pushberichten is de standaarddoeldimensie: **Toepassingen voor abonnees nms:appSubscriptionRcp**, die is gekoppeld aan de tabel met ontvangers.

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
