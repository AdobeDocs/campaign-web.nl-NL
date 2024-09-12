---
audience: end-user
title: Aan de slag met de AI Assistant Content Accelerator
description: Aan de slag met de AI Assistant Content Accelerator
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: aea828da825a416dece6c4bee1da6d4e570e4e48
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 1%

---

# Werken met de AI Assistant Content Accelerator  {#generative-gs}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="AI Assistant-versnelling voor inhoud"
>abstract="Met AI Assistant kunt u marketingcampagnes op verschillende kanalen, zoals e-mail, SMS en Push, intuïtief, eenvoudig en probleemloos maken en tegelijk tijd besparen, de efficiëntie verbeteren en betere resultaten behalen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"


>[!CONTEXTUALHELP]
>id="acw_generation_settings"
>title="AI-assistent"
>abstract="Nadat u de levering hebt gemaakt en gepersonaliseerd, kunt u de AI Assistant gebruiken om de inhoud te verbeteren. Deze functie vereenvoudigt het proces van personalisatie en inhoudverbetering door u toe te staan om de inhoud te verfijnen door te beschrijven wat u wilt produceren."


>[!CONTEXTUALHELP]
>id="acw_generation_context"
>title="Context definiëren met AI Assistant in Campagne"
>abstract="Om de geselecteerde inhoud als input voor inhoudsgeneratie te gebruiken, activeer **Verbeteren met huidige inhoud** knevel. U kunt ook uw merkmiddelen uploaden om deze als bron te gebruiken. Als u de geselecteerde inhoud niet gebruikt, zijn het uploaden en selecteren van merkelementen verplicht."

>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Algemene AI-termen voor Adobe"
>abstract="Voor toegang tot deze functie moet u akkoord gaan met de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen. Controleer de nauwkeurigheid van de uitvoer van deze functie en zorg ervoor dat deze geschikt is voor uw gebruiksscenario."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generation AI-gebruikersrichtlijnen"

>[!INFO]
>
>Ga in een hands-on ervaring met [ binnen onze interactieve demo ](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator), die wordt ontworpen om u zijn eigenschappen te laten onderzoeken en volledig zijn mogelijkheden te begrijpen.


Naarmate de marketing-industrie concurrerender wordt, zoeken merken efficiënte manieren om op efficiënte en snelle wijze effectvolle inhoud te genereren. AI Assistant in Adobe Campaign Web for Content Acceleration, aangedreven door Microsoft Azure OpenAI en Adobe Firefly, is de AI-functionaliteit van de Adobe voor het genereren van inhoud die een revolutie betekent in de manier waarop marketers professionele en merkconsistente inhoud creëren op verschillende kanalen, zoals E-mail, SMS en Push. Met geavanceerde GenAI-modellen en een goed begrip van de richtlijnen voor merken genereert AI Assistant automatisch persoonlijke, aantrekkelijke en effectieve inhoud die is gebaseerd op het marketingdoel, met inhoud die is geoptimaliseerd voor stijlen, lay-outs, kleurtinten en meer met een merk.

Met AI Assistant kunt u marketingcampagnes op verschillende kanalen, zoals e-mail, SMS en Push, intuïtief, eenvoudig en probleemloos maken en tegelijk tijd besparen, de efficiëntie verbeteren en betere resultaten behalen.

>[!IMPORTANT]
>
>* Alvorens te beginnen gebruikend dit vermogen, lees uit verwante [ Grafieken en Beperkingen ](#generative-guardrails).
>
>* U moet met a [ gebruikersovereenkomst ](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) akkoord gaan alvorens u de Medewerker AI in het Web van Adobe Campaign voor de Versnelling van de Inhoud kunt gebruiken. Neem voor meer informatie contact op met uw Adobe-vertegenwoordiger.

## De AI Assistant-versnelling voor inhoud openen {#generative-access}

De AI Assistant Content Accelerator voor e-mails, pushberichten en SMS is nu beschikbaar voor algemene beschikbaarheid (GA) en is beschikbaar voor alle gebruikers. Vereiste machtigingen en stappen voor het verlenen van toegang aan gebruikers worden hieronder beschreven.

+++  Leer hoe u machtigingen voor het genereren van inhoud toewijst

1. **creeer het Profiel van het Product** - in [ Admin Console ](https://stage.adminconsole.adobe.com/) creeer een productprofiel met het volgende specifieke patroon:
   `Campaign - <instance-name> - AIAssistant`

1. **voeg gebruikers** toe - voeg vereiste gebruiker aan dat productprofiel toe,
of
   **creeer de Groep van de Gebruiker** en voeg die gebruikersgroep aan productprofiel toe en voeg gebruikers aan dat productprofiel toe.

Leer hoe te om toestemmingen in Campagne in [ te bepalen deze sectie ](../get-started/permissions.md).

+++

## Afvoerkanalen en beperkingen {#generative-guardrails}

De algemene richtlijnen voor het gebruik van de AI-assistent in Adobe Campaign Web for Content Acceleration voor het genereren van e-mailberichten vindt u hieronder:

* De kwaliteit van de gegenereerde inhoud wordt sterk beïnvloed door het marketingdoel dat/de marketingprompt die u definieert. Gebruik een duidelijk gedefinieerde prompt voor een juiste interpretatie van het GenAI-model. 
* Upload merkmiddelen voor nauwkeurige informatie over de inhoud van het merk. Anders is de inhoud gebaseerd op algemeen beschikbare informatie. De geüploade inhoud kan de volgende indelingen hebben: PDF, JPEG, PNG- of ZIP-bestanden (met ondersteunde bestandsindelingen).
* De maximale grootte voor geüploade brandmiddelen is 50 MB. Grotere bestanden of veel afbeeldingen kunnen werken, maar de verwerkingstijd neemt toe.
* Gebruik [ ingebouwde e-mailmalplaatjes ](../email/create-email-templates.md), merkspecifiek malplaatje of douanemalplaatje om uw e-mailinhoud tot stand te brengen gebruikend de Versneller van de Inhoud. E-mailsjablonen met maximaal 8-10 afbeeldingen worden aanbevolen.
* Zorg ervoor dat u eventuele problematische uitvoerbestanden meldt met het blokje omhoog, omlaag of de vlagpictogrammen bij het selecteren van varianten.
* Op het gebruik van de AI-assistent zijn de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen van toepassing. [Meer informatie](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Als onderdeel van de toezegging van de Adobe om het gebruik van generatieve AI-tools bij het maken van media transparanter te maken, zal de Adobe Content credentials toepassen wanneer inhoud of een project dat een Firefly bevat, wordt gedownload of geëxporteerd. [Meer informatie](https://helpx.adobe.com/firefly/using/content-credentials.html)

De volgende beperkingen gelden voor AI Assistant in Adobe Campaign Web for Content Acceleration:

* AI Assistant in Adobe Campaign Web for Content Acceleration wordt momenteel alleen ondersteund in het Engels. Niet-Engelse invoer kan leiden tot inconsistente of onjuiste resultaten. Problemen die voortvloeien uit niet-Engelse antwoorden worden momenteel niet behandeld of verbeterd.
* Alleen beschikbaar voor de e-mail-, push- en SMS-kanalen.
* GenAI-inhoud is mogelijk niet altijd correct: geef uw feedback zodat onze technici de modellen kunnen verfijnen.
* U kunt meerdere merkmiddelen uploaden, maar u kunt slechts één voor een specifieke generatie gebruiken.

## Mogelijkheden voor het genereren van inhoud voor AI Assistant {#generative-features}

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="generative-content.md">
<img alt="E-mailgeneratie" src="assets/do-not-localize/text-genai.jpeg">
</a>
<div>
<a href="generative-content.md"><strong> E-mailgeneratie met de Medewerker AI </strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="SMS-generatie" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong> generatie van SMS met de Medewerker AI </strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Push generation" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong> het bericht van de duw generatie met de Medewerker AI </strong></a>
</div>
<p></td>
</tr></table>
