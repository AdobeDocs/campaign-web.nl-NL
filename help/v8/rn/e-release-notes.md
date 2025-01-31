---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de volgende versie van het Gebruikersinterface van het Web van de Campagne komen
hide: true
hidefromtoc: true
exl-id: a4c6ecb7-d657-46de-aa55-90c4cb45164b
source-git-commit: 965681fabb7696f745f4f958e2961197395c30bb
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 2%

---

# Vroege aanvullende informatie {#e-release}

De gebruikersinterface van het Web van Adobe Campaign levert onophoudelijk nieuwe eigenschappen, verhogingen aan bestaande eigenschappen, en insectenmoeilijke situaties. Alle veranderingen worden geconsolideerd aan het eind van elke maand in de [ versienota&#39;s ](release-notes.md).

**de vroege versienota&#39;s hieronder zijn onderworpen aan verandering zonder voorafgaande kennisgeving tot de datum van de versiebeschikbaarheid**. De verbindingen, de schermen en de bijgewerkte documentatie worden gepubliceerd in de [ versienota&#39;s ](release-notes.md), bij de versiedatum.

## Release januari 1925 {#25-1-release}

**de datum van de Versie**: 5 Feb, 2025

De volgende functies en verbeteringen zijn beschikbaar vanaf de release in januari.

### Functies {#25-1-features}


<table>
<thead>
<tr>
<th><strong>Visuele fragmenten maken en gebruiken</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Visuele fragmenten zijn vooraf gedefinieerde visuele blokken die u kunt hergebruiken voor meerdere e-mailleveringen of in inhoudssjablonen. Deze functie is nu beschikbaar voor alle klanten die op de server bouwen 8.6.4 en hoger.</p>
<p>Raadpleeg de <a href="../content/use-visual-fragments.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Een systeem van derden gebruiken om leveringen te verzenden</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt Externe leveringen, en Externe leveringsmalplaatjes, in het Webgebruikersinterface van de Campagne nu bepalen. In deze modus worden berichten gegenereerd in een invoerbestand dat kan worden gedeeld met uw externe provider. De externe leveringswijze is de standaardwijze voor het directe postkanaal.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Controle en filterlevering die met typologieën verzenden</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt nu typologieën en typologische regels maken in de Adobe Campaign Web User Interface. Een typologie is een verzameling typologische regels waarmee u het verzenden van leveringen kunt beheren, filteren en prioriteren. De technologieën bevestigen uw leveringen altijd vereiste elementen (zoals een unsubscription verbinding of een onderwerpregel), of het filtreren regels bevatten om groepen van uw voorgenomen doel (zoals abonnees, concurrenten, of niet-loyaliteitklanten) uit te sluiten.</p>
<img src="assets/do-not-localize/typology.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Uw opsommingen beheren</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt opsommingen nu rechtstreeks maken via de Adobe Campaign Web User Interface. Een opsomming is een lijst met waarden die door het systeem worden voorgesteld om velden te vullen. Gebruik opsommingen om de waarden van deze velden te standaardiseren, hulp bij gegevensinvoer of gebruik binnen query's.</p>
<img src="assets/do-not-localize/enumerations.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Aangepaste opties maken</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U hebt nu toegang tot technische opties in de Adobe Campaign Web User Interface en kunt uw eigen aangepaste opties maken die aan uw wensen voldoen. Dit is met name handig wanneer u werkt met JavaScript-code-workflowactiviteiten om tussenliggende gegevens op te slaan.</p>
<img src="assets/do-not-localize/options.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>JavaScript-codes definiëren en aanroepen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt nu JavaScript-codes maken in de Adobe Campaign Web User Interface. Op deze manier kunt u herbruikbare functies maken die in verschillende workflows kunnen worden gebruikt, net als in een bibliotheek.</p>
<img src="assets/do-not-localize/javascript.gif">
<!--p>For more information, refer to the <a href="../administration/external-account.md">detailed documentation</a>.</p-->
</td>
</tr>
</tbody>
</table>

### Verbeteringen {#25-1-improvements}

* De weergave van aangepaste velden in de interface aanpassen:

   * U kunt nu aanvullende aangepaste velden selecteren die u wilt weergeven in de interface
   * U kunt nu regels instellen voor de weergave van aangepaste velden van het koppelingstype, zoals het beperken van lijstwaarden op basis van de invoer van een ander veld
   * U kunt nu velden in de interface flexibeler rangschikken: velden kunnen zich uitstrekken over één kolom of worden gegroepeerd in subsecties voor een betere organisatie
   * U kunt nu specifieke velden instellen als alleen-lezen

* Recente filters en Favorieten: als u kenmerken die vaak worden gebruikt snel wilt hergebruiken, kunt u deze nu toevoegen aan Favorieten. Hierdoor zijn ze gemakkelijk toegankelijk voor toekomstige taken. Naast favorieten kunt u ook de laatst geselecteerde kenmerken weergeven en gebruiken.


