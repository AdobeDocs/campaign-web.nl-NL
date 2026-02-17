---
title: Campagne v8 Web User Interface Opmerkingen bij vorige release
description: 2024 Campagne Web User Interface-releases
exl-id: 430dc1ba-dfa9-4d51-b4ed-f3f048da6ec0
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '2532'
ht-degree: 7%

---

# Opmerkingen bij de release 2024 {#2024-release}

Deze pagina maakt een lijst van alle veranderingen en verbeteringen beschikbaar met **2024 versies**. De recentste vrije nota&#39;s zijn beschikbaar in [&#x200B; deze pagina &#x200B;](release-notes.md).


## Release oktober 1924 {#24-10-release}

**de datum van de Versie**: 29 okt, 2024

De volgende functies en verbeteringen zijn beschikbaar vanaf de release in oktober.

### Functies

<table>
<thead>
<tr>
<th><strong>Externe accounts</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U hebt nu de mogelijkheid om externe accounts direct via de Adobe Campaign Web User Interface in te stellen en te beheren. Met deze nieuwe functie kunt u eenvoudig verschillende typen externe accounts configureren, zoals het stuiteren van e-mailberichten (POP3) of uitvoeringsinstanties.</p>
<p>Raadpleeg de <a href="../administration/external-account.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transactieberichten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Transactieberichten (Message Center) zijn nu beschikbaar in de webgebruikersinterface van Campagne. Deze invoegtoepassing is ontworpen voor het activeren van berichten die worden gegenereerd op basis van gebeurtenissen die worden geactiveerd via informatiesystemen en kan zijn: factuur, orderbevestiging, bevestiging van verzending, wijziging van het wachtwoord, kennisgeving van onbeschikbaarheid van het product, rekeningoverzicht, aanmaak van websiteaccount, enz.</p>
<p>Raadpleeg de <a href="../transactional-messaging/transactional.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>


### Verbeteringen

* **de activiteiten van het Werkschema** - u kunt een activiteit en al zijn kindknopen van een overgang aan een andere binnen een werkschema nu bewegen. Een specifieke **knoop van de Beweging** is beschikbaar in de de eigenschappen van de activiteit ruit om dit uit te voeren. [Meer informatie](../workflows/orchestrate-activities.md#move)

* **de verrijkingsactiviteit van het Werkschema**

   * U kunt een Alias en een Etiket nu bepalen wanneer het creëren van een nieuw gebied in de **Verrijking** activiteit. [Meer informatie](../workflows/activities/enrichment.md#collection-settings)
   * U kunt aanbiedingen voor elk profiel in de **Verrijking** activiteit nu toevoegen. [Meer informatie](../workflows/activities/enrichment.md##add-offers)

* **Distributie van waarden** - wanneer de toegang tot van de lijst van gebieden voor verpersoonlijking, kunt u nu controleren hoe de waarden voor elk gebied worden verdeeld. Een specifiek popup venster toont het aantal en het percentage voor elke waarde. [Meer informatie](../query/build-query.md#distribution-values-query)

* **Versie en systeeminfo** - u kunt tot details over uw instantieversies, zowel voor de cliëntconsole als het Gebruikersinterface van het Web nu toegang hebben. In deze nieuwe sectie worden ook alle ingebouwde pakketten weergegeven die in uw omgeving zijn geïnstalleerd. [Meer informatie](../get-started/user-interface.md#user-interface-about)

* **Lijsten** - u kunt de waarden van een lijst nu gemakkelijk opnieuw in orde brengen. [Meer informatie](../get-started/work-with-folders.md)

* **Levering** - de variabele van de Levering is nu toegankelijk van verpersoonlijkingsgebieden. [Meer informatie](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)


## Updates september {#9-2024}

<table>
<thead>
<tr>
<th><strong>AI-assistent</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Als je bericht klaar en op maat gemaakt hebt, ga je naar het volgende niveau met AI Assistant in Adobe Campaign Web. Met dit krachtige gereedschap kunt u de impact van uw inhoud optimaliseren door een reeks aansprekende tekst, hoofdtitels en visueel aantrekkelijke afbeeldingen te genereren.</p>
<p>Ga zelf in een hands-on ervaring met <a href="https://experienceleague.adobe.com/en/apps/journey-optimizer/ai-assistant-content-accelerator"> binnen onze levende eigenschapvoorproef </a>, die wordt ontworpen om u zijn eigenschappen eerst te laten onderzoeken en volledig zijn mogelijkheden te begrijpen.</a></p>
<p>Raadpleeg de <a href="../content/generative-gs.md">gedetailleerde documentatie</a> voor meer informatie.</p>
<img src="assets/do-not-localize/ai-content-webui.gif"/>
<p>Beschikbaarheidsdatum: september 12</p>
</td>
</tr>
</tbody>
</table>

## Release van augustus {#24-8-release}

**de datum van de Versie**: Sept 3, 2024

De volgende functies en verbeteringen zijn beschikbaar vanaf de release in augustus.

* **parameters SMTP** - de montages SMTP zijn nu beschikbaar in de montages van de e-maillevering. [Meer informatie](../advanced-settings/delivery-settings.md#smtp)

* **Globale variabelen** - u kunt globale variabelen nu bepalen om waarden voor uw leveringen te bepalen. [Meer informatie](../advanced-settings/delivery-settings.md#variables-delivery)

### Nieuwe functies in beperkte beschikbaarheid {#acs-24-8}

>[!AVAILABILITY]
>
>De volgende mogelijkheden zijn in Beperkte Beschikbaarheid (LA). Zij zijn beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kunnen niet op een ander milieu worden opgesteld.
>
>Verwijs naar de volgende documentatiepagina&#39;s: [&#x200B; overgang Campaign Standard aan Campagne v8 &#x200B;](../rn/acs-migration.md) en [&#x200B; Eigenschappen voor de gebruikers van Campaign Standard &#x200B;](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html){target="_blank"}.

* **Branding voor Directe Post** - de Technische beheerders kunnen één of verscheidene merken nu bepalen om de parameters te centraliseren die de identiteit van een merk beïnvloeden. Dit zijn onder andere het merklogo, het domein van de toegangs-URL voor de landingspagina&#39;s of de instellingen voor de tracking van berichten. U kunt deze merken nu maken en deze koppelen aan berichten of bestemmingspagina&#39;s. Deze configuratie wordt beheerd in malplaatjes. [Meer informatie](../administration/branding/branding-assign.md)

* **Abonnementen met het Aanvoeren van pagina&#39;s** - u kunt een het landen pagina aan de dienst nu verbinden, en een bevestigingsbericht verzenden wanneer de gebruikers het bevestigen. [Meer informatie](../landing-pages/lp-content.md#lp-message){target="_blank"}.

* **Visuele fragmenten** - u kunt visuele inhoudsfragmenten nu archiveren. [Meer informatie](../content/create-fragment.md#archive)

* **Captcha in het landen van pagina&#39;s** - u kunt nu Captcha toevoegen om uw landende pagina tegen spam en misbruik te beschermen dat door bots wordt veroorzaakt. Dit is niet opdringerig voor uw klanten omdat het geen enkele interactie van hen vereist en gebaseerd is op interacties met uw site. [Meer informatie](../landing-pages/create-lp.md#captcha)

<!--
* **Rest APIs** - As a Campaign Standard migrated user, you can now use Rest APIs to work with transactional messages. [Read more](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html){target="_blank"}.-->


## Release-aantekeningen juli {#24-7-release}

**de datum van de Versie**: 30-31 juli, 2024

De volgende functies en verbeteringen zijn beschikbaar vanaf de release in juli.

### Inhoudsfragmenten {#24-7-1}

U kunt nu inhoudsfragmenten maken en gebruiken. Een inhoudsfragment is een herbruikbare component waarnaar in een of meer berichten kan worden verwezen. Wanneer u een fragment wijzigt, wordt alle inhoud die het fragment gebruikt, bijgewerkt. Met deze functionaliteit kunt u meerdere blokken met aangepaste inhoud samenstellen die marketinggebruikers kunnen gebruiken om snel inhoud van berichten samen te stellen in een verbeterd ontwerpproces.

Er zijn twee typen fragmenten beschikbaar:

* **de fragmenten van de Uitdrukking** zijn vooraf bepaalde uitdrukkingen die van een specifieke ingang in de uitdrukkingsredacteur beschikbaar zijn.
* **Visuele fragmenten** zijn vooraf bepaalde visuele blokken die u over veelvoudige e-mailleveringen, of in inhoudsmalplaatjes kunt hergebruiken. [Meer informatie](../content/fragments.md)

  >[!AVAILABILITY]
  >
  >**de Visuele fragmenten** zijn in Beperkte Beschikbaarheid (LA). Dit vermogen wordt beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kan niet op een ander milieu worden opgesteld.

### Overvulgroep {#24-7-2}

A **de groep van de Vulling** is een lijst van zaadadressen. Het wordt gebruikt om specifieke adressen in uw leveringen te omvatten, en dan doelprofielen die niet aan de bepaalde doelcriteria voldoen. Op deze manier kunnen ontvangers die buiten het leveringspubliek vallen, de levering ontvangen, net als elke andere doelontvanger. U kunt zaadadressen gebruiken wanneer het verzenden van proefdrukken, of om uw postingslijst te beschermen. [Meer informatie](../audience/trap-group.md)

### Sjablonen voor pushmeldingen {#24-7-3}

U kunt nu uitgebreide pushmeldingen verzenden. Een uitgebreide pushmelding is een verbeterde vorm van mobiele meldingen die verder gaat dan eenvoudige tekstberichten door het opnemen van multimedia-elementen, zoals afbeeldingen, interactieve knoppen of andere rijke media-inhoud. Met deze versie is een set sjablonen voor uitgebreide pushmeldingen nu beschikbaar voor uw iOS- en Android-apps.

[Meer informatie](../push/rich-push.md)

>[!AVAILABILITY]
>
>Voor deze functie is een update naar Campagne v8.6.3 <!--or v8.7.2--> vereist. Leer meer in de console van de Cliënt van de Campagne v8 [&#x200B; versienota&#39;s &#x200B;](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes){target="_blank"}.

### Verbeteringen {#improvements-24-7}

**het beheer van Omslagen** - u kunt toestemmingen en beperkingen op omslagen nu beheren.

## Release-aantekeningen juni {#24-6-release}

**de datum van de Versie**: 18-19 juni, 2024

De volgende functies en verbeteringen zijn beschikbaar voor alle gebruikers vanaf de release in juni.


### Abonnementen en programma&#39;s {#24-6-4}

U kunt nu plannen en programma&#39;s maken om uw campagnes te organiseren. Door een mappenhiërarchie te definiëren, kunt u uw campagnes in programma&#39;s en uw programma&#39;s in plannen organiseren. [Meer informatie](../administration/plans-programs.md)

### Verbeteringen {#improvements-24-6}

* **Verzoening in de activiteit van de Verrijking**: De **verrijking** activiteit kan nu worden gebruikt om gegevens van het het gegevensbestandschema van de Campagne met gegevens van een ander schema, of met gegevens te verzoenen die uit een tijdelijk schema zoals gegevens komen die gebruikend een het dossieractiviteit van de Lading worden geupload. U kunt deze optie bijvoorbeeld gebruiken om het land van een profiel dat is opgegeven in een geüpload bestand, te combineren met een van de landen die beschikbaar zijn in de specifieke tabel van de Campagne-database. [Meer informatie](../workflows/activities/enrichment.md)


### Nieuwe functie in Beperkte Beschikbaarheid {#acs-24-6}

>[!AVAILABILITY]
>
>De volgende mogelijkheden zijn beperkt beschikbaar (LA). Het beperkte zich tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kan niet op een ander milieu worden opgesteld.

* **levering alarmerend**

De voorziening voor leveringswaarschuwingen is een systeem voor waarschuwingsbeheer dat een groep gebruikers in staat stelt automatisch meldingen te ontvangen die informatie bevatten over de uitvoering van hun leveringen. [Meer informatie](../msg/delivery-alerting.md)


## Release-aantekeningen mei {#24-5-release}

**de datum van de Versie**: 21 mei, 2024

De volgende functies en verbeteringen zijn beschikbaar voor alle gebruikers vanaf de release mei.

### Audit trail  {#24-5-1}

Het nieuwe **spoor van de Controle** vermogen verstrekt een gedetailleerd en chronologisch verslag van alle acties en gebeurtenissen die aan uw instantie van Adobe Campaign in real time zijn gemaakt. Het biedt een geschikte methode aan om alle veranderingen in uw gegevens van de Campagne te vinden, richtend vragen zoals: de status van werkschema&#39;s, de recentste individuen om hen te wijzigen, of de activiteiten die door gebruikers binnen de instantie worden uitgevoerd. [Meer informatie](../reporting/audit-trail.md)

### Aangepaste velden {#24-5-2}

**de gebieden van de Douane** zijn extra attributen die aan uit-van-de-doosschema&#39;s door de console van Adobe Campaign worden toegevoegd. In de webgebruikersinterface van Campagne zijn deze aangepaste velden nu zichtbaar in verschillende schermen, bijvoorbeeld de details van een profiel of een testprofiel. In de webgebruikersinterface kunt u geen aangepaste velden maken, maar u kunt nu de manier wijzigen waarop ze worden weergegeven. [Meer informatie](../administration/schemas-custom-fields.md)

### Koppelingen maken tussen tabellen {#24-5-3}

U kunt verbindingen met een andere lijst in de **het werkschemaactiviteit van de Verrijking** nu tot stand brengen. Gebruik de nieuwe **sectie van de definitie van de Verbinding** in de activiteitenparameters om een verband tussen de het werk lijstgegevens en het gegevensbestand van Adobe Campaign tot stand te brengen. Als u bijvoorbeeld gegevens laadt uit een bestand dat het rekeningnummer, land en e-mail van ontvangers bevat, kunt u nu een koppeling maken naar de landentabel om deze gegevens in hun profielen bij te werken. [Meer informatie](../workflows/activities/enrichment.md#create-links)

### Algemene verbeteringen {#improvements-24-5}

* **Directe post** - u kunt hefboomwerking de uitdrukkingsredacteur nu om de attributen aan vertoning in direct-mail extractiedossiers te selecteren. [Meer informatie](../direct-mail/content-direct-mail.md)

* **beheer van de Omslag** - u kunt een subomslag van een verschillend type dan de ouderomslag nu tot stand brengen. [Meer informatie](../get-started/permissions.md#folders)

* **Globalization** - als deel van onze aan de gang zijnde inspanning om een verenigde gebruikerservaring te leveren, harmoniseren wij de terminologie die in de producten en apps van Adobe Experience Cloud wordt gebruikt. Dit is van invloed op de Duitse term &quot;Titel&quot;, die wordt gewijzigd in &quot;Label&quot; wanneer deze betrekking heeft op de naam van een object. De wijzigingen worden geleidelijk doorgevoerd in de gebruikersinterface en de documentatie.


## Release-aantekeningen april {#april-24-4-release}

**de datum van de Versie**: 2 mei, 2024

### Nieuwe functies {#new-24-4}

De volgende functies zijn beschikbaar voor alle gebruikers vanaf de release van april.

**Nieuwe werkschemaactiviteiten**

* **gegevens van de Update** - gebruik deze activiteit om massa updates op gebieden in het gegevensbestand uit te voeren. Met verschillende opties kunt u de gegevensupdate aanpassen. [Meer informatie](../workflows/activities/update-data.md)
* **de diensten van het Abonnement** - Gebruik deze activiteit om veelvoudige profielen aan/van de dienst in één enkele actie in te tekenen of af te melden. [Meer informatie](../workflows/activities/subscription-services.md)
* **Extraheer dossier** - gebruik deze activiteit om gegevens van Adobe Campaign naar een ander systeem als extern dossier uit te voeren. [Meer informatie](../workflows/activities/extract-file.md)
* **dossier van de Overdracht** - gebruik deze activiteit om dossiers, test voor dossieraanwezigheid, of lijstdossiers op een server te ontvangen of te verzenden. Het gebruikte protocol kan of server-aan-server protocol of het protocol van HTTP zijn. [Meer informatie](../workflows/activities/transfer-file.md)
* **Test** - gebruik deze activiteit om overgangen toe te laten die op gespecificeerde voorwaarden worden gebaseerd. [Meer informatie](../workflows/activities/test.md)
* **code van JavaScript** - gebruik deze activiteit om een de codefragment van JavaScript in de context van een werkschema uit te voeren. [Meer informatie](../workflows/activities/javascript-code.md)
* **Extern signaal** - gebruik deze activiteit om de uitvoering van een werkschema van een ander werkschema, of een API vraag teweeg te brengen. [Meer informatie](../workflows/activities/external-signal.md)
* **Incrementele vraag** - gebruik deze activiteit om het gegevensbestand op een geplande basis te vragen. Telkens wanneer deze activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten. Hierdoor kunt u alleen nieuwe elementen als doel instellen. [Meer informatie](../workflows/activities/incremental-query.md)

**de rijke malplaatjes van het Bericht van de Duw**

U kunt nu uitgebreide pushberichten verzenden via Android. Een veeleisende pushmelding is een verbeterde vorm van mobiele meldingen die verder gaat dan eenvoudige tekstberichten door het opnemen van multimedia-elementen, zoals afbeeldingen, interactieve knoppen of andere rijke media-inhoud. [Meer informatie](../push/rich-push.md)

Merk op dat deze eigenschap in **Beperkte Beschikbaarheid** (LA) is.


### Nieuwe functies in beperkte beschikbaarheid {#acs-24-4}

>[!AVAILABILITY]
>
>De volgende mogelijkheden zijn in Beperkte Beschikbaarheid (LA). Zij zijn beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kunnen niet op een ander milieu worden opgesteld.
>
>Verwijs naar de volgende documentatiepagina&#39;s: [&#x200B; overgang Campaign Standard aan Campagne v8 &#x200B;](../rn/acs-migration.md) en [&#x200B; Eigenschappen voor de gebruikers van Campaign Standard &#x200B;](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Branding** - als Campaign Standard migreerde gebruiker, kunnen uw technische beheerders één of verscheidene merken nu bepalen om de parameters te centraliseren die de identiteit van een merk beïnvloeden. Dit zijn onder andere het merklogo, het domein van de toegangs-URL voor de landingspagina&#39;s of de instellingen voor de tracking van berichten. U kunt deze merken maken en deze koppelen aan berichten of bestemmingspagina&#39;s. Deze configuratie wordt beheerd in malplaatjes. [Meer informatie](../administration/branding/branding-gs.md)

* **Rest APIs** - als Campaign Standard gemigreerde gebruiker, kunt u Rest APIs gebruiken om integraties voor Adobe Campaign tot stand te brengen en uw eigen ecosysteem te bouwen door Adobe Campaign met het paneel van technologieën te verbinden die u gebruikt. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html)

* **Dynamische Rapportering** - als Campaign Standard gemigreerde gebruiker, kunt u tot Dynamische Rapportering toegang hebben die volledig klantgerichte en real-time rapporten verstrekt om het effect van uw marketing activiteiten te meten. Het voegt toegang tot profielgegevens toe, toelatend demografische analyse door profieldimensies zoals geslacht, stad en leeftijd naast functionele e-mailcampagnegegevens zoals opent en klikt. [Meer informatie](../reporting/dynamic-reporting/get-started-reporting.md)

* **het Bestaan Pagina&#39;s** - de volgende verbeteringen aan het landen van pagina&#39;s zijn slechts beschikbaar aan gebruikers die van Campaign Standard overgaan:

   * U kunt nu naar een standaardlandingspagina voor abonnementen/abonnementen verwijzen wanneer u een service configureert. Als u bij het ontwerpen van een e-mailbericht een koppeling naar die landingspagina definieert, worden gebruikers die het formulier voor de bestemmingspagina verzenden, automatisch geabonneerd op of geabonneerd van deze service. [Meer informatie](../audience/manage-services.md#create-service)
   * Een nieuwe optie in de configuratie van de bestemmingspagina staat anonieme bezoekers toe om tot de landingspagina toegang te hebben. Als u deze optie uitschakelt, kunnen alleen geïdentificeerde gebruikers het formulier openen en verzenden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie in de configuratie van de bestemmingspagina kunt u aanvullende interne gegevens opslaan wanneer de bestemmingspagina wordt verzonden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie kunt u een openingspagina gebruiken voor verschillende services, waardoor deze dynamisch wordt. Als u een koppeling naar een e-mailbericht toevoegt en u een dynamische bestemmingspagina selecteert, kunt u elke gewenste service selecteren. Als u een landingspagina selecteert waaraan een specifieke service is gekoppeld, wordt deze service automatisch gebruikt (u kunt geen andere service selecteren). [Meer informatie](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Voorwaardelijke inhoud wordt nu ondersteund in bestemmingspagina&#39;s. [Meer informatie](../landing-pages/lp-content.md)

### Algemene verbeteringen {#improvements-24-4}

De verbeteringen hieronder zijn beschikbaar aan alle klanten vanaf de release van april.

* De **het dossier van de Lading** activiteit is verbeterd met verscheidene secties die u toestaan om een steekproefdossier te uploaden, om fouten te beheren en, geuploade dossiers te schrappen nadat de activiteit is uitgevoerd. [Meer informatie](../workflows/activities/load-file.md)


* U kunt activiteiten **van een werkschema aan een ander werkschema van een verschillende browser tabel nu kopiëren/kleven.** [Meer informatie](../workflows/orchestrate-activities.md#copy-activities-copy)

* Alle werkschemaactiviteiten staan u nu toe om hun **uitvoeringsopties** te beheren. Hiermee kunt u de uitvoeringsmodus en het gedrag van de activiteit definiëren in het geval van fouten. [Meer informatie](../workflows/orchestrate-activities.md#execution-options-execution)

* &quot;Activeer niet de overgang als de bevolking&quot;optie in de **Gesplitste activiteit** leeg is staat u toe om te kiezen of het werkschema naar de volgende activiteit zou moeten overgaan wanneer het segmentresultaat leeg is. [Meer informatie](../workflows/activities/split.md)

## Opmerkingen bij de release maart {#24-3-release}

>[!AVAILABILITY]
>
>Deze versie is beschikbaar aan alle gebruikers die [&#x200B; Campagne (console) v8.6 versie beginnen &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html). Leer meer over de versies en verbeteringen van de de cliëntconsole van Adobe Campaign in [&#x200B; Campagne v8 (console) documentatie &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html){target="_blank"}.

**de datum van de Versie**: Maart 19-20, 2024

### Direct Mail Channel {#24-3-dm}

**kanaal van 0&rbrace; Directe post &lbrace;is nu beschikbaar voor gebruik in werkschema&#39;s en als standalone leveringen.** Directe post is een off-line kanaal dat u toestaat om een extractiedossiers tot stand te brengen, te personaliseren en te produceren, en het met uw directe postleveranciers te delen om post naar uw klanten te verzenden.

### Nieuwe werkstroomactiviteit gegevensbron wijzigen {#24-3-change-data-source}

De **gegevensbron van de Verandering** richtend activiteit staat u toe om de gegevensbron te veranderen die door de werkende lijst van uw werkschema wordt gebruikt. Deze activiteit verstrekt meer flexibiliteit door u toe te staan om gegevens over uw verschillende gegevensbestanden te beheren en prestaties te verbeteren.

### Verbetering van workflowactiviteit splitsen {#24-3-split}

U kunt **nu gebruiken produceert alle ondergroepen in de zelfde lijst** optie in de **Gesplitste** werkschemaactiviteit om alle ondergroepen in één enkele outputovergang te groeperen.

### Query-modelleraar {#24-3-query-modeler}

* Het querymodel is nu beschikbaar voor gebruik in de e-mail-Designer. Hiermee kunt u voorwaarden maken wanneer u voorwaardelijke inhoud maakt.
* Vooraf gedefinieerde waarden zijn nu beschikbaar voor datumtekstkenmerken wanneer u een aangepaste voorwaarde maakt.
* Operatoren kunnen niet meer worden toegevoegd aan een nieuwe overgang in het diagram. Ze kunnen alleen aan een bestaande overgang worden toegevoegd voordat u componenten filtert om deze samen te groeperen.