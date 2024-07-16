---
solution: Campaign, Campaign v8 Web User Interface
title: Gebruiksgevallen van landingspagina
description: Ontdek de gemeenschappelijkste gebruiksgevallen met het landen van pagina's in het Gebruikersinterface van het Web van de Campagne
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: landen, landingspagina, hoofdletter gebruiken
exl-id: e51cf54c-9db1-4704-bc5b-0df098d67c7d
source-git-commit: e5a17ad1f8316d201dc3b4bc6ce20d61aea7a9c9
workflow-type: tm+mt
source-wordcount: '1287'
ht-degree: 0%

---

# Een openingspagina gebruiken {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="URL met voorzichtigheid kopiëren"
>abstract="Als u de landingspagina volledig wilt testen of er gebruik van wilt maken, kunt u deze koppeling niet rechtstreeks in een webbrowser of in uw leveringen kopiëren en plakken. In plaats daarvan, gebruik de **Simuleer inhoud** functie om het te testen, en de stappen te volgen die in documentatie worden beschreven om behoorlijk gebruik van uw het landen pagina te maken."

>[!CONTEXTUALHELP]
>id="acw_landingpages_templates"
>title="URL met voorzichtigheid kopiëren"
>abstract="Wanneer het creëren van een het landen pagina, staan vier uit-van-de-doos malplaatjes u toe om verschillende gebruiksgevallen uit te voeren: voeg of werk een profiel aan het gegevensbestand van de Campagne bij, abonneer klanten aan de dienst, unsubscribe hen van de dienst, of opt gebruikers uit."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/landing-pages/create-lp.html#create-landing-page" text="Een landingspagina maken"

Als u uw landingspagina op de juiste manier wilt gebruiken, moet u deze als een koppeling in een levering opgeven met de speciale optie.

>[!CAUTION]
>
>Als u de openingspagina volledig wilt benutten, kunt u de koppeling die wordt weergegeven in het gepubliceerde leveringsdashboard, niet rechtstreeks kopiëren naar uw leveringen of naar een webpagina. Leer hoe u dit op de juiste wijze doet in deze sectie.

In de [!DNL Adobe Campaign Web] interface, staan vier uit-van-de-doos malplaatjes u toe om verschillende gebruiksgevallen uit te voeren. De belangrijkste stappen blijven echter hetzelfde en worden hieronder beschreven.

1. [ creeer een het landen pagina ](create-lp.md#create-landing-page) en selecteer het malplaatje van uw keus, volgens uw gebruiksgeval.

1. Definieer de eigenschappen en instellingen van de bestemmingspagina.

   ![](assets/lp-uc-properties.png){zoomable="yes"}

1. Afhankelijk van uw geval selecteert u de pagina **[!UICONTROL Acquisition]** , **[!UICONTROL Subscription]** , **[!UICONTROL Unsubscription]** of **[!UICONTROL Denylist]** .

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina.

   ![](assets/lp-uc-form.png){zoomable="yes"}

1. Bewerk de inhoud volgens de geselecteerde sjabloon:

   * [Verwerving](#lp-acquisition)
   * [Abonnement](#lp-subscription)
   * [Abonnement opzeggen](#lp-unsubscription)
   * [Lijst van gewezen personen](#lp-denylist)

1. Wijzig desgewenst de rest van de inhoud, sla de wijzigingen op en sluit de inhoud.

1. Bewerk indien nodig de pagina **[!UICONTROL Confirmation]** en de pagina&#39;s **[!UICONTROL Error]** en **[!UICONTROL Expiration]** . De pagina **[!UICONTROL Confirmation]** wordt weergegeven aan de ontvangers zodra ze het formulier verzenden.

   ![](assets/lp-uc-confirmation-page.png){zoomable="yes"}

1. [ Test ](create-lp.md#test-landing-page) en [ publiceert ](create-lp.md#publish-landing-page) uw het landen pagina.

1. Creeer een [ e-mail ](../email/create-email.md) levering om verkeer aan de het landen pagina te drijven.

1. [ Tussenvoegsel een verbinding ](../email/message-tracking.md#insert-links) in uw berichtinhoud. Selecteer **[!UICONTROL Landing page]** als de **[!UICONTROL Link type]** en kies de openingspagina die u hebt gemaakt.

   ![](assets/lp-uc-email-link.png){zoomable="yes"}

   >[!NOTE]
   >
   >Om uw bericht te kunnen verzenden, zorg ervoor de het landen pagina u selecteert nog niet verlopen is. [Meer informatie](create-lp.md#create-landing-page)

Nadat de ontvangers het e-mailbericht hebben ontvangen, klikt u op de koppeling naar de bestemmingspagina en verzendt u het formulier:

* Ze worden doorgestuurd naar de bevestigingspagina.

* Alle andere handelingen die op de landingspagina zijn gedefinieerd, worden toegepast. Bijvoorbeeld, zullen de gebruikers aan uw dienst worden geabonneerd, of zij zullen geen verdere mededelingen van u ontvangen.

Hieronder volgen enkele voorbeelden van het gebruik van [!DNL Adobe Campaign] -bestemmingspagina&#39;s in de verschillende mogelijke gebruiksgevallen.

## Profielverwerving {#lp-acquisition}

Met de eerste sjabloon kunt u een profiel toevoegen aan of bijwerken naar de Campagne-database.

1. Wanneer [ creërend uw het landen pagina ](create-lp.md#create-landing-page), selecteer het **[!UICONTROL Acquisition]** malplaatje.

1. Selecteer in de eigenschappen van de bestemmingspagina de optie **[!UICONTROL Pre-fill with the data referenced in the form]** om alle bestaande informatie uit het profiel vooraf te laden en het maken van duplicaten te voorkomen.

1. Selecteer de pagina **[!UICONTROL Acquisition]** om de inhoud ervan te bewerken.

1. Bewerk de tekstvelden naar wens op basis van de gegevens die u wilt verzamelen in uw profielen.

1. Daarnaast kunt u een selectievakje toevoegen waarin u uw klanten uitnodigt zich te abonneren op uw nieuwsbrief. [ leer hoe te om de dienst ](../audience/manage-services.md) tot stand te brengen

   ![](assets/lp-uc-acquisition-page.png){zoomable="yes"}

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Het overzicht en [ publiceert ](create-lp.md#publish-landing-page) uw het landen pagina.

1. Creeer een [ e-mail ](../email/create-email.md) en [ voeg een verbinding ](../email/message-tracking.md#insert-links) aan uw het landen pagina toe.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, wordt hun profiel toegevoegd aan de Campagne-database of bijgewerkt met de informatie die ze hebben verstrekt.

![](assets/lp-uc-profile-updated.png){zoomable="yes"}

Als ze ervoor hebben gekozen uw nieuwsbrief te ontvangen, worden ze geabonneerd op de bijbehorende service.

![](assets/lp-uc-newsletter-subscriber.png){zoomable="yes"}

## Abonnement op een service {#lp-subscription}

>[!CONTEXTUALHELP]
>id="acw_landingpages_subscription"
>title="De bestemmingspagina van uw abonnement instellen"
>abstract="Met een abonnementspagina kunnen uw klanten zich abonneren op een service."

Één van de gemeenschappelijkste gebruiksgevallen bestaat uit het uitnodigen van uw klanten om [ aan de dienst ](../audience/manage-services.md) (zoals een nieuwsbrief of een gebeurtenis) in te tekenen door een het landen pagina. Voer de onderstaande stappen uit.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Begin door een bevestigingsmalplaatje voor gebruikers te creëren die aan uw gebeurtenis intekenen, zodat u het gemakkelijk kunt selecteren wanneer het creëren van de dienst. [Meer informatie](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png){zoomable="yes"}

1. Maak een abonnementsservice waarmee de geregistreerde gebruikers op uw gebeurtenis worden opgeslagen. [ leer hoe te om de dienst ](../audience/manage-services.md) tot stand te brengen

1. Selecteer de sjabloon die u hebt gemaakt als de bevestigingse-mail die de gebruikers ontvangen bij het abonneren.

   ![](assets/lp-uc-subscription-service.png){zoomable="yes"}

1. [ creeer een het landen pagina ](create-lp.md#create-landing-page) om uw ontvangers toe te laten om voor uw gebeurtenis te registreren. Selecteer de sjabloon **[!UICONTROL Subscription]** .

1. Selecteer de pagina **[!UICONTROL Subscription]** om de inhoud ervan te bewerken.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina en vouw de sectie **[!UICONTROL Checkbox 1]** uit.

1. Selecteer in het veld **[!UICONTROL Subscriptions & services]** de service die u voor de gebeurtenis hebt gemaakt. Laat de optie **[!UICONTROL Subscribe in if checked]** ingeschakeld.

   ![](assets/lp-uc-subscription-checkbox-1.png){zoomable="yes"}
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Het overzicht en [ publiceert ](create-lp.md#publish-landing-page) uw het landen pagina.

1. Creeer een [ e-mail ](../email/create-email.md) en [ voeg een verbinding ](../email/message-tracking.md#insert-links) toe om verkeer aan de registratie het landen pagina te drijven.

1. Ontwerp de e-mail om aan te kondigen dat de registratie nu open voor uw gebeurtenis is.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, worden ze doorgestuurd naar de bevestigingspagina en worden ze toegevoegd aan de abonnementenlijst.

## Abonnement opzeggen {#lp-unsubscription}

U kunt uw klanten toelaten om van de dienst af te zien gebruikend een het landen pagina.

1. Zorg ervoor u een bevestigingsmalplaatje voor gebruikers hebt gecreeerd die van uw dienst afmelden, zodat u het gemakkelijk kunt selecteren wanneer het creëren van de dienst. [Meer informatie](../audience/manage-services.md#create-confirmation-message)

1. In uw [ abonnementsdienst ](../audience/manage-services.md), selecteer het malplaatje dat u als bevestigingse-mail creeerde de gebruikers op het afmelden zullen ontvangen.

1. [ creeer een het landen pagina ](create-lp.md#create-landing-page). Selecteer de sjabloon **[!UICONTROL Unsubscription]** .

1. Selecteer de pagina **[!UICONTROL Unsubscription]** om de inhoud ervan te bewerken.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina.

1. U kunt een sectie **[!UICONTROL Checkbox]** toevoegen, de service selecteren en de optie **[!UICONTROL Unsubscribe if checked]** selecteren.

   ![](assets/lp-uc-unsubscription-checkbox-1.png){zoomable="yes"}

1. U kunt ook de sectie **[!UICONTROL Call to action]** uitvouwen en de optie **[!UICONTROL Additional updates]** selecteren. Selecteer de service en controleer de optie **[!UICONTROL Opt out]** .

   ![](assets/lp-uc-unsubscription-call-to-action.png){zoomable="yes"}

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Het overzicht en [ publiceert ](create-lp.md#publish-landing-page) uw het landen pagina.

1. Creeer een [ e-mail ](../email/create-email.md) en [ voeg een verbinding ](../email/message-tracking.md#insert-links) aan de het landen pagina toe.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, worden ze doorgestuurd naar de bevestigingspagina voor abonnementen en worden ze verwijderd van de betreffende abonnementsservice.

## Lijst van gewezen personen {#lp-denylist}

Het is een wettelijke vereiste dat ontvangers de mogelijkheid krijgen om zich niet meer te abonneren op het ontvangen van communicatie van een merk. Daarom moet u een **unsubscribe verbinding** in elk e-mailbericht altijd omvatten dat naar ontvangers wordt verzonden. Nadat u op deze koppeling hebt geklikt, worden de ontvangers naar een bestemmingspagina geleid, inclusief een knop om te bevestigen dat ze het programma willen afsluiten.

U kunt een landingspagina van **[!UICONTROL Denylist]** instellen waarmee gebruikers zich kunnen afmelden voor alle leveringen.

1. Wanneer [ creërend uw het landen pagina ](create-lp.md#create-landing-page), selecteer het **[!UICONTROL Denylist]** malplaatje.

1. Selecteer de pagina **[!UICONTROL Denylist]** om de inhoud ervan te bewerken.

1. Vouw de sectie **[!UICONTROL Call to action]** uit en selecteer de optie **[!UICONTROL Additional updates]** .

1. Selecteer **[!UICONTROL Channel (email)]** in de bijbehorende vervolgkeuzelijst om uw ontvangers de mogelijkheid te bieden alleen af te zien van e-mailcommunicatie. U kunt ook **[!UICONTROL By all channel]** selecteren om ze allemaal te kiezen via alle communicatie op alle kanalen.

   ![](assets/lp-uc-denylist.png){zoomable="yes"}

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Het overzicht en [ publiceert ](create-lp.md#publish-landing-page) uw het landen pagina.

1. Creeer een [ e-mail ](../email/create-email.md) en [ voeg een verbinding ](../email/message-tracking.md#insert-links) aan uw het landen pagina toe om gebruikers toe te laten om uit het ontvangen van mededelingen te kiezen.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, worden ze doorgestuurd naar de bevestigingspagina van de lijst van gewezen personen en wordt hun profiel bijgewerkt met de informatie die ze hebben verstrekt.

Blader naar het menu **[!UICONTROL Profiles]** en selecteer dat profiel om te controleren of de keuze van het corresponderende profiel is bijgewerkt.

Als u bijvoorbeeld de optie **[!UICONTROL Channel (email)]** op de bestemmingspagina wilt bijwerken, wordt de optie **[!UICONTROL No longer contact by email]** ingeschakeld.

![](assets/lp-uc-denylist-profile.png){zoomable="yes"}

Dit profiel ontvangt geen e-mailberichten van uw merk tenzij u zich opnieuw abonneert.
