---
audience: end-user
title: Aan de slag met de AI Assistant
description: Aan de slag met de AI Assistant
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: 7de6d85036eac7289e7fcf3a82a7c11be12d9c6e
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# Aan de slag met de AI Assistant {#generative-gs}

>[!BEGINSHADEBOX]

**Lijst van inhoud**

* Aan de slag met de AI Assistant
* [E-mailgeneratie met AI Assistant](generative-content.md)
* [SMS genereren met de AI Assistant](generative-sms.md)
* [Pushmeldingen genereren met de AI Assistant](generative-push.md)

>[!ENDSHADEBOX]

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

Naarmate de marketing-industrie concurrerender wordt, zoeken merken efficiënte manieren om op efficiënte en snelle wijze effectvolle inhoud te genereren. AI Assistant in Campaign, aangedreven door Azure OpenAI, is de AI-functionaliteit van Adobe voor het genereren van inhoud die een revolutie betekent in de manier waarop marketers professionele en merkconsistente inhoud maken op verschillende kanalen, zoals E-mail, SMS, Push. Met geavanceerde GenAI-modellen en een goed begrip van de richtlijnen voor merken genereert AI Assistant automatisch persoonlijke, aantrekkelijke en effectieve inhoud die is gebaseerd op het marketingdoel, met inhoud die is geoptimaliseerd voor stijlen, lay-outs, kleurtinten en meer met een merk.

Met AI Assistant kunt u marketingcampagnes op verschillende kanalen, zoals e-mail, SMS en Push, intuïtief, eenvoudig en probleemloos maken en tegelijk tijd besparen, de efficiëntie verbeteren en betere resultaten behalen.

>[!NOTE]
>
>Deze functie is beschikbaar in de Beta-versie en kan zonder voorafgaande kennisgeving worden gewijzigd.

## Afvoerkanalen en beperkingen {#generative-guardrails}

De algemene richtlijnen voor het gebruik van de AI-assistent in Campaign voor het genereren van e-mail worden hieronder weergegeven:

* De kwaliteit van de gegenereerde inhoud wordt sterk beïnvloed door het marketingdoel dat/de marketingprompt die u definieert. Gebruik een duidelijk gedefinieerde prompt voor een juiste interpretatie van het GenAI-model. 
* Upload merkmiddelen voor nauwkeurige informatie over de inhoud van het merk. Anders is de inhoud gebaseerd op algemeen beschikbare informatie. De geüploade inhoud kan de volgende indelingen hebben: PDF, JPEG, PNG- of ZIP-bestanden (met ondersteunde bestandsindelingen).
* De maximale grootte voor geüploade brandmiddelen is 50 MB. Grotere bestanden of veel afbeeldingen kunnen werken, maar de verwerkingstijd neemt toe.
* Gebruik een Adobe Campaign authored e-mailmalplaatjes, bij voorkeur [ ingebouwde e-mailmalplaatjes ](../email/create-email-templates.md), een merkspecifiek malplaatje of douanemalplaatje om uw e-mailinhoud tot stand te brengen. E-mailsjabloon met maximaal 8-10 afbeeldingen wordt aanbevolen.
* Zorg ervoor dat u eventuele problematische uitvoerbestanden meldt met het blokje omhoog, omlaag of de vlagpictogrammen bij het selecteren van varianten.
* Op het gebruik van de AI-assistent zijn de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen van toepassing. [Meer informatie](https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

De volgende beperkingen gelden voor AI Assistant in Campaign:

* Ondersteunde taal is alleen Engels.
* Alleen beschikbaar voor de e-mail-, push- en SMS-kanalen.
* GenAI-inhoud is mogelijk niet altijd correct: geef uw feedback zodat onze technici de modellen kunnen verfijnen.
* U kunt meerdere merkmiddelen uploaden, maar u kunt slechts één voor een specifieke generatie gebruiken.

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
