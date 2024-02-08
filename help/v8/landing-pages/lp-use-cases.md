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
source-git-commit: 40c1ac49e9c297e0431331df612cc4a1ae804723
workflow-type: tm+mt
source-wordcount: '1067'
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

1. [Een openingspagina maken](create-lp.md#create-landing-page) en selecteer de sjabloon van uw keuze, afhankelijk van uw gebruiksgeval:

   * [Verwerving](#lp-acquisition)
   * [Abonnement](#lp-subscription)
   * [Abonnement opzeggen](#lp-unsubscription)
   * [Lijst van gewezen personen](#lp-denylist)

1. Definieer de eigenschappen en instellingen van de bestemmingspagina.

   ![](assets/lp-uc-properties.png)

1. Afhankelijk van uw geval selecteert u de **[!UICONTROL Acquisition]**, **[!UICONTROL Subscription]**, **[!UICONTROL Unsubscription]** of **[!UICONTROL Denylist]** pagina.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina.

   ![](assets/lp-uc-form.png)

1. Voer zo veel andere updates uit op de labels en velden van de bestemmingspagina als u nodig hebt. Bewerk de rest van de inhoud naar wens, sla de wijzigingen op en sluit de inhoud.

1. Volg de onderstaande stappen voor elk gebruik.

1. Bewerk de **[!UICONTROL Confirmation]** en de **[!UICONTROL Error]** en **[!UICONTROL Expiration]** pagina&#39;s. Het wordt weergegeven aan de ontvangers wanneer ze het registratieformulier verzenden.

   ![](assets/lp-uc-confirmation-page.png)

1. Testen en [publish](create-lp.md#publish-landing-page) uw openingspagina.

1. Een [email](../email/create-email.md) levering om verkeer aan de landingspagina te drijven.

1. [Een koppeling invoegen](../email/message-tracking.md#insert-links) in uw berichtinhoud. Selecteren **[!UICONTROL Landing page]** als de **[!UICONTROL Link type]** en kiest u [landingspagina](create-lp.md#configure-primary-page) die u hebt gemaakt.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Om uw bericht te kunnen verzenden, zorg ervoor de het landen pagina u selecteert nog niet verlopen is. Leer hoe u de vervaldatum kunt bijwerken [in deze sectie](create-lp.md#create-landing-page).

Zodra zij het e-mailbericht ontvangen, als uw ontvangers op de koppeling naar de landingspagina klikken en het landingspagina-formulier verzenden, worden ze naar de bevestigingspagina geleid en worden alle andere acties toegepast die in uw bestemmingspagina zijn gedefinieerd (gebruikers worden bijvoorbeeld geabonneerd op uw service of ontvangen geen andere communicatie van u).

Hieronder ziet u enkele voorbeelden van het gebruik van [!DNL Adobe Campaign] het landen van pagina&#39;s om uw klanten te hebben binnen of uit van het ontvangen van wat of elk van uw mededelingen kiezen.

## Profielverwerving {#lp-acquisition}

1. [Een openingspagina maken](create-lp.md#create-landing-page). Selecteer de **[!UICONTROL Acquisition]** sjabloon.

1. Definieer de eigenschappen en instellingen van de bestemmingspagina.

   ![](assets/lp-uc-properties.png)

1. Selecteer de **[!UICONTROL Acquisition]** pagina om de inhoud te bewerken.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina.

## Abonnement op een service {#lp-subscription}

Een van de meest gebruikelijke gebruiksgevallen is het uitnodigen van uw klanten om [abonneren op een service](../audience/manage-services.md) (zoals een nieuwsbrief of een gebeurtenis) door een landingspagina. Voer de onderstaande stappen uit.

<!--For example, let's say you organize an event next month and you want to launch an event registration campaign. To do this, you're going to send an email including a link to a landing page that will enable your recipients to register for this event. The users who register will be added to the subscription list that you created for this purpose.-->

1. Begin door een bevestigingsmalplaatje voor gebruikers te creëren die aan uw gebeurtenis intekenen, zodat u het gemakkelijk kunt selecteren wanneer het creëren van de dienst. [Meer informatie](../audience/manage-services.md#create-confirmation-message)

   ![](assets/lp-uc-confirmation-email.png)

1. Maak een abonnementsservice waarmee de geregistreerde gebruikers op uw gebeurtenis worden opgeslagen. [Leer hoe u een service maakt](../audience/manage-services.md)

1. Selecteer de sjabloon die u hebt gemaakt als de bevestigingse-mail die de gebruikers ontvangen bij het abonneren.

   ![](assets/lp-uc-subscription-service.png)

1. [Een openingspagina maken](create-lp.md#create-landing-page) om uw ontvangers in staat te stellen zich voor uw gebeurtenis te registreren. Selecteer de **[!UICONTROL Subscription]** sjabloon.

   <!--![](assets/lp-uc-subscription-template.png)-->

1. Definieer de eigenschappen en instellingen van de bestemmingspagina.

   <!--![](assets/lp-uc-properties.png)-->

1. Selecteer de **[!UICONTROL Subscription]** pagina om de inhoud te bewerken.

   ![](assets/lp-uc-subscription-page-edit.png)

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina en vouw de **[!UICONTROL Checkbox 1]** sectie.

   In de **[!UICONTROL Subscriptions & services]** Selecteer de service die u voor uw gebeurtenis hebt gemaakt. Laat de **[!UICONTROL Subscribe if checked]** optie ingeschakeld.

   ![](assets/lp-uc-subscription-checkbox-1.png)

1. U kunt bijvoorbeeld een extra selectievakje toevoegen om een abonnement op uw nieuwsbrief aan te bieden.

<!--

1. You can also update the profiles who register for your event for the email channel. Expand the **[!UICONTROL Call to action]** section and select Additional updates.

    ![](assets/lp-uc-subscription-call-to-action.png)-->

1. Voer zo veel andere updates uit op de labels en velden van de bestemmingspagina als u nodig hebt. Bewerk de rest van de inhoud naar wens, sla de wijzigingen op en sluit de inhoud.

1. Bewerk de **[!UICONTROL Confirmation]** en de **[!UICONTROL Error]** en **[!UICONTROL Expiration]** pagina&#39;s. Het wordt weergegeven aan de ontvangers wanneer ze het registratieformulier verzenden.

   ![](assets/lp-uc-confirmation-page.png)

1. Testen en [publish](create-lp.md#publish-landing-page) uw openingspagina.

1. Een **E-mail** levering om verkeer naar de registratiepagina te leiden. Ontwerp de e-mail om aan te kondigen dat de registratie nu open voor uw gebeurtenis is.

1. [Een koppeling invoegen](../email/message-tracking.md#insert-links) in uw berichtinhoud. Selecteren **[!UICONTROL Landing page]** als de **[!UICONTROL Link type]** en kiest u [landingspagina](create-lp.md#configure-primary-page) die u voor registratie hebt gemaakt.

   ![](assets/lp_subscription-uc-link.png)

   >[!NOTE]
   >
   >Om uw bericht te kunnen verzenden, zorg ervoor de het landen pagina u selecteert nog niet verlopen is. Leer hoe u de vervaldatum kunt bijwerken [in deze sectie](create-lp.md#create-landing-page).

Als de ontvangers eenmaal een e-mail hebben ontvangen en op de koppeling naar de bestemmingspagina klikken en het formulier van de bestemmingspagina verzenden, worden ze doorgestuurd naar de bevestigingspagina en worden ze toegevoegd aan de abonnementenlijst.

## Abonnement opzeggen {#lp-unsubscription}

1. [Een openingspagina maken](create-lp.md#create-landing-page). Selecteer de **[!UICONTROL Unsubscription]** sjabloon.

1. Definieer de eigenschappen en instellingen van de bestemmingspagina.

1. Selecteer de **[!UICONTROL Unsubscription]** pagina om de inhoud te bewerken.

1. De inhoud van de pagina wordt weergegeven. Selecteer het deel dat overeenkomt met het formulier voor de landingspagina.

## Optie-out-bestemmingspagina&#39;s instellen {#lp-denylist}

Het is een wettelijke vereiste dat ontvangers de mogelijkheid krijgen om zich niet meer te abonneren op het ontvangen van communicatie van een merk. Meer informatie over de toepasselijke wetgeving vindt u in het [Documentatie Experience Platform](https://experienceleague.adobe.com/docs/experience-platform/privacy/regulations/overview.html#regulations){target="_blank"}.

Daarom moet u altijd een **afmelden, koppeling** in elke e-mail die naar ontvangers wordt verzonden:

* Nadat u op deze koppeling hebt geklikt, worden de ontvangers naar een bestemmingspagina geleid, inclusief een knop om te bevestigen dat ze het programma willen afsluiten.
* Als u op de knop Weigeren klikt, worden de profielgegevens bijgewerkt met deze informatie.

U kunt een **[!UICONTROL Denylist]** landingspagina waarmee gebruikers zich kunnen afmelden voor alle leveringen.

Als u gebruikers de mogelijkheid wilt geven zich af te melden voor alle leveringen, moet u een **[!UICONTROL Denylist]** openingspagina.

Wanneer een gebruiker op de koppeling naar de bestemmingspagina klikt, wordt de **[!UICONTROL No longer contact (by any channel)]** in het profiel wordt automatisch geselecteerd.

een **[!UICONTROL Opt-out]** selectievakje en kies voor bijwerken **[!UICONTROL Channel (email)]**: het profiel dat het selectievakje Weigeren inschakelt op de bestemmingspagina wordt uitgeschakeld voor alle communicatie.

Als een ontvanger op de koppeling voor het opzeggen van het abonnement in de e-mail klikt nadat het bericht is ontvangen, wordt de bestemmingspagina weergegeven.

![](assets/lp_opt-out-submit-form.png)

Indien de ontvanger het vakje aankruist en het formulier verzendt:

* De ontvanger van het gekozen-uit wordt opnieuw gericht aan het scherm van het bevestigingsbericht.

* De profielgegevens worden bijgewerkt en zullen geen mededelingen van uw merk tenzij opnieuw geabonneerd ontvangen.

Ga naar Profielen en selecteer het profiel om te controleren of de keuze van het corresponderende profiel is bijgewerkt.







