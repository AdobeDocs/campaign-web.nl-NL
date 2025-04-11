---
audience: end-user
title: Machtigingsbeheer in de gebruikersinterface van het Web voor campagne
description: Meer informatie over machtigingen in de gebruikersinterface van Campagne Web
exl-id: c95b854b-ebbe-4985-8f75-fb6bc795a399
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Machtigingen {#permissions}

Elke gebruiker in Adobe Campaign heeft specifieke machtigingen en beperkingen in de toepassing. De gebruiker kan tot een operatorgroep behoren en de toestemmingen van de groep erven.

Op basis van hun machtigingen kan een operator:

* Toegang tot bepaalde mogelijkheden
* Toegang tot bepaalde gegevens
* Toegang tot bepaalde handelingen (maken, wijzigen, verwijderen)

Een gedetailleerde procedure voor vestiging toestemmingen in Adobe Campaign is beschikbaar in [ Adobe Campaign v8 (console) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/gs-permissions) {target="_blank"}.

## Machtigingen voor mappen {#folder-permissions}

Op basis van uw rechten kunt u machtigingen voor mappen weergeven en beheren in de **[!UICONTROL Folder settings]** .

Hieronder ziet u een voorbeeld van een leveringsmap:

![ Voorbeeld van omslagmontages in Adobe Campaign ](assets/folder_settings.png){zoomable="yes"}

In de sectie **[!UICONTROL Security]** van **[!UICONTROL Folder settings]** kunt u operatoren of groepen weergeven en beheren (toevoegen of verwijderen) die toegang hebben tot de map.

![ Voorbeeld van de montages van de omslagveiligheid in Adobe Campaign ](assets/folder_security.png){zoomable="yes"}

U kunt rechtstreeks op de machtigingen klikken en deze wijzigen in **[!UICONTROL Allowed]** of **[!UICONTROL Denied]** .

![ Voorbeeld van ontkende toestemmingen in de montages van de omslagveiligheid ](assets/folder_security_denied.png){zoomable="yes"}

Als de optie **[!UICONTROL Propagate]** is ingeschakeld, zijn alle machtigingen die voor een map zijn gedefinieerd, van toepassing op alle submappen. Deze machtigingen kunnen voor elke submap worden overschreven.

Als de optie **[!UICONTROL System folder]** is geselecteerd, hebben alle operatoren toegang, ongeacht hun machtigingen.

U kunt ook [ de toestemmingen op omslagen in de console van Adobe Campaign ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/folder-permissions) beheren {target="_blank"}.

Alle toestemmingen in het gebruikersinterface van het Web van de Campagne synchroniseren met de toestemmingen van de Console van de Cliënt van de Campagne.