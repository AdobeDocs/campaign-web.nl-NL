---
title: Campagne v8 Web User Interface Opmerkingen bij vorige release
description: 2026 Campagne Web User Interface-releases
exl-id: 40735c57-94ae-4646-8c3d-68197569fbd4
source-git-commit: 0cc09a983d412889f2b734a5bfb30bf422247ec0
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Opmerkingen bij de release 2026 {#2026-release}

Deze pagina maakt een lijst van alle veranderingen en verbeteringen beschikbaar met **2026 versies**. De recentste versienota&#39;s zijn beschikbaar in [&#x200B; deze pagina &#x200B;](release-notes.md).

## Release van februari &#39;26 {#26-2-release}

_feb 17, 2026_

### Nieuwe functies {#26-2-features}

<!--table>
<thead>
<tr>
<th><strong>Delivery scheduling compute process</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now use a delivery scheduling compute process similar to the one available in Adobe Campaign Standard. This feature allows you to calculate sending dates based on recipient timezones, enabling you to send communications at the optimal time for each recipient. This is particularly useful for organizations operating across multiple timezones, as it allows you to target regions with different timezones using a single delivery configuration.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Themes in the Email Designer (Beta)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Themes provide an improved authoring experience for emails by allowing you to define reusable theme styles that fit your brand guidelines. You can now use theme variables in fragments, ensuring consistent styling across your email templates. This feature enables you to build emails faster with predefined modules that abstract content elements such as titles, descriptions, images, and links, while maintaining brand consistency.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Tijdlijnweergave in campagneoverzicht</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De campagnevoorraad bevat nu een tijdlijnweergave waarmee u campagnes in de loop van de tijd kunt visualiseren en beheren: schakelen tussen lijst en tijdlijn, navigeren per week, maand of dag, de knop Vandaag gebruiken om naar de huidige datum te gaan en campagnedetails (status, workflows, leveringen) openen in een rechterdeelvenster—met dezelfde filters en zoekopdracht als de lijstweergave.</p>
<p>Voor meer informatie, verwijs naar de <a href="../campaigns/manage-campaigns.md#timeline"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Schema authoring (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt schema's van het Web van de Campagne direct tot stand brengen en beheren Gebruikersinterface. Met deze functie kunt u nieuwe tabellen maken, bestaande schema's uitbreiden en aangepaste formulieren maken. U kunt de structuren van douanegegevens bepalen om uw specifieke bedrijfsbehoeften te steunen zonder toegang tot de Console van de Cliënt te vereisen.</p>
<p>Opmerking: deze mogelijkheid is alleen beschikbaar voor een aantal organisaties (Beperkte beschikbaarheid) en wordt in een toekomstige release globaal geïmplementeerd.</p>
<p>Voor meer informatie, verwijs naar de <a href="../administration/schemas.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<!--

### Improvement {#26-2-improvements}

* Brand guidelines now include a Colors section that defines standards for your brand's color system, ensuring consistent use of primary, secondary, accent, and neutral colors across all experiences. 
[Learn more](../content/brands-personalize.md)-->

## Release januari 1926 {#26-1-release}

_jan 27, 2026_

### Nieuwe functies {#26-1-features}

<table>
<thead>
<tr>
<th><strong>Meertalige leveringsmogelijkheden (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De meertalige leveringsfunctie is nu beschikbaar voor alle klanten (GA). Met deze functie kunt u meerdere berichten verzenden in verschillende talen in de Adobe Campaign Web User Interface. U kunt de standaardtaal van uw levering kiezen evenals de verschillende talen waarin de levering kan worden verzonden. U kunt deze leveringen ook voorvertonen in de talen die u hebt gekozen. 
<p>Voor meer informatie, verwijs naar de <a href="../msg/multilingual.md"> gedetailleerde documentatie </a>.</p>
<p>De meertalige pushmeldingen zijn als volgt verbeterd:</p>
<ul>
<li>U kunt nu snel alle taalvarianten vullen door een CSV-bestand te uploaden dat uw meertalige inhoud bevat. <a href="../msg/multilingual.md#csv-upload"> las meer </a>
</li>
<li>Rijke pushmeldingen worden nu ondersteund.</li>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Profielverrijking in Transactieberichten (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De profielverrijking in Transactionele Berichten is nu beschikbaar aan alle klanten (GA). Naast e-mails worden nu ook SMS- en pushberichten ondersteund. Met deze functie kunt u transactieberichten personaliseren door Adobe Campaign-databasevelden te koppelen aan de inhoud van het bericht. U kunt doeltoewijzingen, verrijkingskolommen, en een verzoeningssleutel selecteren om nauwkeurige, real-time verpersoonlijking te verzekeren terwijl het handhaven van prestatiesdrempels.</p>
<p>Voor meer informatie, verwijs naar de <a href="../transactional-messaging/profile-enrichment.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Adobe Experience Manager-kopieën voor levende en talen</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Dankzij de integratie van Adobe Experience Manager-inhoud hebt u tijdens het maken van leveringen rechtstreeks toegang tot alle taal en live kopieën die in Adobe Experience Manager zijn gemaakt. U kunt inhoud in real time vernieuwen om de nieuwste Adobe Experience Manager-versies op te halen. Deze integratie voorkomt handmatige synchronisatie van inhoud tussen Adobe Experience Manager en Campagne en stroomlijnt uw meertalige campagneworkflow.</p>
<p>Voor meer informatie, verwijs naar de <a href="../integrations/aem-multilingual.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Inhoudsexperimenten - A/B-tests</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Met contentexperimenten in Adobe Campaign Web kunt u meerdere leveringsvarianten voor A/B-tests definiëren om te meten welke het beste voor uw doelpubliek presteert. U kunt de leveringsinhoud, het onderwerp, of de afzender variëren om verschillende versies te testen en te bepalen welke variant de beste resultaten veroorzaakt. U kunt A/B-tests uitvoeren op verschillende e-mailelementen, zoals onderwerpregel, naam van de afzender en e-mailinhoud.</p>
<p>Voor meer informatie, verwijs naar de <a href="../email/ab-testing.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Continue leveringsactiviteit</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Met de activiteit Continue levering kunt u nieuwe ontvangers toevoegen aan een bestaande levering. Dit leveringstype vermijdt het moeten een nieuwe levering tot stand brengen telkens als, die het voor laagvolumealarm of berichten efficiënter maakt die worden verzonden zoals nodig. Een ononderbroken levering leidt tot één enkele leveringsinstantie. Alle leveringslogbestanden (wideLog) en trackinglogboeken verwijzen naar deze ene levering, waardoor de bewaking en rapportage worden vereenvoudigd.</p>
<p>Voor meer informatie, verwijs naar de <a href="../workflows/activities/continuous-delivery.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Goedkeuringsbeheer voor campagnes</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Het goedkeuringsproces helpt meerdere belanghebbenden te coördineren en zorgt voor kwaliteitscontrole voordat leveringen worden verzonden. Gebruik goedkeuringen wanneer uw organisatie validatie van verschillende teams vereist, zoals marketingmanagers die inhoud controleren of gegevensanalisten die doelgroepen valideren.</p>
<p>Voor meer informatie, verwijs naar de <a href="../campaigns/campaign-approvals.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

### Verbeteringen {#26-1-improvements}

* Dynamische rapportage ondersteunt nu pushberichten en SMS. [&#x200B; Leer meer &#x200B;](../reporting/dynamic-reporting/get-started-reporting.md)
* Vooraf gedefinieerde filters - Met een nieuwe optie Gedeeld filter kunt u een vooraf gedefinieerd filter beschikbaar maken voor andere gebruikers in uw organisatie. [&#x200B; Leer meer &#x200B;](../get-started/predefined-filters.md#share-filter)
* Velden voor persoonlijke voorkeur die zijn gemaakt in Adobe Experience Manager, zoals Naam, E-mail, Datum en adres, worden nu opgenomen en beschikbaar wanneer u de inhoudssjabloon gebruikt.
* De evaluatie van de kwaliteit van de inhoud controleert nu op leesbaarheid, coherentie, en doeltreffendheid kwesties onafhankelijk van merkrichtlijnen, het identificeren van onduidelijk overseinen, inconsistente toon, of structurele hiaten. [&#x200B; Leer meer &#x200B;](../content/brands-score.md)
