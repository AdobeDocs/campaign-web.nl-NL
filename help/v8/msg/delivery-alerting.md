---
audience: end-user
title: Afleveringswaarschuwing
description: Leer hoe u werkt met waarschuwingsberichten voor leveringen.
source-git-commit: 8c7893dfaa394158ba98172b4025e05e4ab3343c
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Aan de slag met meldingen over levering {#gs-delivery-alerting}

De Alerting van de levering is een waakzaam beheersysteem dat groepen gebruikers toelaat om e-mailberichten met informatie over hun levering automatisch te ontvangen uitvoeren. Ontvangers kunnen de lopende leveringen die door Adobe Campaign worden verwerkt, volgen en passende maatregelen nemen als zich problemen voordoen.

Meldingen kunnen worden aangepast op basis van specifieke waarschuwingscriteria die zijn gedefinieerd via de Adobe Campaign Web User Interface.

Raadpleeg voor meer informatie over het beheren van leveringsfouten de [Adobe Campaign v8 (console)-documentatie](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/failures/delivery-failures#send){target="_blank"}

## E-mailmeldingsinhoud {#content}

E-mailmeldingen bevatten de volgende secties:

* **Samenvatting**: Hiermee geeft u het aantal leveringen weer dat voldoet aan de gedefinieerde criteria, met labels en kleuren voor elk criterium.
* **Details**: geeft voor elk criterium alle gedefinieerde leveringscriteria voor het dashboard en de bijbehorende leveringen weer.

![](assets/alerting-email.png)

## Waarschuwingen over levering instellen {#set-up}

Om u te helpen opstelling deze alarm, staat het Gebruikersinterface van het Web van de Campagne u toe om tot stand te brengen en te leiden:

* **Waarschuwingsdashboards**: Geef ontvangers op, stel waarschuwingscriteria in voor opname in het dashboard en open een geschiedenis met verzonden waarschuwingen. [Leer hoe u met dashboards werkt](../msg/delivery-alerting-dashboards.md)
* **Beoordelingscriteria voor aflevering**: De gebruikersinterface van het Web van de campagne verstrekt vooraf bepaalde alarmerende criteria (leveringen met lage productie, leveranties de waarvan voorbereiding ontbrak...) die u aan uw dashboard kunt toevoegen. U kunt ook uw eigen criteria maken die aan uw behoeften voldoen. [Leer hoe u met criteria werkt](../msg/delivery-alerting-criteria.md)

Stel dat u gebruikers met beheerrechten alleen op de hoogte wilt stellen van mislukte leveringen en dat u gebruikers op de hoogte wilt stellen van leveringen met een hoge soft bounce-foutenverhouding. Hiertoe maakt u twee aparte dashboards met de juiste criteria voor elke groep ontvangers.

>[!NOTE]
>
>Als u dashboards en waarschuwingscriteria wilt openen en configureren, moet u beschikken over **administratierechten** of maakt deel uit van de **Leveringstoezichthouders** beveiligingsgroep. Standaardgebruikers hebben geen toegang tot dashboards in de Adobe Campaign-interface, maar kunnen waarschuwingsberichten ontvangen. [Meer informatie over toegang en machtigingen](../get-started/permissions.md)
