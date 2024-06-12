---
audience: end-user
title: De interface detecteren
description: Adobe Campaign Web-gebruikersinterface
exl-id: 0908c827-aa91-469f-824b-8e3de543876d
source-git-commit: 178d17b81db4ee3f3a445812ac1af6e5f9adbc57
workflow-type: tm+mt
source-wordcount: '1660'
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

![](assets/home.png){zoomable="yes"}

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

  ![](assets/more-actions.png){zoomable="yes"}{width="70%" align="left"}

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

<!--
## Contextual Help {#user-interface-help} 

A contextual help is available in the interface. When available, click on the `?` icon to display help information and related documentation links. 

![](assets/do-not-localize/context-help.png){zoomable="yes"}{width="40%" align="left"}

Currently released as a Beta version within the new Campaign Web user interface, the **AI-powered Knowledge Assistant** embedded within contextual help revolutionizes documentation searching and answering how-to questions with effortlessly sifting through vast documentation repositories, instantly pinpointing the precise information you need.

Thanks to Campaign Gen AI's capabilities, this assistant transforms your experience, making information retrieval and problem-solving a breeze. Whether you're seeking guidance in a complex task or navigating extensive documents, our AI-powered Knowledge Assistant is your ultimate companion, providing unmatched efficiency and accuracy in every interaction.

Learn more in [this section](using-ai.md).

-->

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

<!-- Workflow settings -->

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_initscript"
>title="Initialisatiescript"
>abstract="Initialisatiescript"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_properties"
>title="Uitvoereigenschappen"
>abstract="Uitvoereigenschappen"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_error"
>title="Uitvoerfout"
>abstract="Uitvoerfout"

>[!CONTEXTUALHELP]
>id="acw_workflow_settings_execution_initscript"
>title="Initialisatiescript voor uitvoering"
>abstract="Initialisatiescript voor uitvoering"

<!-- Delivery alerting -->

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria"
>title="Dashboard voor leveringswaarschuwingscriteria"
>abstract="Dashboard voor leveringswaarschuwingscriteria"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboards"
>title="Dashboard voor aflevering"
>abstract="Dashboard voor aflevering"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create"
>title="Waarschuwingscriteria voor levering maken"
>abstract="Waarschuwingscriteria voor levering maken"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_indicators"
>title="Indicatoren die moeten worden toegevoegd aan signaleringen"
>abstract="Indicatoren die moeten worden toegevoegd aan signaleringen"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_alert"
>title="Type waarschuwing"
>abstract="Type waarschuwing"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_criteria_create_frequency"
>title="Criteriumfrequentie"
>abstract="Criteriumfrequentie"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_add"
>title="Beoordelingscriteria voor aflevering"
>abstract="Beoordelingscriteria voor aflevering"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_general"
>title="Algemene parameters voor leveringswaarschuwingen"
>abstract="Afleveringswaarschuwing"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_create_criteria_parameters"
>title="Parameters van de leveringsalarmeringscriteria"
>abstract="Afleveringswaarschuwing"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_alerts"
>title="Verzonden leveringswaarschuwingen"
>abstract="Verzonden leveringswaarschuwingen"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_history"
>title="Geschiedenis van leveringswaarschuwingen"
>abstract="Geschiedenis van leveringswaarschuwingen"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_dashboard_create"
>title="Waarschuwingsdashboard voor levering maken"
>abstract="Waarschuwingsdashboard voor levering maken"

>[!CONTEXTUALHELP]
>id="acw_delivery_alerting_filter"
>title="Een waarschuwingscriterium maken"
>abstract="Als u uw eigen leveringsfilters wilt maken, maakt u een nieuw, vooraf gedefinieerd filter in de Campagne v8-console via de **Administratie** > **Configuratie** > **Vooraf gedefinieerde filters** knooppunt."

<!-- IDs -->


>[!CONTEXTUALHELP]
>id="acw_schema_editcustomfields"
>title="Aangepaste kenmerken bewerken"
>abstract="Aangepaste kenmerken bewerken"
