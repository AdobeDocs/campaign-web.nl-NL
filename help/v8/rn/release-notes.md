---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 385c931c9fae7386c2a2f1ef471a9cd7c4a47696
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 5%

---

# Aanvullende informatie  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie "
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

## Release-aantekeningen juni {#24-6-release}

**Releasedatum**: 18-19 juni 2024

De volgende functies en verbeteringen zijn beschikbaar voor alle gebruikers vanaf de release in juni.
<!--
### Visual fragments {#24-6-1}

You can now author, use, and manage **visual** fragments to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process.

### Seed lists {#24-6-2}

A seed list, aka. **Trap group**, is a list of seed addresses. It is used to include specific addresses in your deliveries, and then target profiles who do not match the defined target criteria. This way, recipients who are out of the delivery audience can receive the delivery, as any other target recipient would. You can use seed addresses when sending proofs, or to protect your mailing list.-->

### Afleveringswaarschuwing {#24-6-3}

De voorziening voor leveringswaarschuwingen is een systeem voor waarschuwingsbeheer dat een groep gebruikers in staat stelt automatisch meldingen te ontvangen die informatie bevatten over de uitvoering van hun leveringen. [Meer informatie](../msg/delivery-alerting.md)

### Abonnementen en programma&#39;s {#24-6-4}

U kunt nu plannen en programma&#39;s maken om uw campagnes te organiseren. Door een mappenhiërarchie te definiëren, kunt u uw campagnes in programma&#39;s en uw programma&#39;s in plannen organiseren. [Meer informatie](../administration/plans-programs.md)

### Verbeteringen {#improvements-24-6}

* **Afstemming van verrijkingsactiviteiten**: De verrijkingsactiviteit kan nu worden gebruikt om gegevens van het het gegevensbestandschema van de Campagne met gegevens van een ander schema, of met gegevens te verzoenen die uit een tijdelijk schema zoals gegevens komen die gebruikend een het dossieractiviteit van de Lading worden geupload. U kunt deze optie bijvoorbeeld gebruiken om het land van een profiel dat is opgegeven in een geüpload bestand, te combineren met een van de landen die beschikbaar zijn in de specifieke tabel van de Campagne-database. [Meer informatie](../workflows/activities/enrichment.md)

## Release-aantekeningen mei {#24-5-release}

**Releasedatum**: 21 mei 2024

De volgende functies en verbeteringen zijn beschikbaar voor alle gebruikers vanaf de release mei.

### Audit trail  {#24-5-1}

De nieuwe **Audittrail** biedt een gedetailleerd en chronologisch overzicht van alle acties en gebeurtenissen die in real-time aan uw Adobe Campaign-exemplaar zijn uitgevoerd. Het biedt een geschikte methode aan om alle veranderingen in uw gegevens van de Campagne te vinden, richtend vragen zoals: de status van werkschema&#39;s, de recentste individuen om hen te wijzigen, of de activiteiten die door gebruikers binnen de instantie worden uitgevoerd. [Meer informatie](../reporting/audit-trail.md)

### Aangepaste velden {#24-5-2}

**Aangepaste velden** zijn extra kenmerken die via de Adobe Campaign-console aan de out-of-the-box-schema&#39;s worden toegevoegd. In de webgebruikersinterface van Campagne zijn deze aangepaste velden nu zichtbaar in verschillende schermen, bijvoorbeeld de details van een profiel of een testprofiel. In de webgebruikersinterface kunt u geen aangepaste velden maken, maar u kunt nu de manier wijzigen waarop ze worden weergegeven. [Meer informatie](../administration/custom-fields.md)

### Koppelingen maken tussen tabellen {#24-5-3}

U kunt nu koppelingen maken met een andere tabel in het dialoogvenster **Verrijking** workflowactiviteit. De nieuwe **Koppelingsdefinitie** in de activiteitsparameters om een koppeling tot stand te brengen tussen de gegevens van de werkende lijst en het gegevensbestand van Adobe Campaign. Als u bijvoorbeeld gegevens laadt uit een bestand dat het rekeningnummer, land en e-mail van ontvangers bevat, kunt u nu een koppeling maken naar de landentabel om deze gegevens in hun profielen bij te werken. [Meer informatie](../workflows/activities/enrichment.md#create-links)

<!--
### Content fragments {#24-5-4}

* You can now author, use, and save **visual fragments** to quickly assemble your emails and content templates. A fragment is a prebuilt reusable component that can be referenced in multiple emails across Adobe Campaign for an improved and accelerated design process. [Learn more](../email/fragments.md)

* You can now author, use, and manage **expression fragments** to quickly build personalized content. A fragment is a prebuilt reusable component that can be referenced in multiple contents across Adobe Campaign for an improved and accelerated design process.-->


### Algemene verbeteringen {#improvements-24-5}

* **Directe post** - U kunt nu de expressie-editor gebruiken om de kenmerken te selecteren die u wilt weergeven in bestanden voor directe mailextractie. [Meer informatie](../direct-mail/content-direct-mail.md)

* **Mapbeheer** - U kunt nu een submap van een ander type maken dan de bovenliggende map. [Meer informatie](../get-started/permissions.md#folders)


<!--* **Execution options for workflows** - You can now define execution options for your workflows, such as the maximum duration, the affinity, or the time zone.-->

* **Globalisatie** - Als onderdeel van onze voortdurende inspanningen om een uniforme gebruikerservaring te bieden, harmoniseren we de terminologie die wordt gebruikt in de Adobe Experience Cloud-producten en -toepassingen. Dit is van invloed op de Duitse term &quot;Titel&quot;, die wordt gewijzigd in &quot;Label&quot; wanneer deze betrekking heeft op de naam van een object. De wijzigingen worden geleidelijk doorgevoerd in de gebruikersinterface en de documentatie.


## Release-aantekeningen april {#april-24-4-release}

**Releasedatum** 2 mei 2024

### Nieuwe functies {#new-24-4}

De volgende functies zijn beschikbaar voor alle gebruikers vanaf de release van april.

**Nieuwe workflowactiviteiten**

* **Gegevens bijwerken** - Gebruik deze activiteit om massa-updates op gebieden in het gegevensbestand uit te voeren. Met verschillende opties kunt u de gegevensupdate aanpassen. [Meer informatie](../workflows/activities/update-data.md)
* **Abonnementsdiensten** - Gebruik deze activiteit om meerdere profielen in te schrijven op of af te melden bij een service in één actie. [Meer informatie](../workflows/activities/subscription-services.md)
* **Bestand uitpakken** - Gebruik deze activiteit om gegevens van Adobe Campaign naar een ander systeem als extern dossier uit te voeren. [Meer informatie](../workflows/activities/extract-file.md)
* **Bestand overbrengen** - Gebruik deze activiteit om bestanden te ontvangen of te verzenden, om te testen op bestandsaanwezigheid of om bestanden op een server weer te geven. Het gebruikte protocol kan of server-aan-server protocol of het protocol van HTTP zijn. [Meer informatie](../workflows/activities/transfer-file.md)
* **Testen** - Gebruik deze activiteit om overgangen toe te laten die op gespecificeerde voorwaarden worden gebaseerd. [Meer informatie](../workflows/activities/test.md)
* **JavaScript-code** - Gebruik deze activiteit om een JavaScript codefragment in de context van een werkschema uit te voeren. [Meer informatie](../workflows/activities/javascript-code.md)
* **Extern signaal** - Gebruik deze activiteit om de uitvoering van een werkschema van een andere werkschema, of een API vraag teweeg te brengen. [Meer informatie](../workflows/activities/external-signal.md)
* **Incrementele query** - Gebruik deze activiteit om het gegevensbestand op een geplande basis te vragen. Telkens wanneer deze activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten. Hierdoor kunt u alleen nieuwe elementen als doel instellen. [Meer informatie](../workflows/activities/incremental-query.md)

**Sjablonen voor uitgebreide pushmeldingen**

U kunt nu uitgebreide pushmeldingen verzenden via Android. Een veeleisende pushmelding is een verbeterde vorm van mobiele meldingen die verder gaat dan eenvoudige tekstberichten door het opnemen van multimedia-elementen, zoals afbeeldingen, interactieve knoppen of andere rijke media-inhoud. [Meer informatie](../push/rich-push.md)

Deze functie bevindt zich in **Beperkte beschikbaarheid** (LA).


### Nieuwe functies in beperkte beschikbaarheid {#acs-24-4}

>[!AVAILABILITY]
>
>De volgende mogelijkheden zijn in Beperkte Beschikbaarheid (LA). Ze zijn beperkt tot klanten die migreren **van Adobe Campaign Standard naar Adobe Campaign v8**, en kan niet worden ingezet op een andere omgeving.
>
>Raadpleeg de volgende documentatiepagina&#39;s: [Overgang van Campaign Standard naar Campagne v8](../rn/acs-migration.md) en [Functies voor Campaigns Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Branding** - Als gemigreerde gebruiker van een Campaign Standard kunnen uw technische beheerders nu een of meerdere merken definiëren om de parameters die de identiteit van een merk beïnvloeden, te centraliseren. Dit zijn onder andere het merklogo, het domein van de toegangs-URL voor de landingspagina&#39;s of de instellingen voor de tracking van berichten. U kunt deze merken maken en deze koppelen aan berichten of bestemmingspagina&#39;s. Deze configuratie wordt beheerd in malplaatjes. [Meer informatie](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest APIs** - Als gemigreerde gebruiker van een Campaign Standard kunt u Rest API&#39;s gebruiken om integratie voor Adobe Campaign te maken en uw eigen ecosysteem te bouwen door Adobe Campaign te koppelen aan het deelvenster met technologieën dat u gebruikt. [Meer informatie](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Dynamische rapportage** - Als gemigreerde gebruiker van het Campaign Standard, kunt u tot Dynamische Rapportering toegang hebben die volledig klantgerichte en real-time rapporten verstrekt om de invloed van uw marketing activiteiten te meten. Het voegt toegang tot profielgegevens toe, toelatend demografische analyse door profieldimensies zoals geslacht, stad en leeftijd naast functionele e-mailcampagnegegevens zoals opent en klikt. [Meer informatie](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Openingspagina&#39;s** - De volgende verbeteringen aan bestemmingspagina&#39;s zijn alleen beschikbaar voor gebruikers die van Campaign Standard overgaan:

   * U kunt nu naar een standaardlandingspagina voor abonnementen/abonnementen verwijzen wanneer u een service configureert. Als u bij het ontwerpen van een e-mailbericht een koppeling naar die landingspagina definieert, worden gebruikers die het formulier voor de bestemmingspagina verzenden, automatisch geabonneerd op of geabonneerd van deze service. [Meer informatie](../audience/manage-services.md#create-service)
   * Een nieuwe optie in de configuratie van de bestemmingspagina staat anonieme bezoekers toe om tot de landingspagina toegang te hebben. Als u deze optie uitschakelt, kunnen alleen geïdentificeerde gebruikers het formulier openen en verzenden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie in de configuratie van de bestemmingspagina kunt u aanvullende interne gegevens opslaan wanneer de bestemmingspagina wordt verzonden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie kunt u een openingspagina gebruiken voor verschillende services, waardoor deze dynamisch wordt. Als u een koppeling naar een e-mailbericht toevoegt en u een dynamische bestemmingspagina selecteert, kunt u elke gewenste service selecteren. Als u een landingspagina selecteert waaraan een specifieke service is gekoppeld, wordt deze service automatisch gebruikt (u kunt geen andere service selecteren). [Meer informatie](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Voorwaardelijke inhoud wordt nu ondersteund in bestemmingspagina&#39;s. [Meer informatie](../landing-pages/lp-content.md)

### Algemene verbeteringen {#improvements-24-4}

De verbeteringen hieronder zijn beschikbaar aan alle klanten vanaf de release van april.
<!--**Workflow - Copy/Paste into another tab**: -->

* De **Bestand laden** De activiteit is verbeterd met verscheidene secties toelatend u om een steekproefdossier te uploaden, fouten te beheren en geuploade dossiers te schrappen nadat de activiteit is uitgevoerd. [Meer informatie](../workflows/activities/load-file.md)


* U kunt nu **kopiëren/plakken-activiteiten** van een workflow naar een andere workflow vanuit een ander browsertabblad. [Meer informatie](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Met alle workflowactiviteiten kunt u nu hun **uitvoeringsopties**. Hiermee kunt u de uitvoeringsmodus en het gedrag van de activiteit definiëren in het geval van fouten. [Meer informatie](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* De optie &quot;De overgang niet activeren als de populatie leeg is&quot; in het dialoogvenster **Gesplitste activiteit** staat u toe om te kiezen of het werkschema naar de volgende activiteit zou moeten overgaan wanneer het segmentresultaat leeg is. [Meer informatie](../workflows/activities/split.md)



## Opmerkingen bij de release maart {#24-3-release}

>[!AVAILABILITY]
>
>Deze versie is beschikbaar voor alle gebruikers die beginnen [Campagne (console) v8.6-release](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html). Meer informatie over de release en upgrades van de Adobe Campaign-clientconsole in [Campagne v8 (console)-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html){target="_blank"}.

**Releasedatum**: 19-20 maart 2024

### Direct Mail Channel {#24-3-dm}

**Directe post** kanaal is nu beschikbaar voor gebruik in werkschema&#39;s en als standalone leveringen. Directe post is een off-line kanaal dat u toestaat om een extractiedossiers tot stand te brengen, te personaliseren en te produceren, en het met uw directe postleveranciers te delen om post naar uw klanten te verzenden.

### Nieuwe werkstroomactiviteit gegevensbron wijzigen {#24-3-change-data-source}

De **Gegevensbron wijzigen** Door doelactiviteit toe te wijzen, kunt u de gegevensbron wijzigen die wordt gebruikt door de werktabel van uw werkstroom. Deze activiteit verstrekt meer flexibiliteit door u toe te staan om gegevens over uw verschillende gegevensbestanden te beheren en prestaties te verbeteren.

### Verbetering van workflowactiviteit splitsen {#24-3-split}

U kunt nu de opdracht **Alle subsets in dezelfde tabel genereren** in de **Splitsen** workflowactiviteit om alle subsets te groeperen in één uitvoerovergang.

### Query-modelleraar {#24-3-query-modeler}

* Het querymodel is nu beschikbaar voor gebruik in de e-mailontwerper. Hiermee kunt u voorwaarden maken wanneer u voorwaardelijke inhoud maakt.
* Vooraf gedefinieerde waarden zijn nu beschikbaar voor datumtekstkenmerken wanneer u een aangepaste voorwaarde maakt.
* Operatoren kunnen niet meer worden toegevoegd aan een nieuwe overgang in het diagram. Ze kunnen alleen aan een bestaande overgang worden toegevoegd voordat u componenten filtert om deze samen te groeperen.
