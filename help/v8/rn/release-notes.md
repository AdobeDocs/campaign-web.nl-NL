---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: e825b7859bff299906725eddf3ba014ed0b5e1b7
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 13%

---

# Aanvullende informatie  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie "
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

De veranderingen en de verbeteringen beschikbaar met vorige versies worden vermeld in [ 2024 ](release-notes-24.md) en [ 2025 ](release-notes-25.md).

## Release van april 1925 {#25-4-release}

**de datum van de Versie**: 29 april, 2025


### Nieuwe functies {#25-4-features}

De volgende functies zijn beschikbaar voor alle gebruikers vanaf de release van april.

<table>
<thead>
<tr>
<th><strong>Kanaal van callcenter</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Het kanaal van het vraagcentrum is nu beschikbaar in het Gebruikersinterface van het Web van de Campagne. Dit kanaal verwijst naar een communicatie die methode wordt gebruikt om mededelingen of interactie te beheren en te volgen die via een callcenter worden behandeld — typisch telefoonvraag die door agenten aan klanten of vooruitzichten wordt gemaakt.</p>
<img src="assets/do-not-localize/call-center.gif">
<p>Raadpleeg de <a href="../call-center/gs-call-center.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Nieuwe regelbouwer</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Een nieuwe regelbouwer is nu beschikbaar om u te helpen complexe voorwaarden in een verbeterde gebruikersinterface bepalen. U kunt van oud naar de nieuwe regelbouwer schakelen zoals nodig.</p>
<img src="assets/do-not-localize/rule-builder-release.gif">
<p>Raadpleeg de <a href="../query/query-modeler-overview.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Ontwerpen van externe accounts</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Als beheerder van de Campagne, kunt u opstelling nieuwe verbindingen met externe systemen van het gebruikersinterface van het Web van de Campagne nu.
U kunt ook bestaande externe accounts weergeven, bijwerken en beheren.</p>
<p>Raadpleeg de <a href="../administration/external-account.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

### Verbeteringen {#25-4-improvements}

**Algemene interfaceverbeteringen**

* De veldbeschrijving, Toevoegen aan Favorieten en Distributie van waardeopties voor schemakenmerken zijn nu beter zichtbaar in de gebruikersinterface. Raadpleeg de [gedetailleerde documentatie](../get-started/attributes.md) voor meer informatie.
* In de interface worden de datum en tijd nu weergegeven volgens de primaire taal die is ingesteld in de Experience League-voorkeuren. Deze verbetering is alleen beschikbaar voor verschillende talen. Om de volledige lijst van gesteunde talen te zien, verwijs naar de [ gedetailleerde documentatie ](https://experienceleague.adobe.com/en/docs/core-services/interface/features/browser-language){target=_blank}.

<!--
ko * Built-in options are now only visible in the list of options if the **Show advanced options** toggle is activated.
ko * The typology rules creation screen has been updated to facilitate the selection of the type of rule.
-->

**E-mailRedacteur**: Om toegankelijkheid in het Web UI van de Campagne te verbeteren, zijn twee nieuwe gebieden nu beschikbaar in E-mail Designer: zij beantwoorden aan het `title` element en lang attribuut in het `html` element van uw e-mailinhoud. In de sectie Hoofdtekst van e-mail kunt u deze instellingen definiëren in aanvulling op het veld Voorkop. Raadpleeg de [gedetailleerde documentatie](../email/metadata.md) voor meer informatie.

<!--
**Workflow**: You can now select an existing Javascript code in workflow properties or in a Javascript activity.    
-->

**Schemas**

* U kunt het tijdelijke schema van een lijst van het Web van de Campagne nu uitgeven gebruikersinterface. Raadpleeg de [gedetailleerde documentatie](../audience/manage-audience.md) voor meer informatie.
* U kunt nu de aangepaste velden van een schema voorvertonen in een voorbeeldscherm. Raadpleeg de [gedetailleerde documentatie](../administration/custom-fields.md#add) voor meer informatie.
* U kunt nu aangepaste velden in de lijst verplaatsen door ze te slepen en neer te zetten. Raadpleeg de [gedetailleerde documentatie](../administration/custom-fields.md#add) voor meer informatie.


### Nieuwe functies in beperkte beschikbaarheid {#25-4-features-la}

>[!AVAILABILITY]
>
>De volgende mogelijkheden zijn in Beperkte Beschikbaarheid (LA). Zij zijn beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kunnen niet op een ander milieu worden opgesteld. Ze vereisen een upgrade van de Campagneserver naar v8.7.4.
>
>Verwijs naar de volgende documentatiepagina&#39;s: [ overgang Campaign Standard aan Campagne v8 ](../rn/acs-migration.md) en [ Eigenschappen voor de gebruikers van Campaign Standard ](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Meertalige leveringsverwezenlijking** - u kunt veelvoudige e-mailleveringen in verschillende talen in het Gebruikersinterface van het Web van Adobe Campaign nu verzenden. Met de functie Meertalige levering kunt u de standaardtaal van uw levering kiezen en de verschillende talen waarin de levering kan worden verzonden. U kunt deze leveringen ook voorvertonen in de talen die u hebt gekozen. Raadpleeg de [gedetailleerde documentatie](../email/edit-content.md) voor meer informatie.

* **Dynamische Rapportering voor Meertalig** - de Dynamische rapportering is nu beschikbaar voor meertalige e-mailleveringen. Raadpleeg de [gedetailleerde documentatie](../reporting/global-reports.md) voor meer informatie.

* **de REST API van SMS steun (LA)** - De Transactionele WEERGAVE API van het Overseinen is nu beschikbaar voor het kanaal van SMS. Wanneer zowel e-mail als mobilePhone aanwezig zijn in de lading, kunt u het &quot;wishedChannel&quot;gebied gebruiken om het kanaal te specificeren. Indien niet opgegeven, wordt de e-mail standaard gebruikt, tenzij wishedChannel expliciet om SMS verzoekt. Raadpleeg de [gedetailleerde documentatie](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/apis/managing-transactional-messages){target=_blank} voor meer informatie.

