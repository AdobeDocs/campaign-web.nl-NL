---
audience: end-user
title: Informatie over quarantaine
description: Begrijp het beheer van quarantaineadressen
exl-id: 4fddabbe-39ab-418b-a87c-f86fe96fa28b
source-git-commit: 3e99bf1453ef38ec915dc82828f44c7d7ffb2acd
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Quarantainebeheer {#quarantines}

Adobe Campaign beheert quarantaineadressen voor e-mail, push, SMS-kanalen.

De quarantaine is slechts op een **e-mailadres** van toepassing, a **telefoonaantal**, of a **apparatenteken**, maar niet op het profiel zelf. Een profiel waarvan het e-mailadres in quarantaine is geplaatst, kan bijvoorbeeld zijn profiel bijwerken en een nieuw adres invoeren. Dit profiel kan dan opnieuw worden geactiveerd door leveringsacties. Eveneens, als twee profielen gebeuren om het zelfde telefoonaantal te hebben, zullen zij allebei worden beïnvloed als het aantal quarantined is.

>[!CAUTION]
>
>Quarantine in Adobe Campaign is hoofdlettergevoelig.

## Wat is quarantaine {#quarantines-what}

De quarantaine is de manier om **de ongeldige adressen in leveringen** te beheren.

Als een levering een hoog tarief van ongeldige adressen heeft, kan het als spam worden beschouwd. Als u deze adressen beheert met quarantaine, hoeft u niet op de lijst met ongewenste personen staan te worden door internetproviders. Dit is belangrijk voor je reputatie.

Wanneer een adres in quarantined in Adobe Campaign is, zal het profiel automatisch van het doel tijdens leveringsanalyse worden uitgesloten.

Quarantine helpt u de verzendkosten van SMS te verlagen door onjuiste telefoonnummers uit te sluiten van leveringen.

Leer meer over quarantines in de [ Campagne v8 (console) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines) {target="_blank"}.


## Waarom een adres naar quarantaine wordt verzonden {#quarantines-why}

Veel redenen kunnen een adres naar quarantaine sturen:

* Voor SMS: onjuiste telefoonnummers
* Voor SMS, wanneer het profiel op een SMS-bericht met een sleutelwoord zoals &quot;STOP&quot;antwoordt
* Voor e-mail, wanneer uw bericht als spam wordt gemeld. Het bericht wordt automatisch opnieuw gericht naar een technische brievenbus die door Adobe wordt geleid. Het e-mailadres van de gebruiker wordt dan automatisch verzonden naar quarantaine met de Gevoegde op lijst van gewenste personen status.
* Een e-mailadres kan in quarantaine worden geplaatst, bijvoorbeeld wanneer de brievenbus volledig is, als het adres niet bestaat, of als de e-mailserver niet beschikbaar is.

Leer meer over leveringsmislukkingen in de [ Campagne v8 (console) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures) {target="_blank"}.

## Locatie van de quarantaineadressen {#quarantines-where}

U kunt alle quarantaineadressen van uw instantie weergeven in **[!UICONTROL Explorer]** > **[!UICONTROL Administration]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Non deliverables Management]** > **[!UICONTROL Non deliverables and addresses]** . Deze sectie maakt een lijst van quarantined elementen voor e-mail, SMS en de kanalen van het pushbericht.

![](assets/quarantine_location.png){zoomable="yes"}

U kunt het rapport over quarantaine in uw geval ook hebben:

![](assets/quarantine_reports.png){zoomable="yes"}

Voor elke levering, kunt u het samenvattingsrapport van de Levering ook controleren: het toont het aantal adressen in quarantaine in het leveringsdoel:

![](assets/quarantine_delivery.png){zoomable="yes"}

U kunt meer mogelijkheden hebben om de quarantaineadressen in de console van Adobe Campaign te beheren. [Meer informatie](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses)
