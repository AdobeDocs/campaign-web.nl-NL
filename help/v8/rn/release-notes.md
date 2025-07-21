---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 6f09df9a4686a56b56e837536db11a71ba5158f4
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 9%

---

# Aanvullende informatie  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie "
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

De veranderingen en de verbeteringen beschikbaar met vorige versies worden vermeld in [ 2024 ](release-notes-24.md) en [ 2025 ](release-notes-25.md).

## Updates van juli 1925 {#25-7-updates}

>[!AVAILABILITY]
>
>Voor deze updates moet uw server zijn geüpgraded naar 8.8.1 min. Verwijs naar de de versienota&#39;s van de Console van de Cliënt [ ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

Eerder vrijgegeven in Beperkte Beschikbaarheid, zijn de volgende mogelijkheden nu beschikbaar aan alle milieu&#39;s (Algemene Beschikbaarheid):

* **Meertalige leveringsverwezenlijking** - u kunt veelvoudige e-mailleveringen in verschillende talen in het Gebruikersinterface van het Web van Adobe Campaign nu verzenden. Met de functie Meertalige levering kunt u de standaardtaal van uw levering kiezen en de verschillende talen waarin de levering kan worden verzonden. U kunt deze leveringen ook voorvertonen in de talen die u hebt gekozen. [Meer informatie](../email/edit-content.md#multilingual-delivery).

<!--
* **Visual fragments** - You can now create, use and archive content fragments. Visual fragments are pre-defined visual blocks that you can reuse across multiple email deliveries, or in content templates. [Learn more](https://experienceleague.adobe.com/docs/campaign-web/v8/content/manage-reusable-content/fragments/fragments.html){target="_blank"}
-->

* **het Alarm van de Levering** - de het alarmerende eigenschap van de Levering is een waakzaam beheersysteem dat een groep gebruikers toelaat om berichten automatisch te ontvangen die informatie over de uitvoering van hun leveringen bevatten. [Meer informatie](../msg/delivery-alerting.md)

* **het Bestaan van pagina&#39;s verbeteringen** - de volgende verbeteringen aan het landen van pagina&#39;s zijn nu beschikbaar:

   * U kunt nu naar een standaardlandingspagina voor abonnementen/abonnementen verwijzen wanneer u een service configureert. Als u bij het ontwerpen van een e-mailbericht een koppeling naar die landingspagina definieert, worden gebruikers die het formulier voor de bestemmingspagina verzenden, automatisch geabonneerd op of geabonneerd van deze service. [Meer informatie](../audience/manage-services.md#create-service)
   * Een nieuwe optie in de configuratie van de bestemmingspagina staat anonieme bezoekers toe om tot de landingspagina toegang te hebben. Als u deze optie uitschakelt, kunnen alleen geïdentificeerde gebruikers het formulier openen en verzenden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie in de configuratie van de bestemmingspagina kunt u aanvullende interne gegevens opslaan wanneer de bestemmingspagina wordt verzonden. [Meer informatie](../landing-pages/create-lp.md#create-landing-page)
   * Met een nieuwe optie kunt u een openingspagina gebruiken voor verschillende services, waardoor deze dynamisch wordt. Als u een koppeling naar een e-mailbericht toevoegt en u een dynamische bestemmingspagina selecteert, kunt u elke gewenste service selecteren. Als u een landingspagina selecteert waaraan een specifieke service is gekoppeld, wordt deze service automatisch gebruikt (u kunt geen andere service selecteren). [Meer informatie](../landing-pages/create-lp.md#define-actions-on-form-submission)
   * Voorwaardelijke inhoud wordt nu ondersteund in bestemmingspagina&#39;s. [Meer informatie](../landing-pages/lp-content.md)
   * U kunt een landingspagina aan de dienst verbinden, en een bevestigingsbericht verzenden wanneer de gebruikers het bevestigen. [Meer informatie](../landing-pages/lp-content.md#lp-message)
   * U kunt Captcha toevoegen om uw landingspagina te beschermen tegen spam en misbruik veroorzaakt door bots. Dit is niet opdringerig voor uw klanten omdat het geen enkele interactie van hen vereist en gebaseerd is op interacties met uw site. [Meer informatie](../landing-pages/create-lp.md#captcha)

Eerder vrijgegeven in Beperkte Beschikbaarheid, zijn de volgende mogelijkheden nu beschikbaar **op bestelling**:

* **Dynamische Rapportering** - u kunt tot Dynamische Rapportering nu toegang hebben die volledig klantgerichte en rapporten in real time verstrekt om het effect van uw marketing activiteiten te meten. Het voegt toegang tot profielgegevens toe, toelatend demografische analyse door profieldimensies zoals geslacht, stad en leeftijd naast functionele e-mailcampagnegegevens zoals opent en klikt. Dynamische rapportage is ook beschikbaar voor meertalige e-mailleveringen en transactieberichten. [Meer informatie](../reporting/dynamic-reporting/get-started-reporting.md)

* **Gecentraliseerde Branding** - Uw technische beheerders kunnen één of verscheidene merken nu bepalen om de parameters te centraliseren die de identiteit van een merk beïnvloeden. Dit zijn onder andere het merklogo, het domein van de toegangs-URL voor de landingspagina&#39;s of de instellingen voor de tracking van berichten. U kunt deze merken maken en deze koppelen aan berichten of bestemmingspagina&#39;s. Deze configuratie wordt beheerd in malplaatjes. Brandingsopties zijn beschikbaar voor alle kanalen, waaronder SMS en Direct mail. [Meer informatie](../administration/branding/branding-gs.md){target="_blank"}

  >[!NOTE]
  >
  >Deze functie is alleen beschikbaar voor nieuwe implementaties.

Naast de hierboven vermelde functies wordt deze release ook geleverd met een aantal functies die beschikbaar zijn in de Client Console:

* [ Nieuwe SMS verzendende schakelaar ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/sms/sms.html). (FDA-omgevingen)
* [ Rest APIs ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/developer/apis/get-started-apis.html) (op bestelling, milieu&#39;s FDA)

Verwijs naar de de versienota&#39;s van de Console van de Cliënt [ ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html){target="_blank"}.

<!--
ACC * **Branding** - Branding options are now available for all channels, including SMS and Direct mail. [Read more](https://experienceleague.adobe.com/docs/experience-cloud/campaign/branding/branding-gs.html){target="_blank"}
web - * **Branding for Direct Mail** - Technical administrators can now define one or several brands to centralize the parameters that affect a brand's identity. This includes the brand logo, the domain of the landing pages' access URL, or message tracking settings. You can now create these brands and link them to messages or landing pages. This configuration is managed in templates. [Learn more](https://experienceleague.adobe.com/en/docs/experience-cloud/campaign/branding/branding-assign)
ACC - Branding - As a Campaign Standard migrated user, your technical administrators can now define one or several brands to centralize the parameters that affect a brand’s identity. This includes the brand logo, the domain of the landing pages’ access URL, or message tracking settings. You can create these brands and link them to messages or landing pages. This configuration is managed in templates. Read more
Previously released in Limited Availability, the following capability is now available **on demand, only for [Campaign FDA deployments](../architecture/fda-deployment.md)**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available by default **for new implementations**, and available **on demand for existing environments**. To gain access, contact your Adobe representative.
Previously released in Limited Availability, the following capability is now available **on demand**. To gain access, contact your Adobe representative.
-->