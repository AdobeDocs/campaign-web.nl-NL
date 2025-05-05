---
audience: end-user
title: Informatie over quarantaine
description: Begrijp het beheer van quarantaineadressen
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---

# Quarantainebeheer {#quarantines}

Adobe Campaign beheert quarantaineadressen voor e-mail, duw, en de kanalen van SMS.

De quarantaine is slechts op een **e-mailadres** van toepassing, a **telefoonaantal**, of a **apparatenteken**, maar niet op het profiel zelf. Een profiel waarvan het e-mailadres in quarantaine is geplaatst, kan bijvoorbeeld worden bijgewerkt met een nieuw adres. Het profiel kan dan opnieuw worden geactiveerd door leveringsacties. Op dezelfde manier, als twee profielen het zelfde telefoonaantal delen, zullen allebei worden beïnvloed als het aantal quarantined is.

>[!CAUTION]
>
>Quarantine in Adobe Campaign is hoofdlettergevoelig.

## Wat is quarantaine {#quarantines-what}

De quarantaine is de methode die wordt gebruikt om **ongeldige adressen in leveringen** te beheren.

Als een levering een hoog tarief van ongeldige adressen heeft, kan het als spam worden beschouwd. Als u deze adressen beheert met quarantaine, voorkomt u dat ze door internetproviders worden gevoegd op lijst van gewenste personen. Dit is belangrijk voor het behoud van uw reputatie.

Wanneer een adres in quarantined in Adobe Campaign is, wordt het profiel automatisch uitgesloten van het doel tijdens leveringsanalyse.

Quarantine verlaagt de verzendkosten van SMS door onjuiste telefoonnummers uit te sluiten van leveringen.

Leer meer over quarantines in de [ Campagne v8 (console) documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/failures/quarantines){target="_blank"} .

## Waarom een adres naar quarantaine wordt verzonden {#quarantines-why}

Vele redenen kunnen een adres naar quarantaine verzenden:

* Voor SMS: onjuiste telefoonnummers
* Voor SMS, wanneer het profiel op een SMS-bericht met een sleutelwoord zoals &quot;STOP&quot;antwoordt
* Voor e-mail, wanneer uw bericht als spam wordt gemeld. Het bericht wordt automatisch opnieuw gericht aan een technische brievenbus die door Adobe wordt beheerd. Het e-mailadres van de gebruiker wordt dan automatisch verzonden naar quarantaine met de Gevoegde op lijst van gewenste personen status.
* Een e-mailadres kan in quarantaine worden geplaatst, bijvoorbeeld wanneer de brievenbus volledig is, als het adres niet bestaat, of als de e-mailserver niet beschikbaar is.

Leer meer over leveringsmislukkingen in de [ Campagne v8 (console) documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/failures/delivery-failures){target="_blank"} .

## Locatie van de quarantaineadressen {#quarantines-where}

U kunt alle quarantaineadressen in uw instantie weergeven via **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Non deliverables Management]** > **[!UICONTROL Non deliverables and addresses]** . Deze sectie maakt een lijst van quarantined elementen voor e-mail, SMS, en de kanalen van het pushbericht.

![ plaats van de quarantaine in de interface van Adobe Campaign ](assets/quarantine_location.png){zoomable="yes"}

U kunt tot een rapport over quarantaine in uw geval ook toegang hebben:

![ Quarantine rapporten in de interface van Adobe Campaign ](assets/quarantine_reports.png){zoomable="yes"}

Voor elke levering, kunt u het overzichtsrapport van de Levering controleren. Het toont het aantal adressen in quarantaine in het leveringsdoel:

![ Samenvattingsrapport van de Levering die quarantined adressen ](assets/quarantine_delivery.png){zoomable="yes"} tonen

U kunt meer opties onderzoeken om quarantaineadressen in de console van Adobe Campaign te beheren. [Meer informatie](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses).