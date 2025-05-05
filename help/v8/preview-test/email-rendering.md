---
audience: end-user
title: E-mailrendering testen
description: Leer hoe u uw e-mailrendering kunt testen in de gebruikersinterface van het Campagne Web
exl-id: 5cdbce8b-3969-470d-8019-1edc58433146
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 1%

---

# De rendering van e-mail testen {#email-rendering}

Voordat u uw e-mail verzendt, moet u ervoor zorgen dat uw bericht optimaal wordt weergegeven voor ontvangers op verschillende webclients en apparaten.

Om dit te bereiken, gebruik uw **rekening 0&rbrace; Litmus &lbrace;binnen [!DNL Adobe Campaign] aan voorproef uw e-mail die onmiddellijk in verschillende contexten teruggeeft.** Op deze manier kunt u de compatibiliteit met belangrijke bureaubladtoepassingen, webmailservices, mobiele apparaten en nog veel meer controleren.

>[!CAUTION]
>
>Als u e-mailrendering gebruikt in Campagne, wordt een proefdruk verzonden naar een systeem van derden. Door uw Litmus-account aan te sluiten met [!DNL Campaign] , geeft u aan dat Adobe niet verantwoordelijk is voor de gegevens die u naar die derde kunt verzenden. Het beleid van Litmus voor het bewaren van e-mailgegevens is op deze e-mails van toepassing, met inbegrip van personalisatiegegevens die in deze proefdrukken kunnen worden omvat. Om tot dergelijke gegevens toegang te hebben of te schrappen, contacteer Litmus rechtstreeks.

Voer de volgende voorwaarden uit om toegang te krijgen tot rendermogelijkheden via e-mail:

* Heb een Litmus account.
* Selecteer profielen en/of testprofielen. Leer hoe in [ deze sectie ](preview-content.md).

Voer vervolgens de onderstaande stappen uit.

1. In [ geef inhoud ](../email/edit-content.md) scherm of in [ E-mail Designer ](../email/get-started-email-designer.md) uit, klik de **[!UICONTROL Simulate content]** knoop.

1. Selecteer de knop **[!UICONTROL Render email]**.

   ![ Simuleer inhoudsknoop in de e-mailredacteur ](assets/simulate-rendering-button.png){zoomable="yes"}

1. Klik **verbind uw rekening van de Samenhang** in de hogere juiste sectie.

   ![ de optie van de de rekeningsverbinding van de Leiding in de e-mailteruggevende interface ](assets/simulate-rendering-litmus.png){zoomable="yes"}

1. Voer uw gegevens in en meld u aan.

   ![ Login van de rekening Litmus scherm ](assets/simulate-rendering-credentials.png){zoomable="yes"}

1. Klik de **test van de Looppas** knoop om e-mailvoorproeven te produceren.

1. Bekijk uw e-mailinhoud in populaire desktops, mobiele clients en webclients.

   ![ E-mail teruggevende voorproeven over verschillende cliënten ](assets/simulate-rendering-previews.png){zoomable="yes"}

<!--
TO CHECK IF user is directed to Litmus or if the email rendering is shown directly in the Campaign UI.

CONTENT ABOVE COPIED FROM AJO

If not redirecting to Litmus:

To test the email rendering, follow these steps:

1. Access the email content creation screen, then click **[!UICONTROL Simulate content]**.

1. Click the **[!UICONTROL Render email]** button.

    The left pane provides various desktop, mobile, and web-based email clients. Select the desired email client to display a preview of your email in the right pane. 

    ![Preview pane showing email rendering across selected clients](assets/render-context.png){zoomable="yes"}

    >[!NOTE]
    >
    >The email clients list provides a sample of the major mail clients. Additional email clients are available from the filter button next to the top search bar.

 -->