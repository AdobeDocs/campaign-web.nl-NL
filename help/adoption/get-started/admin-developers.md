---
title: Ga aan de slag met Adobe Campaign v8 voor beheerders en ontwikkelaars.
description: Deze zelfstudie geeft een overzicht van de belangrijkste functies voor beheer en gegevensbeheer van Campaign v8. Het is bedoeld voor beheerders en de technische markeertekens die van Campaign Standard naar Campaign v8 migreren.
role: Admin, Developer
level: Beginner, Experienced
exl-id: 1554f85f-22e1-4b51-a916-194ea0d24816
source-git-commit: 2093338e3ba9f31954561171029ec0f7336c73c4
workflow-type: tm+mt
source-wordcount: '2777'
ht-degree: 3%

---

# Aan de slag met beheerders en ontwikkelaars {#acs-gs-admin}

Deze pagina bevat een overzicht van de belangrijkste functies voor beheer en gegevensbeheer van Campaign v8. Het is voor beheerders en technische marketers die van Campaign Standard aan Campaign v8 overgaan.

De belangrijkste wijziging voor u is de introductie van de clientconsole, de native toepassing die communiceert met de Adobe Campaign-toepassingsserver.

De de cliëntconsole van de Campagne centraliseert alle mogelijkheden en montages. Het wordt gesynchroniseerd met het de gebruikersinterface van het Web van de Campagne, die consistentie over beide milieu&#39;s verzekert.

![](assets/client_console.png){zoomable="yes"}

[ Leer meer over het gebruikersinterface van de cliëntconsole van Adobe Campaign v8 ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/new/campaign-ui#ui-access){target="_blank"}.

## Campagne v8-architectuur {#acs-gs-admi-archi}

De architectuur van de campagne is gedetailleerd in de documentatie van Campagne v8 (console). Leer grondbeginselen in [ deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/config/architecture/general-architecture){target="_blank"}.

Nuttige koppeling om te beginnen:

* De componenten van Adobe Campaign en globale architectuur worden beschreven in [ deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/new/ac-components){target="_blank"}.

* Verwijs naar [ Begonnen met de architectuur van de Campagne ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/config/architecture/architecture){target="_blank"} om de architectuur van de Campagne te begrijpen alvorens te beginnen om uw instantie te structureren.

<!--Two deployment models are available: **Campaign FDA deployment** (P1-P3) and **Campaign Enterprise (FFDA)** deployment (P4). As a customer transitioning from Campaign Standard, your deployment model is **Campaign FDA**.-->

* Transactioneel overseinen (het Centrum van het Bericht) is de Campagne v8 module die voor het beheren van teweeggebrachte berichten wordt ontworpen. Het baseert zich op een specifiek architectuurmodel dat in [ dit sectie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/config/architecture/architecture#transac-msg-archi){target="_blank"} wordt gedetailleerd.

## Campagne-clientconsole {#acs-gs-console}

### De clientconsole installeren {#acs-gs-admin-console}

De taken van het beleid en van de configuratie worden uitgevoerd in de cliëntconsole. De eerste stap is het instellen van uw omgeving.

Campagne-clientconsole is een native toepassing die communiceert met de Adobe Campaign-toepassingsserver via standaard internetprotocollen, zoals SOAP en HTTP. De de cliëntconsole van de campagne centraliseert alle mogelijkheden en montages, en vereist minimale bandbreedte aangezien het op een lokaal geheime voorgeheugen baseert. Campagne-clientconsole is ontworpen voor eenvoudige implementatie en kan worden geïmplementeerd vanuit een internetbrowser, automatisch worden bijgewerkt. Hiervoor is geen specifieke netwerkconfiguratie nodig omdat alleen HTTP(S)-verkeer wordt gegenereerd.

In de volgende video wordt uitgelegd hoe u de Adobe Campaign Client Console kunt downloaden en installeren en hoe u de verbinding met uw instantie kunt beheren.

>[!VIDEO](https://video.tv.adobe.com/v/3449887?quality=12&learn=on&captions=dut){transcript=true}

Voor meer informatie, zie [ verbinden met Campagne met de cliëntconsole ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/new/connect){target="_blank"}.

De clientconsole moet in een ondersteunde omgeving worden geïnstalleerd. Leer meer in [ de verenigbaarheidsmatrijs van de Campagne v8 (console) ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/releases/compatibility-matrix#ClientConsoleoperatingsystems){target="_blank"}.

### De interface van de clientconsole detecteren  {#acs-gs-ui}

In deze zelfstudie leert u meer over de Adobe Campaign v8-gebruikersinterface en hoe u door de hoofdfuncties kunt navigeren.

>[!VIDEO](https://video.tv.adobe.com/v/3426441?quality=12&learn=on&captions=dut){transcript=true}

Zie [ Werk met de cliëntconsole ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/new/campaign-ui){target="_blank"} voor meer details.

## De omgeving beheren {#acs-gs-admin-env}

Zodra de cliëntconsole wordt geïnstalleerd, volg de stappen in deze documentatie om de verbinding aan de toepassingsserver tot stand te brengen: [ Verbinding aan de documentatie van de toepassingsserver ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/new/connect#create-your-connection){target="_blank"}.

Beveiligingspraktijken zijn diep verankerd in onze interne processen en tools voor softwareontwikkeling en -bewerkingen en worden rigoureus gevolgd door onze interfunctionele teams om incidenten op een snelle manier te voorkomen, op te sporen en erop te reageren. Leer meer in [ beste praktijken van de Veiligheid van de Campagne ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/privacy/security){target="_blank"}.

### Toegangsrechten en machtigingen {#acs-gs-admin-rights}

Met Adobe Campaign kunt u de rechten definiëren en beheren die aan gebruikers zijn toegewezen. Deze machtigingen worden gedefinieerd door machtigingen voor groepen van operatoren, benoemde rechten en machtigingen voor mappen te combineren.

Als Campaign Standard-gebruiker die overschakelt naar Campagne v8, blijven uw machtigingen en toegangsrechten gelijk. Adobe heeft beveiligingsgroepen verplaatst naar de groepen met deelnemers aan Campagne v8 en uw machtigingen per organisatie zijn overgebracht naar mapmachtigingen. Campagnegebruikers   gebruik hun Adobe ID om verbinding te maken met Campagne v8 en kan vervolgens dezelfde aanmelding en hetzelfde wachtwoord gebruiken als in Campaign Standard.

De campagne [ omslagen ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/config/configuration/folders-and-views){target="_blank"} zijn knopen in de ontdekkingsboomstructuur van de cliëntconsole. Gebaseerd op hun type, bevatten zij bepaalde soorten gegevens. Programma&#39;s worden geconcretiseerd door mappen in Campaign v8. U kunt mappen maken en machtigingen voor deze mappen beheren om de toegang te beperken. [Meer informatie](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/admin/permissions/folder-permissions){target="_blank"}.

Leer meer in de [ documentatie van de toestemmingen van de Gebruiker ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/admin/permissions/gs-permissions){target="_blank"}.


### Campaign-configuratiescherm {#acs-gs-admin-cp}

Net als bij Campaign Standard kunt u het Configuratiescherm gebruiken om uw omgeving te beheren. Voor versie 8 biedt het Configuratiescherm extra mogelijkheden.

Met het Configuratiescherm kunt u de efficiëntie van uw werk als productbeheerder van Adobe Campaign verhogen. Zo kunt u instellingen beheren en het gebruik van elk exemplaar bijhouden. Met de intuïtieve interface kunt u eenvoudig het gebruik van belangrijke elementen bewaken en beheertaken uitvoeren, zoals het toevoegen van IP-adressen aan de lijst van gewenste IP-adressen, SFTP-opslagbewaking, sleutelbeheer, enzovoort.

Leer meer in de [ zelfstudies van het Controlebord ](https://experienceleague.adobe.com/nl/docs/control-panel-learn/tutorials/control-panel-overview){target="_blank"} en de [ documentatie van het Controlebord ](https://experienceleague.adobe.com/docs/control-panel/using/control-panel-home.html?lang=nl){target="_blank"}.

* **voegt IP adressen** toe - het Controlebord van de Campagne staat u aan opstelling toe nieuwe verbindingen aan uw instanties door IP adreswaaiers aan de lijst van gewenste personen toe te voegen. Leer meer in [ IP toestaan lijstdocumentatie ](https://experienceleague.adobe.com/nl/docs/control-panel/using/instances-settings/ip-allow-listing-instance-access){target="_blank"}

* **Subdomain configuratie** - u kunt een onderafdeling van uw domein (technisch een &quot;DNS streek&quot;) voor gebruik met Adobe Campaign vormen.
Leer meer in de [ documentatie van de Subdomeindelegatie ](https://experienceleague.adobe.com/nl/docs/control-panel/using/subdomains-and-certificates/subdomains-branding){target="_blank"}

* **beheert servers SFTP** - in het Controlebord, kunt u met alle servers in wisselwerking staan SFTP die met de instanties van de Campagne worden verbonden die u toegang tot hebt. Leer meer in de [ het beheersdocumentatie van SFTP ](https://experienceleague.adobe.com/nl/docs/control-panel/using/sftp-management/about-sftp-management){target="_blank"}


### Audit trail {#acs-gs-admin-audit-trail}

Zoals reeds beschikbaar in Campaign Standard, kan het spoor van de Controle in Campagne v8 worden gebruikt om tot de volledige geschiedenis van veranderingen toegang te hebben die binnen uw instantie worden aangebracht.

In Adobe Campaign Web User Interface, verstrekt het de spoorvermogen van de Controle gebruikers volledige zicht in alle wijzigingen die aan belangrijke entiteiten binnen uw instantie worden aangebracht, typisch die die beduidend een vlotte verrichting van de instantie beïnvloeden. Leer meer in de [ documentatie van het spoor van de Controle ](../../v8/reporting/audit-trail.md)

### Gegevenspakketten {#acs-gs-admin-audit-packages}

Net als in Campaign Standard kunnen beheerders pakketten definiëren voor het uitwisselen van bronnen tussen verschillende Adobe Campaign-instanties via gestructureerde XML-bestanden. Dit kunnen configuratieparameters of data zijn.

Met gegevenspakketten kunt u aangepaste instellingen en gegevens van uw platform exporteren en importeren. Een pakket kan verschillende typen configuraties en componenten bevatten, al dan niet gefilterd. Leer hoe te met gegevenspakketten in Campagne v8 in [ te werken deze documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/packages){target="_blank"}.

<!--
MISSING LINKS: 

- System options
- Data Encryption/Decryption-->

### De gebruikersinterface aanpassen {#acs-gs-admin-ui}

U kunt de gebruikersinterface in de clientconsole op verschillende manieren aanpassen, zoals:

* **Lijst en gegevensvertoning** - Richtlijnen voor het beheren van gebruikersinterfacemontages zoals lijsten, eenheden, of gegevensvertoning zijn beschikbaar in dit document: [ documentatie van de gebruikersinterfacemontages ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/config/configuration/ui-settings){target="_blank"}

* **het beheer van de Omslag** - de Omslagen zijn voorwerpen in Adobe Campaign die u toestaan om uw componenten en gegevens te organiseren. Zij worden ook gebruikt om toestemmingen te beheren. Leer hoe te [ met omslagen ](../../v8/get-started/work-with-folders.md) werken.

* **de gebieden van de Douane** - de gebieden van de Douane zijn extra attributen die aan uit-van-de-doosschema&#39;s door de console van Adobe Campaign worden toegevoegd. Deze aangepaste velden worden op verschillende schermen weergegeven, bijvoorbeeld de details van een profiel of een testprofiel. Leer meer in de [ documentatie van de douanegebiedsconfiguratie ](../../v8/administration/custom-fields.md).

## De branding configureren {#acs-gs-admin-branding}

Elk bedrijf heeft merkrichtlijnen die zowel visuele elementen als technische details bepalen. Wat Adobe Campaign Standard betreft, helpt Adobe Campaign v8 u deze richtlijnen centraal te beheren, zodat u bij alles wat u doet een consistent merkimago aan uw klanten kunt presenteren, van logo&#39;s in e-mails tot de URL&#39;s en domeinen die in uw campagnes worden gebruikt. Als technisch beheerder kunt u in Adobe Campaign meerdere merken maken en beheren.

Leer meer in de [ Brandende documentatie ](https://experienceleague.adobe.com/nl/docs/experience-cloud/campaign/branding/branding-gs){target="_blank"}

## Begrijpen hoe u gegevensmodellen maakt {#acs-gs-admin-data-model-creation}

Net als Campaign Standard wordt Adobe Campaign v8 geleverd met het vooraf gedefinieerde gegevensmodel. Adobe Campaign vertrouwt op een Cloud-database die tabellen bevat die aan elkaar zijn gekoppeld. Leer meer in de [ modeldocumentatie van Gegevens ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/datamodel){target="_blank"}.

Een schema is een XML-document dat is gekoppeld aan een databasetabel. De code definieert de gegevensstructuur en beschrijft de SQL-definitie van de tabel. Zie de [ documentatie van de schepping van Schema&#39;s ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}

Leer hoe u een schema maakt en hoe u een bestaand schema in Campagne v8 uitbreidt in deze video:

>[!VIDEO](https://video.tv.adobe.com/v/337939?quality=12&learn=on){transcript=true}

Net als de mogelijkheden die beschikbaar zijn in Campaign Standard, kunt u aangepaste bronnen maken. IN Campagne v8, zijn de douanemiddelen douane of uitgebreide **schema&#39;s**.

* Leer hoe te met schema in [ te werken deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/shemas-forms/schemas){target="_blank"}.

* Leer hoe te om een bestaand schema in [ uit te breiden deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/shemas-forms/extend-schema){target="_blank"}.

* Leer hoe te om een nieuw schema in [ tot stand te brengen deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/shemas-forms/create-schema){target="_blank"}.

* Wanneer u een schema maakt of uitbreidt, moet u de bijbehorende invoerformulieren maken of wijzigen om deze wijzigingen zichtbaar te maken voor eindgebruikers. Met een invoerformulier kunt u een instantie bewerken die is gekoppeld aan een gegevensschema vanuit de Adobe Campaign-clientconsole. Het formulier wordt geïdentificeerd door de naam en naamruimte ervan. Zie de [ documentatie van de de vormenverwezenlijking van de Input ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/shemas-forms/forms){target="_blank"}.

## Werkstromen en gegevensbeheer {#acs-gs-admin-data-management}

Net als bij Adobe Campaign Standard bevat Adobe Campaign v8 een workflowmodule waarmee u het volledige scala aan processen en taken in de verschillende modules van de toepassingsserver kunt ordenen. Met deze uitgebreide grafische omgeving kunt u processen ontwerpen, zoals segmentatie, uitvoering van campagnes, bestandsverwerking, menselijke participatie, enzovoort. Deze processen worden uitgevoerd en bijgehouden door de workflowengine. Leer hoe te met werkschema&#39;s in Campagne v8 in [ te beginnen deze documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/data/workflows){target="_blank"}.

Zie de koppelingen naar andere nuttige bronnen hieronder:

* In deze video ziet u welke doeldimensies en werktabellen zijn en hoe Adobe Campaign gegevens in verschillende gegevensbronnen beheert:

  >[!VIDEO](https://video.tv.adobe.com/v/3452599?quality=12&learn=on&captions=dut){transcript=true}

* Met de campagne kunt u contactpersonen toevoegen aan de Cloud-database. U kunt een dossier laden, veelvoudige contactupdates plannen en automatiseren, gegevens op het Web verzamelen, of profielinformatie direct in de ontvankelijke lijst ingaan.  Leer meer in de [ gegevens van de Invoer (console) documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/data/import){target="_blank"}.

* U kunt uw verschillende rapporten eenvoudig exporteren naar de PDF- of CSV-indeling, zodat u deze kunt delen, bewerken of afdrukken. Leer meer in de [ documentatie van de Gegevens van de Uitvoer ](../../v8/reporting/export-reports.md).

## REST API&#39;s {#acs-gs-admin-apis}

Campagne REST API&#39;s zijn bedoeld om u in staat te stellen integratie voor Adobe Campaign te maken en uw eigen ecosysteem te bouwen door Adobe Campaign te koppelen aan het deelvenster met technologieën dat u gebruikt.

Als Campaign Standard-gebruiker die overschakelt naar Campagne v8, zijn REST API&#39;s beschikbaar voor u.

Leer meer in de [ Rest API documentatie ](https://experienceleague.adobe.com/nl/docs/experience-cloud/campaign/apis/get-started-apis){target="_blank"}.

Houd er rekening mee dat sommige aanbevelingen en beperkingen van toepassing zijn op REST API&#39;s bij de overgang van Campaign Standard naar Campaign v8. Zij zijn vermeld in [ deze pagina ](https://experienceleague.adobe.com/nl/docs/experience-cloud/campaign/apis/limitations){target="_blank"}. Specifieke beperkingen zijn ook van toepassing bij de overgang naar Campagne v8 zoals vermeld in de onderstaande Opmerking bij Beschikbaarheid:

>[!AVAILABILITY]
>
>* PKEY-waarden veranderen tussen bestaande Campaign Standard-instantie en gemigreerde Campagne v8-instantie. Als PKEY&#39;s worden opgeslagen in een externe database, moet de implementatie zodanig worden gewijzigd dat ze Adobe Campaign v8-API&#39;s met hoofdfuncties moeten aanroepen die koppelingen met PKEY&#39;s en volgende API-aanroepen mogelijk maken. Dit moet dynamisch gebeuren door de toetsen /hrefs van vorige API-aanroepen te gebruiken &#x200B;
>
>* In Campagne v8, voor het zelfde lichaam waar het voertuig met profiel verbonden was, &#x200B; zouden wij een fout firstName bezit niet geldig voor `cusVehicle` krijgen maar een verzoeklichaam met enkel de attributen zonder verbinding werkt prima. `{ "vehicleNumber": "20009", "vehicleName": "Model E", "vehicleOwner":{   "firstName":"tester 11", "lastName":"Smith 11" } }&#x200B;`
>
>* De tijdzone wordt aan de gebruiker weergegeven als onderdeel van de `profileAndServicesExt/profile` REST API-aanroep en niet als onderdeel van de `profileAndServices/profile` REST API-aanroep omdat deze wordt toegevoegd aan een uitgebreid schema als onderdeel van gegevensmigratie. &#x200B;
>
>* De `ccpaOptOut` wordt alleen aan de gebruiker weergegeven als onderdeel van de `profileAndServicesExt/profile` REST API-aanroep en niet als onderdeel van de `profileAndServices/profile` REST API-aanroep omdat deze wordt toegevoegd in een uitgebreid schema als onderdeel van gegevensmigratie.
>


<!--
## Working with templates - TO REMOVE?



Workflow templates contain pre-configured settings and activities which can be reused for creating new workflows.
[Workflow template documentation](../../v8/workflows/create-workflow.md)


You can design your landing page content, and save it for future reuse. See the [landing page template documentation](../../v8/landing-pages/lp-templates.md).

Each event can trigger a personalized message. For this to happen, you need to create a message template to match each event type. Templates contain the necessary information for personalizing the transactional message. See the [Transactional messaging template documentation](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/real-time/transactional-template)

Using a workflow template is a best practice if you need to regularly import files with the same structure. See the [Import template documentation](https://experienceleague.adobe.com/nl/docs/campaign/automation/workflows/use-cases/data-management/recurring-import-workflow){target="_blank"}
-->

## Privacy en toestemming

Wanneer u van Campaign Standard naar Campaign v8 gaat, is het belangrijk om te controleren hoe privacyregels van invloed zijn op uw gegevensbewerkingen. Afhankelijk van uw zaken en de jurisdicties waarin u werkt, kunnen de klanten het wettelijke recht hebben om tot de gegevens toegang te hebben u over hen houdt, of om zijn schrapping te verzoeken.

In Campagne v8, moeten alle privacyverzoeken door de **Adobe Privacy Service** integratie worden beheerd. Leer meer in [ Campagne v8 (console) documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/privacy/privacy).

Houd er rekening mee dat uw Campaign Standard-omgeving actief blijft gedurende een periode na de overgang. Tijdens deze tijd, kunnen de privacyverzoeken in beide systemen aankomen. Om naleving te garanderen en hiaten te voorkomen, moet u uw Adobe Transition Manager coördineren om verzoeken in beide omgevingen op de juiste wijze af te handelen.

## Abonnementsdiensten {#acs-gs-admin-sub}

Net als in Campaign Standard kunt u als beheerder abonnementenservices maken en marketers kunnen berichten verzenden naar hun abonnees. Belangrijke concepten en implementatiestappen worden uitgelijnd met Campaign Standard. Hieronder vindt u nuttige koppelingen en video.

Leer lidmaatschappen instellen en beheren en leden targeten.

>[!VIDEO](https://video.tv.adobe.com/v/3426562?quality=12&learn=on&captions=dut){transcript=true}

* Zie de documentatie van het gebruikersinterface van het Web van de abonnementsdiensten [&#128279;](../../v8/audience/manage-subscribers.md).

* Zie ook de documentatie om de abonnementendiensten in de cliëntconsole in [ te plaatsen deze sectie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/audience/subscriptions){target="_blank"}.

## Berichten en leveringen{#acs-gs-msg}

### Leveringskanalen configureren {#acs-gs-admin-channels}

Als Campaign Standard helpt Adobe Campaign v8 u kanaalcampagnes te verzenden, waaronder e-mails, SMS, pushmeldingen en directe mails, en de doeltreffendheid van deze campagnes te meten aan de hand van verschillende speciale rapporten. Deze berichten worden ontworpen en verzonden door leveringen, en kunnen voor elke ontvanger worden gepersonaliseerd. De kernfuncties omvatten het richten, het bepalen en het personaliseren van berichten, de uitvoering van mededelingen, en de bijbehorende operationele rapporten. Het belangrijkste functionele toegangspunt is de leveringsmedewerker. Dit toegangspunt leidt tot meerdere mogelijkheden die door Adobe Campaign worden gedekt.

Als beheerder, moet u uw kanaalconfiguraties bepalen. Raadpleeg de onderstaande koppelingen voor meer informatie.

* **E-mail** - De e-mailmontages zijn allen gedetailleerd in [ deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/emails/email-parameters){target="_blank"}.
* **SMS** - Leer hoe te om uw kanaal van SMS in [ te vormen deze documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/sms/sms){target="_blank"}.
* **duw berichten** - De Stappen om het kanaal van dupberichten te vormen zijn gedetailleerd [ in deze sectie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/push/push-data-collection){target="_blank"}.
* **Transactioneel overseinen** - Stappen om [ Transactioneel overseinen ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/real-time/transactional){target="_blank"} in Campagne v8 te vormen zijn gedetailleerd [ in deze sectie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/config/configuration/transactional-msg-settings)

### Externe accounts {#acs-gs-ext-accounts}

Als beheerder, bent u verantwoordelijk voor het vormen van en het handhaven van de externe rekeningen van de Campagne. Net als in Campaign Standard worden externe accounts gebruikt door technische processen, zoals technische workflows of workflows voor campagnes.

Het overgangsproces naar Campaign v8 zorgt voor uw bestaande externe Campaign Standard-accounts.

Leer meer in de [ Externe rekeningsdocumentatie ](../../v8/administration/external-account.md).


<!--
**Email**

MISSING LINKS :
- general email channel parameters 
- email routing accounts 
- email processing rules 
- email properties
-->

<!--
MISSING LINKS: 
- Setting external account 
- Adding vender details etc. -->

<!--
**Mobile app**
MISSING LINKS: 
- Configuring a mobile application using AEP SDKs 
- Sync Mobile app AEPSDK  
- Setting up your application in Adobe Campaign 
- Channel-specific application configuration
-->

### Dynamische inhoud {#acs-gs-dyn-content}

Met Campagne kunt u dynamische inhoud maken en persoonlijke berichten verzenden. Personalization-mogelijkheden kunnen worden gecombineerd om uw berichten te verbeteren en een aangepaste gebruikerservaring te creëren.

Met Campagne v8 kunt u als beheerder dynamische inhoudsblokken definiëren en hoe u deze kunt gebruiken om de inhoud van uw e-maillevering in deze video aan te passen:

>[!VIDEO](https://video.tv.adobe.com/v/342088?quality=12&learn=on){transcript=true}

Nuttige koppelingen:

* [ worden begonnen met verpersoonlijking ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/personalize/personalize){target="_blank"}
* [ de verpersoonlijkingsblokken van het Gebruik ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/personalize/personalization-blocks){target="_blank"}
* [ creeer voorwaardelijke inhoud ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/personalize/conditions){target="_blank"}
* [ de gegevensbronnen van Personalization ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/personalize/personalization-data){target="_blank"}

### Afleveringssjablonen {#acs-gs-templates}

Het gebruik van leveringssjablonen is een vereiste in Campagne v8, zoals in Campaign Standard.

Voor een versnelde en verbeterde ontwerpprocedure, creeer leveringsmalplaatjes om douaneinhoud en montages over uw campagnes gemakkelijk te hergebruiken. Met deze functie kunt u de creatieve vormgeving standaardiseren, zodat u sneller campagnes kunt uitvoeren en lanceren. Leer hoe te om leveringsmalplaatjes in [ Web van de Campagne gebruikersinterface ](../../v8/msg/delivery-template.md) tot stand te brengen. Zie ook hoe te om leveringsmalplaatjes in de cliëntconsole in [ tot stand te brengen deze sectie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/create-templates){target="_blank"}.

### Typologische regels {#acs-gs-admin-rules}

Als beheerder, bent u verantwoordelijk voor het creëren van en het handhaven van typologieregels voor uw leveringen. Hetzelfde als in Adobe Campaign Standard, in Campagne v8, zijn de typologische regels bedrijfsregels die u toestaan om controles en het filtreren op uw bericht uit te voeren alvorens het te verzenden.

Wanneer u vanuit een Campaign Standard-omgeving overschakelt naar Campaign v8, worden uw typologieregels verplaatst naar Campaign v8.

In Campaign v8 worden typologische regels geleverd met een specifieke &#39;Game-on&#39;-functie voor optimalisatie van campagnes. Deze module waarmee u het verzenden van leveringen kunt beheren, filteren en controleren. Om conflicten tussen campagnes te vermijden kan Adobe Campaign diverse combinaties testen door specifieke beperkingsregels toe te passen. Dit garandeert dat de verzonden berichten voldoen aan de behoeften en verwachtingen van klanten en het communicatiebeleid van het bedrijf. Leer meer in de [ documentatie van de Typologieregels ](https://experienceleague.adobe.com/nl/docs/campaign/automation/campaign-optimization/campaign-typologies){target="_blank"}.

### Quarantainebeheer {#acs-gs-admin-quarantine}

Alle in quarantaine geplaatste adressen en quarantaineregels zijn van uw milieu van Campaign Standard naar Campagne v8 gemigreerd. Er is geen specifieke actie nodig voor quarantainebeheer.

Als beheerder, krijg vertrouwd met quarantainebeheer in Campagne v8 die van [ begint deze pagina ](../../v8/audience/quarantine.md). Zie ook de gedetailleerde documentatie van de cliëntconsole over quarantainebeheer in [ deze sectie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/send/failures/quarantines#access-quarantined-addresses){target="_blank"}.


## Adobe Campaign-integratie beheren {#acs-gs-integrations}

U kunt uw instantie Campagne met de oplossingen van Adobe Experience Cloud verbinden om mogelijkheden te combineren. Adobe Campaign wordt geleverd met verschillende connectors waarmee u kunt communiceren met externe toepassingen, verbinding kunt maken met database-engines, gegevens kunt delen en synchroniseren. Leer hoe te om uw oplossingen in [ deze documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/connect/integration){target="_blank"} te combineren.

Als Campaign Standard-gebruiker die migreert naar Campaign v8, geldt het volgende voor u:

* Als u deze integratie met Campaign Standard gebruikte, zijn uw **Adobe Analytics** en **Audience Manager** configuraties en gegevens gemigreerd door Adobe.
* Als uw milieu van Campaign Standard met **Adobe Experience Manager** werd geïntegreerd, adviseert Adobe u om naar **Adobe Experience Manager as a Cloud Service** te bewegen zodat u dit vermogen kunt gebruiken wanneer het ontwerpen van e-mails in het gebruikersinterface van het Web van de Campagne, en het gestroomlijnde beheer van de inhoud en de vormen van de e-maillevering direct binnen uw milieu van Adobe Experience Manager vergemakkelijken. Leer meer in [ deze pagina ](../../v8/integrations/aem-content.md).
Campagne kan ook worden geïntegreerd met Adobe Experience Manager 6.5. Om deze integratie te vormen, verwijs naar [ deze documentatie ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/connect/ac-aem){target="_blank"}.
* Als uw milieu van Campaign Standard met **Trekkers** werd geïntegreerd, moet u opstelling en deze integratie vormen in Campagne v8 zoals die in [ wordt gedetaillerd deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/connect/ac-triggers){target="_blank"}.
* Als uw milieu van Campaign Standard met **Adobe Target** werd geïntegreerd, moet u opstelling en deze integratie vormen in Campagne v8 zoals die in [ wordt gedetailleerd deze pagina ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/connect/ac-at){target="_blank"}.
