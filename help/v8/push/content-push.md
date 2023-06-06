---
audience: end-user
title: Een levering met pushberichten ontwerpen
description: Leer hoe u een pushmelding ontwerpt met Adobe Campaign Web
badge: label="Alpha" type="Positief"
source-git-commit: 7fa6a5adb22b4fc4569b93383a8e269703944582
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 6%

---

# Een pushaanbieding ontwerpen {#content-push}

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_android_content"
>title="Android-inhoud induwen"
>abstract="Definieer de inhoud van de push-Android."

>[!CONTEXTUALHELP]
>id="acw_deliveries_push_ios_content"
>title="iOS-inhoud doordrukken"
>abstract="Definieer de push-iOS-inhoud."

## Bericht {#push-message}

>[!BEGINTABS]

>[!TAB Android]

Met Firebase Cloud Messaging kunt u kiezen uit twee typen berichten:

* De **Gegevensbericht**, afgehandeld door de clienttoepassing. De berichten worden verzonden rechtstreeks naar de mobiele toepassing die het android bericht aan het apparaat zal produceren en tonen. Gegevensberichten bevatten alleen aangepaste toepassingsvariabelen.

   Klik op de knop **[!UICONTROL Message]** en gebruik de uitdrukkingseditor om inhoud te definiëren, gegevens aan te passen en dynamische inhoud toe te voegen.

* Het Meldingsbericht, dat automatisch wordt afgehandeld door de FCM SDK. FCM geeft automatisch het bericht weer op de apparaten van uw gebruikers namens de client-app. Meldingsberichten bevatten een vooraf gedefinieerde set parameters en opties, maar kunnen nog steeds verder worden aangepast met aangepaste toepassingsvariabelen.

   Als u uw bericht wilt samenstellen, klikt u op de knop **[!UICONTROL Title]** en **[!UICONTROL Body]** velden. Gebruik de uitdrukkingsredacteur om inhoud te bepalen, gegevens te personaliseren en dynamische inhoud toe te voegen.

   Als u uw pushmelding verder wilt aanpassen, kunt u een afbeelding kiezen die u aan uw pushmelding wilt toevoegen, het pictogram van het bericht dat u op de apparaten van uw profielen wilt weergeven en de kleur van het bericht.

>[!TAB iOS]

Als u uw bericht wilt samenstellen, klikt u op de knop **[!UICONTROL Title]** en **[!UICONTROL Body]** velden. Gebruik de uitdrukkingsredacteur om inhoud te bepalen, gegevens te personaliseren en dynamische inhoud toe te voegen.

U kunt een **[!UICONTROL Subtitle]**, waarde van de ondertitelparameter van de iOS-berichtlading. Zie deze sectie.

In de modus Silent Push kan een melding &quot;silent&quot; worden verzonden naar een mobiele toepassing. De gebruiker wordt niet op de hoogte gesteld van de aankomst van de melding. Deze wordt rechtstreeks naar de toepassing overgedragen.

>[!ENDTABS]

## Geavanceerde instellingen {#push-advanced}

>[!BEGINTABS]

>[!TAB Android]

* **[!UICONTROL Sound]**: Stel het geluid in dat moet worden afgespeeld wanneer het apparaat het bericht ontvangt.

* **[!UICONTROL Notification Count]**: Stel het aantal nieuwe ongelezen gegevens in dat u rechtstreeks op het toepassingspictogram wilt weergeven.

* **[!UICONTROL Channel ID]**: Stel de kanaal-id van uw melding in. De app moet een kanaal met deze kanaal-id maken voordat meldingen met deze kanaal-id worden ontvangen.

* **[!UICONTROL Click action]**: Stel de handeling in die aan een gebruiker is gekoppeld, en klik op het bericht.

* **[!UICONTROL Tag]**: Stel de id in die wordt gebruikt om bestaande meldingen in de meldingslade te vervangen.

* **[!UICONTROL Priority]**: Plaats de prioritaire niveaus van uw bericht aan gebrek, minimum, laag of hoog. Raadpleeg de FCM-documentatie voor meer informatie.

* **[!UICONTROL Visibility]**: Stel de zichtbaarheidsniveaus van uw melding in op openbaar, privé of geheim. Raadpleeg de FCM-documentatie voor meer informatie.

* **[!UICONTROL Sticky]**: Indien gedeactiveerd, wordt het bericht automatisch verworpen wanneer de gebruiker het klikt. Als deze optie is geactiveerd, wordt het bericht nog steeds weergegeven, zelfs wanneer de gebruiker erop klikt.

>[!TAB iOS]

* **[!UICONTROL Critical alert mode]**: Schakel deze optie in om geluid toe te voegen aan uw melding, zelfs als de telefoon van de gebruiker is ingesteld op de focusmodus of als de iPhone is gedempt.

* **[!UICONTROL Clean Badge]**: Schakel deze optie in om de waarde van de badge te vernieuwen.

* **[!UICONTROL Notification count]**: Stel een nummer in dat wordt gebruikt om het aantal nieuwe ongelezen gegevens direct op het toepassingspictogram weer te geven.

* **[!UICONTROL Volume]**: volume van uw geluid van 0 tot 100.

* **[!UICONTROL Mutable content]** (alleen iOS): Verzendt de markering voor gemuteerde inhoud in de pushlading en zorgt ervoor dat de inhoud van het pushbericht kan worden gewijzigd door een uitbreiding van de berichtgevingsservice die is opgegeven in iOS SDK. Zie [Apple Developer documentatie](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/ModifyingNotifications.html) voor meer informatie hierover. Schakel deze optie in als u wilt dat de mobiele toepassing media-inhoud kan downloaden.

* **[!UICONTROL Relevance score]**: een relevantiescore instellen van 0 tot 100. Het systeem gebruikt dit om de berichten in het berichtoverzicht te sorteren.

* **[!UICONTROL Interruption level]**:

   * **[!UICONTROL Active]**: Het systeem stelt de melding standaard in, licht het scherm aan en kan een geluid afspelen. Meldingen doorbreken niet door de focusmodi.

   * **[!UICONTROL Passive]**: Het systeem voegt het bericht toe aan de meldingslijst zonder het scherm te belichten of een geluid af te spelen. Meldingen doorbreken niet door de focusmodi.

   * **[!UICONTROL Time sensitive]**: Het systeem presenteert de melding onmiddellijk, licht het scherm op, kan een geluid afspelen en door de modus Focus breken. Voor dit niveau is geen speciale toestemming van Apple vereist.

   * **[!UICONTROL Critical]**: Het systeem presenteert onmiddellijk het bericht, licht omhoog het scherm, en mijdt de demtschakelaar of nadrukwijzen. Voor dit niveau is een speciale machtiging van Apple vereist.

* **[!UICONTROL Thread-id]**: identifier die wordt gebruikt om gerelateerde meldingen te groeperen.

* **[!UICONTROL Category]**: naam van de rubriek-id die knoppen voor handelingen weergeeft. Met deze meldingen kan de gebruiker sneller verschillende taken uitvoeren als reactie op een melding zonder de applicatie te openen of erin te moeten navigeren.

* **[!UICONTROL Target content ID]**: identifier die wordt gebruikt om aan te geven welk toepassingsvenster moet worden verzonden wanneer de melding wordt geopend.

* **[!UICONTROL Launch image]**: naam van het startafbeeldingsbestand dat moet worden weergegeven. Als de gebruiker ervoor kiest de toepassing te starten, wordt de geselecteerde afbeelding weergegeven in plaats van het startscherm van de toepassing.

>[!ENDTABS]

<!--Sounds must be included in the application and defined when the service is created. Refer to this section.-->



