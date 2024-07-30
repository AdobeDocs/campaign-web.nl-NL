---
audience: end-user
title: Machtigingsbeheer in de gebruikersinterface van het Web voor campagne
description: Meer informatie over machtigingen in de gebruikersinterface van Campagne Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: f352f4e726eff50527d0b9a04d0506600c12b822
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Machtigingen {#permissions}

Elke gebruiker in Adobe Campaign heeft zijn eigen toestemmingen en beperkingen in de toepassing. De gebruiker kan deel uitmaken van een operatorgroep en neemt de machtigingen van de groep over.

Volgens zijn machtigingen kan een operator:

* Toegang tot bepaalde mogelijkheden
* Toegang tot bepaalde gegevens
* Toegang tot bepaalde handelingen (maken, wijzigen, verwijderen)

De gedetailleerde procedure aan opstellingstoestemmingen in Adobe Campaign is beschikbaar in [ Adobe Campaign v8 (console) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) {target="_blank"}.

## Machtigingen voor mappen {#folder-permissions}

Volgens uw rechten kunt u de machtigingen voor mappen in de **[!UICONTROL Folder settings]** weergeven en beheren.

Hieronder ziet u een voorbeeld van een leveringsmap:

![](assets/folder_settings.png){zoomable="yes"}

In de sectie **[!UICONTROL Security]** van **[!UICONTROL Folder settings]** kunt u operatoren of groepen weergeven en beheren (toevoegen of verwijderen) die toegang hebben tot de map.

![](assets/folder_security.png){zoomable="yes"}

U kunt rechtstreeks op de machtigingen klikken en deze wijzigen **[!UICONTROL Allowed]** of **[!UICONTROL Denied]** .

![](assets/folder_security_denied.png){zoomable="yes"}

Als de optie **[!UICONTROL Propagate]** is ingeschakeld, worden alle machtigingen die voor een map zijn gedefinieerd, toegepast op alle submappen. Deze machtigingen kunnen voor elke submap worden overgeladen.

Als de optie **[!UICONTROL System folder]** is ingeschakeld, hebben alle operatoren toegang, ongeacht hun machtigingen.

U kunt ook [ de toestemmingen op omslagen in de console van Adobe Campaign ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions) beheren {target="_blank"}.

Alle toestemmingen in het gebruikersinterface van het Web van de Campagne worden gesynchroniseerd omhoog met de toestemmingen van de Console van de Cliënt van de Campagne.
