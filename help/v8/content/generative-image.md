---
audience: end-user
title: Generatieve inhoud
description: Leer hoe u afbeeldingen genereert met AI Assistant
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 2%

---

# Afbeeldingen genereren met AI Assistant {#generative-image}

>[!IMPORTANT]
>
>Alvorens te beginnen om dit vermogen te gebruiken, lees verwante [&#x200B; Grafieken en Beperkingen &#x200B;](generative-gs.md#generative-guardrails).
></br>
>
>U moet met a [&#x200B; gebruikersovereenkomst &#x200B;](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html){target="_blank"} akkoord gaan alvorens AI Medewerker in het Web van Adobe Campaign te gebruiken. Neem voor meer informatie contact op met uw Adobe-vertegenwoordiger.

Met AI Assistant in Adobe Campaign Web kunt u aansprekende visuele inhoud maken die uw berichten verbetert via e-mail, webpagina&#39;s, bestemmingspagina&#39;s en pushberichten. Met AI Assistant kunt u afbeeldingen genereren en optimaliseren, zodat uw inhoud visueel aantrekkelijk is en uitgelijnd op uw merk.

## Voor e-mail- en landingspagina&#39;s {#email-web-channels}

Met AI Assistant kunt u complete visuele ervaringen genereren voor uw e-mailcampagnes en bestemmingspagina&#39;s. Met deze functie kunt u on-brand, opvallende afbeeldingen produceren die op digitale aanraakpunten op uw publiek passen.

### Toegang en configuratie {#access-configure}

Als u afbeeldingen wilt genereren met AI Assistant, stelt u eerst de levering in en opent u de inhoudeditor. Voer de onderstaande stappen uit om uw werkruimte voor te bereiden en het deelvenster AI Assistant te openen.

1. Creeer en vorm uw levering:

   * **E-mail**: Na het creëren van en het vormen van uw e-maillevering, klik **[!UICONTROL Edit content]**. [Meer informatie](../email/create-email-content.md)
   * **het Bestaan Pagina**: Na het creëren van en het vormen van uw het landen pagina, klik **[!UICONTROL Edit content]**. [Meer informatie](../landing-pages/create-lp.md)

1. Selecteer het element dat u wilt wijzigen met AI Assistant en open het menu **[!UICONTROL AI Assistant]** .

   ![&#x200B; Screenshot die de selectie van de tekstcomponent in het Web van Adobe Campaign toont &#x200B;](assets/image-genai-1.png){zoomable="yes"}

### Inhoud genereren {#generate-content}

1. Schakel de optie **[!UICONTROL Reference style]** voor AI Assistant in om nieuwe inhoud aan te passen op basis van de geselecteerde inhoud.

1. Selecteer **[!UICONTROL Brand]** om te zorgen dat door AI gegenereerde inhoud wordt uitgelijnd op de specificaties van uw merk. [&#x200B; leer meer &#x200B;](brands.md) op Banden.

1. Stel de inhoud nauwkeurig af door te beschrijven wat u wilt genereren in het veld **[!UICONTROL Prompt]** .

   Als u hulp nodig hebt die uw herinnering creeert, toegang **[!UICONTROL Prompt Library]**, die een diverse waaier van snelle ideeën verstrekt om uw leveringen te verbeteren. [&#x200B; Leer meer op snelle beste praktijken &#x200B;](ai-assistant-prompting-guide.md)

   ![&#x200B; Schermafbeelding die snelle bibliotheek voor beeldgeneratie tonen in het Web van Adobe Campaign &#x200B;](assets/image-genai-2.png){zoomable="yes"}

1. Tik uw vraag met de optie **[!UICONTROL Image settings]** :

   * **[!UICONTROL Aspect ratio]** - Bepaal de breedte en hoogte van het element. Kies van gemeenschappelijke verhoudingen zoals 16 :9, 4 :3, 3 :2, of 1 :1, of ga een douanegrootte in.
   * **[!UICONTROL Content type]**: Categoriseer de aard van het visuele element, waarbij onderscheid wordt gemaakt tussen verschillende vormen van visuele representatie, zoals foto&#39;s, afbeeldingen of illustraties.
   * **[!UICONTROL Visual intensity]**: U kunt de invloed van de afbeelding bepalen door de intensiteit aan te passen. Bij een lagere instelling (2) wordt het uiterlijk zachter, terwijl bij een hogere instelling (10) de afbeelding levendiger wordt.
   * **[!UICONTROL Color & tone]**: pas de algemene weergave van de kleuren en de sfeer of de sfeer die worden weergegeven aan.
   * **[!UICONTROL Lighting]**: wijzig de belichting in de afbeelding om de atmosfeer te bepalen en specifieke elementen te markeren.
   * **[!UICONTROL Composition]**: plaats elementen in het kader van de afbeelding.

     ![&#x200B; Schermafbeelding die beeldmontagesopties tonen in het Web van Adobe Campaign &#x200B;](assets/image-genai-4.png){zoomable="yes"}

1. Klik in het menu **[!UICONTROL Reference content]** op **[!UICONTROL Upload file]** om een merkelement toe te voegen dat inhoud bevat die extra context-AI-assistent kan bieden of selecteer een eerder geüpload element.

   Eerder geüploade bestanden zijn beschikbaar in de vervolgkeuzelijst **[!UICONTROL Uploaded reference content]** . Schakel eenvoudig de elementen in die u wilt opnemen in uw generatie.

1. Als u tevreden bent met de snelle configuratie, klikt u op **[!UICONTROL Generate]** .

### Verfijnen en voltooien {#refine-finalize}

1. Blader door het gegenereerde bestand **[!UICONTROL Variations]** .

1. Klik op het percentagepictogram om uw **[!UICONTROL Brand Alignment Score]** weer te geven en eventuele onjuiste uitlijningen met uw merk te identificeren.

   Leer meer op [&#x200B; de groeperingsscore van het Merk &#x200B;](../content/brands-score.md).

   ![](assets/image-genai-3.png){zoomable="yes"}

1. Klik op **[!UICONTROL Preview]** om een schermvullende versie van de geselecteerde variant weer te geven of op **[!UICONTROL Apply]** om de huidige inhoud te vervangen.

1. Kies **[!UICONTROL Generate Similar]** als u verwante afbeeldingen met deze variant wilt weergeven.

1. Open het **[!UICONTROL Brand Alignment]** lusje om te zien hoe uw inhoud zich op uw [&#x200B; merkrichtlijnen &#x200B;](../content/brands.md) richt.

1. Klik op **[!UICONTROL Select]** als u de juiste inhoud hebt gevonden.

1. Nadat u de inhoud van uw bericht hebt gedefinieerd, klikt u op de knop **[!UICONTROL Simulate content]** om de weergave te beheren en de instellingen voor aanpassing te controleren met testprofielen. [Meer informatie](../preview-test/preview-content.md)

1. Bekijk en activeer uw inhoud:
   * **E-mail**: Wanneer u uw inhoud, publiek en programma hebt bepaald, bent u klaar om uw e-maillevering voor te bereiden. [Meer informatie](../monitor/prepare-send.md)
   * **het Bestaan Pagina**: Zodra uw het landen pagina klaar is, kunt u het publiceren om het voor gebruik in een bericht ter beschikking te stellen. [Meer informatie](../landing-pages/create-lp.md)

## Voor mobiele kanalen {#mobile-channels}

Met AI Assistant kunt u aansprekende tekst genereren voor pushberichten en SMS-berichten, zodat u mobiele communicatie kunt maken die aandacht krijgt en op alle mobiele aanraakpunten op uw publiek kan reageren.

### Toegang en configuratie {#mobile-access-configure}

Als u tekst voor mobiele kanalen wilt genereren met AI Assistant, stelt u eerst de levering in en opent u de AI Assistant. De stappen voor toegang tot AI Assistant verschillen enigszins, afhankelijk van het feit of u werkt met pushberichten of SMS-berichten.

1. Uw mobiele levering maken en configureren:

   * **Duw berichten**: Na het creëren van en het vormen van uw levering van het dupbericht, klik **[!UICONTROL Edit content]**. [Meer informatie](../push/create-push.md)
   * **SMS**: Na het creëren van en het vormen van uw levering van SMS, klik **[!UICONTROL Edit content]**. [Meer informatie](../sms/create-sms.md)

1. Vul **[!UICONTROL Basic details]** in voor levering. Klik op **[!UICONTROL Edit content]** als u klaar bent.

1. Pas uw bericht naar wens aan:

   * **duw berichten**: [&#x200B; Leer meer &#x200B;](../push/content-push.md)
   * **SMS**: [&#x200B; Leer meer &#x200B;](../sms/content-sms.md)

1. Open het menu **[!UICONTROL Show AI Assistant]** .

   ![&#x200B; Schermafbeelding die het Hulpmenu van AI van de Show tonen &#x200B;](assets/push-img-1.png){zoomable="yes"} toont

### Inhoud genereren {#mobile-generate-content}

Nadat u de AI Assistant hebt geopend, kunt u de instellingen voor het genereren van afbeeldingen aanpassen en afbeeldingen maken die zijn afgestemd op uw merk en die uw doelstellingen ondersteunen.

1. Selecteer **[!UICONTROL Brand]** om te zorgen dat door AI gegenereerde inhoud wordt uitgelijnd op de specificaties van uw merk. [&#x200B; leer meer &#x200B;](brands.md) op Banden.

1. Verfijn de inhoud door te beschrijven wat u wilt genereren in het veld **[!UICONTROL Prompt]** .

   Als u hulp bij het ontwerpen van uw herinnering zoekt, toegang **[!UICONTROL Prompt Library]** die een diverse waaier van snelle ideeën verstrekt om uw campagnes te verbeteren. [&#x200B; Leer meer op snelle beste praktijken &#x200B;](ai-assistant-prompting-guide.md)

   ![&#x200B; AI Medewerker met het gebied en de opties van de Vragen &#x200B;](assets/push-img-2.png){zoomable="yes"}

1. Selecteer **[!UICONTROL Image]** als u alleen elementen wilt genereren.

1. Kies uw **[!UICONTROL Image settings]** :

   * **[!UICONTROL Content type]**: Categoriseer de aard van het visuele element, waarbij onderscheid wordt gemaakt tussen verschillende vormen van visuele representatie, zoals foto&#39;s, afbeeldingen of illustraties.
   * **[!UICONTROL Visual intensity]**: U kunt de invloed van de afbeelding bepalen door de intensiteit aan te passen. Bij een lagere instelling (2) wordt het uiterlijk zachter en minder sterk, terwijl bij een hogere instelling (10) de afbeelding levendiger en visueel krachtiger wordt.
   * **[!UICONTROL Lighting]**: pas de belichting in de afbeelding aan om de atmosfeer te bepalen en specifieke elementen te markeren.
   * **[!UICONTROL Composition]**: plaats elementen in het kader van de afbeelding.

     ![&#x200B; Schermafbeelding die de montagesopties van het Beeld tonen &#x200B;](assets/push-img-3.png){zoomable="yes"}

1. Klik in het menu **[!UICONTROL Reference content]** op **[!UICONTROL Upload file]** om een merkelement toe te voegen dat inhoud bevat die extra context-AI-assistent kan bieden of selecteer een eerder geüpload element.

   Eerder geüploade bestanden zijn beschikbaar in de vervolgkeuzelijst **[!UICONTROL Uploaded reference content]** . Schakel eenvoudig de elementen in die u wilt opnemen in uw generatie.

1. Klik op **[!UICONTROL Generate]** als de vraag gereed is.

### Verfijnen en voltooien {#mobile-refine-finalize}

Nadat u variaties in de afbeelding voor uw mobiele berichten hebt gegenereerd, kunt u de resultaten perfectioneren om ervoor te zorgen dat deze precies aan uw vereisten voldoen.

1. Blader na het genereren door de **[!UICONTROL Variations]** .

1. Klik op het percentagepictogram om uw **[!UICONTROL Brand Alignment Score]** weer te geven en eventuele onjuiste uitlijningen met uw merk te identificeren.

   Leer meer op [&#x200B; de groeperingsscore van het Merk &#x200B;](../content/brands-score.md).

   ![](assets/push-img-4.png){zoomable="yes"}

1. Klik op **[!UICONTROL Preview]** om door **[!UICONTROL Variations]** te bladeren.

1. Open het **[!UICONTROL Brand Alignment]** lusje om te zien hoe uw inhoud zich op uw [&#x200B; merkrichtlijnen &#x200B;](brands.md) richt.

1. Klik op **[!UICONTROL Select]** zodra u de juiste inhoud hebt gevonden.

Zodra u de inhoud, het publiek en het programma hebt gedefinieerd, bereidt u de levering voor. [Meer informatie](../monitor/prepare-send.md)
