---
title: Externe account beheren
description: Leer hoe te om CRM externe rekeningen te vormen
source-git-commit: 934a37cfebfacd2df0b7610285252d883611f252
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 0%

---

# Externe CRM-rekening {#external-crm}

Gebruik een extern CRM-type account om Adobe Campaign te verbinden met een database van derden.

De configuratie-instellingen voor deze externe account zijn afhankelijk van de specifieke database-engine waarmee u verbinding maakt. In de onderstaande secties vindt u gedetailleerde instructies voor de installatie van elke ondersteunde database.

## MICROSOFT DYNAMICS CRM

Met de externe Microsoft Dynamics CRM-account kunt u uw Campagne-instantie verbinden met uw externe Microsoft Dynamics CRM-database.

In Adobe Campaign Web User Interface, vorm uw externe rekening van Microsoft Dynamics CRM.

1. [ creeer uw externe rekening ](external-account.md) en selecteer **[!UICONTROL External database]** als externe rekening **[!UICONTROL Type]** en Microsoft Dynamics CRM als **[!UICONTROL Provider type]**.

1. Klik op **[!UICONTROL Create]**.

1. Als u de **[!UICONTROL Microsoft Dynamics CRM]** externe account wilt configureren, vult u de volgende velden in:

   ![ Scherenshot die de gebieden van de de externe rekeningsconfiguratie van Microsoft Dynamics CRM toont.](assets/crm-microsoft-1.png)

   +++ Voor het type CRM OAuth: Wachtwoordreferenties

   * **[!UICONTROL Server]**: voer de URL van uw Microsoft CRM-server in.

     Als u de URL van uw Microsoft CRM-server wilt opzoeken, meldt u zich aan bij uw Microsoft Dynamics CRM-account, selecteert u Dynamics 365 en opent u vervolgens uw app. De server URL wordt getoond in uw browser adresbar, bijvoorbeeld:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Account]**: geef de account op die wordt gebruikt om u aan te melden bij Microsoft CRM.

   * **[!UICONTROL Password]**: voer het wachtwoord in dat aan het opgegeven account is gekoppeld.

   * **[!UICONTROL Client identifier]**: voer de client-id in die u vindt in de Microsoft Azure Management Portal.

   * **[!UICONTROL CRM version]**: kies Dynamics CRM 365 CRM-versie.

   +++

   </br>

   +++ Voor het type CRM O-auth: Certificaat

   * **[!UICONTROL Server]**: voer de URL van uw Microsoft CRM-server in.

     Als u de URL van uw Microsoft CRM-server wilt opzoeken, meldt u zich aan bij uw Microsoft Dynamics CRM-account, selecteert u Dynamics 365 en opent u vervolgens uw app. De server URL wordt getoond in uw browser adresbar, bijvoorbeeld:`https://myserver.crm.dynamics.com/`.

   * **[!UICONTROL Private Key(Base64 encoded)]**: geef de persoonlijke sleutel op die is gecodeerd in de Base64-indeling.

     Hiertoe kunt u de hulp van een Base64-encoder gebruiken of de opdrachtregel `base64 -w0 private.key` voor Linux.

   * **[!UICONTROL Custom Key identifier]**: voer de aangepaste sleutel-id in die voor het certificaat wordt gebruikt.

   * **[!UICONTROL Key ID]**: voer de sleutel-id in die aan het certificaat is gekoppeld.

   * **[!UICONTROL Client identifier]**: voer de client-id in die u vindt in het Microsoft Azure Management

   * **[!UICONTROL CRM version]**: kies Dynamics CRM 365 CRM-versie.

   +++

1. Nadat u de verbinding hebt ingesteld, opent u **[!UICONTROL Microsoft CRM configuration wizard]** om uw lijst met Microsoft CRM-tabellen te genereren.

   Klik op **[!UICONTROL Next]** om de vereiste tabellen te selecteren.

   ![ Scherenshot die de gebieden van de de externe rekeningsconfiguratie van Microsoft Dynamics CRM toont.](assets/crm-microsoft-2.png)

1. Selecteer de Microsoft CRM-tabellen die u wilt ophalen, of voeg een externe tabel toe door de **[!UICONTROL Table label]** en **[!UICONTROL Table internal name]** op te geven en schakel vervolgens de **[!UICONTROL Selected]** -toets in.

   Klik op **[!UICONTROL Next]**.

1. Klik op **[!UICONTROL Start]** om het Microsoft CRM-schema te maken op basis van de geselecteerde tabellen.

1. Volg de aanwijzingen op het scherm om pagina&#39;s van Adobe Campaign Marketing History en Subscription Management rechtstreeks in Microsoft Dynamics CRM in te voegen.

1. Klik op **[!UICONTROL Display marketing history URLs]** om de URL&#39;s voor het integreren van pagina&#39;s met marketinggeschiedenis weer te geven of op **[!UICONTROL Display URLs for lead subscriptions]** om de URL&#39;s voor het integreren van pagina&#39;s met abonnementsbeheer weer te geven.

   ![ Scherenshot die de gebieden van de de externe rekeningsconfiguratie van Microsoft Dynamics CRM toont.](assets/crm-microsoft-3.png)

1. Klik op **[!UICONTROL Save]** als uw externe Microsoft CRM-account is geconfigureerd.

1. Nadat u uw externe account hebt gemaakt, kunt u nu op **[!UICONTROL Synchronizing enumerations...]** klikken om opsommingen automatisch te synchroniseren van Microsoft CRM naar Adobe Campaign Web User Interface.

   ![ Scherenshot die de gebieden van de de externe rekeningsconfiguratie van Microsoft CRM CRM toont.](assets/crm-microsoft-4.png)

1. Selecteer de opsomming van Adobe Campaign die de opsomming van Microsoft CRM aanpast.

   Schakel de optie **[!UICONTROL Replace]** in als u Adobe Campaign-waarden wilt vervangen door Microsoft CRM-waarden.

## Salesforce {#salesforce}

Als u de externe Salesforce-account wilt configureren voor gebruik met Adobe Campaign, moet u de volgende gegevens opgeven:

1. [ creeer uw externe rekening ](external-account.md) en selecteer **[!UICONTROL External database]** als externe rekening **[!UICONTROL Type]** en Salesforce.com als **[!UICONTROL Provider type]**.

   ![ Schermafbeelding die de gebieden van de de externe rekeningsconfiguratie van Salesforce toont.](assets/crm-salesforce-1.png)

1. Klik op **[!UICONTROL Create]**.

1. Als u de **[!UICONTROL Salesforce]** externe account wilt configureren, vult u de volgende velden in:

   * **[!UICONTROL CRM O-Auth type]**: **[!UICONTROL Password credentials]** of **[!UICONTROL Credentials]**

   * **[!UICONTROL Account]**: account waarmee u zich kunt aanmelden bij Salesforce CRM.

   * **[!UICONTROL Password]**: voer het wachtwoord in dat aan het opgegeven account is gekoppeld.

   * **[!UICONTROL Security token]**: voer het Salesforce-beveiligingstoken in dat aan het account is gekoppeld.

   * **[!UICONTROL API version]**: kies Versie 49.

   ![ Schermafbeelding die de gebieden van de de externe rekeningsconfiguratie van Salesforce toont.](assets/crm-salesforce-2.png)

1. Open **[!UICONTROL Salesforce CRM configuration wizard]** om uw Salesforce CRM-tabellijst te genereren en klik vervolgens op **[!UICONTROL Next]** .

   ![ Scherenshot die de gebieden van de de externe rekeningsconfiguratie van Salesforce CRM toont.](assets/crm-salesforce-3.png)

1. Selecteer de Salesforce-tabellen die u wilt ophalen, of voeg een externe tabel toe door de waarden **[!UICONTROL Table label]** en **[!UICONTROL Table internal name]** in te voeren en schakel vervolgens de schakeloptie **[!UICONTROL Selected]** in.

   Klik op **[!UICONTROL Next]**.

1. Klik op **[!UICONTROL Start]** om het Salesforce CRM-schema te maken op basis van de geselecteerde tabellen.

1. Klik op **[!UICONTROL Salesforce link creation wizard...]** om de webkoppelingen in Salesforce te genereren.

   Dan, klik **[!UICONTROL Next]** om de Webverbindingen voor **te terugwinnen leidt** en **Contacten** van Salesforce.

1. Selecteer de koppelingen die u wilt exporteren naar de lijst met Salesforce-webkoppelingen.

1. Volg de instructies op scherm om **de Geschiedenis van de Marketing** op te nemen en **pagina&#39;s van het Beheer van het Abonnement** van het Gebruikersinterface van het Web van Adobe Campaign in Salesforce CRM.

1. Klik op **[!UICONTROL Save]** als uw externe Salesforce CRM-account is geconfigureerd.

1. Nadat u uw externe account hebt gemaakt, kunt u nu op **[!UICONTROL Synchronizing enumerations...]** klikken om opsommingen automatisch te synchroniseren van Salesforce naar Adobe Campaign Web User Interface.

   ![ Scherenshot die de gebieden van de de externe rekeningsconfiguratie van Salesforce CRM toont.](assets/crm-salesforce-4.png)

1. Selecteer de opsomming van Adobe Campaign die de opsomming van Salesforce aanpast.

   Schakel de optie **[!UICONTROL Replace]** in als u Adobe Campaign-waarden wilt vervangen door Salesforce-waarden.

   ![ Scherenshot die de gebieden van de de externe rekeningsconfiguratie van Salesforce CRM toont.](assets/crm-salesforce-5.png)

