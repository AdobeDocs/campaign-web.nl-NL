---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 62e064b5a2e2c0d8b81755d2a8a9ea04c512e6f2
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 9%

---

# Aanvullende informatie  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie "
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

De veranderingen en de verbeteringen beschikbaar met vorige versies worden vermeld in [ 2024 ](release-notes-24.md) en [ 2025 ](release-notes-25.md) pagina&#39;s.

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
<p>Raadpleeg de <a href="../msg/multilingual.md">gedetailleerde documentatie</a> voor meer informatie.</p>
<p>De meertalige pushmeldingen zijn als volgt verbeterd:</p>
<ul>
<li>U kunt nu snel alle taalvarianten vullen door een CSV-bestand te uploaden dat uw meertalige inhoud bevat. <a href="../msg/multilingual.md#csv-upload">Meer informatie</a>
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
<p>Raadpleeg de <a href="../transactional-messaging/profile-enrichment.md">gedetailleerde documentatie</a> voor meer informatie.</p>
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
<p>Raadpleeg de <a href="../integrations/aem-multilingual.md">gedetailleerde documentatie</a> voor meer informatie.</p>
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
<p>Raadpleeg de <a href="../email/ab-testing.md">gedetailleerde documentatie</a> voor meer informatie.</p>
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
<p>Raadpleeg de <a href="../workflows/activities/continuous-delivery.md">gedetailleerde documentatie</a> voor meer informatie.</p>
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
<p>Raadpleeg de <a href="../campaigns/campaign-approvals.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

### Verbeteringen {#26-1-improvements}

* Dynamische rapportage ondersteunt nu pushberichten en SMS. [Meer informatie](../reporting/dynamic-reporting/get-started-reporting.md)
* Vooraf gedefinieerde filters - Met een nieuwe optie Gedeeld filter kunt u een vooraf gedefinieerd filter beschikbaar maken voor andere gebruikers in uw organisatie. [Meer informatie](../get-started/predefined-filters.md#share-filter)
* Velden voor persoonlijke voorkeur die zijn gemaakt in Adobe Experience Manager, zoals Naam, E-mail, Datum en adres, worden nu opgenomen en beschikbaar wanneer u de inhoudssjabloon gebruikt.
* De evaluatie van de kwaliteit van de inhoud controleert nu op leesbaarheid, coherentie, en doeltreffendheid kwesties onafhankelijk van merkrichtlijnen, het identificeren van onduidelijk overseinen, inconsistente toon, of structurele hiaten. [Meer informatie](../content/brands-score.md)
