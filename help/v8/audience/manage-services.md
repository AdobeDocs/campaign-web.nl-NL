---
audience: end-user
title: Werken met abonnementsservices
description: Meer informatie over het openen, maken en beheren van abonnementsservices op Adobe Campaign Web
exl-id: 95b2f2f9-5478-4fdb-9201-9c5bcb7f60b2
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 1%

---

# Abonnementsservices maken en beheren {#manage-services}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list"
>title="Services maken en beheren"
>abstract="Gebruik Adobe Campaign om uw services, zoals nieuwsbrieven, te maken en te controleren en om de abonnementen op of het afmelden van deze services te controleren. Abonnementen gelden alleen voor verzending via e-mail en SMS."

Gebruik Adobe Campaign Web om uw services, zoals nieuwsbrieven, te beheren en te maken en om de abonnementen op of het afmelden van deze services te controleren.

Verschillende diensten kunnen parallel worden gedefinieerd, bijvoorbeeld: nieuwsbrieven voor specifieke productcategorieën, thema&#39;s, of gebieden van een website, abonnementen op verschillende typen waarschuwingsberichten, en real-time berichten.

>[!NOTE]
>
>Abonnementen gelden alleen voor verzending via e-mail en SMS.

## Toegang tot abonnementsservices {#access-services}

Volg onderstaande stappen om abonnementsservices die beschikbaar zijn voor uw platform te openen.

1. Blader onder **[!UICONTROL Customer management]** naar het menu **[!UICONTROL Subscription services]** op de linkernavigatieregel.

   ![ Schermafbeelding die het menu van de Diensten van het Abonnement op de linkernavigatiespoor onder het beheer van de Klant toont ](assets/service-list.png){zoomable="yes"}

1. De lijst met alle bestaande abonnementsservices wordt weergegeven. U kunt de diensten zoeken en filtreren door kanaal, omslag, of regels toevoegen gebruikend [ vraagmodeler ](../query/query-modeler-overview.md).

   ![ Schermschot die de lijst van de abonnementendiensten met filters voor kanaal, omslag, en regels tonen ](assets/service-filters.png){zoomable="yes"}

1. Als u een bestaande service wilt bewerken, klikt u op de naam van de service.

1. Schrap of dupliceer om het even welke dienst gebruikend het drie puntenpictogram naast de de dienstnaam.<!--so all subscribers are unsubscribed - need to mention?-->

## Uw eerste abonnementenservice maken {#create-service}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_properties"
>title="De service-eigenschappen definiëren"
>abstract="Voer het label van de abonnementsservice in en definieer aanvullende opties, zoals een geldigheidsperiode voor de service."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_list_confirm"
>title="Selecteer een bevestigingsbericht"
>abstract="Wanneer een gebruiker zich abonneert op of zich niet abonneert op een service, kunt u een bevestigingsbericht verzenden. Selecteer de sjablonen die u voor dat bericht wilt gebruiken."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Standaardlandingspagina"
>abstract="Selecteer de standaardbestemmingspagina&#39;s verbonden aan deze dienst."

Voer de onderstaande stappen uit om een abonnementenservice te maken.

1. Selecteer de knop **[!UICONTROL Create subscription service]**.

   ![ Schermafbeelding die de Create knoop van de abonnementendienst toont ](assets/service-create-button.png){zoomable="yes"}

1. Selecteer een kanaal: **[!UICONTROL Email]** of **[!UICONTROL SMS]** .

1. Voer in de service-eigenschappen een label in en definieer **[!UICONTROL Additional options]** naar wens.

   ![ Schermafbeelding die de sectie van de de diensteigenschappen met etiket en extra opties tonen ](assets/service-create-properties.png){zoomable="yes"}

1. Standaard worden services opgeslagen in de map **[!UICONTROL Services and Subscriptions]** . U kunt dit wijzigen door naar de gewenste locatie te bladeren. [ Leer hoe te met omslagen ](../get-started/permissions.md#folders) te werken

1. Abonnementen zijn standaard onbeperkt.

   Schakel de optie **[!UICONTROL Unlimited validity period]** uit om een geldigheidsduur voor de service te definiëren. Na afloop van de geldigheidsperiode:
   * Geen enkel profiel kan zich meer abonneren op deze service.
   * Alle abonnees op deze service worden automatisch afgemeld.

   ![ Schermafbeelding die de montages van de geldigheidsperiode voor de dienst van het abonnement toont ](assets/service-create-validity-period.png){zoomable="yes"}

1. Wanneer een gebruiker zich abonneert op of zich niet abonneert op een service, kunt u een bevestigingsbericht verzenden. Selecteer de sjablonen die u voor dat bericht wilt gebruiken, afhankelijk van uw gebruiksscenario. Deze sjablonen moeten worden geconfigureerd met de doeltoewijzing **[!UICONTROL Subscriptions]** . [Meer informatie](#create-confirmation-message)

   ![ Screenshot die de selectie van het bevestigingsbericht toont ](assets/service-create-confirmation-msg.png){zoomable="yes"}

1. Klik op **[!UICONTROL Save and review]**. De nieuwe service wordt toegevoegd aan de lijst **[!UICONTROL Subscription services]** .

1. Selecteer de standaardbestemmingspagina&#39;s voor abonnementen en abonnementen die aan deze service zijn gekoppeld.

   >[!AVAILABILITY]
   >
   >Dit vermogen is in Beperkte Beschikbaarheid (LA). Het is beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kan niet op een ander milieu worden opgesteld.

   ![ Schermafbeelding die de standaard het landen pagina montages voor de abonnementendienst tonen ](assets/service-create-default-lp.png){zoomable="yes"}

   Zodra gedaan, wanneer [ het opnemen van een verbinding ](../email/message-tracking.md) in e-mail, uitgezocht **[!UICONTROL Subscription link]** of **[!UICONTROL Unsubscription link]**. Als gebruikers op die koppeling klikken, worden ze doorgestuurd naar de bestemmingspagina voor abonnementen of abonnementen waarnaar in de service wordt verwezen. <!--After submitting the form, they will be subscribed to / unsubscribed from the service.-->

   ![ Screenshot die de abonnement en unsubscription verbindingsmontages ](assets/service-create-default-lp-link.png){zoomable="yes"} tonen

1. Sla uw wijzigingen op en controleer deze.

U kunt nu het volgende:

* Voeg handmatig abonnees aan deze service toe en trek profielen af. [Meer informatie](../audience/manage-subscribers.md)

* Uw klanten uitnodigen om zich op deze service in te schrijven via een openingspagina. [Meer informatie](../landing-pages/lp-use-cases.md#lp-subscription)

* Verzend berichten naar de abonnees van deze dienst. [ leer hoe ](../msg/send-to-subscribers.md)

## Een bevestigingsbericht maken {#create-confirmation-message}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_delivery_template"
>title="De leveringssjabloon voor abonnementen selecteren"
>abstract="Als u bevestigingsberichten wilt verzenden aan gebruikers die zich op uw service abonneren, moet u een specifieke leveringssjabloon selecteren op basis van de doeltoewijzing van **[!UICONTROL Subscriptions]** , zonder een gedefinieerd doel."

>[!CONTEXTUALHELP]
>id="acw_unsubscriptions_delivery_template"
>title="Selecteer de leveringssjabloon voor abonnementen"
>abstract="Als u bevestigingsberichten wilt verzenden aan gebruikers die zich niet meer abonneren op uw service, moet u een specifieke leveringssjabloon selecteren op basis van de doeltoewijzing van **[!UICONTROL Subscriptions]** , zonder een gedefinieerd doel."

Als u bevestigingsberichten wilt verzenden naar gebruikers die zich op uw service abonneren of zich niet meer bij deze service abonneren, maakt u een leveringssjabloon met de doeltoewijzing **[!UICONTROL Subscriptions]** , zonder een bepaald doel. Volg de onderstaande stappen:

1. Maak een leveringssjabloon voor de bevestiging van het abonnement. [ Leer hoe te om een malplaatje ](../msg/delivery-template.md) tot stand te brengen

1. Selecteer geen publiek voor deze levering. In plaats daarvan, heb toegang tot levering **[!UICONTROL Settings]**, ga naar het [ Publiek ](../advanced-settings/delivery-settings.md#audience) lusje, en selecteer de **[!UICONTROL Subscriptions]** doelafbeelding van de lijst.

   ![ Screenshot die de selectie van de doelafbeelding voor een leveringsmalplaatje tonen ](assets/service-confirmation-template-mapping.png){zoomable="yes"}

   >[!NOTE]
   >
   >Als u de doeltoewijzing van **[!UICONTROL Subscriptions]** niet selecteert, ontvangen uw abonnees niet het bevestigingsbericht. Leer meer over doelafbeeldingen in [ deze sectie ](../audience/targeting-dimensions.md).

1. Bewerk de inhoud van de leveringssjabloon, sla deze op en sluit deze.

   ![ Schermafbeelding die de inhoudsredacteur voor een leveringsmalplaatje toont ](assets/service-confirmation-template.png){zoomable="yes"}

   >[!NOTE]
   >
   >Leer meer over leveringskanalen en hoe te om leveringsinhoud in het [ E-mailkanaal ](../email/create-email.md) en [ het kanaal van SMS ](../sms/create-sms.md) secties te bepalen.

1. Herhaal bovenstaande stappen om een leveringssjabloon te maken voor de bevestiging van het abonnement.

U kunt deze berichten nu selecteren wanneer [ het creëren van de abonnementendienst ](#create-service). Gebruikers die zich abonneren op of zich niet abonneren op die service ontvangen de geselecteerde bevestigingsberichten.

## Abonnementenservices bewaken {#logs-and-reports}

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers"
>title="Aantal abonnees"
>abstract="Klik **berekenen** om het totale aantal abonnees voor deze dienst te krijgen."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_totalnumber_subscribers_report"
>title="Totaal aantal abonnees"
>abstract="De belangrijkste Indicator van Prestaties (KPI) verstrekt een uitvoerige mening van de abonneebasis, die het totale aantal individuen toont die aan deze dienst hebben ingetekend."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overtheperiod_subscribers"
>title="Aantal abonnementen voor de periode"
>abstract="Gebruik de vervolgkeuzelijst om het tijdbereik te wijzigen en het aantal abonnementen en abonnementen over de geselecteerde periode weer te geven."

>[!CONTEXTUALHELP]
>id="acw_subscriptions_overallevolution_subscribers"
>title="Algemene ontwikkeling van abonnementen"
>abstract="Deze grafiek toont de uitsplitsing naar periode, met inbegrip van abonnementen, abonnementen, de ontwikkeling in aantallen, en het loyaliteitspercentage."

Om de doeltreffendheid van uw abonnementsdiensten voor SMS en e-mailkanalen te meten, heb toegang tot de logboeken en de rapporten voor een bepaalde dienst.

1. Selecteer een bestaande service in de lijst **[!UICONTROL Subscription services]** . Klik op **[!UICONTROL Calculate]** om het totale aantal abonnees op te halen.

   ![ Screenshot die het totale aantal abonnees berekening ](assets/service-logs-subscribers-count.png){zoomable="yes"} toont

1. Selecteer **[!UICONTROL Logs]** in het servicedashboard om de lijst met abonnees op deze service weer te geven.

   U kunt het totale aantal abonnees, de naam en het adres van elke ontvanger controleren, en wanneer zij of geabonneerd opzeggen. U kunt ze ook filteren.

   ![ Schermschot die de logboekssectie met abonneedetails ](assets/service-logs.png){zoomable="yes"} tonen

1. Selecteer **[!UICONTROL Reports]** in het servicedashboard. Controleer de volgende indicatoren:

   * De **[!UICONTROL Total numbers of subscribers]** wordt weergegeven.

   * Geef het aantal abonnementen en abonnementen voor een bepaalde periode weer. Gebruik de vervolgkeuzelijst om het tijdbereik te wijzigen.

     ![ Schermafbeelding die de rapportensectie met abonnement en unsubscription-gegevens tonen ](assets/service-reports.png){zoomable="yes"}

   * De grafiek **[!UICONTROL Overall evolution of subscriptions]** toont de uitsplitsing door periode, met inbegrip van abonnementen, unsubscriptions, de evolutie in aantallen, en het loyaliteitspercentage.<!--what is Registered?-->

1. Gebruik de knop **[!UICONTROL Reload]** om de meest recente waarden op te halen uit de uitvoering en het schema van de workflow voor bijhouden.