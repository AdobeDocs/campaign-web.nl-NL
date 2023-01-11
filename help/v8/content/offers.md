---
audience: end-user
title: Aanbiedingen verzenden
description: Aanbiedingen verzenden
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: db197206700d3d3973d9cad459aa2f56ab76f213
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Aanbiedingen verzenden {#offers-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Aanbiedingsinstellingen"
>abstract="TBC"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Geavanceerde instellingen voor aanbiedingen"
>abstract="TBC"

>[!NOTE]
>
>Deze documentatie is in opbouw en wordt regelmatig bijgewerkt. De definitieve versie van deze inhoud zal in Januari 2023 klaar zijn.

Met Adobe Campaign v8 Web kunt u met uw e-mailaanbiedingen die in de console zijn gemaakt, verzenden via de **[!UICONTROL Interaction]** module. Voor meer informatie over Interactie en hoe te om een aanbiedingencatalogus in de console te beheren, verwijs naar [Campagne V8-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html)

De stappen voor het verzenden van voorstellen met een e-mail zijn als volgt:

1. [Configureer de aanbiedingen die u wilt voorstellen](#configure),
1. [De aanbiedingen in de e-mail invoegen](#insert).

## Configureer de aanbiedingen die u wilt voorstellen {#configure}

Klik op de knop **[!UICONTROL Offers]** van het e-mailinhoudsopgavescherm en configureer de aanbiedingen die u wilt voorstellen.

![](assets/create-content-offers.png)

1. Selecteer **[!UICONTROL Offer space]** die overeenkomt met uw aanbiedingsomgeving.

1. Selecteer een specifieke **[!UICONTROL Offer category]** waarin de aanbiedingen worden gesorteerd.

   Als er geen categorie is opgegeven, zal de motor van de aanbieding rekening houden met alle aanbiedingen in de omgeving, tenzij een **[!UICONTROL Offer theme]** is geselecteerd.

   >[!NOTE]
   >
   >Thema&#39;s zijn sleutelwoorden die stroomopwaarts in de categorieën worden gedefinieerd. Ze fungeren als een filter en u kunt het aantal voorstellen dat moet worden gepresenteerd, verfijnen door ze in een set categorieën te selecteren.

1. Gebruik de **[!UICONTROL Propositions]** veld voor het aantal voorstellen dat u in de e-mail wilt invoegen.

1. Selecteer **[!UICONTROL Exclude non-eligible recipients]** indien nodig.

   Met deze optie kunt u de uitsluiting activeren of deactiveren van ontvangers voor wie onvoldoende geschikte voorstellen zijn.

   * Als de optie wordt toegelaten, zullen de ontvangers die niet genoeg voorstellen hebben van de levering worden uitgesloten.
   * Als de optie is uitgeschakeld, worden deze ontvangers niet uitgesloten, maar hebben ze niet het gewenste aantal voorstellen.

1. Selecteer indien nodig de **[!UICONTROL Hide everything if no offer is selected]** optie.

   Met deze optie kunt u kiezen hoe het bericht wordt verwerkt als een van de voorstellen niet bestaat.

   * Als de optie is ingeschakeld, wordt de representatie van het ontbrekende voorstel niet weergegeven en wordt er geen inhoud weergegeven in het bericht voor dit voorstel.
   * Als de optie is uitgeschakeld, wordt het bericht zelf geannuleerd tijdens het verzenden en ontvangen de ontvangers geen berichten meer.

Nadat u de voorstellen hebt geconfigureerd voor voorstellen in uw e-mail, kunt u deze invoegen in de e-mail met de Expressieeditor. [Leer hoe u aanbiedingen in de e-mail invoegt](#insert)

## Aanbiedingen in de e-mail invoegen {#insert}

Aanbiedingen worden aan een e-mail toegevoegd met de Expressieeditor. Zij kunnen worden ingevoegd:

* in de onderwerpregel van de e-mail,
* in de hoofdtekst van de e-mail door personalisatie toe te staan in om het even welke inhoudscomponent. [Leer hoe u inhoudscomponenten kunt toevoegen](content-components.md)

>[!NOTE]
>
>Voordat u een voorstel invoegt, moet u controleren of u [geconfigureerd voor voorstellen via e-mail](#configure).

Voer de volgende stappen uit om een aanbieding in te voegen met de Expressieeditor:

1. Open de Expressieeditor en selecteer vervolgens de **[!UICONTROL Propositions]** -menu.

   De beschikbare voorstellingen worden in de lijst weergegeven. Het aantal voorstellen wordt bepaald wanneer het vormen van de aanbiedingen om voor te stellen.

   ![](assets/offer-insertion.png)

1. Voeg de voorstellen in het e-mailonderwerp of de tekst toe met behulp van de verpersoonlijkingsgebieden, renderfuncties of kenmerken die beschikbaar zijn voor elk voorstel.

   ![](assets/offer-inserted.png)
