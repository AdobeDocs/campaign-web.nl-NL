---
audience: end-user
title: Aan de slag met de AI Assistant
description: Aan de slag met de AI Assistant
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
source-git-commit: 3729a6159affbbb30d2cdab91d1e42dbf9df9c86
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 1%

---

# Werken met de AI Assistant {#generative-gs}


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
>title="Adobe Generative AI-termen"
>abstract="Voor toegang tot deze functie moet u akkoord gaan met de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen. Controleer de nauwkeurigheid van de uitvoer van deze functie en zorg ervoor dat deze geschikt is voor uw gebruiksscenario."
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generative AI-gebruikersrichtlijnen"

>[!INFO]
>
>Ga in een hands-on ervaring met [ binnen onze levende eigenschapvoorproef ](https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator), die wordt ontworpen om u zijn eigenschappen te laten onderzoeken en volledig zijn mogelijkheden te begrijpen.


Naarmate de marketing-industrie concurrerender wordt, zoeken merken efficiënte manieren om op efficiënte en snelle wijze effectvolle inhoud te genereren. AI Assistant in Adobe Campaign Web, aangedreven door Microsoft Azure OpenAI en Adobe Firefly, is een Adobe AI-functie voor het genereren van inhoud die een revolutie betekent in de manier waarop marketers professionele en merkconsistente inhoud maken op verschillende kanalen, zoals E-mail, SMS, Push. Met geavanceerde GenAI-modellen en een goed begrip van de richtlijnen voor merken genereert AI Assistant automatisch persoonlijke, aantrekkelijke en effectieve inhoud die is gebaseerd op het marketingdoel, met inhoud die is geoptimaliseerd voor stijlen, lay-outs, kleurtinten en meer met een merk.

Met AI Assistant kunt u marketingcampagnes op verschillende kanalen, zoals e-mail, SMS en Push, intuïtief, eenvoudig en probleemloos maken en tegelijk tijd besparen, de efficiëntie verbeteren en betere resultaten behalen.

>[!IMPORTANT]
>
>* Alvorens te beginnen gebruikend dit vermogen, lees uit verwante [ Grafieken en Beperkingen ](#generative-guardrails).
>
>* U moet met a [ gebruikersovereenkomst ](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html) akkoord gaan alvorens u de Medewerker AI in het Web van Adobe Campaign kunt gebruiken. Neem voor meer informatie contact op met uw Adobe-vertegenwoordiger.

## De AI-assistent openen {#generative-access}

De AI Assistant voor e-mails, pushberichten en SMS bevindt zich nu in de algemene beschikbaarheid (GA) en is beschikbaar voor alle gebruikers. Vereiste machtigingen en stappen voor het verlenen van toegang aan gebruikers worden hieronder beschreven.

+++  Leer hoe u machtigingen voor het genereren van inhoud toewijst

1. **creeer het Profiel van het Product** - in [ Admin Console ](https://stage.adminconsole.adobe.com/) creeer een productprofiel met het volgende specifieke patroon:
   `Campaign - <instance-name> - AIAssistant`

1. **voeg gebruikers** toe - voeg vereiste gebruiker aan dat productprofiel toe,
of
   **creeer de Groep van de Gebruiker** en voeg die gebruikersgroep aan productprofiel toe en voeg gebruikers aan dat productprofiel toe.

Leer hoe te om toestemmingen in Campagne in [ te bepalen deze sectie ](../get-started/permissions.md).

+++

## Afvoerkanalen en beperkingen {#generative-guardrails}

De algemene richtlijnen voor het gebruik van de AI Assistant in Adobe Campaign Web voor het genereren van e-mail worden hieronder weergegeven:

* De kwaliteit van de gegenereerde inhoud wordt sterk beïnvloed door het marketingdoel dat/de marketingprompt die u definieert. Gebruik een duidelijk gedefinieerde prompt voor een juiste interpretatie van het GenAI-model. 
* Upload merkmiddelen voor nauwkeurige informatie over de inhoud van het merk. Anders is de inhoud gebaseerd op algemeen beschikbare informatie. De geüploade inhoud kan de volgende indelingen hebben: PDF-, JPEG-, PNG- of ZIP-bestanden (met ondersteunde bestandsindelingen).
* De maximale grootte voor geüploade brandmiddelen is 50 MB. Grotere bestanden of veel afbeeldingen kunnen werken, maar de verwerkingstijd neemt toe.
* Het gebruik [ ingebouwde e-mailmalplaatjes ](../email/create-email-templates.md), merkspecifieke malplaatje of douanemalplaatje om uw e-mailinhoud tot stand te brengen gebruikend AI medewerker. E-mailsjablonen met maximaal 8-10 afbeeldingen worden aanbevolen.
* Zorg ervoor dat u eventuele problematische uitvoerbestanden meldt met het blokje omhoog, omlaag of de vlagpictogrammen bij het selecteren van varianten.
* Op het gebruik van de AI-assistent zijn de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen van toepassing. [Meer informatie](https://www.adobe.com/legal/licenses-terms/adobe-dx-gen-ai-user-guidelines.html)
* Als onderdeel van de toezegging van Adobe om de transparantie bij het gebruik van generatieve AI-tools bij het maken van media te bevorderen, zal Adobe Content Credentials toepassen wanneer inhoud of een project dat een door Firefly gegenereerd element bevat, wordt gedownload of geëxporteerd. [Meer informatie](https://helpx.adobe.com/firefly/using/content-credentials.html)

De volgende beperkingen gelden voor AI Assistant in Adobe Campaign Web:

* AI Assistant in Adobe Campaign Web wordt momenteel alleen ondersteund in het Engels. Niet-Engelse invoer kan leiden tot inconsistente of onjuiste resultaten. Problemen die voortvloeien uit niet-Engelse antwoorden worden momenteel niet behandeld of verbeterd.
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
