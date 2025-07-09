---
audience: end-user
title: Afleveringswaarschuwing
description: Leer hoe u werkt met waarschuwingsberichten voor leveringen.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 037b04475370b1a34ecec31ef2a774866278ce65
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Aan de slag met meldingen over levering {#gs-delivery-alerting}

Leveringswaarschuwing is een waarschuwingssysteem waarmee groepen gebruikers automatisch e-mailmeldingen kunnen ontvangen met informatie over de uitvoering van hun levering. Ontvangers houden toezicht op de lopende leveringen die door Adobe Campaign worden verwerkt en nemen passende maatregelen als zich problemen voordoen.

Meldingen worden aangepast op basis van specifieke waarschuwingscriteria die zijn gedefinieerd via de Adobe Campaign Web User Interface.

Voor meer informatie bij het beheren van leveringsmislukkingen, verwijs naar [ Adobe Campaign v8 (console) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}.

## E-mailmeldingsinhoud {#content}

E-mailmeldingen bevatten de volgende secties:

* **Samenvatting**: Toont het aantal leveringen die aan uw bepaalde criteria voldoen, met etiketten en kleuren voor elk criterium.
* **Details**: Maakt een lijst van alle bepaalde leveringscriteria voor het dashboard en de overeenkomstige leveringen voor elk criterium.

![ Beschrijving: Dit het schermschot toont de lay-out van het e-mailbericht, met inbegrip van de samenvatting en detailssecties.](assets/alerting-email.png)

## Waarschuwingen over levering instellen {#set-up}

Aan opstelling deze alarm, staat het Gebruikersinterface van het Web van de Campagne u toe om tot stand te brengen en te leiden:

* **de alarmerende dashboards van de levering**: Specificeer ontvangers, plaats alarmerende criteria om in het dashboard te omvatten, en toegang tot een geschiedenis van verzonden alarm. [ Leer hoe te met dashboards ](../msg/delivery-alerting-dashboards.md) te werken.
* **de alarmerende criteria van de Levering**: Het interface van de Gebruiker van het Web van de Campagne verstrekt vooraf bepaalde alarmerende criteria, zoals leveringen met lage productie of leveringen de waarvan voorbereiding ontbrak. U kunt deze criteria aan uw dashboard toevoegen of uw eigen criteria creëren om aan uw behoeften te passen. [ Leer hoe te met criteria ](../msg/delivery-alerting-criteria.md) te werken.

Stel bijvoorbeeld dat u gebruikers met beheerrechten alleen op de hoogte stelt van mislukte leveringen en marketinggebruikers op de hoogte brengt van leveringen met een hoge soft bounce error ratio. Hiertoe maakt u twee aparte dashboards met de juiste criteria voor elke groep ontvangers.

>[!NOTE]
>
>Om tot dashboards en alarmerende criteria toegang te hebben en te vormen, moet u **beleidsrechten** hebben of deel van de **Toezicht van de Levering** veiligheidsgroep uitmaken. Standaardgebruikers hebben geen toegang tot dashboards in de Adobe Campaign-interface, maar kunnen waarschuwingsberichten ontvangen. [ leer meer over toegang en toestemmingen ](../get-started/permissions.md).