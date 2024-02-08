---
solution: Journey Optimizer
product: journey optimizer
title: Gebruiksgevallen van landingspagina
description: Ontdek de meest gebruikelijke gebruiksgevallen bij bestemmingspagina's in Journey Optimizer
feature: Landing Pages, Subscriptions
topic: Content Management
role: User
level: Intermediate
keywords: landen, landingspagina, hoofdletter gebruiken
source-git-commit: 7c6a485496dcac65722375d0c55402abe1ebbf59
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 0%

---

# Een openingspagina gebruiken {#lp-use-cases}

>[!CONTEXTUALHELP]
>id="acw_landingpages_url"
>title="URL met voorzichtigheid kopiëren"
>abstract="Als u de landingspagina volledig wilt testen of er gebruik van wilt maken, kunt u deze koppeling niet rechtstreeks in een webbrowser of in uw leveringen kopiëren en plakken. Gebruik in plaats daarvan de opdracht **Inhoud simuleren** gebruiken om de landingspagina te testen en de in de documentatie beschreven stappen te volgen om de landingspagina correct te gebruiken."

Als u uw landingspagina op de juiste manier wilt gebruiken, moet u deze als een koppeling in een levering opgeven met de speciale optie.

>[!CAUTION]
>
>Als u de openingspagina volledig wilt benutten, kunt u de koppeling die wordt weergegeven in het gepubliceerde leveringsdashboard, niet rechtstreeks kopiëren naar uw leveringen of naar een webpagina.

In de [!DNL Adobe Campaign Web] De interface, vier uit-van-de-doos malplaatjes staat u toe om verschillende gebruiksgevallen uit te voeren. De belangrijkste stappen blijven echter hetzelfde en worden hieronder beschreven.

1. [Een openingspagina maken](create-lp.md#create-landing-page) en selecteer de sjabloon van uw keuze, afhankelijk van het gebruikte geval.

1. Definieer de eigenschappen en instellingen van de bestemmingspagina.

   ![](assets/lp-uc-properties.png)

1. Afhankelijk van uw geval selecteert u de **[!UICONTROL Acquisition]**, **[!UICONTROL Subscription]**, **[!UICONTROL Unsubscription]** of **[!UICONTROL Denylist]** pagina.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina.

   ![](assets/lp-uc-form.png)

1. Bewerk de inhoud volgens de geselecteerde sjabloon:

   * [Verwerving](#lp-acquisition)
   * [Abonnement](#lp-subscription)
   * [Abonnement opzeggen](#lp-unsubscription)
   * [Lijst van gewezen personen](#lp-denylist)

1. Wijzig desgewenst de rest van de inhoud, sla de wijzigingen op en sluit de inhoud.

1. Bewerk de **[!UICONTROL Confirmation]** en de **[!UICONTROL Error]** en **[!UICONTROL Expiration]** pagina&#39;s. De **[!UICONTROL Confirmation]** Deze pagina wordt weergegeven aan de ontvangers nadat ze het formulier hebben verzonden.

   ![](assets/lp-uc-confirmation-page.png)

1. [Testen](create-lp.md#test-landing-page) en [publish](create-lp.md#publish-landing-page) uw openingspagina.

1. Een [email](../email/create-email.md) levering om verkeer aan de landingspagina te drijven.

1. [Een koppeling invoegen](../email/message-tracking.md#insert-links) in uw berichtinhoud. Selecteren **[!UICONTROL Landing page]** als de **[!UICONTROL Link type]** en kiest u de openingspagina die u hebt gemaakt.

   ![](assets/lp-uc-email-link.png)

   >[!NOTE]
   >
   >Om uw bericht te kunnen verzenden, zorg ervoor de het landen pagina u selecteert nog niet verlopen is. [Meer informatie](create-lp.md#create-landing-page)

Nadat de ontvangers het e-mailbericht hebben ontvangen, klikt u op de koppeling naar de bestemmingspagina en verzendt u het formulier:

* Ze worden doorgestuurd naar de bevestigingspagina.

* Alle andere handelingen die op de landingspagina zijn gedefinieerd, worden toegepast. Bijvoorbeeld, zullen de gebruikers aan uw dienst worden geabonneerd, of zij zullen geen verdere mededelingen van u ontvangen.

Hieronder ziet u enkele voorbeelden van het gebruik van [!DNL Adobe Campaign] het landen van pagina&#39;s in de verschillende mogelijke gebruiksgevallen.

## Profielverwerving {#lp-acquisition}

Met de eerste sjabloon kunt u een profiel toevoegen aan of bijwerken naar de Campagne-database.

1. Wanneer [uw openingspagina maken](create-lp.md#create-landing-page), selecteert u de **[!UICONTROL Acquisition]** sjabloon.

1. Selecteer in de eigenschappen van de bestemmingspagina de optie **[!UICONTROL Pre-fill with the data referenced in the form]** om bestaande informatie van het profiel vooraf te laden en het maken van duplicaten te voorkomen.

1. Selecteer de **[!UICONTROL Acquisition]** pagina om de inhoud te bewerken.

1. Bewerk de tekstvelden naar wens op basis van de gegevens die u wilt verzamelen in uw profielen.

1. Daarnaast kunt u een selectievakje toevoegen waarin u uw klanten uitnodigt zich te abonneren op uw nieuwsbrief. [Leer hoe u een service maakt](../audience/manage-services.md)

   ![](assets/lp-uc-acquisition-page.png)

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Herziening en [publish](create-lp.md#publish-landing-page) uw openingspagina.

1. Een [email](../email/create-email.md) en [een koppeling toevoegen](../email/message-tracking.md#insert-links) op uw openingspagina.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, wordt hun profiel toegevoegd aan de Campagne-database of bijgewerkt met de informatie die ze hebben verstrekt.

![](assets/lp-uc-profile-updated.png)

Als ze ervoor hebben gekozen uw nieuwsbrief te ontvangen, worden ze geabonneerd op de bijbehorende service.

![](assets/lp-uc-newsletter-subscriber.png)

## Abonnement op een service {#lp-subscription}

Een van de meest gebruikelijke gebruiksgevallen is het uitnodigen van uw klanten om [abonneren op een service](../audience/manage-services.md) (zoals een nieuwsbrief of een gebeurtenis) door een landingspagina. Voer de onderstaande stappen uit.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Begin door een bevestigingsmalplaatje voor gebruikers te creëren die aan uw gebeurtenis intekenen, zodat u het gemakkelijk kunt selecteren wanneer het creëren van de dienst. [Meer informatie](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png)

1. Maak een abonnementsservice waarmee de geregistreerde gebruikers op uw gebeurtenis worden opgeslagen. [Leer hoe u een service maakt](../audience/manage-services.md)

1. Selecteer de sjabloon die u hebt gemaakt als de bevestigingse-mail die de gebruikers ontvangen bij het abonneren.

   ![](assets/lp-uc-subscription-service.png)

1. [Een openingspagina maken](create-lp.md#create-landing-page) om uw ontvangers in staat te stellen zich voor uw gebeurtenis te registreren. Selecteer de **[!UICONTROL Subscription]** sjabloon.

1. Selecteer de **[!UICONTROL Subscription]** pagina om de inhoud te bewerken.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina en vouw de **[!UICONTROL Checkbox 1]** sectie.

1. In de **[!UICONTROL Subscriptions & services]** selecteert u de service die u voor uw gebeurtenis hebt gemaakt. Laat de **[!UICONTROL Subscribe in if checked]** optie ingeschakeld.

   ![](assets/lp-uc-subscription-checkbox-1.png)
<!--
1. You can add an additional checkbox to offer subscription to your newsletter for example.-->

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Herziening en [publish](create-lp.md#publish-landing-page) uw openingspagina.

1. Een [email](../email/create-email.md) en [een koppeling toevoegen](../email/message-tracking.md#insert-links) om het verkeer naar de registratiepagina van de landing te leiden.

1. Ontwerp de e-mail om aan te kondigen dat de registratie nu open voor uw gebeurtenis is.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, worden ze doorgestuurd naar de bevestigingspagina en worden ze toegevoegd aan de abonnementenlijst.

## Abonnement opzeggen {#lp-unsubscription}

U kunt uw klanten toelaten om van de dienst af te zien gebruikend een het landen pagina.

1. Zorg ervoor u een bevestigingsmalplaatje voor gebruikers hebt gecreeerd die van uw dienst afmelden, zodat u het gemakkelijk kunt selecteren wanneer het creëren van de dienst. [Meer informatie](../audience/manage-services.md#create-confirmation-message)

1. In uw [abonnementsservice](../audience/manage-services.md), selecteert u de sjabloon die u hebt gemaakt als de bevestigingse-mail die de gebruikers ontvangen wanneer ze zich niet meer abonneren.

1. [Een openingspagina maken](create-lp.md#create-landing-page). Selecteer de **[!UICONTROL Unsubscription]** sjabloon.

1. Selecteer de **[!UICONTROL Unsubscription]** pagina om de inhoud te bewerken.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina.

1. U kunt een **[!UICONTROL Checkbox]** selecteert u de service en selecteert u de **[!UICONTROL Unsubscribe if checked]** -optie.

   ![](assets/lp-uc-unsubscription-checkbox-1.png)

1. U kunt ook de **[!UICONTROL Call to action]** en selecteert u de **[!UICONTROL Additional updates]** -optie. Selecteer de service en controleer de **[!UICONTROL Opt out]** -optie.

   ![](assets/lp-uc-unsubscription-call-to-action.png)

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Herziening en [publish](create-lp.md#publish-landing-page) uw openingspagina.

1. Een [email](../email/create-email.md) en [een koppeling toevoegen](../email/message-tracking.md#insert-links) op de landingspagina.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, worden ze doorgestuurd naar de bevestigingspagina voor abonnementen en worden ze verwijderd van de betreffende abonnementsservice.

## Lijst van gewezen personen {#lp-denylist}

Het is een wettelijke vereiste dat ontvangers de mogelijkheid krijgen om zich niet meer te abonneren op het ontvangen van communicatie van een merk. Daarom moet u altijd een **afmelden, koppeling** in elke e-mail die naar ontvangers wordt verzonden. Nadat u op deze koppeling hebt geklikt, worden de ontvangers naar een bestemmingspagina geleid, inclusief een knop om te bevestigen dat ze het programma willen afsluiten.

U kunt een **[!UICONTROL Denylist]** landingspagina waarmee gebruikers zich kunnen afmelden voor alle leveringen.

1. Wanneer [uw openingspagina maken](create-lp.md#create-landing-page), selecteert u de **[!UICONTROL Denylist]** sjabloon.

1. Selecteer de **[!UICONTROL Denylist]** pagina om de inhoud te bewerken.

1. Breid uit **[!UICONTROL Call to action]** en selecteert u de **[!UICONTROL Additional updates]** -optie.

1. Selecteer in de bijbehorende vervolgkeuzelijst de optie **[!UICONTROL Channel (email)]** om uw ontvangers de mogelijkheid te bieden alleen af te zien van e-mailcommunicatie. U kunt ook **[!UICONTROL By all channel]** voor het kiezen van hen allen van alle mededelingen op alle kanalen.

   ![](assets/lp-uc-denylist.png)

1. Pas de inhoud naar wens aan en sla uw wijzigingen op.

1. Herziening en [publish](create-lp.md#publish-landing-page) uw openingspagina.

1. Een [email](../email/create-email.md) en [een koppeling toevoegen](../email/message-tracking.md#insert-links) op uw landingspagina om gebruikers de mogelijkheid te bieden af te zien van het ontvangen van communicatie.

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier verzenden, worden ze doorgestuurd naar de bevestigingspagina van de lijst van gewezen personen en wordt hun profiel bijgewerkt met de informatie die ze hebben verstrekt.

Blader naar de **[!UICONTROL Profiles]** en selecteert u dat profiel.

Als u bijvoorbeeld ervoor kiest om de **[!UICONTROL Channel (email)]** in uw landingspagina, de **[!UICONTROL No longer contact by email]** Deze optie wordt ingeschakeld.

![](assets/lp-uc-denylist-profile.png)

Dit profiel ontvangt geen e-mailberichten van uw merk tenzij u zich opnieuw abonneert.











