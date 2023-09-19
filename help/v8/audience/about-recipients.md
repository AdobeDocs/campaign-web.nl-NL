---
title: Werken met ontvangers en publiek
description: Leer hoe te met ontvangers het Web van de Campagne werken
badge: label="Beta"
source-git-commit: 269cbb51f070b0f9f771691497ffa07bb94e2d49
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 2%

---


# Werken met ontvangers en publiek {#about-recipients}

## Ontvangers {#recipients}

>[!CONTEXTUALHELP]
>id="acw_recipients_list"
>title="Ontvangers"
>abstract="Een ontvanger is een profiel dat is bedoeld voor het ontvangen van berichten die door Adobe Campaign worden verzonden. In Adobe Campaign zijn ontvangers de standaardprofielen voor het verzenden van leveringen (e-mails, SMS). In deze lijst kunt u het profiel van de ontvanger weergeven op basis van uw machtigingen. Gebruik de filteropties om door deze lijst te bladeren. U kunt een kleine set kenmerken van de ontvanger bewerken en bijwerken."

Een ontvanger is een profiel dat is bedoeld voor het ontvangen van berichten die door Adobe Campaign worden verzonden. In Adobe Campaign zijn ontvangers de standaardprofielen voor het verzenden van leveringen (e-mails, sms’en, enzovoort). De ontvangende gegevens die in het gegevensbestand worden opgeslagen laten u toe tot publiek dat om het even welke bepaalde levering zal ontvangen, en om verpersoonlijkingsgegevens in uw leveringsinhoud toe te voegen. Andere typen profielen worden opgeslagen in de database. Ze zijn ontworpen voor verschillende toepassingen. Zaadprofielen worden bijvoorbeeld gemaakt om uw leveringen te testen voordat ze naar het uiteindelijke publiek worden verzonden.

Ontvangers kunnen alleen worden toegevoegd vanuit de Campagne-clientconsole. Ze zijn echter zichtbaar in het campagneweb, vanaf het **Ontvangers** de binnenkomst van de linkernavigatielijn.

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

Bovendien kunt u het abonnement op en het abonnement van uw ontvangers op services zoals nieuwsbrieven beheren. [Leer hoe u met abonnementsservices werkt](create-service.md)

## Doelgroepen {#audiences}

Het publiek is het belangrijkste doel van uw levering: de ontvangers die de berichten ontvangen. Het type publiek hangt van de doelafbeelding af die in het leveringsmalplaatje wordt bepaald. [Meer weten over een leveringssjabloon](../msg/delivery-template.md).

Om de populatie van een publiek te bepalen, kunt u:

* [Nieuw publiek maken](create-audience.md) van de **[!UICONTROL Audiences]** menu,
* [Bestaande doelgroep selecteren](add-audience.md) gemaakt als een lijst in de clientconsole,
* [Een Adobe Experience Platform-publiek selecteren](aep-audience.md),
* [Een nieuw publiek maken](segment-builder.md) met de regelbouwer door filtercriteria te definiëren en te combineren,
* [Een publiek uit een extern bestand gebruiken](file-audience.md). Deze optie is alleen beschikbaar voor zelfstandige e-mailleveringen en kan niet worden gebruikt in campagneleveringen.

Wanneer u zich richt op een publiek, kunt u ook definiëren **controlegroepen** om te voorkomen dat berichten naar een deel van uw publiek worden verzonden en om de impact van uw campagnes te meten. [Leer hoe u een controlegroep instelt](control-group.md)

>[!NOTE]
>
>Wanneer het verzenden van berichten in de context van een campagnewerkschema, wordt het publiek bepaald in een specifiek **publiek opbouwen** workflowactiviteit. In deze context kunt u geen publiek uit een bestand laden voor e-maillevering en wordt het publiek alleen gedefinieerd in deze toegewijde activiteit. Leer hoe u het publiek van uw levering kunt definiëren in een campagneworkflow [in deze sectie](../workflows/activities/build-audience.md)
