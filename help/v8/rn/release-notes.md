---
title: Opmerkingen bij de laatste release
description: Ontdek nieuwe eigenschap die met het Web van de Campagne Gebruikersinterface komt
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: ba187eaebf299e5d2ee303c4e15180d35a9e6180
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 6%

---

# Aanvullende informatie  {#latest-release}

<!--Last update: **March 19, 2024**-->

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

## Release-aantekeningen april {#april-24-4-release}

**Releasedatum**: 30 april 2024

### Nieuwe functies {#new-24-4}

De volgende functies zijn beschikbaar voor alle gebruikers vanaf de release van april.

**Nieuwe workflowactiviteiten**

* **Gegevens bijwerken** - Gebruik deze activiteit om massa-updates op gebieden in het gegevensbestand uit te voeren. Met verschillende opties kunt u de gegevensupdate aanpassen. [Meer informatie](../workflows/activities/update-data.md)
* **Abonnementsdiensten** - Gebruik deze activiteit als u zich op meerdere profielen wilt abonneren op of een abonnement wilt nemen op een service in één actie. [Meer informatie](../workflows/activities/subscription-services.md)
* **Bestand uitpakken** - Gebruik deze activiteit om gegevens van Adobe Campaign naar een ander systeem als extern dossier uit te voeren. [Meer informatie](../workflows/activities/extract-file.md)
* **Bestand overbrengen** - Gebruik deze activiteit om bestanden te ontvangen of te verzenden, om te testen op bestandsaanwezigheid of om bestanden op een server weer te geven. Het gebruikte protocol kan of server-aan-server protocol of het protocol van HTTP zijn. [Meer informatie](../workflows/activities/transfer-file.md)
* **Testen** - Gebruik deze activiteit om overgangen toe te laten die op gespecificeerde voorwaarden worden gebaseerd. [Meer informatie](../workflows/activities/test.md)
* **JavaScript-code** - Gebruik deze activiteit om een JavaScript codefragment in de context van een werkschema uit te voeren. [Meer informatie](../workflows/activities/javascript-code.md)
* **Extern signaal** - Gebruik deze activiteit om de uitvoering van een werkschema van een andere werkschema,* of een API vraag teweeg te brengen. [Meer informatie](../workflows/activities/external-signal.md)
* **Incrementele query** - Gebruik deze activiteit om het gegevensbestand op een geplande basis te vragen. Telkens wanneer deze activiteit wordt uitgevoerd, worden de resultaten van de vorige uitvoeringen uitgesloten. Hierdoor kunt u alleen nieuwe elementen als doel instellen. [Meer informatie](../workflows/activities/incremental-query.md)

**Sjablonen voor uitgebreide pushmeldingen**

U kunt nu uitgebreide pushmeldingen verzenden via Android. Een veeleisende pushmelding is een verbeterde vorm van mobiele meldingen die verder gaat dan eenvoudige tekstberichten door het opnemen van multimedia-elementen, zoals afbeeldingen, interactieve knoppen of andere rijke media-inhoud. [Meer informatie](../push/rich-push.md)

Deze functie bevindt zich in **Beperkte beschikbaarheid** (LA).

<!--
* **Audit Trail**

The Audit trail feature constantly records a detailed log of actions and events taking place within the Adobe Campaign instance in real-time. It offers a convenient method to access a chronological record of data, addressing queries such as: the status of workflows, the latest individuals to modify them, or the activities performed by users within the instance.
-->

### Nieuwe functies in beperkte beschikbaarheid {#acs-24-4}

>[!AVAILABILITY]
>
>De volgende mogelijkheden zijn in Beperkte Beschikbaarheid (LA). Ze zijn beperkt tot klanten die migreren **van Adobe Campaign Standard naar Adobe Campaign v8**, en kan niet worden ingezet op een andere omgeving.
>
>Raadpleeg de volgende documentatiepagina&#39;s: [Overgang van Campaign Standard naar Campagne v8](../rn/acs-migration.md) en [Functies voor Campaigns Standard](https://experienceleague.adobe.com/docs/experience-cloud/campaign/campaign-standard-migration-home.html).

* **Branding** - Als gemigreerde gebruiker van een Campaign Standard kunnen uw technische beheerders nu een of meerdere merken definiëren om de parameters die de identiteit van een merk beïnvloeden, te centraliseren. Dit zijn onder andere het merklogo, het domein van de toegangs-URL voor de landingspagina&#39;s of de instellingen voor de tracking van berichten. U kunt deze merken maken en deze koppelen aan berichten of bestemmingspagina&#39;s. Deze configuratie wordt beheerd in malplaatjes. [Meer informatie](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html)

* **Rest APIs** - Als gemigreerde gebruiker van een Campaign Standard kunt u Rest API&#39;s gebruiken om integratie voor Adobe Campaign te maken en uw eigen ecosysteem te bouwen door Adobe Campaign te koppelen aan het deelvenster met technologieën dat u gebruikt. [Meer informatie](https://experienceleague.adobe.com/docs/experience-cloud/campaign/apis/get-started-apis.html)

* **Dynamische rapportage** - Als gemigreerde gebruiker van het Campaign Standard, kunt u tot Dynamische Rapportering toegang hebben die volledig klantgerichte en real-time rapporten verstrekt om de invloed van uw marketing activiteiten te meten. Het voegt toegang tot profielgegevens toe, toelatend demografische analyse door profieldimensies zoals geslacht, stad en leeftijd naast functionele e-mailcampagnegegevens zoals opent en klikt. [Meer informatie](https://experienceleague.adobe.com/docs/experience-cloud/campaign/reporting/get-started-reporting.html)

* **Verbetering bestandsactiviteit laden** - de **Bestand laden** De activiteit is verbeterd met verscheidene secties toelatend u om een steekproefdossier te uploaden, fouten te beheren en geuploade dossiers te schrappen nadat de activiteit is uitgevoerd. [Meer informatie](../workflows/activities/load-file.md)

* **Openingspagina&#39;s** - De volgende verbeteringen aan bestemmingspagina&#39;s zijn alleen beschikbaar voor gebruikers die van Campaign Standard overgaan:

   * U kunt nu naar een standaardlandingspagina voor abonnementen/abonnementen verwijzen wanneer u een service configureert. Als u bij het ontwerpen van een e-mailbericht een koppeling naar die landingspagina definieert, worden gebruikers die het formulier voor de bestemmingspagina verzenden, automatisch geabonneerd op of geabonneerd van deze service. [Meer informatie](../audience/manage-services.md#create-service)
   * Een nieuwe optie in de configuratie van de bestemmingspagina staat anonieme bezoekers toe om tot de landingspagina toegang te hebben. Als u deze optie uitschakelt, kunnen alleen geïdentificeerde gebruikers het formulier openen en verzenden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie in de configuratie van de bestemmingspagina kunt u aanvullende interne gegevens opslaan wanneer de bestemmingspagina wordt verzonden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie kunt u een openingspagina gebruiken voor verschillende services, waardoor deze dynamisch wordt. Als u een koppeling naar een e-mailbericht toevoegt en u een dynamische bestemmingspagina selecteert, kunt u elke gewenste service selecteren. Als u een landingspagina selecteert waaraan een specifieke service is gekoppeld, wordt deze service automatisch gebruikt (u kunt geen andere service selecteren). [Meer informatie](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Voorwaardelijke inhoud wordt nu ondersteund in bestemmingspagina&#39;s. [Meer informatie](../landing-pages/lp-content.md)

### Algemene verbeteringen {#improvements-24-4}

De verbeteringen hieronder zijn beschikbaar aan alle klanten vanaf de release van april.
<!--**Workflow - Copy/Paste into another tab**: -->

* U kunt activiteiten nu kopiëren/plakken van een workflow naar een andere workflow vanuit een ander browsertabblad. [Meer informatie](../workflows/orchestrate-activities.md#copy-activities-copy)

<!--**Workflow - Execution options**: -->

* Met alle workflowactiviteiten kunt u nu de uitvoeringsopties ervan beheren. Hiermee kunt u de uitvoeringsmodus en het gedrag van de activiteit definiëren in het geval van fouten. [Meer informatie](../workflows/orchestrate-activities.md#execution-options-execution)

<!-- **Workflow - Split Activity - Support Skipping Empty Transition**: -->

* De optie &quot;De overgang niet activeren als de populatie leeg is&quot; in het dialoogvenster **Gesplitste activiteit** staat u toe om te kiezen of het werkschema naar de volgende activiteit zou moeten overgaan wanneer het segmentresultaat leeg is. [Meer informatie](../workflows/activities/split.md)

<!--* **Support of custom fields**-->

* Aangepaste velden zijn aanvullende kenmerken die via de Adobe Campaign-console aan de out-of-the-box-schema&#39;s worden toegevoegd. In de webgebruikersinterface van Campagne zijn deze aangepaste velden nu zichtbaar in verschillende schermen, bijvoorbeeld de details van een profiel of een testprofiel. In de webgebruikersinterface kunt u geen aangepaste velden maken, maar u kunt nu de manier wijzigen waarop ze worden weergegeven. [Meer informatie](../administration/custom-fields.md)


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
