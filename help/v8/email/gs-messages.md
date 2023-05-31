---
audience: end-user
title: Aan de slag met berichten en leveringen in Campagne v8 Web
description: Leer hoe te met leveringen te werken en berichten met het Web van de Campagne te verzenden
badge: label="Alpha" type="Positief"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: acc3f2cdc50fc8727a472d427c2f8077775a8744
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 1%

---

# Aan de slag met berichten{#gs-messages}


Met Adobe Campaign kunt u kanaalcampagnes verzenden, waaronder e-mailberichten, SMS-berichten en pushmeldingen, en de doeltreffendheid ervan meten aan de hand van verschillende speciale rapporten. Deze berichten worden ontworpen en verzonden door leveringen, en kunnen voor elke ontvanger worden gepersonaliseerd. Deze leveringen kunnen op zichzelf staan of in de context van een marketingcampagne worden opgenomen.

Adobe Campaign v8 wordt geleverd met de volgende leveringskanalen:

* **E-mailkanaal**: Met e-mailleveringen kunt u persoonlijke e-mails sturen naar de doelgroep. Leer hoe u een e-mail maakt en verzendt in [deze pagina](../email/create-email.md).

* **SMS-kanaal**: Met leveringen op mobiele kanalen kunt u persoonlijke SMS naar de doelgroep sturen.  Meer informatie over het maken en verzenden van SMS [deze pagina](../sms/create-sms.md).

* **Mobiel toepassingskanaal**: Met levering voor mobiele apps kunt u meldingen verzenden naar iOS- en Android-systemen.  Meer informatie over het maken en verzenden van pushmeldingen in [deze pagina](../push/gs-push.md).

## Een levering maken {#create-delivery}

U kunt zelfstandige leveringen maken via de **[!UICONTROL Deliveries]** van het linkermenu, of creeer leveringen in het kader van een marketing campagne, van **[!UICONTROL Campaigns]** links.

>[!BEGINTABS]

>[!TAB Een zelfstandige levering maken]

Voer de volgende stappen uit om een zelfstandige levering te maken:

1. Bladeren naar de **[!UICONTROL Deliveries]** en klik op de knop **[!UICONTROL Create delivery]** knop.

   ![](assets/create-a-delivery.png)

1. Kies een kanaal voor de levering. Meer informatie over leveringskanalen en hoe u in deze secties leveringsinhoud kunt definiëren:

   * [E-mailkanaal](../email/create-email.md)
   * [Push-meldingskanaal](../push/gs-push.md)
   * [Sms-kanaal](../sms/create-sms.md)

1. Bepaal het leveringspubliek, voor het belangrijkste doel en de controlegroep. Meer informatie over publiek in [deze sectie](../audience/about-audiences.md).
1. Bepaal de berichtinhoud.
1. (optioneel) Bepaal het leveringsschema. Als geen programma wordt bepaald, worden de berichten verzonden onmiddellijk na het klikken van **[!UICONTROL Send]** knop.
1. Klik op de knop  **[!UICONTROL Review and send]** om uw instellingen te controleren.
1. Gebruik de  **[!UICONTROL Simulate content]** om uw levering, en verpersoonlijkingsmontages te testen. Meer informatie over berichtsimulatie vindt u in [deze sectie](../preview-test/preview-test.md).
1. Klik op de knop  **[!UICONTROL Prepare]** om de doelpopulatie te berekenen en de berichten te genereren. De voorbereidingsstap kan een paar minuten duren. Wanneer de voorbereiding volledig is, zijn de berichten klaar om te verzenden. Blader in het geval van een fout naar de **Logboeken** om waarschuwingen en waarschuwingen te controleren.
1. Controleer de resultaten en klik op de knop  **[!UICONTROL Send]** om te beginnen met het verzenden van berichten.
1. Blader naar de **Rapporten** voor toegang tot belangrijke metriek. Meer informatie over leveringsrapporten vindt u in [deze sectie](../reporting/delivery-reports.md).

>[!TAB Een levering maken in een campagne]

Voer de volgende stappen uit om een levering in een campagne te maken:

1. Maak een campagne of open een bestaande campagne. Meer informatie over [marketingcampagnes](../campaigns/gs-campaigns.md).
1. Maak een workflow of open een bestaande workflow.
1. Een **[!UICONTROL Build audience]** en klik op de knop `+`knop.

   ![](assets/add-delivery-in-wf.png)

   De **[!UICONTROL Build audience]** activiteit wordt nader omschreven in [deze sectie](../workflows/workflow-activities.md#targeting).

1. Selecteer een leveringsactiviteit: **[!UICONTROL Email]**, **[!UICONTROL SMS]**, **[!UICONTROL Push notification (Android)]** of **[!UICONTROL Push notification (iOS)]**. Meer informatie over de activiteiten van het leveringskanaal in een workflow en hoe u in deze [sectie](../workflows/workflow-activities.md#channel).
1. Start de workflow en controleer logbestanden.

U kunt ook leveringen in een campagne toevoegen zonder een workflow te maken. Om dit te bereiken, doorblader aan **[!UICONTROL Deliveries]** tabblad van uw campagne en klik op de knop **[!UICONTROL Create delivery]** knop.

![](assets/new-campaign-delivery.png)

De stappen van de configuratie zijn gelijkaardig zoals voor standalone leveringen.

Voor meer informatie over hoe te om een campagne te vormen en leveringen te beheren die tot een campagne behoren, verwijs naar [deze sectie](../campaigns/gs-campaigns.md).

>[!ENDTABS]


## Aanpassing toevoegen{#personalization}

Berichten die door Adobe Campaign worden geleverd, kunnen op verschillende manieren worden gepersonaliseerd. [Meer informatie over personalisatiemogelijkheden](../personalization/personalize.md).

Met Campagne kunt u dynamische inhoud maken en persoonlijke berichten verzenden. U kunt aanpassingsmogelijkheden combineren om uw berichten te verbeteren en een aangepaste gebruikerservaring te creëren.

U kunt de inhoud van het bericht aanpassen door:

* Dynamisch invoegen **personalisatievelden**

   De gebieden van de verpersoonlijking worden gebruikt voor verpersoonlijking op het eerste niveau van uw berichten. U kunt om het even welk gebied selecteren beschikbaar in het gegevensbestand van de verpersoonlijkingsredacteur. Voor een levering, kunt u om het even welk gebied selecteren met betrekking tot de ontvanger, het bericht of de levering. Deze verpersoonlijkingsattributen kunnen in de onderwerpregel of het lichaam van uw berichten worden opgenomen. [Meer informatie](../personalization/personalize.md)

* Vooraf gedefinieerde invoegen **inhoudsblokken**

   De campagne wordt geleverd met een reeks verpersoonlijkingsblokken die een specifieke rendering bevatten die u in uw leveringen kunt invoegen. U kunt bijvoorbeeld een logo, een wensbericht of een koppeling naar de spiegelpagina van het bericht toevoegen. Inhoudsblokken zijn beschikbaar bij een speciale vermelding in de personalisatie-editor. [Meer informatie](../personalization/personalize.md#ootb-content-blocks)

* Maken **voorwaardelijke inhoud**

   Configureer voorwaardelijke inhoud om bijvoorbeeld dynamische personalisatie toe te voegen op basis van het profiel van de ontvanger. Tekstblokken en/of afbeeldingen worden ingevoegd wanneer een bepaalde voorwaarde waar is. [Meer informatie](../personalization/conditions.md)

* Toevoegen **persoonlijke aanbiedingen**

   Voeg persoonlijke aanbiedingen in uw berichtinhoud in, afhankelijk van de locatie van de ontvanger, het huidige weer of de laatste kooporder.


## Bekijk uw leveringen en test deze

Nadat de inhoud van uw bericht is gedefinieerd, kunt u deze voorvertonen om de weergave van uw berichten te bepalen en de instellingen voor de personalisatie te controleren met testprofielen. [Meer informatie](../preview-test/preview-test.md)


## Logbestanden voor aflevering en bijhouden{#gs-tracking-logs}

Het controleren van uw leveringen nadat deze zijn verzonden, is een belangrijke stap om ervoor te zorgen dat uw marketingcampagnes efficiënt zijn en uw klanten bereiken. U kunt controleren na het verzenden van een levering, evenals begrijpen hoe de leveringsmislukkingen en quarantines worden beheerd.

## Een levering dupliceren{#delivery-duplicate}

U kunt een kopie van een bestaande levering maken, vanuit de leveringslijst of vanaf het bezorgdashboard.

Voer de volgende stappen uit om een levering te dupliceren uit de lijst met leveringen:

1. Klik op de drie puntenknop rechts naast de naam van de levering die u wilt dupliceren.
1. Selecteer  **[!UICONTROL Duplicate]**.
1. Herhaling bevestigen: het nieuwe leveringsdashboard opent in het centrale scherm.


Voer de volgende stappen uit om een levering te dupliceren vanaf het dashboard:

1. Open de levering en klik op de knop  **[!UICONTROL ...More]** op de bovenste sectie van het scherm.
1. Selecteer  **[!UICONTROL Duplicate]**.
1. Herhaling bevestigen: de nieuwe levering vervangt de huidige levering in het centrale scherm.

