---
audience: end-user
title: E-mailrendering testen
description: Leer hoe u uw e-mailrendering kunt testen in de gebruikersinterface van het Campagne Web
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 1%

---


# De rendering van e-mail testen {#email-rendering}

Voordat u uw e-mail verzendt, moet u ervoor zorgen dat uw bericht op een optimale manier aan de ontvangers wordt weergegeven op verschillende webclients en -apparaten.

Om dit te doen, kunt u uw **Litmus** rekening in [!DNL Adobe Campaign] hefboomwerking om onmiddellijk voorproef uw e-mail terug te geven in verschillende contexten en verenigbaarheid in belangrijke Desktops en toepassingen (webmail, berichtdienst, mobiel, enz.) te controleren.

>[!CAUTION]
>
>Als u e-mailrendering gebruikt in Campagne, wordt een proefdruk verzonden naar een systeem van derden. Door uw Litmus-account aan te sluiten met [!DNL Campaign] , geeft u aan dat Adobe niet verantwoordelijk is voor de gegevens die u naar die derde kunt verzenden. Het beleid voor het bewaren van gegevens per e-mail is van toepassing op deze e-mailberichten, inclusief personalisatiegegevens die in deze proefdrukken kunnen worden opgenomen. Als u dergelijke gegevens wilt openen of verwijderen, moet u rechtstreeks contact opnemen met Litmus.

Voor toegang tot rendermogelijkheden via e-mail moet u:

* Een Litmus-account hebben
* Selecteer profielen en/of testprofielen - leer hoe in [ deze sectie ](preview-content.md)

Voer vervolgens de onderstaande stappen uit.

1. In [ geef inhoud ](../email/edit-content.md) scherm of in [ E-mail Designer ](../email/get-started-email-designer.md) uit, klik de **[!UICONTROL Simulate content]** knoop.

1. Selecteer de knop **[!UICONTROL Render email]**.

   ![](assets/simulate-rendering-button.png){zoomable="yes"}

1. Klik **verbind uw rekening van de Samenhang** in de hogere juiste sectie.

   ![](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. Voer uw gegevens in en meld u aan.

   ![](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. Klik de **test van de Looppas** knoop om e-mailvoorproeven te produceren.

1. Controleer uw e-mailinhoud in populaire desktops, mobiele en webclients.

   ![](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->
