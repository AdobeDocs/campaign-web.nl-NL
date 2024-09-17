---
audience: end-user
title: Je berichten bijhouden
description: Leer hoe u koppelingen toevoegt en verzonden berichten bijhoudt
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 2%

---

# Koppelingen toevoegen en berichten bijhouden {#tracking}

Gebruik de e-mailontwerper om koppelingen naar uw inhoud toe te voegen en de verzonden berichten bij te houden om het gedrag van de ontvangers te controleren.

## Koppelingen invoegen {#insert-links}

Bij het ontwerpen van een bericht kunt u koppelingen naar uw inhoud toevoegen.

>[!NOTE]
>
>Wanneer het volgen wordt toegelaten, worden alle verbindingen inbegrepen in de berichtinhoud gevolgd.

Volg onderstaande stappen om koppelingen in te voegen in uw e-mailinhoud:

1. Selecteer een element en klik op **[!UICONTROL Insert link]** op de contextuele werkbalk.

1. Kies het type koppeling dat u wilt maken:

   ![](assets/message-tracking-insert-link.png){zoomable="yes"}

   * **[!UICONTROL External link]**: voeg een koppeling in naar een externe URL.

     >[!AVAILABILITY]
     >
     >De volgende mogelijkheden (koppeling naar **[!UICONTROL Landing page]** , **[!UICONTROL Subscription link]** en **[!UICONTROL Unsubscription link]** ) bevinden zich in de beperkte beschikbaarheid (LA). Zij zijn beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kunnen niet op een ander milieu worden opgesteld.

   * **[!UICONTROL Landing page]**: voeg een koppeling in naar een bestemmingspagina. Als u een dynamische openingspagina selecteert (met de optie **[!UICONTROL Service from URL]** geselecteerd), kunt u om het even welke dienst van de lijst selecteren. [Meer informatie](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable="yes"}

   * **[!UICONTROL Subscription link]**: voeg een koppeling in naar een abonnementenservice. Wanneer gebruikers op de koppeling klikken, worden ze naar de bestemmingspagina van het abonnement verwezen in de geselecteerde service. [Meer informatie](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable="yes"}

   * **[!UICONTROL Unsubscription link]**: voeg een koppeling in naar een service zonder abonnement. Wanneer abonnees op de koppeling klikken, worden ze naar de bestemmingspagina geleid waarnaar in de geselecteerde service wordt verwezen. [Meer informatie](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. Voer de gewenste URL in het desbetreffende veld in of selecteer een openingspagina of een service en definieer de koppelingsinstellingen en -stijlen.

1. Voeg een **[!UICONTROL Label]** en een **[!UICONTROL Link]** toe.

1. Sla uw wijzigingen op.

1. Nadat de koppeling is gemaakt, kunt u deze nog steeds wijzigen via het tabblad **[!UICONTROL Settings]** .

   * U kunt de koppeling bewerken en de **[!UICONTROL Target]** ervan wijzigen.
   * U kunt de koppeling onderstrepen of niet door de bijbehorende optie in te schakelen.

   ![](assets/message-tracking-link-settings.png){zoomable="yes"}

>[!NOTE]
>
>E-mailberichten van het type Marketing moeten een opt-out-koppeling bevatten, die niet vereist is voor transactiemeldingen. De berichtcategorie (**[!UICONTROL Marketing]** of **[!UICONTROL Transactional]**) wordt bepaald op het niveau van de kanaaloppervlakte en wanneer het creëren van het bericht.

In al uw e-mailberichten moet een specifieke koppeling naar de spiegel worden toegevoegd. Leer meer over de spiegelpagina in [ deze sectie ](mirror-page.md).

## Beheer van bijhouden {#manage-tracking}

[ E-mail Designer ](create-email-content.md) staat u toe om bijgehouden URLs, zoals het uitgeven van het volgende type voor elke verbinding te beheren.

1. Klik op het pictogram **[!UICONTROL Links]** in het linkerdeelvenster om de lijst weer te geven met alle URL&#39;s van de inhoud die u wilt bijhouden.

   In deze lijst kunt u een gecentraliseerde weergave gebruiken en elke URL in de e-mailinhoud opzoeken.

1. Als u een koppeling wilt bewerken, klikt u op het bijbehorende potloodpictogram.

   ![](assets/message-tracking-edit-links.png){zoomable="yes"}

1. U kunt de **[!UICONTROL Tracking Type]** indien nodig wijzigen:

   ![](assets/message-tracking-edit-a-link.png){zoomable="yes"}

   Voor elke bijgehouden URL kunt u de modus Tekstspatiëring instellen op een van de volgende waarden:

   * **[!UICONTROL Tracked]**: activeert tracering op deze URL.
   * **[!UICONTROL Opt out]**: beschouwt deze URL als een niet-geabonneerde of niet-geabonneerde URL.
   * **[!UICONTROL Mirror page]**: beschouwt deze URL als een URL van een spiegelpagina.
   * **[!UICONTROL Never]**: activeert het bijhouden van deze URL nooit. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Voeg een **[!UICONTROL Category]** aan uw koppeling toe om bijgehouden koppelingen te groeperen en klik op **[!UICONTROL Save]** .

   ![](assets/message-tracking-edit-a-link_2.png){zoomable="yes"}

1. Na het verzenden van de levering hebt u toegang tot uw leveringsrapport. In het menu **[!UICONTROL Tracking]** geeft het rapport **[!UICONTROL URLs and click streams]** aan welke URL&#39;s van uw levering het meest zijn bezocht. [Meer informatie](../reporting/gs-reports.md)
