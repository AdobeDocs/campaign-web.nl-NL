---
audience: end-user
title: Afleveringswaarschuwing
description: Leer hoe u werkt met waarschuwingsberichten voor leveringen.
exl-id: 120afaa0-7017-4644-b6db-229b4a5c8a91
source-git-commit: 39dcf11797339ee9800da6c5a32b1a1c3470529a
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 0%

---

# Aan de slag met meldingen over levering {#gs-delivery-alerting}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Afleveringswaarschuwing"
>abstract="Delivery Alerting is nu beschikbaar in Campaign. Deze mogelijkheid is een waarschuwingsbeheersysteem waarmee groepen gebruikers automatisch e-mailmeldingen kunnen ontvangen met informatie over de uitvoering van hun levering."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"

De Alerting van de levering is een waakzaam beheersysteem dat groepen gebruikers toelaat om e-mailberichten met informatie over hun levering automatisch te ontvangen uitvoeren. Ontvangers kunnen de lopende leveringen die door Adobe Campaign worden verwerkt, volgen en passende maatregelen nemen als zich problemen voordoen.

Meldingen kunnen worden aangepast op basis van specifieke waarschuwingscriteria die zijn gedefinieerd via de Adobe Campaign Web User Interface.

Voor meer informatie op hoe te om leveringsmislukkingen te beheren, verwijs naar [ Adobe Campaign v8 (console) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send) {target="_blank"}

## E-mailmeldingsinhoud {#content}

E-mailmeldingen bevatten de volgende secties:

* **Samenvatting**: Toont het aantal leveringen die aan uw bepaalde criteria voldoen, met etiketten en kleuren voor elk criterium.
* **Details**: Maakt een lijst van alle bepaalde leveringscriteria voor het dashboard en de overeenkomstige leveringen voor elk criterium.

![](assets/alerting-email.png)

## Waarschuwingen over levering instellen {#set-up}

Om u te helpen opstelling deze alarm, staat het Gebruikersinterface van het Web van de Campagne u toe om tot stand te brengen en te leiden:

* **de alarmerende dashboards van de levering**: Specificeer ontvangers, plaats alarmerende criteria om in het dashboard te omvatten, en toegang tot een geschiedenis van verzonden alarm. [ Leer hoe te met dashboards ](../msg/delivery-alerting-dashboards.md) te werken
* **de alarmerende criteria van de Levering**: Het Gebruikersinterface van het Web van de campagne verstrekt vooraf bepaalde alarmerende criteria (leveringen met lage productie, leveringen de waarvan voorbereiding ontbrak...) die u aan uw dashboard kunt toevoegen. U kunt ook uw eigen criteria maken die aan uw behoeften voldoen. [ Leer hoe te met criteria ](../msg/delivery-alerting-criteria.md) te werken

Stel dat u gebruikers met beheerrechten alleen op de hoogte wilt stellen van mislukte leveringen en dat u gebruikers op de hoogte wilt stellen van leveringen met een hoge soft bounce-foutenverhouding. Hiertoe maakt u twee aparte dashboards met de juiste criteria voor elke groep ontvangers.

>[!NOTE]
>
>Om tot dashboards en alarmerende criteria toegang te hebben en te vormen, moet u **beleidsrechten** hebben of deel van de **Toezicht van de Levering** veiligheidsgroep uitmaken. Standaardgebruikers hebben geen toegang tot dashboards in de Adobe Campaign-interface, maar kunnen waarschuwingsberichten ontvangen. [ leer meer op toegang en toestemmingen ](../get-started/permissions.md)
