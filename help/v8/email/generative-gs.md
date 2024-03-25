---
audience: end-user
title: Aan de slag met de AI Assistant
description: Aan de slag met de AI Assistant
badge: label="Beta"
exl-id: 0d00cb47-e740-407c-ac42-824f2fee44a6
hide: true
hidefromtoc: true
source-git-commit: af67094638cfc3c5c64385203340918f0f8f2482
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# Aan de slag met de AI Assistant {#generative-gs}

>[!BEGINSHADEBOX]

**Inhoudsopgave**

* **[Aan de slag met de AI Assistant](generative-gs.md)**
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
>abstract="Als u de geselecteerde inhoud wilt gebruiken als invoer voor het genereren van inhoud, activeert u de optie **Verbeteren met huidige inhoud** schakelen. U kunt ook uw merkmiddelen uploaden om deze als bron te gebruiken. Als u de geselecteerde inhoud niet gebruikt, zijn het uploaden en selecteren van merkelementen verplicht."


>[!CONTEXTUALHELP]
>id="acw_emagica_generate"
>title="Algemene AI-termen voor Adobe"
>abstract="Voor toegang tot deze functie moet u akkoord gaan met de Adobe Experience Cloud Generative AI-gebruikersrichtlijnen. Alle aanwijzingen, contextgegevens of aanvullende informatie of andere gegevens die u aan deze functie verstrekt, moeten zijn gekoppeld aan een specifieke context, die uw brandingmaterialen, website-inhoud, gegevens, schema&#39;s voor dergelijke gegevens, sjablonen of andere vertrouwde documenten kan bevatten en geen persoonlijke gegevens mag bevatten (persoonlijke gegevens omvatten alles wat u terug kunt koppelen naar een specifiek individu). U moet de nauwkeurigheid van de uitvoer van deze functie controleren en controleren of deze geschikt is voor uw gebruiksgeval"
>additional-url="https://www.adobe.com/legal/licenses-terms/adobe-gen-ai-user-guidelines.html" text="Adobe Generation AI-gebruikersrichtlijnen"

De AI-assistent is een waardevol hulpmiddel voor het verbeteren van e-mailinhoud. Het vereenvoudigt personalisatie en inhoudsuitbreiding, die uw e-mailleveringen optimaliseren om beter op uw publiek af te stemmen.

Met deze functie bespaart u tijd en bent u verzekerd van consistente kwaliteit door automatisch volledige e-mailinhoud te genereren. Door gebruik te maken van Generative AI kunt u moeiteloos aansprekende e-mails maken, waardoor de effectiviteit en efficiëntie van uw communicatie worden verbeterd.

>[!NOTE]
>
>Deze mogelijkheid is beschikbaar in de versie van de Alpha en kan zonder voorafgaande kennisgeving worden gewijzigd. Het zal begin oktober in werking treden.

## Afvoerkanalen en beperkingen {#generative-guardrails}

De algemene richtlijnen voor het gebruik van de AI-assistent in Campaign voor het genereren van e-mail worden hieronder weergegeven:

* De kwaliteit van de gegenereerde inhoud wordt sterk beïnvloed door het marketingdoel dat/de marketingprompt die u definieert. Gebruik een duidelijk gedefinieerde prompt voor een juiste interpretatie van het GenAI-model. 
* Upload merkmiddelen voor nauwkeurige informatie over de inhoud van het merk. Anders is de inhoud gebaseerd op algemeen beschikbare informatie. De geüploade inhoud kan de volgende indelingen hebben: PDF, JPEG, PNG- of ZIP-bestanden (met ondersteunde bestandsindelingen).
* De aanbevolen grootte voor geüploade brandmiddelen is minder dan 50 MB. Grotere bestanden of veel afbeeldingen kunnen werken, maar de verwerkingstijd neemt toe.
* Gebruik bij voorkeur een door Adobe Campaign geschreven e-mailsjabloon [ingebouwde e-mailsjablonen](../email/create-email-templates.md), een merkspecifieke sjabloon of aangepaste sjabloon om uw e-mailinhoud te maken. E-mailsjabloon met maximaal 8-10 afbeeldingen wordt aanbevolen.


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
<a href="generative-content.md"><strong>E-mailgeneratie met AI Assistant</strong></a>
</div>
<p>
</td>
<td>
<a href="generative-sms.md">
<img alt="SMS-generatie" src="assets/do-not-localize/image-genai.jpeg">
</a>
<div><a href="generative-sms.md"><strong>SMS genereren met de AI Assistant</strong>
</div>
<p>
</td>
<td>
<a href="generative-push.md">
<img alt="Push generation" src="assets/do-not-localize/email-genai.jpeg">
</a>
<div>
<a href="generative-push.md"><strong>Pushmeldingen genereren met de AI Assistant</strong></a>
</div>
<p></td>
</tr></table>
