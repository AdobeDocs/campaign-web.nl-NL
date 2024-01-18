---
audience: end-user
title: Abonnees beheren
description: Leer hoe te om aan de abonnees van de dienst in Adobe Campaign Web te beheren en te leveren
badge: label="Beperkte beschikbaarheid"
exl-id: cf72d27e-365c-4edc-b661-a67c148f0eeb
source-git-commit: 08554d835175cd81f4df057ebfb7952500a12ba4
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# Abonnees beheren {#manage-subscribers}

Eenmaal [een service gemaakt](manage-services.md#create-service), kunt u abonnees toevoegen, ontvangers afmelden, en berichten naar de abonnees van die dienst verzenden.

Abonneenbeheer wordt in deze pagina beschreven. Als u wilt leren hoe u berichten naar uw abonnees kunt verzenden, raadpleegt u [deze sectie](../msg/send-to-subscribers.md).

## Abonnees toevoegen aan uw service {#add-subscribers}

Voer de onderstaande stappen uit om uw abonnees handmatig toe te voegen.

1. Selecteer een bestaande service in het menu **[!UICONTROL Subscription services]** lijst.

1. Ga naar de **[!UICONTROL Subscribers]** en klik op **[!UICONTROL Add subscribers]**.

   ![](assets/service-subscribers-tab.png)

1. Selecteer in de lijst de profielen die u wilt toevoegen en klik op **[!UICONTROL Confirm]**.

   ![](assets/service-subscribers-select-profiles.png)

1. Klikken **[!UICONTROL Send]**<!--if you click cancel, does it mean that no message is sent but recipients are still subscribed, or they are not subscribed? it's 2 different actions in the console)-->om de geselecteerde ontvangers het abonnement te laten krijgen [bevestigingsbericht](manage-services.md#create-confirmation-message) die u hebt gedefinieerd toen [de service maken](manage-services.md#create-service).

   ![](assets/service-subscribers-confirmation-msg.png)

   >[!NOTE]
   >
   >Als u **[!UICONTROL Cancel]**, wordt er geen bevestigingsbericht verzonden naar de geselecteerde profielen, maar deze zijn geabonneerd.

De toegevoegde profielen worden weergegeven in het dialoogvenster **[!UICONTROL Subscribers]** tab. Ze zijn nu geabonneerd op uw service.

## Abonnees van uw service verwijderen {#remove-subscribers}

### Ontvangers handmatig afmelden {#manual-unsubscription}

Eenmaal [toegevoegde abonnees](#add-subscribers) voor uw service, kunt u elk van deze instellingen handmatig afmelden. Voer de onderstaande stappen uit.

1. Selecteer een bestaande service in het menu **[!UICONTROL Subscription services]** lijst.

1. Klik op het pictogram met drie punten naast de gewenste naam van de ontvanger en selecteer **[!UICONTROL Delete]**.

   ![](assets/service-subscribers-delete.png)

1. Verwijderen bevestigen.

1. Klikken **[!UICONTROL Send]** om de geselecteerde ontvanger het abonnement te laten opzeggen [bevestigingsbericht](manage-services.md#create-confirmation-message) die u hebt gedefinieerd toen [de service maken](manage-services.md#create-service).

   ![](assets/service-subscribers-delete-confirmation.png)

De ontvanger wordt verwijderd uit de **[!UICONTROL Subscribers]** en is niet meer geabonneerd op uw service.

### Ontvangers automatisch afmelden {#automatic-unsubscription}

Een abonnementsservice kan een beperkte duur hebben. Ontvangers worden automatisch afgemeld wanneer de geldigheidsperiode verstrijkt.

Deze periode wordt opgegeven wanneer [de service maken](manage-services.md#create-service). Van de **[!UICONTROL Additional options]**, schakelt u de **[!UICONTROL Unlimited validity period]** en stelt een geldigheidsperiode voor de dienst vast.

![](assets/service-create-validity-period.png)

Nadat de gespecificeerde duur verloopt, worden alle abonnees automatisch geabonneerd van die dienst.
