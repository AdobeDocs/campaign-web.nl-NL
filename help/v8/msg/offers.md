---
audience: end-user
title: Aanbiedingen toevoegen aan uw berichten
description: Meer informatie over het toevoegen en verzenden van aanbiedingen
exl-id: abc3c36d-d475-4474-b4fe-685cf23ff89d
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---


# Aanbiedingen toevoegen aan uw berichten {#offers-content}

In de gebruikersinterface van Adobe Campaign Web kunt u aanbiedingen toevoegen aan uw leveringen. Deze aanbiedingen zijn beschikbaar op **Aanbiedingen** in het linkermenu hebt u toegang tot de lijst met aanbiedingen. Al deze aanbiedingen zijn read-only, en moeten in de de cliëntconsole van de Campagne worden gecreeerd, gebruikend **[!UICONTROL Interaction]** -module. Voor meer informatie over Interactie en hoe te om een aanbiedingscatalogus in de console te beheren, verwijs naar [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction.html){target="_blank"}.


De stappen voor het verzenden van voorstellen met een levering zijn als volgt:

1. [Configureer de aanbiedingen die u wilt voorstellen](#configure)
1. [Voeg de voorstellen in de levering in](#insert)

## Configureer de aanbiedingen die u wilt voorstellen {#configure}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_settings"
>title="Definieer de parameters voor aanbiedingen"
>abstract="Vorm welke aanbiedingen aan de ontvangers zouden moeten worden voorgesteld door een aanbiedingsruimte, naar keuze een categorie en een thema te bepalen, en specificeer het aantal aanbiedingen u in de levering wilt opnemen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_offers_advanced_settings"
>title="Geavanceerde instellingen voor aanbiedingen instellen"
>abstract="U kunt de uitsluiting inschakelen van ontvangers voor wie er onvoldoende geschikte aanbiedingen zijn en u kunt kiezen hoe het bericht wordt verwerkt als een van de voorstellen niet bestaat."

Met Adobe Campaign kunt u tijdens een interactie op een bepaald contact in real time reageren door een of meerdere specifieke aanbiedingen voor te stellen. Deze aanbiedingen kunnen eenvoudige communicatie berichten, speciale aanbiedingen op één of verscheidene producten, of de dienst zijn.

Volg onderstaande stappen om de voorstellen te selecteren die u aan uw levering wilt toevoegen.

1. Klik op de knop **[!UICONTROL Set up offers]** van het scherm voor de editie van de inhoud van de levering.

   ![](assets/offer-setup.png){zoomable=&quot;yes&quot;}

1. Vorm welke aanbiedingen aan de ontvangers zouden moeten worden voorgesteld.

   Selecteer eerst de optie **[!UICONTROL Offer space]** die overeenkomt met uw aanbiedingsomgeving. Leer hoe u een aanbiedingsruimte maakt in het dialoogvenster [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-settings/interaction-offer-spaces.html){target="_blank"}.

   ![](assets/offer-create-content.png){zoomable=&quot;yes&quot;}

1. Als u de keuze van de motor met aanbiedingen wilt verfijnen, selecteert u een specifieke **[!UICONTROL Offer category]** waarin de aanbiedingen worden gesorteerd.

   Wanneer u een map selecteert, worden alle submappen automatisch opgenomen en kunnen deze niet worden verwijderd. Let erop dat de [!DNL Campaign] interface weerspiegelt dit gedrag niet.

   >[!NOTE]
   >
   >Als er geen categorie is opgegeven, houdt de Offertenmotor rekening met alle aanbiedingen in de omgeving, tenzij een **[!UICONTROL Offer theme]** is geselecteerd.

1. (optioneel) Voer een thema in om categorieën te filteren. Thema&#39;s zijn trefwoorden die stroomopwaarts in de categorieën zijn gedefinieerd. Ze fungeren als een filter en u kunt het aantal voorstellen dat moet worden gepresenteerd, verfijnen door ze in een set categorieën te selecteren.

1. Gebruik de **[!UICONTROL Propositions]** veld om het aantal voorstellen op te geven dat u in de levering wilt invoegen.

1. Selecteer de **[!UICONTROL Exclude non-eligible recipients]** indien nodig.

   Met deze optie kunt u de uitsluiting activeren of deactiveren van ontvangers voor wie onvoldoende geschikte aanbiedingen zijn:

   * Als de optie is ingeschakeld, worden ontvangers die onvoldoende voorstellen hebben, uitgesloten van de levering.
   * Als de optie is uitgeschakeld, worden deze ontvangers niet uitgesloten, maar kunnen ze niet het gewenste aantal voorstellen hebben.

1. Selecteer indien nodig de **[!UICONTROL Hide everything if no offer is selected]** -optie.

   Met deze optie kunt u kiezen hoe het bericht wordt verwerkt als een van de voorstellen niet bestaat:

   * Als de optie is ingeschakeld, wordt de representatie van het ontbrekende voorstel niet weergegeven en wordt er geen inhoud weergegeven in het bericht voor dit voorstel.
   * Als de optie is uitgeschakeld, wordt het bericht zelf geannuleerd tijdens het verzenden en kunnen ontvangers geen berichten meer ontvangen.

Zodra u de voorstellen hebt gevormd om in uw levering voor te stellen, kunt u hen in de leveringsinhoud opnemen.

## Aanbiedingen in de levering invoegen {#insert}

Aanbiedingen kunnen in de levering worden toegevoegd met de [expressie-editor](../personalization/gs-personalization.md#access). Zij kunnen in de onderwerpregel of in het leveringsorgaan worden ingevoegd.

>[!CAUTION]
>
>Voordat u een voorstel in een levering invoegt, moet u ervoor zorgen dat u [geconfigureerd voor voorstellen met die levering](#configure).

Volg onderstaande stappen om een aanbieding in te voegen met de expressieeditor.

1. Open de onderwerpregel of de inhoud van een levering.

1. Plaats de cursor van de muis op de plaats waar u de aanbieding wilt invoegen en open de expressieeditor met behulp van het verpersoonlijkingspictogram.

   ![](assets/offer-insert-perso-icon.png){zoomable=&quot;yes&quot;}

1. Selecteer de **[!UICONTROL Propositions]** -menu. De beschikbare voorstellingen worden in de lijst weergegeven.

   >[!NOTE]
   >
   >Het aantal voorstellen wordt gedefinieerd wanneer [aanbiedingen instellen](#configure) voor de huidige levering.

1. Definieer elke voorstelling met behulp van de personalisatievelden, renderfuncties of beschikbare kenmerken.

   ![](assets/offer-inserted.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Het aantal beschikbare voorstellen hangt van de manier af de motorvraag wordt gevormd en hun orde hangt van de prioriteit van aanbiedingen af. Meer informatie in het dialoogvenster [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/offers/interaction-best-practices.html){target="_blank"}.

1. Sla uw wijzigingen op.

1. Voltooi de inhoud, test en verzend uw levering. [Meer informatie](gs-messages.md)

Wanneer een ontvanger de levering ontvangt, wordt de juiste aanbieding getoond aan dat specifieke profiel.
