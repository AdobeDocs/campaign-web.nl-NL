---
audience: end-user
title: Aan de slag met AI Assistant
description: Aan de slag met AI-assistent
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# Werken met AI-assistent {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI-assistent"
>abstract="Nadat u de levering hebt gemaakt en aangepast, gebruikt u AI Assistant om de inhoud te verbeteren. Deze functie vereenvoudigt personalisatie en de verbetering van de inhoud door u toe te staan om de inhoud te verfijnen door te beschrijven wat u wilt produceren."

>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Context definiëren met AI Assistant in Campagne"
>abstract="Om de geselecteerde inhoud als input voor inhoudsgeneratie te gebruiken, activeer **Verbeteren met huidige inhoud** knevel. U kunt ook uw merkmiddelen uploaden om deze als bron te gebruiken. Als u de geselecteerde inhoud niet gebruikt, zijn uploaden en selecteren van merkelementen verplicht."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Adobe Generative AI-termen"
>abstract="De toegang tot deze functie hangt af van uw toestemming voor de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen. Controleer of de uitvoer van deze functie nauwkeurig is en of deze geschikt is voor uw gebruiksscenario."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI-gebruikersrichtlijnen"

>[!INFO]
>
>Ga in een hands-on ervaring met [&#x200B; binnen onze levende eigenschapvoorproef &#x200B;](https://experienceleague.adobe.com/nl/apps/journey-optimizer/ai-assistant-content-accelerator), die wordt ontworpen om u zijn eigenschappen te laten onderzoeken en volledig zijn mogelijkheden te begrijpen.

Aangezien de marketing industrie concurrerender wordt, zoeken de merken efficiënte manieren om impactful inhoud snel te produceren. AI Assistant in Adobe Campaign Web, aangedreven door Microsoft Azure OpenAI en Adobe Firefly, is een Adobe AI-functie voor het genereren van inhoud die de manier transformeert waarop marketers professionele en merkconsistente inhoud maken via verschillende kanalen, zoals e-mail, SMS en pushberichten. Met geavanceerde GenAI-modellen en een goed begrip van de richtlijnen voor merken genereert AI Assistant automatisch persoonlijke, aantrekkelijke en effectieve inhoud op basis van het marketingdoel, waarbij de inhoud wordt geoptimaliseerd voor stijlen met een merknaam, lay-outs, kleurtinten en meer.

AI Assistant vereenvoudigt het maken en uitvoeren van marketingcampagnes via verschillende kanalen, zoals e-mail-, SMS- en pushmeldingen, bespaart tijd, verbetert de efficiëntie en maakt betere resultaten mogelijk.

>[!IMPORTANT]
>
>* Alvorens dit vermogen te gebruiken, herzie verwante [&#x200B; Grafieken en Beperkingen &#x200B;](#generative-guardrails).
>
>* U moet met a [&#x200B; gebruikersovereenkomst &#x200B;](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) akkoord gaan alvorens AI Medewerker in het Web van Adobe Campaign te gebruiken. Neem voor meer informatie contact op met uw Adobe-vertegenwoordiger.

## AI-assistent openen {#generative-access}

AI Assistant voor e-mails, pushmeldingen, bestemmingspagina en SMS bevindt zich nu in de algemene beschikbaarheid (GA) en is beschikbaar voor alle gebruikers. Vereiste machtigingen en stappen voor het verlenen van toegang aan gebruikers worden hieronder beschreven.

+++ Leer hoe u machtigingen voor het genereren van inhoud toewijst

1. **creeer het Profiel van het Product** - in [&#x200B; Admin Console &#x200B;](https://stage.adminconsole.adobe.com/), creeer een productprofiel met het volgende specifieke patroon:
   `Campaign - <instance-name> - AIAssistant`

1. **voeg gebruikers** toe - voeg de vereiste gebruiker aan dat productprofiel toe,\
   of\
   **creeer de Groep van de Gebruiker** en voeg die gebruikersgroep aan het productprofiel toe, dan voeg gebruikers aan dat productprofiel toe.

Leer hoe te om toestemmingen in Campagne in [&#x200B; te bepalen deze sectie &#x200B;](../get-started/permissions.md).

+++

## Afvoerkanalen en beperkingen {#generative-guardrails}

De algemene richtlijnen voor het gebruiken van AI Medewerker in het Web van Adobe Campaign voor e-mailgeneratie zijn hieronder vermeld:

* De kwaliteit van de gegenereerde inhoud hangt sterk af van het marketingdoel of de vraag die u definieert. Gebruik een duidelijk gedefinieerde prompt voor een juiste interpretatie van het GenAI-model.
* Upload merkmiddelen om nauwkeurige, on-brand inhoud te garanderen. Anders is de inhoud gebaseerd op openbaar beschikbare informatie. De geüploade inhoud kan de volgende indelingen hebben: PDF-, JPEG-, PNG- of ZIP-bestanden (met ondersteunde bestandsindelingen).
* De maximale grootte voor geüploade merkenmiddelen is 50 MB. Grotere bestanden of een groot aantal afbeeldingen kan de verwerkingstijd verhogen.
* Gebruik [&#x200B; ingebouwde e-mailmalplaatjes &#x200B;](../content/create-email-templates.md), merkspecifieke malplaatjes, of douanesjablonen om uw e-mailinhoud tot stand te brengen gebruikend AI Medewerker. E-mailsjablonen met maximaal 8-10 afbeeldingen worden aanbevolen.
* Geef bij het selecteren van varianten aan welke problematische uitvoer dan ook de pictogrammen thumbs-up, thumbs-down of Markering moet gebruiken.
* Op uw gebruik van AI Assistant zijn de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen van toepassing. [Meer informatie](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html).
* Als onderdeel van de Adobe-toezegging om het gebruik van generatieve AI-gereedschappen bij het maken van media transparant te maken, past Adobe Content Credentials toe wanneer inhoud of een project dat een door Firefly gegenereerd element bevat, wordt gedownload of geëxporteerd. [Meer informatie](https://helpx.adobe.com/nl/firefly/using/content-credentials.html).

De volgende beperkingen gelden voor AI Assistant in Adobe Campaign Web:

* AI Assistant in Adobe Campaign Web wordt momenteel alleen ondersteund in het Engels. Niet-Engelse invoer kan leiden tot inconsistente of onjuiste resultaten. Kwesties die voortvloeien uit niet-Engelse antwoorden zullen op dit moment niet worden behandeld of verbeterd.
* Alleen beschikbaar voor de e-mail-, push- en SMS-kanalen.
* GenAI-inhoud is mogelijk niet altijd nauwkeurig. Deel uw feedback zodat engineers de modellen kunnen verfijnen.
* U kunt meerdere merkmiddelen uploaden, maar u kunt slechts één voor een specifieke generatie gebruiken.

## Mogelijkheden voor het genereren van inhoud voor AI Assistant {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-full-content.md">
<img alt="[Volledige inhoud genereren met AI Assistant]" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-full-content.md"><strong> Volledige inhoudsgeneratie met Medewerker AI </strong></a>
</div>
<p>
</td>
<td>
<a href="generative-text.md">
<img alt="[Tekstinhoud genereren met AI Assistant]" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-text.md"><strong> generatie van de Tekst met AI Medewerker </strong>
</div>
<p>
</td>
<td>
<a href="generative-image.md">
<img alt="[Afbeelding genereren met AI Assistant]" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-image.md"><strong> generatie van het Beeld met AI Medewerker </strong></a>
</div>
<p></td>
</tr></table>