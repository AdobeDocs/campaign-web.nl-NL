---
audience: end-user
title: Een meertalige levering configureren
description: Leer hoe u een meertalige levering configureert
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 0%

---

# Een meertalige levering configureren {#multilingual-delivery}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Talen toevoegen"
>abstract="Op dit tabblad vindt u een lijst met talen waarin de levering wordt verzonden. U kunt meer talen toevoegen door op de knop Taal toevoegen te klikken of door een andere taal via dit tabblad te dupliceren."

>[!CONTEXTUALHELP]
>id="acw_multilingual_file_upload"
>title="Taalvarianten importeren"
>abstract="In dit dialoogvenster kunt u een taalvariant toevoegen door een CSV-bestand te importeren. Het bestand vult automatisch alle beschikbare velden voor de geselecteerde taal in. U kunt het bestand slepen en neerzetten of het van de computer kiezen voordat u het bevestigt."

In het Web UI van de Campagne, kunt u opstelling uw leveringen als meertalig, die u toestaat om berichten te verzenden die op de aangewezen taal van een profiel worden gebaseerd. Wanneer geen voorkeur wordt bepaald, wordt het bericht verzonden in de standaardtaal.

Bij een meertalige aflevering is het taalbeheer gebaseerd op varianten. Elke variant vertegenwoordigt één taal. Tijdens het creëren van de levering, kunt u veelvoudige taalvarianten toevoegen om het aantal vereiste talen in uw bericht aan te passen. U kunt de standaardtaal ook op elk gewenst moment wijzigen nadat u deze varianten hebt toegevoegd.

De meertalige mogelijkheid is momenteel beschikbaar voor e-mail, pushberichten, transactionele berichten en SMS.

Voer de volgende stappen uit om meertalige leveringen in te stellen:

1. Voeg een taalvariant toe, [ lees meer ](#add-variant)
1. Bepaal de inhoud voor elke variant, [ lees meer ](#define-content)
1. Beheer taalvarianten, [ lees meer ](#manage-variant)

## Een taalvariant toevoegen{#add-variant}

Ga als volgt te werk om taalvarianten te maken:

1. Klik op het bezorgdashboard op het potloodpictogram om het scherm voor de editie van de leveringsinhoud te openen en klik vervolgens op **[!UICONTROL Add language]** .

   >[!IMPORTANT]
   >
   >De **[!UICONTROL Add language]** knoop is slechts beschikbaar als de doeldimensie het **2} schema van de Taal {bevat.** Meer over schema&#39;s en doeldimensies leren, gelieve te verwijzen naar de [ gedetailleerde documentatie ](../audience/targeting-dimensions.md).

   ![](assets/edit-content_2.png){zoomable="yes"}

1. Van **voeg taal** drop-down toe, selecteer de taal om toe te voegen, dan bevestig. Voor duw berichten, kunt u een Csv- dossier [ ook uploaden om alle taalvarianten in één keer in te voeren.](#csv-upload)

   De eerste taal die u toevoegt, wordt automatisch als de standaardtaal ingesteld en de bestaande inhoud wordt de standaardversie. Wanneer extra talen worden toegevoegd, wordt hun inhoud eerst gekopieerd uit de standaardtaal.

   ![](assets/edit-content_3.png){zoomable="yes"}

   >[!NOTE]
   >
   >De talen beschikbaar door deze lijst hangen van de waarden af die door het **attribuut van de Taal** {zijn bepaald (waarden zoals: systeem, gebruiker, dbenum, enz.). Leer meer over opsommingsbeheer in deze [ sectie ](../administration/enumerations.md).

1. Herhaal deze bewerking om andere talen toe te voegen. In het deelvenster **[!UICONTROL Languages]** links ziet u de lijst met talen die u hebt gekozen, het aantal talen en de standaardtaal.

   Als u bijvoorbeeld Engels, Frans en Zweeds hebt gekozen, kunt u deze drie talen zien, zoals hieronder wordt getoond:

   ![](assets/edit-content_9.png){zoomable="yes"}

   Leren hoe te om taalvarianten te beheren, verwijs naar deze [ sectie ](#manage-variant).

## De inhoud voor elke variant definiëren{#define-content}

Wanneer talen zijn ingesteld, definieert u de inhoud van de levering voor elke taal.

1. Selecteer een taal in het deelvenster **[!UICONTROL Languages]** aan de linkerkant van het scherm voor de editie van de leveringsinhoud.

   ![](assets/edit-content_11.png){zoomable="yes"}

1. Bepaal de inhoud van uw bericht voor deze taal. Leer meer in deze [ sectie ](../msg/create-deliveries.md).

1. Herhaal deze bewerking voor elke taal.

<!--
>[!BEGINTABS]

>[!TAB Email delivery]

1. From the delivery content edition screen, choose a language and click the **[!UICONTROL Edit email body]** button. You can also hover over the email preview and select **[!UICONTROL Open email designer]**.

    ![](assets/edit-content_11.png){zoomable="yes"}

1. Define the content of your email for this language. [Read more](../email/get-started-email-designer.md#start-authoring)

1. Repeat this operation for each language.

>[!TAB SMS delivery]

1. From the delivery content edition screen, choose a language.

1. Edit the content of the SMS message for this language. [Read more](../sms/create-sms.md)

    ![](assets/edit-content_11-sms.png){zoomable="yes"}

1. Repeat this operation for each language.

>[!ENDTABS]

-->

Klik op de knop **[!UICONTROL Simulate content]** en kies profielen om een voorvertoning van de levering weer te geven. Controleer of de juiste inhoud voor elk profiel wordt weergegeven.

![](assets/edit-content_5.png){zoomable="yes"}

## Taalvarianten beheren{#manage-variant}

In het linkerpaneel, wordt alle informatie van de taalvariant getoond. Als u alle talen wilt verwijderen, klikt u op de knop Uitvouwen en klikt u op **[!UICONTROL Delete all variants]** .

![](assets/edit-content_13.png){zoomable="yes"}

In de lijst met taalvarianten kunt u de volgende handelingen uitvoeren:

* **geeft** uit: verander de taal terwijl het houden van de bijbehorende inhoud.
* **Reeks als gebrek**: plaats de taal als gebrek. Wanneer voor een profiel geen taal is gedefinieerd, wordt het bericht verzonden in de standaardtaal.
* **Dupliceer**: dupliceer de inhoud die voor deze taal wordt bepaald en kies een verschillende variant.
* **Schrapping**: schrap de variant en zijn bijbehorende inhoud.

![](assets/edit-content_13-sms.png){zoomable="yes"}

## Taalvarianten importeren uit CSV (pushmeldingen) {#csv-upload}

Voor pushberichten kunt u snel alle taalvarianten vullen door een CSV-bestand met uw meertalige inhoud te uploaden. Deze functie stroomlijnt het maken van meertalige campagnes door het mogelijk te maken inhoud offline voor te bereiden en bulksgewijs te importeren.

* **Efficiëntie**: voeg veelvoudige talen en hun inhoud in één enkele verrichting toe
* **Consistentie**: verzeker uniform overseinen over alle taalvarianten
* **Collaboration**: laat inhoudsteams toe om vertalingen in vertrouwde spreadsheethulpmiddelen voor te bereiden
* **Bulk beheer**: beheer en werk gemakkelijk grote aantallen taalvarianten bij

### Vereisten {#csv-best-practices}

Volg deze aanbevolen procedures om te zorgen dat CSV-bestanden correct worden geïmporteerd:

* **gebruik de nauwkeurige kolomstructuur**: Alle 14 kolommen moeten in uw Csv- dossier aanwezig zijn, zelfs als u wat leeg verlaat. Ontbrekende kolommen leiden tot importfout. U kunt een andere volgorde gebruiken, maar alle kolommen moeten aanwezig zijn.
* **precies de kolomnamen van de Gelijke**: De namen van de kolom zijn case-sensitive. Gebruik `title` niet `Title` , `badge` niet `Bbadge` , `locale` niet `Locale` .
* **de landinstellingscodes van het Gebruik in kleine letters**: De scènecodes van het formaat zoals `en_us`, `fr_fr`, `de_de` (in kleine letters met onderstrepingsteken), niet `en_US` of `en-us`.
* **Vul verplichte kolommen**: De `locale` en `language` kolommen moeten waarden voor elke rij bevatten. Lege waarden leiden tot importfout.
* **houd scènes uniek**: Elke scènecode moet slechts eenmaal in uw Csv- dossier verschijnen. Dubbele landinstellingen worden geweigerd.
* **sparen als UTF-8**: Sparen altijd uw Csv- dossier met het coderen UTF-8 om internationale karakters correct te steunen.
* **prijsopgave komma-bevattende inhoud**: Als uw titel of berichtlichaam komma&#39;s bevat, sluit het volledige gebied in dubbele citaten in: `"Hello, welcome!"`.
* **Gebruik correct numerieke waarden**: voor vlagkolommen (isContentAvailable, isMutableContent, silentPush), gebruik `1` voor waar, `0` voor vals, of verlaat leeg voor gebrek.
* **bevestigt JSON formaat**: Als het gebruiken van de kolom customFields, zorg ervoor uw JSON behoorlijk geformatteerd is: `{"key":"value"}` met correcte citaten en steunen.
* **Test met minimale gegevens eerst**: Begin met eenvoudige 2-3 taal CSV om uw formaat te verifiëren alvorens grote dossiers te creëren.

>[!NOTE]
>
>De structuur van de kolom is gedetailleerd in deze [ sectie ](#csv-columns).

### Het CSV-bestand importeren {#csv-steps}

Ga als volgt te werk om taalvarianten uit een CSV-bestand te importeren:

1. Klik in de inhoudseditor voor levering op **[!UICONTROL Add language]** .

   ![ Schermafbeelding die de Add taalknoop in de redacteur van de de inhoudsopgave van het dupmelding tonen ](assets/multilingual-csv.png){zoomable="yes"}

1. Selecteer het CSV-bestand door het naar het uploadgebied te slepen of klik om naar de computer te bladeren.

   Het systeem valideert de bestandsindeling en de inhoud. Als de validatie mislukt, geven foutberichten aan welke kolommen of gegevens onjuist zijn. Los de problemen in uw CSV-bestand op en upload het opnieuw. Zie deze [ sectie ](#csv-troubleshooting).

   ![ Schermafbeelding die succesvolle bevestiging CSV met alle ingevoerde talen tonen ](assets//multilingual-csv2.png){zoomable="yes"}

1. Controleer de geïmporteerde inhoud in het deelvenster Taalvarianten om te controleren of alle correct geladen vertalingen zijn.

   ![ Schermschot die de voorproef van ingevoerde meertalige inhoudvarianten ](assets/multilingual-csv3.png){zoomable="yes"} tonen

### Kolomstructuur {#csv-columns}

Hier is de juiste kolomstructuur die moet worden gebruikt:

>[!NOTE]
>
>U kunt een andere volgorde gebruiken, maar alle kolommen moeten aanwezig zijn. Voor meer beste praktijken, zie deze [ sectie ](#csv-best-practices).

1. **titel**: (Vereiste) titel van het Bericht
1. **messageBody**: (vereiste) berichtlichaam van het Bericht
1. **geluid**: De naam van het correcte dossier (b.v., `default`, `custom_sound.mp3`) - verlaat leeg voor gebrek
1. **badge**: Het aantal van de badge aan vertoning op app pictogram (iOS) - gebruik slechts aantallen
1. **deplinkURI**: Diep verbind URL om te openen wanneer het bericht wordt getikt - verlaten leeg als niet gebruikt
1. **categorie**: De categorie van het bericht herkenningsteken voor douaneacties (iOS) - verlaten leeg als niet gebruikt
1. **iosMediaAttachmentURL**: URL van media gehechtheid voor de berichten van iOS - verlaten leeg als niet gebruikt
1. **androidMediaAttachmentURL**: URL van media gehechtheid voor de berichten van Android - verlaten leeg als niet gebruikt
1. **isContentAvailable**: Inhoud beschikbare vlag (iOS) - gebruik `1` voor waar, `0` voor vals, verlaten leeg voor gebrek (0)
1. **isMutableContent**: Mutable inhoudmarkering (iOS) - gebruik `1` voor waar, `0` voor vals, verlaten leeg voor gebrek (0)
1. **customFields**: De gegevens van de Douane in formaat JSON (b.v., `{"key1":"value1","key2":"value2"}`) - verlaten leeg als niet gebruikt
1. **scène**: (Vereiste) code van de Taal - bijvoorbeeld, `en_us`, `fr_fr`, `de_de` - **verplicht, moet uniek per rij** zijn
1. **taal**: (Vereiste) Naam van de Taal - b.v., `English-United States`, `French-France` - **verplicht**
1. **silentPush**: De stille drukker - gebruik `1` voor stil duwen, `0` voor regelmatig, verlaten leeg voor gebrek (0)

### Voorbeeld van een CSV-bestand {#csv-examples}

Hier volgt een eenvoudig voorbeeld van de verplichte velden:

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
Welcome!,Thank you for joining us,,,,,,,,,, en_us,English-United States,0
Bienvenue !,Merci de nous avoir rejoint,,,,,,,,,,fr_fr,French-France,0
Willkommen!,Vielen Dank für Ihre Anmeldung,,,,,,,,,, de_de,German-Germany,0
¡Bienvenido!,Gracias por unirte a nosotros,,,,,,,,,, es_es,Spanish-Spain,0
```

Hier volgt een voorbeeld met optionele velden:

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
Welcome!,Thank you for joining us,default,1,,,https://example.com/welcome-en.jpg,https://example.com/welcome-en.jpg,,,, en_us,English-United States,0
Bienvenue !,Merci de nous avoir rejoint,default,1,,,https://example.com/welcome-fr.jpg,https://example.com/welcome-fr.jpg,,,, fr_fr,French-France,0
Willkommen!,Vielen Dank für Ihre Anmeldung,default,1,,,https://example.com/welcome-de.jpg,https://example.com/welcome-de.jpg,,,, de_de,German-Germany,0
¡Bienvenido!,Gracias por unirte a nosotros,default,1,,,https://example.com/welcome-es.jpg,https://example.com/welcome-es.jpg,,,, es_es,Spanish-Spain,0
```

Hier volgt een voorbeeld met aangepaste velden

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
New Collection,Discover our latest products,default,1,,,,,,,"{"campaign":"summer2025","segment":"premium"}",en_us,English-United States,0
Nouvelle Collection,Découvrez nos derniers produits,default,1,,,,,,,"{"campaign":"summer2025","segment":"premium"}",fr_fr,French-France,0
```

>[!NOTE]
>
>Voor uitgebreide pushberichten met carrousels of actieknoppen gebruikt Campaign een andere configuratiemethode dan CSV-import. Vorm rijke duw inhoud direct in de leveringsredacteur na het invoeren van basis meertalige inhoud.

### Personalization in CSV-bestanden {#csv-personalization}

Als u verpersoonlijkingsvelden wilt gebruiken in uw CSV-inhoud, moet u `<span>` -tags gebruiken:

```csv
title,messageBody,sound,badge,deeplinkURI,category,iosMediaAttachmentURL,androidMediaAttachmentURL,isContentAvailable,isMutableContent,customFields,locale,language,silentPush
"Hello <span class=""nl-dce-field nl-dce-done"" data-nl-expr=""recipient.firstName"">recipient.firstName</span>","Your order has shipped!",,,,,,,,,,en_us,English-United States,0
"Bonjour <span class=""nl-dce-field nl-dce-done"" data-nl-expr=""recipient.firstName"">recipient.firstName</span>","Votre commande a été expédiée !",,,,,,,,,,fr_fr,French-France,0
```

Tijdens levering, vervangt de Campagne deze placeholders met daadwerkelijke ontvankelijke gegevens.

### Problemen oplossen {#csv-troubleshooting}

| Fout | Oorzaak | Oplossing |
|-------|-------|----------|
| Ontbrekende vereiste kolommen | CSV-bestand bevat niet alle 14 kolommen | Zorg ervoor dat uw CSV alle 14 kolommen heeft in de exacte volgorde die hierboven wordt weergegeven. Gebruik lege waarden voor ongebruikte kolommen. |
| Ongeldige waarden voor landinstelling/taal | locale of taalkolommen zijn leeg | Zowel moeten de scène als de taalkolommen waarden voor elke rij hebben |
| Landinstellingen dupliceren | Dezelfde landinstellingscode wordt meerdere keren weergegeven | Elke landinstellingswaarde moet uniek zijn - dubbele rijen verwijderen |
| Problemen met de codering van bestanden | CSV-bestand gebruikt incompatibele codering | Het CSV-bestand opslaan met UTF-8-codering |
| Kolomfout | Rijen hebben een verschillend aantal kolommen dan kopteksten | Zorg ervoor dat alle rijen exact 14 kolommen hebben die overeenkomen met de koptekst |
| Ongeldige numerieke waarden | badge, isContentAvailable, isMutableContent of silentPush niet-numerieke waarden bevatten | Alleen getallen gebruiken: 0 of 1 voor vlaggen of blanco laten voor standaardwaarde |
| Malformed JSON | customFields column contains invalid JSON | Controleer of de JSON-syntaxis correct is: `{"key":"value"}` of laat leeg |
| Kolomnaam komt niet overeen | Kolomnamen komen niet exact overeen | Kolomnamen zijn hoofdlettergevoelig - gebruik de exacte namen die hierboven worden weergegeven (bijvoorbeeld `badge` , niet `Badge` of `BADGE` ) |

>De beste praktijken zijn vermeld in deze [ sectie ](#csv-best-practices). De structuur van de kolom is gedetailleerd in deze [ sectie ](#csv-columns).

