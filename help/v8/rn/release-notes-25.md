---
title: Campagne v8 Web User Interface Opmerkingen bij vorige release
description: 2025 Campagne Web User Interface-releases
exl-id: eecb4b18-4826-47a6-88b2-f2ed7b576d3e
source-git-commit: 336845c8d21a39c9f9124a5c6f7d0667cd111dcb
workflow-type: tm+mt
source-wordcount: '2664'
ht-degree: 11%

---

# Opmerkingen bij de release 2025 {#2025-release}

Deze pagina maakt een lijst van alle veranderingen en verbeteringen beschikbaar met **2025 versies**. De recentste vrije nota&#39;s zijn beschikbaar in [&#x200B; deze pagina &#x200B;](release-notes.md).

## Release september 1925 {#25-9-release}

_sep 23, 2025_

De volgende functies zijn beschikbaar vanaf de release van september.

<table>
<thead>
<tr>
<th><strong>Aangepast kanaal voor API-leveringen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt nu rechtstreeks vanuit de gebruikersinterface van Adobe Campaign leveringen ordenen en uitvoeren op basis van aangepaste API-kanalen. Deze leveringen kunnen op zichzelf staan of deel uitmaken van een workflow. De configuratie van het aangepaste API-kanaal wordt uitgevoerd in de console.</p>
<p>Raadpleeg de <a href="../call-center/gs-custom-channel.md">gedetailleerde documentatie</a> voor meer informatie.</p>
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
<p>Als beheerder van de Campagne, kunt u opstelling nieuwe verbindingen met externe systemen van het gebruikersinterface van het Web van de Campagne nu. U kunt ook bestaande externe accounts weergeven, bijwerken en beheren.</p>
<p>Raadpleeg de <a href="../administration/create-external-account.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>E-mailinhoud vergrendelen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Met Campagne kunt u nu inhoud in e-mailsjablonen vergrendelen door de volledige sjabloon of specifieke structuren en componenten te vergrendelen. Hierdoor kunt u onbedoelde bewerkingen of verwijderingen voorkomen, waardoor u meer controle hebt over de aanpassing van de sjabloon en de efficiëntie en betrouwbaarheid van uw e-mailcampagnes verbetert.</p>
<p>Raadpleeg de <a href="../content/content-locking.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Integration with Adobe GenStudio</strong><br/></th>  LA? sort? Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>To enhance marketing efficiency and to maintain brand consistency, you can now seamlessly integrate GenStudio for Performance Marketing experiences with Campaign. This enables you to leverage GenStudio's AI-power content creation alongside Campaign's advanced orchestration capabilities.<p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dark mode support in the Email designer</strong><br/></th> -> pas sept, modifier composant... -> Juliette
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The Email Designer now offers the ability to switch to dark mode view, where you can additionally define specific custom settings. Note that the final rendering depends on the recipient's email client, and not all email clients support dark mode.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>>
<thead>
<tr>
<th><strong>Multilingual capabilities for transactional messaging and push notifications (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple transactional messages and push notifications in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Profile enrichment in Transactional Messages (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>This capability allows you to personalize transactional messages (Email, SMS, Push) by linking Adobe Campaign database fields to the message content. You can select target mappings, enrichment columns, and a reconciliation key to ensure accurate, real-time personalization while maintaining performance thresholds.</p>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Dynamic reporting for transactional messaging (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Note: this capability is only available for a set of organizations (Limited Availability), and will be rolled out globally in a future release.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->


### Verbeteringen {#25-9-improvements}

* Er is een set nieuwe operatoren toegevoegd bij het instellen van een voorwaarde met behulp van de voorwaardelijke-inhoudmogelijkheden van e-mail Designer.
* De het filtreren dimensie is nu beschikbaar in **bouwt publiek** werkschemaactiviteit. Als u deze wilt weergeven of wijzigen, klikt u op het pictogram naast de doeldimensie. [Meer informatie](../workflows/activities/build-audience.md#build-audience-configuration).
<!--

NEO-84915 Stop button for deliveries???? ->>> met pas, juste bouton ajouté dans webUI meme comportement que console. bleu, marche, marche pas.
NEO-90345 WebUI - Extended operators for dynamic content ->>>> deja mis
NEO-88858 WebUI - Send proof from execution recurring delivery -> bug
NEO-89777 Content locking on create email template -> juliette
NEO-90365 Multi-lingual – Identify fields editable from variants???? -> fix pour SMS
query activity -> query ds workflow fitleting dimentsion 

-->

## Release van augustus 1925 {#25-8-release}

Deze versie wordt geleverd met een aantal opgeloste problemen, waaronder:

* Het proces voor het dupliceren van profielen is verbeterd en afgestemd op het gedrag van de clientconsole. Hierdoor is een consistente ervaring voor beide interfaces gegarandeerd. Hiermee verhelpt u een probleem dat kan voorkomen dat de gedupliceerde profielen worden gemaakt.

* De optie **[!UICONTROL Email BCC]** werkt nu in het scherm voor de leveringsconfiguratie met Momentum (Enhanced MTA). Deze functionaliteit was eerder alleen beschikbaar in de clientconsole.

## Release juli 1925 {#25-7-release}

### Nieuwe functies {#25-7-features}

De volgende functies zijn beschikbaar vanaf de release in juli.

<!--table>
<thead>
<tr>
<th><strong>Multilingual email and SMS</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now send multiple email and SMS deliveries in different languages in Adobe Campaign Web UI. The multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen.
</p>
<p>For Multilingual email, your server must be upgraded to 8.8.1 minimum. Refer to the Client Console <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=nl-NL" target="_blank">release notes</a>.
<p>For more information, refer to the <a href="../email/edit-content.md#multilingual-delivery">detailed documentation</a>.</p>
</td>
</tr>
</tbody>
</table-->

<!--table>
<thead>
<tr>
<th><strong>Custom channel for API deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now, directly from Adobe Campaign Web UI, orchestrate and execute deliveries based on custom API channels. These deliveries can be standalone or part of a workflow. The configuration of the custom API channel is performed in the console.</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

<table>
<thead>
<tr>
<th><strong>Ondersteuning voor aangepaste CSS in de Designer-e-mail</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Wanneer u e-mailberichten ontwerpt, kunt u nu uw eigen aangepaste CSS rechtstreeks toevoegen in de e-mailtoepassing van de Designer. Met deze functie kunt u geavanceerde en specifieke stijlen toepassen, voor meer flexibiliteit en controle over de weergave van uw inhoud.</p>
<p>Raadpleeg de <a href="../email/custom-css.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Merken</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt nu uw eigen merken maken en aanpassen om uw visuele en verbale identiteit in verschillende communicatie duidelijk te definiëren. Met de merkuitlijningsscore kunt u in real-time feedback ontvangen over hoe goed uw inhoud de toon, stijl en richtlijnen van uw merk weerspiegelt, zodat u bij elke boodschap die u verzendt, consistent onder het merk kunt blijven.
</p>
<p>Raadpleeg de <a href="../content/brands.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Afleveringswaarschuwing</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De voorziening voor leveringswaarschuwingen is een systeem voor waarschuwingsbeheer dat een groep gebruikers in staat stelt automatisch meldingen te ontvangen die informatie bevatten over de uitvoering van hun leveringen.</p>
<p>Raadpleeg de <a href="../msg/delivery-alerting.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>Landing pages improvements</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>The following improvements to landing pages are now available:</p>
<ul>
    <li>You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. <a href="../audience/manage-services.md#create-service">Read more</a></li>
    <li>A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. <a href="../landing-pages/create-lp.md#create-landing-page">Read more</a></li>
    <li>A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). <a href="../landing-pages/create-lp.md#define-actions-on-form-submission">Read more</a></li>
    <li>Conditional content is now supported in landing pages. <a href="../landing-pages/lp-content.md">Read more</a></li>
    <li>You can link a landing page to a service, and send a confirmation message when users validate it. <a href="../landing-pages/lp-content.md#lp-message">Read more</a></li>
    <li>You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. <a href="../landing-pages/create-lp.md#captcha">Read more</a></li>
</ul>
</td>
</tr>
</tbody>
</table-->


<table>
<thead>
<tr>
<th><strong>Dynamische rapportage</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt tot Dynamische Rapportering nu toegang hebben die volledig klantgerichte en real-time rapporten verstrekt om het effect van uw marketing activiteiten te meten. Het voegt toegang tot profielgegevens toe, toelatend demografische analyse door profieldimensies zoals geslacht, stad en leeftijd naast functionele e-mailcampagnegegevens zoals opent en klikt. Dynamische rapportage is ook beschikbaar voor meertalige e-mailleveringen en transactieberichten.</p>
<p>Deze mogelijkheid is alleen op aanvraag beschikbaar. Neem contact op met uw Adobe-vertegenwoordiger voor toegang. De upgrade van uw server moet minimaal 8.8.1 uitvoeren. Verwijs naar de de versienota's van de Console van de Cliënt <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=nl-NL" target="_blank"> </a>.
<p>Raadpleeg de <a href="../reporting/dynamic-reporting/get-started-reporting.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Gecentraliseerde branding</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Uw technische beheerders kunnen nu een of meerdere merken definiëren om de parameters die de identiteit van een merk beïnvloeden, te centraliseren. Dit zijn onder andere het merklogo, het domein van de toegangs-URL voor de landingspagina's of de instellingen voor de tracking van berichten. U kunt deze merken maken en deze koppelen aan berichten of bestemmingspagina's. Deze configuratie wordt beheerd in malplaatjes. Brandingsopties zijn beschikbaar voor alle kanalen, waaronder SMS en Direct mail.</p>
<p>Deze mogelijkheid is alleen op aanvraag beschikbaar voor nieuwe implementaties. Neem contact op met uw Adobe-vertegenwoordiger voor toegang. De upgrade van uw server moet minimaal 8.8.1 uitvoeren. Verwijs naar de de versienota's van de Console van de Cliënt <a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=nl-NL" target="_blank"> </a>.
<p>Raadpleeg de <a href="../administration/branding/branding-gs.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

Naast de hierboven vermelde functies wordt deze release ook geleverd met een aantal functies die beschikbaar zijn in de Client Console:

* [&#x200B; Nieuwe SMS die schakelaar &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=nl-NL) verzenden (milieu&#39;s FDA)
* [&#x200B; Rest APIs &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=nl-NL) (op bestelling, milieu&#39;s FDA)

Verwijs naar de de versienota&#39;s van de Console van de Cliënt [&#x200B; &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=nl-NL){target="_blank"}.

<!--

### Features previously in Limited Availability {#25-7-limited} 

>[!AVAILABILITY]
>
>To benefit from these updates, your server must be upgrated to 8.8.1 mininum. Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=nl-NL){target="_blank"}.

Previously released in Limited Availability, the following capabilities are now available to all environments (General Availability):

* **Multilingual delivery creation** - You can now send multiple email deliveries in different languages in Adobe Campaign Web User Interface. The Multilingual delivery feature allows you to choose the default language of your delivery as well as the different languages in which the delivery can be sent. You can also preview these deliveries in the languages you have chosen. [Read more](../email/edit-content.md#multilingual-delivery).


* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html?lang=nl-NL){target="_blank"}

* **Delivery alerting** - The Delivery alerting feature is an alert management system that enables a group of users to automatically receive notifications containing information on the execution of their deliveries. [Read more](../msg/delivery-alerting.md)


* **Landing pages improvements** - The following improvements to landing pages are now available:

    * You can now reference a default subscription/unsubscription landing page when configuring a service. When designing an email, if you define a link to that landing page, users submitting the landing page form are automatically subscribed to or unsubscribed from this service. [Read more](../audience/manage-services.md#create-service)
    * A new option in the landing page configuration allows anonymous visitors to access the landing page. If you unselect this option, only identified users can access and submit the form. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option in the landing page configuration allows to store additional internal data when the landing page is being submitted. [Read more](../landing-pages/create-lp.md#create-landing-page)
    * A new option enables to use a landing page for several services, making it dynamic. When adding a link to an email, if you select a dynamic landing page, you can select any service. If you select a landing page that has a specific service associated, this service will be automatically used (you cannot select another one). [Read more](../landing-pages/create-lp.md#define-actions-on-form-submission)
    * Conditional content is now supported in landing pages. [Read more](../landing-pages/lp-content.md)
    * You can link a landing page to a service, and send a confirmation message when users validate it. [Learn more](../landing-pages/lp-content.md#lp-message)
    * You can add captcha to protect your landing page from spam and abuse caused by bots. This is non-intrusive for your customers since it does not require any interaction from them and is based on interactions with your site. [Learn more](../landing-pages/create-lp.md#captcha)

Previously released in Limited Availability, the following capabilities are now available **on demand**:

* **Dynamic Reporting** - You can now access Dynamic Reporting which provides fully customizable and real-time reports to measure the impact of your marketing activities. It adds access to profile data, enabling demographic analysis by profile dimensions such as gender, city and age in addition to functional email campaign data like opens and clicks. Dynamic reporting is also available for multilingual email deliveries and transactional messages. [Read more](../reporting/dynamic-reporting/get-started-reporting.md)

* **Centralized Branding** -  Your technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Branding options are available for all channels, including SMS and Direct mail. [Read more](../administration/branding/branding-gs.md){target="_blank"}

    >[!NOTE]
    >
    >This feature is only available for new implementations.

In addition to the features listed above, this release also comes with a set of functionalities available in the Client Console:

* [New SMS sending connector](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html?lang=nl-NL) (FDA environments)
* [Rest APIs](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=nl-NL) (on demand, FDA environments)

Refer to the Client Console [release notes](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html?lang=nl-NL){target="_blank"}.

-->

### Verbeteringen {#25-7-improvements}

* U kunt de doelpopulatie nu direct op elke voorwaarde en groep in de regelbouwer berekenen. Klik op het resultaatnummer om de gedetailleerde lijst met records weer te geven. [Meer informatie](../query/build-query.md#validate-query)

* U kunt een vooraf gedefinieerd filter nu rechtstreeks vanuit de regelbuilder bewerken of verwijderen. [Meer informatie](../get-started/predefined-filters.md#manage-predefined-filter)

* Wanneer het vormen van een levering van SMS, in de **sectie van SMS**, hebt u nu toegang tot de **Facultatieve parameters SMPP (TLV)**. Deze parameter is hetzelfde als in de clientconsole. [Meer informatie](../advanced-settings/delivery-settings.md#sms-tab)

* U kunt achtergrondberichten op iOS nu toelaten gebruikend de nieuwe **Beschikbare Inhoud** optie, beschikbaar in de **Geavanceerde montages** sectie van het scherm van de de inhoudsuitgave van iOS. Hiermee wordt de markering `content-available:1` toegevoegd in de payload van `aps` . Leer meer [&#x200B; op deze pagina &#x200B;](../push/content-push.md). Zie ook [&#x200B; deze pagina &#x200B;](../push/rich-push-ios.md)

* De volgende verbeteringen op de bestemmingspagina zijn nu beschikbaar:

   * U kunt nu naar een standaardlandingspagina voor abonnementen/abonnementen verwijzen wanneer u een service configureert. Als u bij het ontwerpen van een e-mailbericht een koppeling naar die landingspagina definieert, worden gebruikers die het formulier voor de bestemmingspagina verzenden, automatisch geabonneerd op of geabonneerd van deze service. [Meer informatie](../audience/manage-services.md#create-service)
   * Een nieuwe optie in de configuratie van de bestemmingspagina staat anonieme bezoekers toe om tot de landingspagina toegang te hebben. Als u deze optie uitschakelt, kunnen alleen geïdentificeerde gebruikers het formulier openen en verzenden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie in de configuratie van de bestemmingspagina kunt u aanvullende interne gegevens opslaan wanneer de bestemmingspagina wordt verzonden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie kunt u een openingspagina gebruiken voor verschillende services, waardoor deze dynamisch wordt. Als u een koppeling naar een e-mailbericht toevoegt en u een dynamische bestemmingspagina selecteert, kunt u elke gewenste service selecteren. Als u een landingspagina selecteert waaraan een specifieke service is gekoppeld, wordt deze service automatisch gebruikt (u kunt geen andere service selecteren). [Meer informatie](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Voorwaardelijke inhoud wordt nu ondersteund in bestemmingspagina&#39;s. [Meer informatie](../landing-pages/lp-content.md)
   * U kunt een landingspagina aan de dienst verbinden, en een bevestigingsbericht verzenden wanneer de gebruikers het bevestigen. [Meer informatie](../landing-pages/lp-content.md#lp-message)
   * U kunt Captcha toevoegen om uw landingspagina te beschermen tegen spam en misbruik veroorzaakt door bots. Dit is niet opdringerig voor uw klanten omdat het geen enkele interactie van hen vereist en gebaseerd is op interacties met uw site. [Meer informatie](../landing-pages/create-lp.md#captcha)

## Release van juni 1925 {#25-6-release}

### Verbeteringen {#25-6-improvements}

* Het rapport van het Overzicht van de Levering is nu beschikbaar voor zowel het Centrum van de Vraag als de kanalen van de Douane. [Meer informatie](../reporting/direct-mail.md)

* Wanneer het vormen van een levering van SMS, hebt u nu toegang tot de specifieke parameters van SMS. Dit zijn dezelfde parameters die beschikbaar zijn in de clientconsole. [Meer informatie](../advanced-settings/delivery-settings.md#sms-tab)

* Uw favoriete mappen worden nu boven aan het linkerdeelvenster op de pagina Verkenner weergegeven, zodat ze gemakkelijker toegankelijk zijn. [Meer informatie](../get-started/work-with-folders.md#favorite-folders)

* De Bouwer van de Regel steunt nu belemmering-en-daling, toestaand u om componenten van uw vraag efficiënter opnieuw te rangschikken. [Meer informatie](../query/build-query.md#drag-and-drop)

* De &quot;menselijke conditie&quot;in de Bouwer van de Regel is verbeterd. Dit is de geschreven, duidelijke-taalversie van uw regels, die bij de bodem van het scherm wordt getoond:

   * Kenmerken worden nu gemarkeerd en het bijbehorende schema wordt weergegeven.
   * U kunt op deze elementen klikken om meer gedetailleerde informatie te bekijken.
   * U kunt nu de menselijke voorwaarde kopiëren met de bijbehorende knop.

* De toegang tot de mappen &#39;Technische workflows&#39; en &#39;Objecten die automatisch worden gemaakt&#39; is nu beperkt om te voorkomen dat ze worden weergegeven. [Meer informatie](../get-started/work-with-folders.md#about-folders)

## Release mei &#39;25 {#25-5-release}

De volgende functies zijn vanaf mei beschikbaar voor alle gebruikers.

<table>
<thead>
<tr>
<th><strong>Brand alignment score (Beta)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De functie voor de uitlijningsscore voor merken biedt duidelijke feedback rechtstreeks in de e-mailontwerper, zodat u kunt zien of uw inhoud wordt uitgelijnd op de toon, stijl en richtlijnen van uw merk. Deze functie is beschikbaar in Beta.</p>
<p>Raadpleeg de <a href="../content/brands-score.md">gedetailleerde documentatie</a> voor meer informatie.</p>
<img src="assets/do-not-localize/brand-score.gif">
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Aangepast kanaal voor externe leveringen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt nu rechtstreeks vanuit de gebruikersinterface van Adobe Campaign leveringen ordenen en uitvoeren op basis van aangepaste externe kanalen. Deze leveringen kunnen op zichzelf staan of deel uitmaken van een workflow. Het maken van het aangepaste externe kanaal dat met een derde is geïntegreerd, wordt uitgevoerd in de console.</p>
<p>Nota: Het melden is niet beschikbaar in het Web UI voor het douanekanaal. U moet naar de clientconsole bladeren om rapporten te openen.</p>
<p>Raadpleeg de <a href="../call-center/gs-custom-channel.md">gedetailleerde documentatie</a> voor meer informatie.</p>
<img src="assets/do-not-localize/custom-channel.gif">
</td>
</tr>
</tbody>
</table>

### Verbeteringen {#25-5-improvements}

Het aanmaakscherm van de typologieregels is bijgewerkt om de selectie van het type regel te vergemakkelijken.

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
<p>Nota: Het melden is niet beschikbaar in het Web UI voor het kanaal van het vraagcentrum. U moet naar de clientconsole bladeren om rapporten te openen.</p>
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
* In de interface worden de datum en tijd nu weergegeven volgens de primaire taal die is ingesteld in de Experience League-voorkeuren. Deze verbetering is alleen beschikbaar voor verschillende talen. Om de volledige lijst van gesteunde talen te zien, verwijs naar de [&#x200B; gedetailleerde documentatie &#x200B;](https://experienceleague.adobe.com/nl/docs/core-services/interface/features/browser-language){target=_blank}.

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
>Verwijs naar de volgende documentatiepagina&#39;s: [&#x200B; overgang Campaign Standard aan Campagne v8 &#x200B;](../rn/acs-migration.md) en [&#x200B; Eigenschappen voor de gebruikers van Campaign Standard &#x200B;](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html?lang=nl-NL).

* **Meertalige leveringsverwezenlijking** - u kunt veelvoudige e-mailleveringen in verschillende talen in het Gebruikersinterface van het Web van Adobe Campaign nu verzenden. Met de functie Meertalige levering kunt u de standaardtaal van uw levering kiezen en de verschillende talen waarin de levering kan worden verzonden. U kunt deze leveringen ook voorvertonen in de talen die u hebt gekozen. Raadpleeg de [gedetailleerde documentatie](../email/edit-content.md) voor meer informatie.

* **Dynamische Rapportering voor Meertalig** - de Dynamische rapportering is nu beschikbaar voor meertalige e-mailleveringen. Raadpleeg de [gedetailleerde documentatie](../reporting/global-reports.md) voor meer informatie.

* **de REST API van SMS steun (LA)** - De Transactionele WEERGAVE API van het Overseinen is nu beschikbaar voor het kanaal van SMS. Wanneer zowel e-mail als mobilePhone aanwezig zijn in de lading, kunt u het &quot;wishedChannel&quot;gebied gebruiken om het kanaal te specificeren. Indien niet opgegeven, wordt de e-mail standaard gebruikt, tenzij wishedChannel expliciet om SMS verzoekt. Raadpleeg de [gedetailleerde documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html?lang=nl-NL){target=_blank} voor meer informatie.

## Release van februari &#39;25 {#25-2-release}

**de datum van de Versie**: 18 feb, 2025

De volgende functies en verbeteringen zijn beschikbaar vanaf de release in februari.

### Functies {#25-2-features}

<table>
<thead>
<tr>
<th><strong>Bedrijfsregels maken (typologieregels)</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt nu typologieën en typologische regels maken in de Adobe Campaign Web User Interface. Met behulp van typologieën kunt u het verzenden van leveringen besturen, filteren en prioriteren. De technologieën worden gebruikt om te bevestigen dat de leveringen altijd verplichte componenten (zoals een unsubscription verbinding of een onderwerpregel) of het filtreren regels bevatten om groepen van uw publiek (zoals abonnees, concurrenten, of niet loyaliteitklanten) uit te sluiten.</p>
<img src="assets/do-not-localize/typology.gif">
<p>Raadpleeg de <a href="../administration/typologies.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Doeltoewijzingen</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt doeltoewijzingen in het Gebruikersinterface van het Web van de Campagne nu tot stand brengen. Doeltoewijzingen bepalen hoe verschillende leveringskanalen (e-mail, SMS, pushmeldingen) worden gekoppeld aan de gegevensvelden van een schema. Met de doeltoewijzing kunt u het doelpubliek definiëren: profielen, begunstigden van contracten, operators, abonnees, vooruitzichten, enz.</p>
<img src="assets/do-not-localize/target-mapping.gif">
<p>Raadpleeg de <a href="../administration/target-mappings.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Schema-details</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt tot de details van een schema nu toegang hebben door zijn naam in de lijst te selecteren. De de gebiedsuitgave van de douane is nu toegankelijk van <b> geeft de knoop van douanegebieden </b> beschikbaar in de schemadetails uit.</p>
<img src="assets/do-not-localize/schemas.gif">
<p>Raadpleeg de <a href="../administration/schemas.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

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
<p>Voor meer informatie over AI Medewerker, verwijs naar de <a href="../content/generative-full-content.md"> gedetailleerde documentatie </a>.</p>
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
