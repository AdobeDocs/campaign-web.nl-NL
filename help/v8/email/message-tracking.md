---
audience: end-user
title: Je berichten bijhouden
description: Leer hoe u koppelingen toevoegt en verzonden berichten bijhoudt
exl-id: ea0d4214-5f14-470c-8791-e8b179ca3a42
source-git-commit: a95a70aa56061106a920584a3501cd4b1434ec8a
workflow-type: tm+mt
source-wordcount: '508'
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

1. Selecteer een element en klik op **[!UICONTROL Insert link]** in de contextuele werkbalk.

1. Kies het type koppeling dat u wilt maken:

   ![](assets/message-tracking-insert-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL External link]**: Voeg een koppeling naar een externe URL in.

     >[!AVAILABILITY]
     >
     >De volgende mogelijkheden (koppeling naar **[!UICONTROL Landing page]**, **[!UICONTROL Subscription link]** en **[!UICONTROL Unsubscription link]**) in Beperkte Beschikbaarheid (LA). Ze zijn beperkt tot klanten die migreren **van Adobe Campaign Standard naar Adobe Campaign v8**, en kan niet worden ingezet op een andere omgeving.

   * **[!UICONTROL Landing page]**: Koppelingen naar bestemmingspagina&#39;s invoegen. Als u een dynamische openingspagina selecteert (met de **[!UICONTROL Service from URL]** (geselecteerd), kunt u om het even welke dienst van de lijst selecteren. [Meer informatie](../landing-pages/create-lp.md#define-actions-on-form-submission)

     ![](assets/email-link-to-landing-page.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Subscription link]**: Voeg een koppeling naar een abonnementenservice in. Wanneer gebruikers op de koppeling klikken, worden ze naar de bestemmingspagina van het abonnement verwezen in de geselecteerde service. [Meer informatie](../audience/manage-services.md#create-service)

     ![](assets/service-create-default-lp-link.png){zoomable=&quot;yes&quot;}

   * **[!UICONTROL Unsubscription link]**: Voeg een koppeling in naar een service zonder abonnement. Wanneer abonnees op de koppeling klikken, worden ze naar de bestemmingspagina geleid waarnaar in de geselecteerde service wordt verwezen. [Meer informatie](../audience/manage-services.md#create-service)

   <!--* **[!UICONTROL Mirror page]**: Add a link to display the email content in a web browser. [Learn more]-->

1. Voer de gewenste URL in het desbetreffende veld in of selecteer een openingspagina of een service en definieer de koppelingsinstellingen en -stijlen.

1. Voeg een **[!UICONTROL Label]** en **[!UICONTROL Link]**.

1. Sla uw wijzigingen op.

1. Als de koppeling eenmaal is gemaakt, kunt u deze nog steeds wijzigen in het menu **[!UICONTROL Settings]** tab.

   * U kunt de koppeling bewerken en de koppeling wijzigen **[!UICONTROL Target]**.
   * U kunt de koppeling onderstrepen of niet door de bijbehorende optie in te schakelen.

   ![](assets/message-tracking-link-settings.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>E-mailberichten van het type Marketing moeten een opt-out-koppeling bevatten, die niet vereist is voor transactiemeldingen. De berichtcategorie (**[!UICONTROL Marketing]** of **[!UICONTROL Transactional]**) wordt gedefinieerd op het niveau van de kanaaloppervlakte en bij het maken van het bericht.

In al uw e-mailberichten moet een specifieke koppeling naar de spiegel worden toegevoegd. Meer informatie over de spiegelpagina vindt u in [deze sectie](mirror-page.md).

## Beheer van bijhouden {#manage-tracking}

De [E-mailDesigner](create-email-content.md) Hiermee kunt u de bijgehouden URL&#39;s beheren, zoals het bewerken van het trackingtype voor elke koppeling.

1. Klik op de knop **[!UICONTROL Links]** in het linkerdeelvenster om de lijst weer te geven met alle URL&#39;s van de inhoud die u wilt bijhouden.

   In deze lijst kunt u een gecentraliseerde weergave gebruiken en elke URL in de e-mailinhoud opzoeken.

1. Als u een koppeling wilt bewerken, klikt u op het bijbehorende potloodpictogram.

   ![](assets/message-tracking-edit-links.png){zoomable=&quot;yes&quot;}

1. U kunt de **[!UICONTROL Tracking Type]** indien nodig:

   ![](assets/message-tracking-edit-a-link.png){zoomable=&quot;yes&quot;}

   Voor elke bijgehouden URL kunt u de modus Tekstspatiëring instellen op een van de volgende waarden:

   * **[!UICONTROL Tracked]**: activeert tracering op deze URL.
   * **[!UICONTROL Opt out]**: beschouwt deze URL als een opt-out- of niet-abonnements-URL.
   * **[!UICONTROL Mirror page]**: beschouwt deze URL als een URL van een spiegelpagina.
   * **[!UICONTROL Never]**: activeert het bijhouden van deze URL nooit. <!--This information is saved: if the URL appears again in a future message, its tracking is automatically deactivated.-->

1. Voeg een **[!UICONTROL Category]** naar uw koppeling om bijgehouden koppelingen te groeperen en klik op **[!UICONTROL Save]**.

   ![](assets/message-tracking-edit-a-link_2.png){zoomable=&quot;yes&quot;}

1. Na het verzenden van de levering hebt u toegang tot uw leveringsrapport. Onder de **[!UICONTROL Tracking]** in het menu **[!UICONTROL URLs and click streams]** het rapport toont welke URLs van uw levering het meest bezochte is. [Meer informatie](../reporting/gs-reports.md)
