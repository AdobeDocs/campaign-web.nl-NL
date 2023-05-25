---
audience: end-user
title: Aan de slag met berichten en leveringen in Campagne v8 Web
description: Leer hoe te met leveringen te werken en berichten met het Web van de Campagne te verzenden
badge: label="Alpha" type="Positief"
exl-id: 2849b58b-6b75-4023-9ecc-eb243c37f00e
source-git-commit: 14e9ef2a45a1c7a2c8e089c536abd950cdb1b0a3
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Ga aan de slag met berichten in het Web van de Campagne {#gs-messages}

Met Adobe Campaign kunt u kanaalcampagnes verzenden, waaronder e-mailberichten, SMS-berichten en pushmeldingen, en de doeltreffendheid ervan meten aan de hand van verschillende speciale rapporten. Deze berichten worden ontworpen en verzonden door leveringen, en kunnen voor elke ontvanger worden gepersonaliseerd. Deze leveringen kunnen op zichzelf staan of in de context van een marketingcampagne worden opgenomen.

Adobe Campaign v8 wordt geleverd met de volgende leveringskanalen:

* **E-mailkanaal**: Met e-mailleveringen kunt u persoonlijke e-mails sturen naar de doelgroep. Leer hoe u een e-mail maakt en verzendt in [deze pagina](../email/create-email.md).

* **SMS-kanaal**: Met leveringen op mobiele kanalen kunt u persoonlijke SMS naar de doelgroep sturen.  Meer informatie over het maken en verzenden van SMS [deze pagina](../sms/create-sms.md).

* **Mobiel toepassingskanaal**: Met levering voor mobiele apps kunt u meldingen verzenden naar iOS- en Android-systemen.  Meer informatie over het maken en verzenden van pushmeldingen in [deze pagina](../push/gs-push.md).

## Een levering maken

U kunt zelfstandige leveringen maken via de **Aflevering** hoofdmenu, of leveranties maken in het kader van een marketingcampagne.

>[!BEGINTABS]

>[!TAB Een zelfstandige levering maken]

Voer de volgende stappen uit om een zelfstandige levering te maken:

1. Bladeren naar de **[!UICONTROL Deliveries]** en klik op de knop **[!UICONTROL Create delivery]** knop.
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
1. Wanneer berichten zijn verzonden, bladert u naar de sectie Rapporten om toegang te krijgen tot de belangrijkste gegevens. Meer informatie over leveringsrapporten vindt u in [deze sectie](../reporting/reports.md).

>[!TAB Een levering maken in een campagne]

Voer de volgende stappen uit om een levering in een campagne te maken:

1. Maak een campagne of open een bestaande campagne.

Voor meer informatie over hoe te om een campagne te vormen,

>[!ENDTABS]


## Geef op hoe berichten moeten worden verzonden{#gs-send-msg}

Nadat u het bericht hebt gemaakt en de inhoud ervan hebt ontworpen en getest, kunt u kiezen hoe u het bericht wilt verzenden.

De campagne biedt een reeks mogelijkheden aan:

* Handmatig berichten verzenden naar het hoofddoel

* Berichten verzenden die zijn gekoppeld aan een [marketingcampagne](../campaigns/gs-campaigns.md)

* Berichten verzenden via een [werkstroom](../workflows/channel-activities.md)


## Aanpassing toevoegen{#personalization}

Berichten die door Adobe Campaign worden geleverd, kunnen op verschillende manieren worden gepersonaliseerd


## Logbestanden voor aflevering en bijhouden{#gs-tracking-logs}

Het controleren van uw leveringen nadat deze zijn verzonden, is een belangrijke stap om ervoor te zorgen dat uw marketingcampagnes efficiënt zijn en uw klanten bereiken. U kunt controleren na het verzenden van een levering, evenals begrijpen hoe de leveringsmislukkingen en quarantines worden beheerd.
