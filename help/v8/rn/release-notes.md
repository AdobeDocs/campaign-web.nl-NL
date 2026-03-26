---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 304e3771ee55777d2eaf7a6c83ee4af3c97aa3b6
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Aanvullende informatie {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie"
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

## Release van maart 1926 {#26-3-release}

### Nieuwe functies {#26-3-features}

<table>
<thead>
<tr>
<th><strong>Schema-authoring (GA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De functie voor het ontwerpen van schema's is nu beschikbaar voor alle klanten (GA). Dit vermogen staat u toe om schema's van het Web van de Campagne direct tot stand te brengen en te beheren Gebruikersinterface. U kunt nieuwe tabellen maken, bestaande schema's uitbreiden en aangepaste formulieren maken. U kunt de structuren van douanegegevens bepalen om uw specifieke bedrijfsbehoeften te steunen zonder toegang tot de Console van de Cliënt te vereisen.</p>
<p>Voor meer informatie, verwijs naar de <a href="../administration/schemas.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Thema's in de e-mail-Designer (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Thema's bieden een verbeterde ontwerpervaring voor e-mails doordat u herbruikbare themastijlen kunt definiëren die aan de richtlijnen van uw merk voldoen. U kunt nu themariabelen in fragmenten gebruiken, zodat u consistent stijlen in uw e-mailsjablonen kunt gebruiken. Met deze functie kunt u sneller e-mails samenstellen met vooraf gedefinieerde modules die elementen in de inhoud, zoals titels, beschrijvingen, afbeeldingen en koppelingen, abstract maken, terwijl de consistentie van uw merk behouden blijft.</p>
<p>Opmerking: deze mogelijkheid is alleen beschikbaar voor een aantal organisaties (Beperkte beschikbaarheid) en wordt in een toekomstige release globaal geïmplementeerd.</p>
<p>Voor meer informatie, verwijs naar de <a href="../email/apply-email-themes.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integratie van aangepaste Firefly-modellen en modellen voor het genereren van images van derden</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Zorgt voor een naadloze integratie van standaard- en aangepaste Firefly-modellen in combinatie met goedgekeurde externe afbeeldingsmodellen voor meer flexibiliteit, controle en uitlijning van merken bij het genereren van afbeeldingen.</p>
<p>Kies het juiste model voor uw behoeften:</p>
<ul><li> <strong> Adobe model </strong> (aangedreven door Firefly Image Model 4) voor directe beeldgeneratie zonder extra opstelling</li><li> <strong> model van de Partner </strong> (aangedreven door Gemini 2.5 Flits) voor gespecialiseerde mogelijkheden</li><li><strong> de modellen van de Douane </strong> (merkspecifieke modellen die op uw eigen activa worden opgeleid) voor de generatie van het merk die precies op uw merkidentiteit, stijl, en visuele richtlijnen richt.</li></ul>
<p>Voor meer informatie, verwijs naar de <a href="../content/generative-models.md"> gedetailleerde documentatie </a>.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Geautomatiseerde leveringsactiviteit</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De <strong> Geautomatiseerde levering </strong> werkschemaactiviteit is nu beschikbaar in het werkschemapalet. U kunt het gebruiken om leveringsacties (voorbereidingen treffen, een proef verzenden, voorbereidingen treffen en beginnen, enz.) direct binnen uw werkschema tot stand te brengen of uit te voeren. Selecteer een bestaande levering die buiten de workflow is gemaakt om deze bij elke uitvoering opnieuw te gebruiken of maak een nieuwe levering van een sjabloon telkens wanneer de activiteit wordt uitgevoerd.</p>
<p><img src="assets/do-not-localize/workflow-automated-delivery.gif"/></p>
<p>Voor meer informatie, verwijs naar <a href="../workflows/activities/automated-delivery.md"> gedetailleerde documentatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Meerdere workflowvertakkingen en activiteiten samenvoegen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>

<p><strong> Veelvoudige takken </strong> worden nu gesteund. In plaats van het gebruiken van a <strong> Fork </strong>, kunt u <strong> vertakking </strong> op de toolbar klikken toevoegen. De <strong> EN-lid </strong> activiteit is ook verbeterd. Het is nu een generische <strong> verbind </strong> activiteit die u tussen EN laat kiezen en OF zich bij opties aansluiten.</p>
<p><img src="assets/do-not-localize/workflow-branches-join.gif"/></p>
<p>Voor meer informatie, verwijs naar <a href="../workflows/orchestrate-activities.md#toolbar"> Orchestrate activiteiten </a> en <a href="../workflows/activities/join.md"> verbind </a> documentatiepagina's.</p>
</td>
</tr>
</tbody>
</table>

### Verbeteringen {#26-3-improvements}

* De **het werkschemaactiviteit van het Begin** is toegevoegd om verenigbaarheid met de Console van de Cliënt te verbeteren. Deze activiteit is optioneel en wordt niet standaard in nieuwe workflows ingevoegd. Deze wordt echter automatisch toegevoegd aan bestaande workflows.
  [&#x200B; Leer meer &#x200B;](../workflows/activities/about-activities.md#flow-control)
* Het gebied van de tijdzoneselectie op de **montages van het Programma** van een levering is bewogen onder het **3&rbrace; gebied van de Datum van het Contact.** [&#x200B; Leer meer &#x200B;](../msg/create-deliveries.md#gs-schedule)