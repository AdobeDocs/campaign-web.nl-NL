---
audience: end-user
title: Abonnees beheren
description: Leer hoe te om aan de abonnees van de dienst in Adobe Campaign Web te beheren en te leveren
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Abonnees beheren {#manage-subscribers}

Zodra u [ de dienst ](manage-services.md#create-service) creeerde, kunt u abonnees toevoegen, ontvangers opzeggen, en berichten verzenden naar de abonnees van die dienst.

Abonneenbeheer wordt in deze pagina beschreven. Leren hoe te om berichten naar uw abonnees te verzenden, verwijs naar [ deze sectie ](../msg/send-to-subscribers.md).

## Abonnees toevoegen aan uw service {#add-subscribers}

Voer de onderstaande stappen uit om uw abonnees handmatig toe te voegen.

1. Selecteer een bestaande service in de lijst **[!UICONTROL Subscription services]** .

1. Ga naar de tab **[!UICONTROL Subscribers]** en klik op **[!UICONTROL Add subscribers]** .

   ![](assets/service-subscribers-tab.png){zoomable="yes"}

1. Selecteer in de lijst de profielen die u wilt toevoegen en klik op **[!UICONTROL Confirm]** .

   ![](assets/service-subscribers-select-profiles.png){zoomable="yes"}

1. Klik **[!UICONTROL Send]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->om de geselecteerde ontvangers te hebben ontvangen het abonnement [ bevestigingsbericht ](manage-services.md#create-confirmation-message) dat u wanneer [ creërend de dienst ](manage-services.md#create-service) bepaalde.

   ![](assets/service-subscribers-confirmation-msg.png){zoomable="yes"}

   >[!NOTE]
   >
   >Als u **[!UICONTROL Cancel]** selecteert, wordt er geen bevestigingsbericht verzonden naar de geselecteerde profielen, maar worden deze geabonneerd.

De toegevoegde profielen worden weergegeven op het tabblad **[!UICONTROL Subscribers]** . Ze zijn nu geabonneerd op uw service.

## Abonnees van uw service verwijderen {#remove-subscribers}

### Abonnement op profielen handmatig opzeggen {#manual-unsubscription}

Zodra u [ abonnees ](#add-subscribers) aan uw dienst toevoegde, kunt u elk van hen manueel opzeggen. Voer de onderstaande stappen uit.

1. Selecteer een bestaande service in de lijst **[!UICONTROL Subscription services]** .

1. Klik op het pictogram met drie punten naast de gewenste naam van de ontvanger en selecteer **[!UICONTROL Delete]** .

   ![](assets/service-subscribers-delete.png){zoomable="yes"}

1. Verwijderen bevestigen.

1. Klik **[!UICONTROL Send]** om de geselecteerde ontvanger te hebben ontvangen het unsubscription [ bevestigingsbericht ](manage-services.md#create-confirmation-message) dat u wanneer [ creërend de dienst ](manage-services.md#create-service) bepaalde.

   ![](assets/service-subscribers-delete-confirmation.png){zoomable="yes"}

De ontvanger wordt verwijderd van het tabblad **[!UICONTROL Subscribers]** en is niet meer geabonneerd op uw service.

### Ontvangers automatisch afmelden {#automatic-unsubscription}

Een abonnementsservice kan een beperkte duur hebben. Profielen worden automatisch afgemeld wanneer de geldigheidsperiode verloopt.

Deze periode wordt gespecificeerd wanneer [ creërend de dienst ](manage-services.md#create-service). Schakel vanuit **[!UICONTROL Additional options]** de optie **[!UICONTROL Unlimited validity period]** uit en definieer een geldigheidsperiode voor de service.

![](assets/service-create-validity-period.png){zoomable="yes"}

Nadat de gespecificeerde duur verloopt, worden alle abonnees automatisch geabonneerd van die dienst.
