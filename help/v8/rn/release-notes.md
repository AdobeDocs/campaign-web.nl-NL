---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 3729a6159affbbb30d2cdab91d1e42dbf9df9c86
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 8%

---

# Aanvullende informatie  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie "
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

De veranderingen en de verbeteringen beschikbaar met vorige versies worden vermeld [ in deze pagina ](release-notes-24.md).

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
<img src="assets/do-not-localize/visual-fragment.gif">
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
<p>U kunt nu externe leveringen en externe leveringssjablonen definiëren in de webinterface van Campagne. In deze modus worden berichten gecompileerd naar een uitvoerbestand dat kan worden gedeeld met uw externe provider. Standaard wordt de externe leveringsmodus gebruikt voor het directe-mailkanaal.</p>
<img src="assets/do-not-localize/external-delivery.gif">
<p>Raadpleeg de <a href="../msg/send-external-deliveries.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<!--
<table>
<thead>
<tr>
<th><strong>Create business rules (typology rules)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now create typologies and typology rules in the Adobe Campaign web interface. A typology is a collection of typology rules that help control, filter, and prioritize deliveries. Typologies ensure that your deliveries always contain required elements (such as an unsubscribe link or subject line) and apply filtering rules to exclude specific groups from your target audience (such as unsubscribers, competitors, or non-loyalty customers).</p>
<img src="assets/do-not-localize/typology.gif">
<p>For more information, refer to the <a href="../administration/typologies.md">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table>
-->

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
<p>Raadpleeg de <a href="../administration/enumerations.md">gedetailleerde documentatie</a> voor meer informatie.</p>
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
<p>Raadpleeg de <a href="../administration/options.md">gedetailleerde documentatie</a> voor meer informatie.</p>
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
<p>Raadpleeg de <a href="../administration/javascript-codes.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Pagina's genereren met de AI Assistant</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De AI-assistent is nu beschikbaar bij de levering van de bestemmingspagina, zodat u tekst, afbeeldingen of volledige paginalay-outs kunt genereren.</p>
<img src="assets/do-not-localize/ai-lp.gif">
<p>Voor meer informatie over AI Medewerker, verwijs naar de <a href="../email/generative-lp.md"> gedetailleerde documentatie </a>.</p>
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

* Externe accounts: het nieuwe type **[!UICONTROL Routing]** kan worden geselecteerd wanneer u een nieuwe externe account maakt. Het staat u toe om een specifieke externe rekening voor gebruik in uw externe leveringen te vormen. [Meer informatie](../administration/external-account.md#routing)