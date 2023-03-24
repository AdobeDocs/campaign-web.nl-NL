---
audience: end-user
title: Aanbiedingen verzenden
description: Aanbiedingen verzenden
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: 4faf949f061f62accc80b5e11f99318c18f59d2e
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Aanbiedingen verzenden {#offers-content}

![](../assets/do-not-localize/badge.png)

Met Adobe Campaign v8 Web kunt u met uw e-mailaanbiedingen die in de console zijn gemaakt, verzenden via de **[!UICONTROL Interaction]** module. Voor meer informatie over Interactie en hoe te om een aanbiedingencatalogus in de console te beheren, verwijs naar [Campagne v8-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.

De stappen voor het verzenden van voorstellen met een e-mail zijn als volgt:

1. [Configureer de aanbiedingen die u wilt voorstellen](#configure),
1. [De aanbiedingen in de e-mail invoegen](#insert).

## Configureer de aanbiedingen die u wilt voorstellen {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Aanbiedingsinstellingen"
>abstract="Vorm welke aanbiedingen aan de ontvangers zouden moeten worden voorgesteld."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Geavanceerde instellingen voor aanbiedingen"
>abstract="Vorm geavanceerde opties op aanbiedingen."

1. Klik op de knop **[!UICONTROL Offers]** in het scherm E-mailinhoud.

   ![](assets/setup-offers.png)

1. Vorm welke aanbiedingen aan de ontvangers zouden moeten worden voorgesteld. Selecteer eerst de **[!UICONTROL Offer space]** die overeenkomt met uw aanbiedingsomgeving.

   ![](assets/create-content-offers.png)

1. Selecteer een specifieke **[!UICONTROL Offer category]** waarin de aanbiedingen worden gesorteerd.

   Als er geen categorie is opgegeven, houdt de Offertenmotor rekening met alle aanbiedingen in de omgeving, tenzij een **[!UICONTROL Offer theme]** is geselecteerd.

   >[!NOTE]
   >
   >Thema&#39;s zijn sleutelwoorden die stroomopwaarts in de categorieën worden gedefinieerd. Ze fungeren als een filter en u kunt het aantal voorstellen dat moet worden gepresenteerd, verfijnen door ze in een set categorieën te selecteren.

1. Gebruik de **[!UICONTROL Propositions]** veld voor het aantal voorstellen dat u in de e-mail wilt invoegen.

1. Selecteer **[!UICONTROL Exclude non-eligible recipients]** indien nodig.

   Met deze optie kunt u de uitsluiting activeren of deactiveren van ontvangers voor wie onvoldoende geschikte voorstellen zijn.

   * Als de optie is ingeschakeld, worden ontvangers die onvoldoende voorstellen hebben, uitgesloten van de levering.
   * Als de optie is uitgeschakeld, worden deze ontvangers niet uitgesloten, maar kunnen ze niet het gewenste aantal voorstellen hebben.

1. Selecteer indien nodig de **[!UICONTROL Hide everything if no offer is selected]** optie.

   Met deze optie kunt u kiezen hoe het bericht wordt verwerkt als een van de voorstellen niet bestaat.

   * Als de optie is ingeschakeld, wordt de representatie van het ontbrekende voorstel niet weergegeven en wordt er geen inhoud weergegeven in het bericht voor dit voorstel.
   * Als de optie is uitgeschakeld, wordt het bericht zelf geannuleerd tijdens het verzenden en kunnen ontvangers geen berichten meer ontvangen.

Nadat u de voorstellen hebt geconfigureerd voor voorstellen in uw e-mail, kunt u deze invoegen in de e-mail met de Expressieeditor. [Leer hoe u aanbiedingen in de e-mail invoegt](#insert)

## Aanbiedingen in de e-mail invoegen {#insert}

Aanbiedingen kunnen in de e-mail worden toegevoegd met de Expressieeditor. Zij kunnen worden ingevoegd:

* In de onderwerpregel van de e-mail:
* In de e-mailhoofdtekst door personalisatie toe te staan in een inhoudscomponent. [Leer hoe u inhoudscomponenten kunt toevoegen](content-components.md)

>[!NOTE]
>
>Voordat u een voorstel invoegt, moet u controleren of u [geconfigureerd voor voorstellen via e-mail](#configure).

Voer de volgende stappen uit om een aanbieding in te voegen met de Expressieeditor:

1. Open de Expressieeditor en selecteer vervolgens de **[!UICONTROL Propositions]** -menu.

   De beschikbare voorstellingen worden in de lijst weergegeven. Het aantal voorstellen wordt bepaald wanneer het vormen van de aanbiedingen om voor te stellen.

   ![](assets/offer-insertion.png)

1. Voeg de voorstellen in het e-mailonderwerp of de tekst toe met behulp van de verpersoonlijkingsgebieden, renderfuncties of kenmerken die beschikbaar zijn voor elk voorstel.

   ![](assets/offer-inserted.png)
