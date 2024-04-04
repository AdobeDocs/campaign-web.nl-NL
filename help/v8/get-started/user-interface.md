---
audience: end-user
title: De interface detecteren
description: Adobe Campaign Web-gebruikersinterface
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 706d42661375c7ef7f95d1e8bf22db235500308d
workflow-type: tm+mt
source-wordcount: '2111'
ht-degree: 1%

---

# De interface detecteren {#user-interface}

De nieuwe Adobe Campaign Web-interface biedt een moderne en intuïtieve gebruikerservaring om het ontwerpen en leveren van marketingcampagnes te vereenvoudigen. Deze nieuwe interface is geïntegreerd met Adobe Experience Cloud-toepassingen en -oplossingen.

Leer hoe u verbinding maakt met Adobe Campaign en de basisbeginselen van Experience Cloud navigatie ontdekt [in dit artikel](connect-to-campaign.md).


>[!NOTE]
>
>Deze documentatie wordt vaak bijgewerkt om de laatste wijzigingen in de gebruikersinterface van het product te weerspiegelen. Sommige schermafbeeldingen kunnen echter enigszins afwijken van uw gebruikersinterface.

## Startpagina campagne {#user-interface-home}

>[!CONTEXTUALHELP]
>id="acw_homepage_recent"
>title="Recenten"
>abstract="De **Recenten** lijst bevat snelkoppelingen naar de onlangs gemaakte en gewijzigde leveringen. In deze lijst staan de datum van het kanaal, de status, de eigenaar, het maken en de wijziging van de datums."

De homepage van de campagne laat u snel en gemakkelijk doorbladeren zeer belangrijke middelen, indicatoren, en componenten.

In het bovenste gedeelte van de startpagina vindt u meer informatie over de nieuwste updates en nieuwe mogelijkheden die beschikbaar zijn in het product, met een koppeling naar Opmerkingen bij de release en gedetailleerde documentatie. Gebruik de pijl-links om functiekaarten te schuiven.

![](assets/home.png){zoomable=&quot;yes&quot;}

De **Belangrijkste prestatie-indicatoren** Hiermee kunt u de doeltreffendheid van uw platform controleren aan de hand van algemene KPI&#39;s. Meer informatie over deze KPI&#39;s vindt u in [deze pagina](../reporting/kpis.md).

De **Recenten** lijst bevat snelkoppelingen naar de onlangs gemaakte en gewijzigde leveringen. In deze lijst staan de datum van het kanaal, de status, de eigenaar, het maken en de wijziging van de datums. Klik op de knop **Meer weergeven** koppeling om meer leveringen te laden.

Daarnaast kunt u de Help-pagina&#39;s voor Adobe Campaign Web openen via **Leren** van de pagina.

## Linkernavigatiemenu {#user-interface-left-nav}

Blader links naar de links om toegang te krijgen tot Adobe Campaign Web-mogelijkheden. Met verschillende koppelingen worden lijsten weergegeven met objecten die kunnen worden gesorteerd en gefilterd. U kunt kolommen ook vormen om alle informatie te tonen u wenst. Zie dit [sectie](#list-screens). Sommige lijstschermen zijn alleen-lezen. Welke items in het navigatiemenu links en in de lijsten worden weergegeven, is afhankelijk van uw gebruikersmachtigingen. Meer informatie over machtigingen in [deze sectie](permissions.md).


### Verkenner {#user-interface-explorer}

>[!CONTEXTUALHELP]
>id="acw_explorer"
>title="Verkenner"
>abstract="De **Verkenner** worden alle Campagne-componenten en -objecten met dezelfde mappenhiërarchie als de component in de clientconsole weergegeven. Blader door al uw componenten, mappen en schema&#39;s van Campagne v8, controleer de bijbehorende machtigingen en maak mappen en submappen vanuit dit menu."

De **Verkenner** worden alle campagnebronnen en -objecten met dezelfde mappenhiërarchie als de map in de clientconsole weergegeven. Blader door al uw componenten, mappen en schema&#39;s van Campagne v8 en maak leveringen, workflows en campagnes.

De items die worden weergegeven in de **Verkenner** zijn afhankelijk van uw gebruikersmachtigingen. U kunt ook mappen en submappen toevoegen als u de juiste rechten hebt. Meer informatie over machtigingen in [deze sectie](permissions.md).

U kunt kolommen vormen om de vertoning aan te passen om alle informatie te bekijken u wenst. Zie dit [sectie](#list-screens). U kunt ook mappen en submappen toevoegen, zoals wordt beschreven in [deze sectie](permissions.md#folders).

Raadpleeg voor meer informatie over de campagnedeskundige, maphiërarchie en bronnen [Campagne v8 (console)-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/new/campaign-ui.html#ac-explorer-ui){target="_blank"}.

### Campaign Management {#user-interface-campaign-management}

In de sectie CAMPAIGN MANAGEMENT hebt u toegang tot marketingcampagnes, leveringen en workflows.

* **Campagnes** - Dit is de lijst van uw campagnes, en campagnemalplaatjes. Standaard kunt u voor elke campagne de begin-/einddatum/aanmaakdatum/laatste wijzigingsdatum, de huidige status en de naam weergeven van de Campagneoperator die de campagne heeft gemaakt. U kunt de lijst filteren op status, begin-/einddatums, map of een geavanceerd filter maken om uw eigen filtercriteria te definiëren. Meer informatie over campagnes [in deze sectie](../campaigns/gs-campaigns.md).

* **Leveringen** - Blader door de lijst met leveringen. Door gebrek, kunt u hun staat, laatste wijzigingsdatum evenals zeer belangrijke KPIs bekijken. U kunt de lijst filteren op status, contactdatum of kanaal. Klik op een e-maillevering om het dashboard te openen voor een overzicht van de leveringsgegevens. Leveringen op andere kanalen zijn alleen-lezen. Meer informatie over leveringen [in deze sectie](../msg/gs-messages.md).

  Gebruik de **Meer handelingen** om een levering te verwijderen of te dupliceren.

  ![](assets/more-actions.png){zoomable=&quot;yes&quot;}{width="70%" align="left"}

* **Workflows** - In dit scherm hebt u toegang tot de volledige lijst met workflows en workflowsjablonen. U kunt hun status, de laatste/volgende uitvoeringsdata controleren en een nieuwe werkstroom of een nieuw werkschemamalplaatje creëren. U kunt de lijst filteren met dezelfde criteria als voor andere objecten. Bovendien kunt u workflows filteren die wel of niet tot een campagne behoren. Meer informatie over workflows [in deze sectie](../workflows/gs-workflows.md).


### Contentmanagement {#user-interface-content-management}

In de sectie CONTENT MANAGEMENT kunt u uw inhoudssjablonen en fragmenten weergeven.

* **Inhoudssjablonen** - Voor een versneld en verbeterd ontwerpproces kunt u zelfstandige sjablonen maken om aangepaste inhoud eenvoudig te hergebruiken in [!DNL Adobe Campaign]. Alleen beschikbaar voor e-mails. Met deze functionaliteit kunnen gebruikers die op inhoud zijn gericht, aan zelfstandige sjablonen werken, zodat marketinggebruikers deze opnieuw kunnen gebruiken en aanpassen in hun eigen e-mailcampagnes. Lees meer in [deze sectie](../email/create-email-templates.md).

<!--
* **Fragments** -
-->

### Klantenbeheer {#user-interface-customer-management}

In de sectie KLANTENBEHEER kunt u uw profielen, publiek en abonnementen bekijken. Deze lijsten zijn alleen-lezen.

* **Profielen** - Profielen maken en beheren en toegang krijgen tot uw database met ontvangers. Standaard kunt u hun e-mailadres, voornaam en achternaam weergeven. Meer informatie over profielen in [deze sectie](../audience/about-recipients.md).
* **Soorten publiek** - Dit is uw lijst met doelgroepen. Standaard kunt u het type, de oorsprong, de datum en het label van de wijziging bekijken. U kunt de lijst filteren op oorsprong. Meer informatie over soorten publiek en lijsten in [deze sectie](../audience/about-recipients.md).
* **Abonnementsdiensten** - Blader door uw abonnementenlijsten. Standaard kunt u het type, de modus en het label ervan bekijken. Leer hoe u abonnementen en abonnementen beheert in [Adobe Campaign v8 (console)-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/subscriptions.html){target="_blank"}.
* **Vooraf gedefinieerde filters** - Vooraf gedefinieerde filters zijn aangepaste filters die worden gemaakt en opgeslagen om in de toekomst beschikbaar te zijn. Zij kunnen als kortere weg tijdens om het even welke het filtreren verrichtingen met de vraagmodeller, bijvoorbeeld worden gebruikt wanneer het filtreren van een lijst van gegevens, of het creëren van het publiek van een levering. Lees meer in [deze sectie](predefined-filters.md).


### Beslissingsbeheer {#decision-management}

>[!CONTEXTUALHELP]
>id="acw_offers_list"
>title="Aanbiedingen"
>abstract="Blader door de lijsten van aanbiedingen en aanbiedingsmalplaatjes die in de console gebruikend zijn gecreeerd **Interactie** -module. Deze lijsten zijn alleen-lezen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/offers.html" text="Aanbiedingen toevoegen aan een levering"

In het gedeelte BESLUIT BEHEER kunt u de aanbiedingen en aanbiedingstemplates bekijken. Deze lijsten zijn alleen-lezen.

* **Aanbiedingen** - Blader door de lijst met aanbiedingen en aanbiedingstemplates die in de console zijn gemaakt met de **Interactie** -module. Standaard kunt u hun status, begin- en einddatum en omgeving bekijken. U kunt de lijst filteren op status en begin- en einddatum. Aanbiedingssjablonen zijn ook beschikbaar.

Meer informatie over het maken en verzenden van aanbiedingen in e-mails en SMS in [deze sectie](../msg/offers.md).

### Rapportage {#left-nav-reporting}

* **Rapporten** - de **Rapport** de ingang biedt een geconsolideerde algemene samenvatting van verkeer en betrokkenheidsmetriek voor elk kanaal binnen uw milieu van de Campagne aan. Deze rapporten bestaan uit verschillende widgets, die elk een duidelijk perspectief bieden op uw campagne of leveringsprestaties. Lees meer in [deze sectie](../reporting/global-reports.md).


## Contextafhankelijke Help {#user-interface-help}

De interface bevat een contextafhankelijke Help. Klik, indien beschikbaar, op de knop `?` pictogram om Help-informatie en verwante documentatiekoppelingen weer te geven.

![](assets/do-not-localize/context-help.png){zoomable=&quot;yes&quot;}{width="40%" align="left"}

Momenteel vrijgegeven als versie van Bèta binnen het nieuwe de gebruikersinterface van het Web van de Campagne, **AI-assistent voor kennis** ingebed in contextuele hulp revolutioneert documentatie het zoeken en het antwoorden van hoe te vragen met moeiteloze sifting door grote documentatiebewaarplaatsen, onmiddellijk het bepalen van de nauwkeurige informatie u nodig hebt.

Dankzij de mogelijkheden van CampagneGen AI transformeert deze assistent uw ervaring, waardoor informatie wordt opgehaald en problemen worden opgelost. Of u nu op zoek bent naar begeleiding in een complexe taak of door uitgebreide documenten navigeert, onze AI-Medewerker van de Kennis is uw ultieme metgezel, die ongeëvenaarde efficiëntie en nauwkeurigheid biedt in elke interactie.

Lees meer in [deze sectie](using-ai.md).


## Meer informatie {#learn-more}

Leer hoe u in uw Campagne-omgeving kunt bladeren, zoeken en filterlijsten kunt gebruiken [op deze pagina](list-filters.md).



<!--
######## This part stores the contextualHelp definition for WebUI BETA ###########
######## These blocks should be dispatched in the appropriate pages when available ###########
######## PLEASE DO NOT DELETE ###########
REFER TO 
https://wiki.corp.adobe.com/pages/viewpage.action?spaceKey=neolane&title=v8+WebUI+Contextual+Help+%3CALPHA%3E-+Official+list
-->

>[!CONTEXTUALHELP]
>id="acw_push_permission_for_segment"
>title="Machtiging vereist"
>abstract="Uw beheerder moet u toestemming verlenen alvorens u een segment kunt tot stand brengen."

>[!CONTEXTUALHELP]
>id="acw_push_overview_edit"
>title="Machtiging vereist"
>abstract="Uw beheerder moet u toestemming verlenen alvorens u een segment kunt tot stand brengen."

<!-- delivery template settings-->

>[!CONTEXTUALHELP]
>id="acw_global_reporting_sending"
>title="Globale rapporten verzenden"
>abstract="Metrische gegevens voor het bijhouden van rapporten zijn zichtbaar in dit scherm"

>[!CONTEXTUALHELP]
>id="acw_global_reporting_tracking"
>title="Globale rapporten bijhouden"
>abstract="Metrische gegevens voor het bijhouden van rapporten zijn zichtbaar in dit scherm"


<!-- FOR BETA (alignment) -->
<!--https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CBETA%3E-+Official+list-->


<!-- FOR GA -->
<!-- Aligned with https://wiki.corp.adobe.com/display/neolane/v8+WebUI+Contextual+Help+%3CGA%3E-+Official+list -->

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_list"
>title="Ontvangers maken"
>abstract="Ontvangers maken"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_cardoverview"
>title="Overzicht van de ontvangerskaart"
>abstract="Overzicht van de ontvangerskaart"

>[!CONTEXTUALHELP]
>id="acw_recipients_creation_touchpoints"
>title="Aanraakpunten ontvangers"
>abstract="Aanraakpunten ontvangers"

>[!CONTEXTUALHELP]
>id="acw_recipients_subscription_selection"
>title="Selectie van abonnementen voor ontvangers"
>abstract="Selectie van abonnementen voor ontvangers"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_eligible_list"
>title="Ontvangers bieden kwalificerende lijst aan"
>abstract="Ontvangers bieden kwalificerende lijst aan"

>[!CONTEXTUALHELP]
>id="acw_recipients_offers_preview_proposition"
>title="Voorvertoning van aanbiedingen van ontvangers"
>abstract="Voorvertoning van aanbiedingen van ontvangers"

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Fragmenten"
>abstract="Fragmenten"

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Fragmenten opslaan"
>abstract="Fragmenten opslaan"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Fragmenten maken"
>abstract="Fragmenten maken"

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Eigenschappen van Fragmenten"
>abstract="Eigenschappen van Fragmenten"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Type fragmenten"
>abstract="Type fragmenten"

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Lijst met fragmenten"
>abstract="Lijst met fragmenten"

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmentdetails"
>abstract="Fragmentdetails"




>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_savefilter"
>title="Voorwaardelijke inhoud opslaan, filter"
>abstract="Voorwaardelijke inhoud opslaan, filter"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_selectfilter"
>title="Voorwaardelijke inhoud selecteren, filter"
>abstract="Voorwaardelijke inhoud selecteren, filter"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectline"
>title="Voorwaardelijke inhoud op onderwerpregel"
>abstract="Voorwaardelijke inhoud op onderwerpregel"

>[!CONTEXTUALHELP]
>id="acw_conditionalcontent_subjectlinecondition"
>title="Voorwaardelijke onderwerpregel voor inhoud"
>abstract="Voorwaardelijke onderwerpregel voor inhoud"


>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_testprofiles"
>title="Testprofielen simuleren"
>abstract="Testprofielen simuleren"

<!--ML: not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_profiles_selection"
>title="Selectie van testprofielen simuleren"
>abstract="Selectie van testprofielen simuleren"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_send_testprofiles"
>title="Testprofielen simuleren en verzenden"
>abstract="Testprofielen simuleren en verzenden"

<!-- ML: beta wiki page - not visible in UI-->

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_email_log"
>title="E-maillogboek simuleren"
>abstract="E-maillogboek simuleren"

<!-- ML: beta wiki page - not visible in UI-->

<!-- FOR POST-GA -->



<!--
Deprecated IDs - to remove in GA: -->

>[!CONTEXTUALHELP]
>id="acw_attributepicker_advancedfields"
>title="Geavanceerde kenmerken weergeven"
>abstract="Alleen de meest voorkomende kenmerken worden standaard weergegeven in de lijst met kenmerken. Activeer **Geavanceerde kenmerken weergeven** schakelt u om alle beschikbare kenmerken voor de huidige lijst in het linkerpalet van de regelbouwer weer te geven, zoals knooppunten, groepen, 1-1 koppelingen, 1-N-koppelingen."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_advancedfields"
>title="Geavanceerde velden voor regelbuilder"
>abstract="Alleen de meest voorkomende kenmerken worden standaard weergegeven in de lijst met kenmerken. Activeer **Geavanceerde kenmerken weergeven** schakelt u om alle beschikbare kenmerken voor de huidige lijst in het linkerpalet van de regelbouwer weer te geven, zoals knooppunten, groepen, 1-1 koppelingen, 1-N-koppelingen."

>[!CONTEXTUALHELP]
>id="acw_rulebuilder_properties_advanced"
>title="Geavanceerde kenmerken van de builder van de regel"
>abstract="Alleen de meest voorkomende kenmerken worden standaard weergegeven in de lijst met kenmerken. Activeer **Geavanceerde kenmerken weergeven** schakelt u om alle beschikbare kenmerken voor de huidige lijst in het linkerpalet van de regelbouwer weer te geven, zoals knooppunten, groepen, 1-1 koppelingen, 1-N-koppelingen."

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_readonlymode"
>title="Deze sjabloon is alleen gereed"
>abstract="U hebt geen machtigingen om deze sjabloon te bewerken. Indien nodig, contacteer uw beheerder om u toegang te verlenen."

<!-- Subscription activity-->

>[!CONTEXTUALHELP]
>id="acw_subscriptions_defaultlp"
>title="Standaardlandingspagina"
>abstract="Selecteer de standaardlandingspagina die aan deze abonnementenservice is gekoppeld."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Abonnementsserviceactiviteiten"
>abstract="Gebruik Adobe Campaign om uw services, zoals nieuwsbrieven, te maken en te controleren en om de abonnementen op of het afmelden van deze services te controleren. Abonnementen gelden alleen voor verzending via e-mail en SMS."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Abonnementsserviceparameters"
>abstract="Selecteer en bevestig de instellingen voor de abonnementsservice."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Uitgaande overgang van abonnementsdiensten"
>abstract="Schakelen tussen **Een uitgaande overgang genereren** om een overgang toe te voegen na de activiteit."


<!--Update file-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata"
>title="Gegevens bijwerken"
>abstract="De **Gegevens bijwerken** de activiteit voert een massa update van de gebieden in het gegevensbestand uit."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_operationtype"
>title="Selecteren hoe gegevens moeten worden bijgewerkt"
>abstract="De **Type bewerking** kunt u het proces kiezen dat op de gegevens in de database moet worden uitgevoerd. Selecteer de eerste optie om gegevens toe te voegen of bij te werken (als deze al is toegevoegd). U kunt ook alleen gegevens toevoegen, alleen gegevens bijwerken of gegevens verwijderen. Selecteer de **Verzamelingen bijwerken en samenvoegen** om een primaire record te selecteren waarnaar duplicaten moeten worden gekoppeld, en om die duplicaten veilig te verwijderen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_recordid"
>title="Registeridentificatie"
>abstract="Geef op hoe de records in de database moeten worden geïdentificeerd: als de gegevens betrekking hebben op een bestaande doeldimensie, selecteert u de optie **De doeldimensie gebruiken** en selecteert u de doeldimensie en -velden die u wilt bijwerken. Geef anders een of meer aangepaste koppelingen op om de gegevens in de database te identificeren of gebruik te maken van afstemmingssleutels."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_fieldsupdate"
>title="Velden selecteren om bij te werken"
>abstract="Selecteer de velden die u wilt bijwerken en de instellingen voor afstemming. U kunt de **Automatisch toewijzen** om automatisch de velden te identificeren die moeten worden bijgewerkt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_advancedoptions"
>title="Geavanceerde opties voor het bijwerken van gegevens"
>abstract="De **Geavanceerde opties** kunt u aanvullende instellingen opgeven voor het beheer van gegevens en duplicaten."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition"
>title="Een uitgaande overgang genereren"
>abstract="Schakelen tussen **Een uitgaande overgang genereren** optie om een uitgaande overgang toe te voegen die aan het eind van de uitvoering van **Gegevens bijwerken** activiteit. De update markeert doorgaans het einde van een doelworkflow en daarom wordt de optie niet standaard geactiveerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_updatedata_outboundtransition_rejects"
>title="Produceer een uitgaande overgang voor verwerpingen."
>abstract="Schakelen tussen **Een uitgaande overgang genereren voor afwijzing** om een uitgaande overgang toe te voegen die records bevat die niet correct zijn verwerkt na de update (bijvoorbeeld als er een duplicaat is). De update markeert doorgaans het einde van een doelworkflow en daarom wordt de optie niet standaard geactiveerd."



<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Extern signaal"
>abstract="De **Extern signaal** Met activiteit kunt u de uitvoering van een set taken in een workflow starten vanuit een API of een andere workflow."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Externe signaalparameters"
>abstract="Externe signaalparameters"


>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Eindtriggers"
>abstract="Eindtriggers"


<!--JavaScript-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript"
>title="JavaScript-code"
>abstract="De **JavaScript-code** een JavaScript-code uitvoeren in de context van een workflow."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_snippet"
>title="JavaScript-fragment"
>abstract="Configureer de uit te voeren code."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/api" text="Meer informatie in de documentatie van Campagne v8 (console)"


>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_execution"
>title="JavaScript uitvoeren"
>abstract="Standaard kan de uitvoeringsfase niet langer duren dan 1 uur. Na deze vertraging wordt het proces afgebroken met een foutbericht en mislukt de uitvoering van de activiteit. Schakelen tussen **Uitvoering stoppen na** om een aangepaste vertraging te definiëren. Als u deze limiet wilt negeren, stelt u de waarde in op 0."

>[!CONTEXTUALHELP]
>id="acw_orchestration_javascript_transition"
>title="Procesfouten"
>abstract="Schakelen tussen **Procesfouten** om een uitgaande overgang toe te voegen die fouten bevat."


<!--ExtractFile-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Bestand extraheren"
>abstract="Bestandsactiviteit extraheren"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Te extraheren bestand"
>abstract="Selecteer het bestand dat u wilt extraheren."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Bestemmingsindeling"
>abstract="Selecteer de indeling."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Nabewerking"
>abstract="Een naverwerkingsstap definiëren"

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Uitgaande overgang"
>abstract="Schakelen tussen **Een uitgaande overgang genereren** optie om een uitgaande overgang toe te voegen na de huidige activiteit."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Procesfouten"
>abstract="Schakelen tussen **Procesfouten** om een uitgaande overgang toe te voegen die fouten bevat."
