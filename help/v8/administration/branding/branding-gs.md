---
title: Branding
description: Ontdek alle tools die beschikbaar zijn om uw brandingsidentiteiten te beheren
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: f6438303-5ae8-47c6-8c34-8e586f4b6fe7
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 13%

---

# Aan de slag met branding {#branding-gs}

>[!AVAILABILITY]
>
>Deze mogelijkheid is alleen op verzoek beschikbaar voor nieuwe implementaties. Neem contact op met uw Adobe-vertegenwoordiger voor toegang.


>[!IMPORTANT]
>
>Merken kunnen niet door eindgebruikers worden gemaakt of gewijzigd. Deze bewerkingen moeten worden uitgevoerd door de technische beheerder van Adobe Campaign. Neem voor elk verzoek contact op met de klantenservice van Adobe.

Elk bedrijf heeft merkrichtlijnen die zowel visuele elementen als technische details bepalen. Adobe Campaign helpt u deze richtlijnen centraal te beheren, zodat u een consistent merkimago aan uw klanten kunt presenteren in alles wat u doet, van logo&#39;s in e-mails tot de URL&#39;s en domeinen die in uw campagnes worden gebruikt.

Technische beheerders kunnen meerdere merken binnen Adobe Campaign maken en beheren. Op deze manier kunt u alle elementen definiëren waaruit uw merkidentiteit bestaat, inclusief logo&#39;s en zelfs instellingen voor het bijhouden van e-mail. Nadat u deze merken hebt gemaakt, kunt u ze gemakkelijk koppelen aan uw leveringen.

U kunt nieuwe entiteiten van uw organisatie toevoegen in Campagne, of een nieuw type van e-mail tot stand brengen dat u onder een verschillend subdomain moet verzenden. Volg onderstaande stappen om dit te doen:

1. **vorm een nieuw subdomain** - voor om het even welk nieuw subdomain dat door Adobe moet worden gebruikt, zal de eerste stap het vormen zijn. U kunt dit door [&#x200B; het Controlebord van de Campagne &#x200B;](https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html?lang=nl) uitvoeren of uit naar uw technisch contact van Adobe reiken. Leer meer over subdomeinconfiguratie [&#x200B; in deze pagina &#x200B;](https://experienceleague.adobe.com/nl/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/campaign/ac-domain-name-setup).

   >[!NOTE]
   >
   >Het configuratiescherm is toegankelijk voor alle gebruikers met beheerdersrechten. De stappen om toegang met beheerdersrechten aan een gebruiker te verlenen worden gedetailleerd beschreven op [deze pagina](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=nl#discover-control-panel).

1. **creeer een leveringsmalplaatje** - Zodra het nieuwe merk beschikbaar is, moeten de beste praktijken minstens één nieuw leeg leveringsmalplaatje tot stand brengen dat dit nieuwe merk van verwijzingen voorziet. [Meer informatie](branding-assign.md).

1. **de leveringsrichtlijnen van de Controle** - alvorens het beginnen gebruiken van het nieuwe domein, zou de strategie met het team van de Leverbaarheid van Adobe moeten worden besproken. Zij zullen helpen om de beste praktijken te bepalen, als een nieuwe affiniteit zou moeten worden gecreeerd om IPs tussen domeinen bijvoorbeeld te verdelen, en/of als een platforminplan zou moeten worden bepaald.

## Compatibiliteitsnotitie {#compatibility-note}

Het nieuwe gecentraliseerde branding model is niet compatibel met [&#x200B; erfenisbranding &#x200B;](https://experienceleague.adobe.com/docs/campaign-classic/using/transactional-messaging/configure-transactional-messaging/additional-configurations.htmml#configuring-multibranding){target="_blank"} configuratie die eerder in de Console van de Cliënt werd gebruikt.

In de erfenisbenadering, uitvoerden de klanten branding door de vorm uit te breiden extAccount en het **Brandend** tabel te gebruiken.

![](assets/branding-legacy.png)

Als uw bestaande omgeving deze oudere configuratie gebruikt, kan deze niet rechtstreeks worden gemigreerd naar het nieuwe gecentraliseerde brandingmodel. Voor de invoering van het nieuwe systeem is een volledige herimplementatie van de branding-instellingen vereist.