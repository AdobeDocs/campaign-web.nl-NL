---
audience: end-user
title: Generatieve inhoud
description: Leer hoe u tekstinhoud kunt genereren met AI Assistant
source-git-commit: 2066f29b0867f82f2130361c8ccdb15889085886
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 2%

---

# Tekst genereren met AI Assistant {#generative-text}

>[!IMPORTANT]
>
>Alvorens te beginnen om dit vermogen te gebruiken, lees verwante [&#x200B; Grafieken en Beperkingen &#x200B;](generative-gs.md#generative-guardrails).
></br>
>
>U moet met a [&#x200B; gebruikersovereenkomst &#x200B;](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} akkoord gaan alvorens AI Medewerker in het Web van Adobe Campaign te gebruiken. Neem voor meer informatie contact op met uw Adobe-vertegenwoordiger.

Met AI Assistant in Adobe Campaign Web kunt u aantrekkelijke tekst genereren die op uw publiek lijkt. Of u nu werkt aan het verbeteren van e-mailkopieën, het maken van overtuigende bestemmingspagina-inhoud, het schrijven van pushberichten of het samenstellen van SMS-tekst, AI Assistant helpt u heldere, onzichtbare communicatie te bieden.

## Voor e-mail- en landingspagina&#39;s {#email-web-channels}

Met AI Assistant kunt u tekstinhoud van hoge kwaliteit genereren voor uw e-mailleveringen en bestemmingspagina&#39;s. Met deze mogelijkheid kunt u aansprekende, on-brand berichten maken die via digitale aanraakpunten verbinding maken met uw publiek.

### Toegang en configuratie {#access-configure}

Voordat u begint tekstinhoud te genereren met AI Assistant, moet u de levering instellen en toegang krijgen tot de inhoudeditor. Voer de volgende stappen uit om uw werkruimte voor te bereiden en het deelvenster AI Assistant te openen.

1. Creeer en vorm uw levering:

   * **E-mail**: Na het creëren van en het vormen van uw e-maillevering, klik **[!UICONTROL Edit content]**. [Meer informatie](../email/create-email-content.md)
   * **het Bestaan Pagina**: Na het creëren van en het vormen van uw het landen pagina, klik **[!UICONTROL Edit content]**. [Meer informatie](../landing-pages/create-lp.md)

1. Selecteer een **[!UICONTROL Text component]** om specifieke inhoud als doel in te stellen en open het menu **[!UICONTROL AI Assistant]** .

   ![&#x200B; Screenshot die de selectie van de tekstcomponent in het Web van Adobe Campaign toont &#x200B;](assets/text-genai-1.png){zoomable="yes"}

### Inhoud genereren {#generate-content}

Leer hoe u duidelijke aanwijzingen maakt, instellingen nauwkeurig afstemt en op maat gemaakte tekst genereert met AI Assistant, zodat uw berichten worden afgestemd op uw merk- en communicatiedoelstellingen.

1. Selecteer **[!UICONTROL Brand]** om te zorgen dat door AI gegenereerde inhoud wordt uitgelijnd op de specificaties van uw merk. [&#x200B; leer meer &#x200B;](brands.md) op Banden.

1. Stel de inhoud nauwkeurig af door te beschrijven wat u wilt genereren in het veld **[!UICONTROL Prompt]** .

   Als u hulp nodig hebt die uw herinnering creeert, toegang **[!UICONTROL Prompt Library]**, die een diverse waaier van snelle ideeën verstrekt om uw leveringen te verbeteren. [&#x200B; Leer meer op snelle beste praktijken &#x200B;](ai-assistant-prompting-guide.md)

   ![&#x200B; Schermafbeelding die snelle bibliotheek in het Web van Adobe Campaign toont &#x200B;](assets/text-genai-2.png){zoomable="yes"}

1. Tik uw vraag met de optie **[!UICONTROL Text settings]** :

   * **[!UICONTROL Communication strategy]**: Kies de meest geschikte communicatiestijl voor de gegenereerde tekst.
   * **[!UICONTROL Languages]**: kies de taal van de gegenereerde inhoud.
   * **[!UICONTROL Tone]**: zorg ervoor dat de toon van uw e-mail op uw publiek afgestemd is. Of u informatief wilt klinken, playful, of overtuigend, AI Medewerker past het bericht dienovereenkomstig aan.
   * **Lengte van de Tekst**: Gebruik de schuif om de gewenste lengte van uw tekst te selecteren.

     ![&#x200B; Schermafbeelding die de opties van tekstmontages in het Web van Adobe Campaign tonen &#x200B;](assets/text-genai-4.png){zoomable="yes"}

1. Klik in het menu **[!UICONTROL Reference content]** op **[!UICONTROL Upload file]** om een merkelement toe te voegen dat inhoud bevat die extra context-AI-assistent kan bieden of selecteer een eerder geüpload element.

   Eerder geüploade bestanden zijn beschikbaar in de vervolgkeuzelijst **[!UICONTROL Uploaded reference content]** . Schakel eenvoudig de elementen in die u wilt opnemen in uw generatie.

1. Klik op **[!UICONTROL Generate]** als de vraag gereed is.

### Verfijnen en voltooien {#refine-finalize}

Leer hoe u de gegenereerde tekst kunt reviseren, verfijningen kunt aanbrengen en personalisatie kunt toepassen om uw inhoud te voltooien, zodat u gepolijst en boeiende berichten kunt maken die u kunt leveren.

1. Blader door het gegenereerde bestand **[!UICONTROL Variations]** .

1. Klik op het percentagepictogram om uw **[!UICONTROL Brand Alignment Score]** weer te geven en eventuele onjuiste uitlijningen met uw merk te identificeren.

   Leer meer op [&#x200B; de groeperingsscore van het Merk &#x200B;](brands-score.md).

   ![](assets/text-genai-6.png){zoomable="yes"}

1. Klik op **[!UICONTROL Preview]** om een schermvullende versie van de geselecteerde variant weer te geven of op **[!UICONTROL Apply]** om de huidige inhoud te vervangen.

1. Navigeer naar de optie **[!UICONTROL Refine]** in het **[!UICONTROL Preview]** -venster voor toegang tot extra aanpassingsfuncties:

   * **[!UICONTROL Use as reference content]**: De gekozen variant fungeert als referentie-inhoud voor het genereren van andere resultaten.
   * **[!UICONTROL Elaborate]**: ga verder met specifieke onderwerpen en geef meer details voor een beter begrip en betrokkenheid.
   * **[!UICONTROL Summarize]**: Beperk de belangrijkste punten tot duidelijke, beknopte samenvattingen om de aandacht te trekken en verdere lezing aan te moedigen.
   * **[!UICONTROL Rephrase]**: herhaal uw bericht op verschillende manieren, zodat u steeds fris schrijft en aantrekkelijk bent voor verschillende soorten publiek.
   * **[!UICONTROL Use simpler language]**: Vereenvoudig uw taal voor meer duidelijkheid en toegankelijkheid voor een groter publiek.
   * **[!UICONTROL Translate]**: Vereenvoudig uw taal voor meer duidelijkheid en toegankelijkheid voor een groter publiek.

   U kunt ook de **[!UICONTROL Tone]** en **[!UICONTROL Communication strategy]** van de tekst wijzigen.

   ![&#x200B; Schermafbeelding die verfijnen opties in het Web van Adobe Campaign toont &#x200B;](assets/text-genai-5.png){zoomable="yes"}

1. Open het **[!UICONTROL Brand Alignment]** lusje om te zien hoe uw inhoud zich op uw [&#x200B; merkrichtlijnen &#x200B;](../content/brands.md) richt.

1. Klik op **[!UICONTROL Select]** als u de juiste inhoud hebt gevonden.

1. Voeg verpersoonlijkingsgebieden in om uw inhoud aan te passen die op profielgegevens wordt gebaseerd. Klik vervolgens op de knop **[!UICONTROL Simulate content]** om de rendering te beheren en controleer de instellingen voor aanpassing met testprofielen. [Meer informatie](../preview-test/preview-content.md)

1. Bekijk en activeer uw inhoud:
   * **E-mail**: Wanneer u uw inhoud, publiek en programma hebt bepaald, bent u klaar om uw e-maillevering voor te bereiden. [Meer informatie](../monitor/prepare-send.md)
   * **het Bestaan Pagina**: Zodra uw het landen pagina klaar is, kunt u het publiceren om het voor gebruik in een bericht ter beschikking te stellen. [Meer informatie](../landing-pages/create-lp.md)

## Voor mobiele kanalen {#mobile-channels}

Met AI Assistant kunt u aansprekende tekstinhoud voor uw pushberichten en SMS-berichten genereren, zodat u aantrekkelijke mobiele communicatie kunt maken die verbinding maakt met uw publiek op alle mobiele aanraakpunten.

### Toegang en configuratie {#mobile-access-configure}

Voordat u begint met het genereren van tekst met AI Assistant voor mobiele kanalen, moet u de levering instellen en de AI-assistent openen.

1. Uw mobiele levering maken en configureren:
   * **Duw berichten**: Na het creëren van en het vormen van uw levering van het dupbericht, klik **[!UICONTROL Edit content]**. [Meer informatie](../push/create-push.md)
   * **SMS**: Na het creëren van en het vormen van uw levering van SMS, klik **[!UICONTROL Edit content]**. [Meer informatie](../sms/create-sms.md)

1. Pas uw bericht naar wens aan:
   * **duw berichten**: [&#x200B; Leer meer &#x200B;](../push/content-push.md)
   * **SMS**: [&#x200B; Leer meer &#x200B;](../sms/content-sms.md)

1. Open het menu **[!UICONTROL Show AI Assistant]** .

   ![&#x200B; Schermafbeelding die het Hulpmenu van AI van de Show tonen &#x200B;](assets/sms-genai-1.png){zoomable="yes"} toont

### Inhoud genereren {#mobile-generate-content}

Zodra u AI Assistant hebt benaderd, kunt u de instellingen voor generatie configureren om mobiele inhoud te maken die aansluit bij uw merk- en leveringsdoelen. Pas tekstparameters aan, voeg merkelementen toe en geef instructies om AI te begeleiden bij het genereren van relevante variaties.

1. Selecteer **[!UICONTROL Brand]** om te zorgen dat door AI gegenereerde inhoud wordt uitgelijnd op de specificaties van uw merk. [&#x200B; leer meer &#x200B;](brands.md) op Banden.

1. Verfijn de inhoud door te beschrijven wat u wilt genereren in het veld **[!UICONTROL Prompt]** .

   Als u hulp bij het ontwerpen van uw herinnering zoekt, toegang **[!UICONTROL Prompt Library]** die een diverse waaier van snelle ideeën verstrekt om uw levering te verbeteren. [&#x200B; Leer meer op snelle beste praktijken &#x200B;](ai-assistant-prompting-guide.md)

   ![&#x200B; AI Medewerker met het gebied en de opties van de Vragen &#x200B;](assets/sms-genai-2.png){zoomable="yes"}

1. **voor Push berichten**, kies het tekstgebied u wilt produceren: **[!UICONTROL Title]**, **[!UICONTROL Subtitle]** en/of **[!UICONTROL Message]**.

1. Volg uw vraag met de optie **[!UICONTROL Text settings]** :

   * **[!UICONTROL Communication strategy]**: Kies de meest geschikte communicatiestijl voor de gegenereerde tekst.
   * **[!UICONTROL Languages]**: kies de taal van de gegenereerde inhoud.
   * **[!UICONTROL Tone]**: De toon zou met uw publiek moeten resoneren. Of u informatief wilt klinken, playful, of overtuigend, AI Medewerker kan het bericht dienovereenkomstig aanpassen.
   * **[!UICONTROL Length]**: selecteer de lengte van de inhoud met de schuifregelaar voor het bereik.

     ![&#x200B; het instellingenpaneel van de Tekst &#x200B;](assets/sms-genai-3.png){zoomable="yes"}

1. Klik in het menu **[!UICONTROL Reference content]** op **[!UICONTROL Upload file]** om een merkelement toe te voegen dat inhoud bevat die extra context-AI-assistent kan bieden of selecteer een eerder geüpload element.

   Eerder geüploade bestanden zijn beschikbaar in de vervolgkeuzelijst **[!UICONTROL Uploaded reference content]** . Schakel eenvoudig de elementen in die u wilt opnemen in uw generatie.

1. Klik op **[!UICONTROL Generate]** als de vraag gereed is.

### Verfijnen en voltooien {#mobile-refine-finalize}

Nadat u tekstvariaties voor uw mobiele berichten hebt gegenereerd, kunt u de resultaten afstemmen om ervoor te zorgen dat deze precies aan uw vereisten voldoen. Controleer de uitlijning van het merk, pas de toon en de taal aan en bereid de inhoud voor activering.

1. Blader na het genereren door de **[!UICONTROL Variations]** .

1. Klik op het percentagepictogram om uw **[!UICONTROL Brand Alignment Score]** weer te geven en eventuele onjuiste uitlijningen met uw merk te identificeren.

   Leer meer op [&#x200B; de groeperingsscore van het Merk &#x200B;](brands-score.md).

   ![&#x200B; verfijnen menu &#x200B;](assets/sms-genai-4.png){zoomable="yes"}

1. Klik op **[!UICONTROL Preview]** om een schermvullende versie van de geselecteerde variant weer te geven of klik op **[!UICONTROL Apply]** om de huidige inhoud te vervangen.

1. Navigeer naar de optie **[!UICONTROL Refine]** in het **[!UICONTROL Preview]** -venster voor toegang tot extra aanpassingsfuncties:

   * **[!UICONTROL Use as reference content]**: De gekozen variant zal als verwijzingsinhoud voor het produceren van andere resultaten dienen.

   * **[!UICONTROL Rephrase]**: herschrijf het bericht terwijl de betekenis behouden blijft. Met deze optie kunt u alternatieve bewoordingen genereren, de stroom verbeteren of de formulering aanpassen zonder het kernbericht te wijzigen.

   * **[!UICONTROL Use simpler language]**: Gebruik AI Assistant om uw taal te vereenvoudigen, zodat een groter publiek helderheid en toegankelijkheid krijgt.

   * **[!UICONTROL Translate]**: Vereenvoudig uw taal voor meer duidelijkheid en toegankelijkheid voor een groter publiek.

   * **[!UICONTROL Change tone]**: pas de toon van het bericht aan om uw communicatie stijl beter aan te passen, d.w.z. het vriendelijker, professioneel, dringend, of inspirerend te maken.

   * **[!UICONTROL Change Communication strategy]**: wijzig de berichtenbenadering op basis van uw doelstellingen, zoals het creëren van urgentie, of het benadrukken van opwindende aantrekkingskracht.

     ![&#x200B; Gegenereerde tekstvariaties met de Score van de Uitlijning van het Merk &#x200B;](assets/sms-genai-5.png){zoomable="yes"}

1. Open het **[!UICONTROL Brand Alignment]** lusje om te zien hoe uw inhoud zich op uw [&#x200B; merkrichtlijnen &#x200B;](brands.md) richt.

1. Klik op **[!UICONTROL Select]** zodra u de juiste inhoud hebt gevonden.

1. Voeg verpersoonlijkingsgebieden in om uw inhoud aan te passen die op profielgegevens wordt gebaseerd. Klik vervolgens op de knop **[!UICONTROL Simulate content]** om de rendering te beheren en controleer de instellingen voor aanpassing met testprofielen. [Meer informatie](../personalization/personalize.md)

1. Bekijk en activeer uw inhoud:
   * **Push bericht**: Wanneer u uw inhoud, publiek en programma hebt bepaald, bent u bereid om uw levering van het dupbericht voor te bereiden. [Meer informatie](../push/send-push.md)
   * **SMS**: Zodra uw SMS klaar is, kunt u het publiceren om het voor gebruik in een bericht ter beschikking te stellen. [Meer informatie](../sms/send-sms.md)
