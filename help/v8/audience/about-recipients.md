---
title: Werken met ontvangers en publiek
description: Leer hoe te met ontvangers het Web van de Campagne werken
badge: label="Beta"
exl-id: 71a1ec92-cd79-4654-9ae3-9a92a01c6279
source-git-commit: bc1b4186b5869d104c6b14e09160f28bf3e28f95
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 1%

---

# Werken met ontvangers en publiek {#about-recipients}

In Adobe Campaign is de doelpopulatie van een levering een publiek. Een publiek is een groep personen die vergelijkbare gedragingen en/of kenmerken delen. Deze verzameling personen kan worden gegenereerd, geselecteerd of geladen [zoals hieronder beschreven](#audiences). In de meeste gevallen bestaat het publiek uit profielen die worden opgeslagen als [ontvangers](#recipients) in Adobe Campaign. U kunt ook met andere doeltoewijzingen werken door de dimensie te wijzigen, zoals uitgelegd [in deze sectie](#targeting-dimensions).

## Wat zijn ontvangers? {#recipients}


>[!CONTEXTUALHELP]
>id="acw_homepage_rn4"
>title="Ontvangers"
>abstract="Creeer nieuwe ontvangers, en controleer hen door krachtige rapporten en hulpmiddelen. Open het profiel van de ontvanger, gebruik de filteropties om door de lijst met ontvangers te bladeren, hun kenmerken te bewerken en bij te werken."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/whats-new.html" text="Zie opmerkingen bij releases"


>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Profielen"
>abstract="Een profiel is een individu dat berichten ontvangt die door Adobe Campaign worden verzonden. In Adobe Campaign zijn ontvangers de standaardprofielen voor het verzenden van leveringen (e-mails, SMS). In deze lijst kunt u het profiel van de ontvanger weergeven op basis van uw machtigingen. Gebruik de filteropties om door deze lijst te bladeren. U kunt een kleine set kenmerken van de ontvanger bewerken en bijwerken."

Een ontvanger is een profiel dat is bedoeld voor het ontvangen van berichten die door Adobe Campaign worden verzonden. In Adobe Campaign zijn ontvangers de standaardprofielen voor het verzenden van leveringen (e-mails, sms’en, enzovoort). De ontvangende gegevens die in het gegevensbestand worden opgeslagen laten u toe tot publiek dat om het even welke bepaalde levering zal ontvangen, en om verpersoonlijkingsgegevens in uw leveringsinhoud toe te voegen. Andere typen profielen worden opgeslagen in de database. Ze zijn ontworpen voor verschillende toepassingen. Zaadprofielen worden bijvoorbeeld gemaakt om uw leveringen te testen voordat ze naar het uiteindelijke publiek worden verzonden.

Ontvangers kunnen alleen worden toegevoegd vanuit de Campagne-clientconsole. Ze zijn echter zichtbaar in het campagneweb, vanaf het **Ontvangers** de binnenkomst van de linkernavigatielijn. U kunt de kenmerken van de ontvanger ook vanuit dat scherm bewerken.

Als u de gegevens van de ontvanger wilt bewerken, klikt u op de drie stippen naast de naam en kiest u **Bewerken...**.

![Een ontvangend profiel bewerken](assets/recipient-edit.png)

U kunt een beperkte set kenmerken bijwerken, namelijk voornaam, achternaam, e-mail en telefoonnummer.

![Een ontvangend profiel bijwerken](assets/recipient-update.png)

>[!NOTE]
>
>Dit beperkte formulier voor het bewerken van profielen is alleen beschikbaar voor het testen van bètaprogramma&#39;s. Het zal in de toekomstige versie worden verbeterd. Hiermee kan de gebruiker snel een e-mailadres en een telefoonnummer aan een profiel toevoegen, zodat hij/zij de e-mail- en sms-kanalen kan testen en de verzonden berichten kan ontvangen.

U kunt de ontvangers filteren met het zoekveld, vanaf het tabblad **Filters tonen** knop.

U kunt ontvangers ook benaderen via de **Verkenner** mappen en submappen weergeven, maken en doorbladeren en maken, en de bijbehorende machtigingen controleren.

![Lijst met ontvangers in de weergave Explorer](assets/recipients-from-explorer.png)

>[!NOTE]
>
>Afhankelijk van uw machtigingen hebt u mogelijk geen toegang tot de volledige lijst met ontvangers die in de database zijn opgeslagen. Meer informatie over machtigingen in [deze sectie](../get-started/permissions.md).

Bovendien kunt u het abonnement op en het abonnement van uw ontvangers op services zoals nieuwsbrieven beheren. Leer hoe u met abonnementsservices werkt in [deze pagina](manage-services.md)

U kunt workflows maken om te dedupliceren, te verrijken, profielen te combineren en een publiek te maken. Meer informatie in [deze sectie](../workflows/gs-workflows.md).

## Wat zijn de doelgroepen? {#audiences}

Het publiek is het belangrijkste doel van uw levering: de ontvangers die de berichten ontvangen. Het type publiek hangt van de doelafbeelding af die in het leveringsmalplaatje wordt bepaald. Meer informatie over leveringssjablonen vindt u in [deze pagina](../msg/delivery-template.md).

Om de populatie van een publiek te bepalen, kunt u:

* [Nieuw publiek maken](create-audience.md) van de **[!UICONTROL Audiences]** menu,
* [Bestaande doelgroep selecteren](add-audience.md) gemaakt als een lijst in de clientconsole of afkomstig uit Adobe Experience Platform;
* [Een nieuw publiek maken](segment-builder.md) met de regelbouwer door filtercriteria te definiëren en te combineren,
* [Een publiek uit een extern bestand gebruiken](file-audience.md). Deze optie is alleen beschikbaar voor zelfstandige e-mailleveringen en kan niet worden gebruikt in campagneleveringen.

Wanneer u zich richt op een publiek, kunt u ook definiëren **controlegroepen** om te voorkomen dat berichten naar een deel van uw publiek worden verzonden en om de impact van uw campagnes te meten. [Leer hoe u een controlegroep instelt](control-group.md)

>[!NOTE]
>
>Wanneer het verzenden van berichten in de context van een campagnewerkschema, wordt het publiek bepaald in een specifiek **publiek opbouwen** workflowactiviteit. In deze context kunt u geen publiek uit een bestand laden voor e-maillevering en wordt het publiek alleen gedefinieerd in deze toegewijde activiteit. Leer hoe u het publiek van uw levering kunt definiëren in een campagneworkflow in [deze sectie](../workflows/activities/build-audience.md)

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
