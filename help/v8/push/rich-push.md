---
audience: end-user
title: Een uitgebreide pushmelding ontwerpen
description: Leer hoe u een uitgebreide pushmelding voor Android ontwerpt met Adobe Campaign Web
exl-id: a87cb933-b564-4fa4-b173-6a94d7e27da5
source-git-commit: bb61fdb34fecb4131d4069965cda8a3a5099b6bc
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# Een uitgebreide pushaanbieding voor Android ontwerpen {#rich-push}


>[!CONTEXTUALHELP]
>id="acw_deliveries_push_remind_later"
>title="Later herinneren, knop"
>abstract="De **Later herinneren** bevat de optie om een herinnering te plannen. Voor het veld Tijdstempel is een waarde vereist die een tijdperk in seconden vertegenwoordigt."

>[!AVAILABILITY]
>
>Deze functie bevindt zich in **Beperkte beschikbaarheid** (LA).

Met Firebase Cloud Messaging kunt u kiezen uit twee typen berichten:

* De **[!UICONTROL Data message]** wordt afgehandeld door de clienttoepassing. Deze berichten worden rechtstreeks verzonden naar de mobiele toepassing die een Android-melding genereert en weergeeft op het apparaat. Gegevensberichten bevatten alleen aangepaste toepassingsvariabelen.

* De **[!UICONTROL Notification message]**, automatisch afgehandeld door de FCM SDK. FCM geeft automatisch het bericht weer op de apparaten van uw gebruikers namens de client-app. Meldingsberichten bevatten een vooraf gedefinieerde set parameters en opties, maar kunnen nog steeds verder worden aangepast met aangepaste toepassingsvariabelen.

![](assets/rich_push.png){zoomable="yes"}

## De inhoud van het bericht definiëren {#push-message}

Nadat u de pushservice hebt gemaakt, kunt u de inhoud ervan definiëren. Er zijn drie sjablonen beschikbaar:

* **Standaardsjabloon** Hiermee kunt u meldingen verzenden met een eenvoudig pictogram en een bijbehorende afbeelding.

* **Standaardsjabloon** U kunt tekst, afbeeldingen en knoppen in uw meldingen opnemen.

* **Carousel-sjabloon** Hiermee kunt u meldingen verzenden met tekst en meerdere afbeeldingen waar gebruikers doorheen kunnen vegen.

Navigeer door de lusjes hieronder om meer te leren over hoe te om deze malplaatjes aan te passen.

>[!BEGINTABS]

>[!TAB Standaardsjabloon]

1. Van de **[!UICONTROL Template]** vervolgkeuzelijst, selecteert u **[!UICONTROL Default]**.

   ![](assets/rich_push_default.png)

1. Als u uw bericht wilt samenstellen, voert u de tekst in het dialoogvenster **[!UICONTROL Title]** en **[!UICONTROL Message]** velden.

   ![](assets/rich_push_default_2.png)

1. Gebruik de uitdrukkingsredacteur om inhoud te bepalen, gegevens te personaliseren en dynamische inhoud toe te voegen. [Meer informatie](../personalization/personalize.md)

1. Definieer de **[!UICONTROL Click action]** gekoppeld aan een gebruiker, klikt u op uw bericht. Dit bepaalt het gedrag wanneer de gebruiker met het bericht communiceert, zoals het openen van een specifiek scherm of het uitvoeren van een specifieke actie in uw app.

1. Als u uw pushmelding verder wilt aanpassen, kunt u een **[!UICONTROL Image]** URL om toe te voegen aan uw pushmelding en de meldingen **[!UICONTROL Icon]** om weer te geven op de apparaten van uw profielen.

   ![](assets/rich_push_default_3.png)

1. Vorm **[!UICONTROL Advanced settings]** van uw pushmelding. [Meer informatie](#push-advanced)

Nadat u de inhoud van uw bericht hebt gedefinieerd, kunt u testabonnees gebruiken om het bericht voor te vertonen en te testen.

>[!TAB Standaardsjabloon]

1. Van de **[!UICONTROL Template]** vervolgkeuzelijst, selecteert u **[!UICONTROL Basic]**.

   ![](assets/rich_push_basic.png)

1. Als u uw bericht wilt samenstellen, voert u de tekst in het dialoogvenster **[!UICONTROL Title]**, **[!UICONTROL Message]** en **[!UICONTROL Expanded message]** velden.

   De **[!UICONTROL Message]** tekst wordt in de samengevouwen weergave weergegeven terwijl de **[!UICONTROL Expanded message]** wordt weergegeven wanneer het bericht wordt uitgebreid.

   ![](assets/rich_push_basic_2.png)

1. Gebruik de uitdrukkingsredacteur om inhoud te bepalen, gegevens te personaliseren en dynamische inhoud toe te voegen. [Meer informatie](../personalization/personalize.md)

1. Voeg de URL toe die de **[!UICONTROL Click action]** gekoppeld aan een gebruiker, klikt u op uw bericht. Dit bepaalt het gedrag wanneer de gebruiker met het bericht communiceert, zoals het openen van een specifiek scherm of het uitvoeren van een specifieke actie in uw app.

1. Selecteer de **[!UICONTROL Link type]** van de URL die u hebt toegevoegd aan de **[!UICONTROL Click action]** veld:

   * **[!UICONTROL Web URL]**: URL&#39;s leiden gebruikers rechtstreeks naar online-inhoud. Als ze klikken, wordt de standaardwebbrowser van het apparaat gevraagd om de opgegeven URL te openen en ernaar te navigeren.

   * **[!UICONTROL Deeplink]**: Diepe koppelingen zijn URL&#39;s die gebruikers begeleiden bij specifieke secties in een app, zelfs als de app is gesloten. Wanneer op deze knop wordt geklikt, wordt een dialoogvenster weergegeven waarin gebruikers kunnen kiezen uit verschillende apps waarmee de koppeling kan worden afgehandeld.

   * **[!UICONTROL Open App]**: Open App URL&#39;s maken het mogelijk rechtstreeks verbinding te maken met inhoud binnen een toepassing. Het laat uw toepassing toe om zich als standaardmanager voor een specifiek type van verbinding te vestigen, die de dialoog overslaat.

   Raadpleeg voor meer informatie over het afhandelen van Android App-koppelingen het gedeelte [Documentatie voor Android-ontwikkelaars](https://developer.android.com/training/app-links).

   ![](assets/rich_push_basic_3.png)

1. Als u uw pushmelding verder wilt aanpassen, kunt u een **[!UICONTROL Image]** URL om toe te voegen aan uw pushmelding en de meldingen **[!UICONTROL Icon]** om weer te geven op de apparaten van uw profielen.

1. Klikken **[!UICONTROL Add button]** en vul de volgende velden in:

   * **[!UICONTROL Label]**: Tekst weergegeven op de knop.
   * **[!UICONTROL Link URI]**: Geef de URI op die moet worden uitgevoerd wanneer u op de knop klikt.
   * **[!UICONTROL Link type]**: Type koppeling ofwel **[!UICONTROL Web URL]**, **[!UICONTROL Deeplink]**, of **[!UICONTROL Open App]**.

   U kunt maximaal drie knoppen opnemen in uw pushmelding. Als u voor de optie **[!UICONTROL Remind later button]**, kunt u maximaal twee knoppen opnemen.

   ![](assets/rich_push_basic_4.png)

1. Klikken **[!UICONTROL Add remind later]** om een optie voor herinnering later aan uw pushmelding toe te voegen. Voer een **[!UICONTROL Label]** en **[!UICONTROL Timestamp]**.

   Het veld Tijdstempel verwacht een waarde die in seconden een tijdperk vertegenwoordigt.

   ![](assets/rich_push_basic_5.png)

1. Vorm **[!UICONTROL Advanced settings]** van uw pushmelding. [Meer informatie](#push-advanced)

Nadat u de inhoud van uw bericht hebt gedefinieerd, kunt u testabonnees gebruiken om het bericht voor te vertonen en te testen.

>[!TAB Carousel-sjabloon]

1. Van de **[!UICONTROL Template]** vervolgkeuzelijst, selecteert u **[!UICONTROL Carousel]**.

   ![](assets/rich_push_carousel.png)

1. Als u uw bericht wilt samenstellen, voert u de tekst in het dialoogvenster **[!UICONTROL Title]**, **[!UICONTROL Message]** en **[!UICONTROL Expanded message]** velden.

   De **[!UICONTROL Message]** tekst wordt in de samengevouwen weergave weergegeven terwijl de **[!UICONTROL Expanded message]** wordt weergegeven wanneer het bericht wordt uitgebreid.

   ![](assets/rich_push_carousel_1.png)

1. Gebruik de uitdrukkingsredacteur om inhoud te bepalen, gegevens te personaliseren en dynamische inhoud toe te voegen. [Meer informatie](../personalization/personalize.md)

1. Voeg de URL toe die de **[!UICONTROL Click action]** gekoppeld aan een gebruiker, klikt u op uw bericht. Dit bepaalt het gedrag wanneer de gebruiker met het bericht communiceert, zoals het openen van een specifiek scherm of het uitvoeren van een specifieke actie in uw app.

1. Selecteer de **[!UICONTROL Link type]** van de URL die u hebt toegevoegd aan de **[!UICONTROL Click action]** veld:

   * **[!UICONTROL Web UR]**L: URL&#39;s leiden gebruikers naar online-inhoud. Als ze klikken, wordt de standaardwebbrowser van het apparaat gevraagd om de opgegeven URL te openen en ernaar te navigeren.

   * **[!UICONTROL Deeplink]**: Diepe koppelingen zijn URL&#39;s die gebruikers begeleiden bij specifieke secties in een app, zelfs als de app is gesloten. Wanneer op deze knop wordt geklikt, wordt een dialoogvenster weergegeven waarin gebruikers kunnen kiezen uit verschillende apps waarmee de koppeling kan worden afgehandeld.

   * **[!UICONTROL Open App]**: Open App URL&#39;s maken het mogelijk rechtstreeks verbinding te maken met inhoud binnen een toepassing. Het laat uw toepassing toe om zich als standaardmanager voor een specifiek type van verbinding te vestigen, die de dialoog overslaat.

   Raadpleeg voor meer informatie over het afhandelen van Android App-koppelingen het gedeelte [Documentatie voor Android-ontwikkelaars](https://developer.android.com/training/app-links).

   ![](assets/rich_push_carousel_2.png)

1. Als u uw pushmelding verder wilt aanpassen, kunt u de **[!UICONTROL Icon]** om weer te geven op de apparaten van uw profielen.

1. Kies hoe de **[!UICONTROL carousel]** wordt geëxploiteerd:

   * **[!UICONTROL Auto]**: doorloopt afbeeldingen automatisch als dia&#39;s, waarbij de overgang met vooraf gedefinieerde intervallen wordt uitgevoerd.
   * **[!UICONTROL Manual]** Met : kunnen gebruikers handmatig tussen dia&#39;s vegen om door de afbeeldingen te navigeren.

     De optie **[!UICONTROL Filmstrip]** gebruiken om voorvertoningen van de vorige en volgende afbeeldingen naast de hoofddia op te nemen.

1. Klikken **[!UICONTROL Add image]** en voer de URL en tekst van de afbeelding in.

   Zorg ervoor dat u minimaal drie en maximaal vijf afbeeldingen opneemt.

   ![](assets/rich_push_carousel_3.png)

1. Verwerk de volgorde van de afbeeldingen met de pijl-omlaag en de pijl-omhoog.

1. Vorm **[!UICONTROL Advanced settings]** van uw pushmelding. [Meer informatie](#push-advanced)

Nadat u de inhoud van uw bericht hebt gedefinieerd, kunt u testabonnees gebruiken om het bericht voor te vertonen en te testen.

>[!ENDTABS]

## Geavanceerde instellingen voor pushmeldingen {#push-advanced}

![](assets/push_content_5.png){zoomable="yes"}

| Parameter | Beschrijving |
|---------|---------|
| **[!UICONTROL Icon color]** | Stel de kleur van het pictogram in met uw Hex-kleurcodes. |
| **[!UICONTROL Title color]** | Stel de kleur van de titel in met uw Hex-kleurcodes. |
| **[!UICONTROL Message text color]** | Stel de kleur van de berichttekst in met uw Hex-kleurcodes. |
| **[!UICONTROL Notification background color]** | Stel de kleur van de achtergrond voor meldingen in met uw Hex-kleurcodes. |
| **[!UICONTROL Sound]** | Stel het geluid in dat moet worden afgespeeld wanneer het apparaat het bericht ontvangt. |
| **[!UICONTROL Notification Count]** | Stel het aantal nieuwe ongelezen gegevens in dat rechtstreeks op het toepassingspictogram moet worden weergegeven. Hierdoor kan de gebruiker snel zien hoeveel meldingen in behandeling zijn. |
| **[!UICONTROL Channel ID]** | Stel de kanaal-id van uw melding in. De app moet een kanaal met deze kanaal-id maken voordat meldingen met deze kanaal-id worden ontvangen. |
| **[!UICONTROL Tag]** | Stel een id in die wordt gebruikt om bestaande meldingen in de meldingslade te vervangen. Dit helpt de accumulatie van meerdere meldingen te voorkomen en zorgt ervoor dat alleen de meest recente relevante kennisgeving wordt weergegeven. |
| **[!UICONTROL Priority]** | Stel het prioriteitsniveau van uw melding in. Dit kan standaard, minimaal, laag of hoog zijn. Het prioriteitsniveau bepaalt het belang en de urgentie van de melding, en beïnvloedt hoe deze wordt weergegeven en of bepaalde systeeminstellingen kunnen worden omzeild. Raadpleeg voor meer informatie hierover [FCM-documentatie](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#notificationpriority). |
| **[!UICONTROL Visibility]** | Stel het zichtbaarheidsniveau van uw melding in. Dit kan openbaar, privé of geheim zijn. Het zichtbaarheidsniveau bepaalt hoeveel van de inhoud van het bericht wordt weergegeven op het vergrendelingsscherm en andere gevoelige gebieden. Raadpleeg voor meer informatie de [FCM-documentatie](https://firebase.google.com/docs/reference/fcm/rest/v1/projects.messages#visibility). |
| **[!UICONTROL Sticky notification]** | Wanneer geactiveerd, blijft het bericht zichtbaar zelfs nadat de gebruiker erop klikt. <br>Indien gedeactiveerd, wordt het bericht automatisch verworpen wanneer de gebruiker met het in wisselwerking staat. Dankzij het plakgedrag blijven belangrijke meldingen langer op het scherm staan. |
| **[!UICONTROL Application variables]** | Hiermee kunt u gedrag voor meldingen definiëren. Deze variabelen kunnen volledig worden aangepast en worden opgenomen in de berichtlading die naar het mobiele apparaat wordt verzonden. |
