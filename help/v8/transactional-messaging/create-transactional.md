---
audience: end-user
title: Transactieberichten maken
description: Leer hoe te om een transactiebericht in het Gebruikersinterface van het Web van de Campagne tot stand te brengen
exl-id: 74e468f5-d9c3-4470-8ff2-68648b5f396f
source-git-commit: 7185e1cbc8ce9dd325bebc20c0ac362d7067f3e9
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# Transactieberichten maken

In transactioneel overseinen, brengt een gebeurtenis het verzenden van een gepersonaliseerd bericht teweeg.
Om dit toe te laten, moet u een berichtmalplaatje voor elk gebeurtenistype tot stand brengen. Deze sjablonen bevatten alle benodigde informatie voor het aanpassen van het transactiebericht.

## Een sjabloon voor een transactiebericht maken {#transactional-template}

In het Gebruikersinterface van het Web van de Campagne, is de eerste stap in transactie overseinenconfiguratie de verwezenlijking van het malplaatje of de directe verwezenlijking van het bericht. Dit verschilt met [ de configuratie van transactionele berichten op cliëntconsole ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/send/real-time/transactional).

Een transactiemalplaatje van het bericht kan worden gebruikt om voorproef de leveringsinhoud die door het profiel wordt ontvangen alvorens het het definitieve publiek bereikt. Bijvoorbeeld, kan een beheerder opstelling en de malplaatjes vormen, die hen voor gebruik door marketing gebruikers klaar maken.

Voer de onderstaande stappen uit om een transactiemalplaatje te maken:

* Ga in de sectie **[!UICONTROL Triggered messages]** naar **[!UICONTROL Transactional messages]** . Op het tabblad **[!UICONTROL Templates]** ziet u alle leveringssjablonen voor transactiemeldingen. Klik op de knop **[!UICONTROL Create transactional message template]** om de sjabloon te maken.

  ![](assets/transactional-templates.png){zoomable="yes"}

* Kies het kanaal van de sjabloon in de nieuwe weergegeven pagina. Wij selecteren bijvoorbeeld **[!UICONTROL Email]** kanaal. U kunt ook vanuit een andere berichtsjabloon werken en deze selecteren in de lijst met sjablonen.

  ![](assets/transactional-template-channel.png){zoomable="yes"}

  Klik nogmaals op de knop **[!UICONTROL Create transactional message]** om het maken van de sjabloon op het geselecteerde kanaal te valideren.

* U hebt nu toegang tot de configuratie van uw transactiemalplaatje voor berichten.

  ![](assets/transactional-template-configuration.png){zoomable="yes"}

### Eigenschappen van Transactieberichten {#transactional-properties}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_properties"
>title="Eigenschappen voor Transactieberichten"
>abstract="Vul dit formulier in om de eigenschappen voor transactiemeldingen te configureren"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_email_properties"
>title="E-maileigenschappen voor Transactieberichten"
>abstract="Dit formulier invullen om de e-maileigenschappen voor transactieberichten te configureren"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_sms_properties"
>title="Eigenschappen van SMS-berichten"
>abstract="Vul dit formulier in om de SMS-eigenschappen voor transactieberichten te configureren"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_push_properties"
>title="Transactieberichten Push-eigenschappen"
>abstract="Vul dit formulier in om de eigenschappen van de Push voor het transactiebericht te configureren"

De sectie **[!UICONTROL Properties]** van een transactiemelding helpt u bij het instellen van:

* De **[!UICONTROL Label]** is de naam die wordt weergegeven in de lijst met transactieberichten. Duidelijk maken voor onderzoek en toekomstig gebruik.
* **[!UICONTROL Internal name]** is een unieke naam die uw bericht onderscheidt van de andere gemaakte berichten.
* In **[!UICONTROL Folder]** wordt de transactiemalplaatje voor berichten gemaakt.
* In **[!UICONTROL Execution folder]** wordt het bericht opgeslagen nadat het is uitgevoerd.
* De **[!UICONTROL Delivery code]**: een code die helpt het bericht voor rapportage te herkennen, indien nodig.
* De **[!UICONTROL Description]**
* **[!UICONTROL Nature]** is de aard van uw levering, zoals vermeld in de opsomming *deliveryNature*. [ leer meer op opsommingen ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/ui-settings#enumerations)

![](assets/template-properties.png){zoomable="yes"}

### Mobiele app {#mobile-app}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_mobileapp"
>title="Transactieberichten voor mobiele apps"
>abstract="In deze sectie kunt u de toepassing selecteren waar u uw bericht wilt duwen."

In deze sectie kunt u de toepassing selecteren waar u uw bericht wilt duwen.

Als u op het onderzoekspictogram klikt, opent u de mobiele toepassing die in uw Adobe Campaign-exemplaar wordt vermeld.

![](assets/transactional-mobileapp.png){zoomable="yes"}

### Contextvoorbeeld {#context-sample}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_context"
>title="Transactionele berichtcontext"
>abstract="In het contextvoorbeeld kunt u een testgebeurtenis maken om een voorvertoning weer te geven van het transactiebericht dat met de profielpersonalisatie is ontvangen."

>[!CONTEXTUALHELP]
>id="acw_transacmessages_addcontext"
>title="Transactionele berichtcontext"
>abstract="In het contextvoorbeeld kunt u een testgebeurtenis maken om een voorvertoning weer te geven van het transactiebericht dat met de profielpersonalisatie is ontvangen. "

In het contextvoorbeeld kunt u een testgebeurtenis maken om een voorvertoning weer te geven van het transactiebericht dat met de profielpersonalisatie is ontvangen.

Deze stap is optioneel. U kunt de sjabloon zonder het contextvoorbeeld gebruiken, maar het nadeel is dat u geen voorvertoning van de gepersonaliseerde inhoud kunt weergeven.

In ons voorbeeld om het wachtwoord in te stellen, verzendt de gebeurtenis de voornaam, achternaam en een gepersonaliseerde koppeling van de gebruiker om zijn wachtwoord opnieuw in te stellen. De context kan worden gevormd zoals hieronder getoond.

De inhoud van de context is afhankelijk van de personalisatie die u nodig hebt.

![](assets/transactional-context.png){zoomable="yes"}

### Inhoud van transactiemalplaatje {#transactional-content}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_content"
>title="Transactionele berichteninhoud"
>abstract="Leer hoe u de inhoud van het transactiebericht maakt"

>[!CONTEXTUALHELP]
>id="acw_transacmessages_personalization"
>title="Transactionele berichtenaanpassing"
>abstract="Leer hoe u de inhoud van het transactiebericht kunt aanpassen"

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_event_context"
>title="Gebeurteniscontext"
>abstract="Dit menu bevat variabelen van de triggergebeurtenis die u kunt gebruiken om de inhoud van het transactiemelding aan te passen."

Het werken aan de inhoud van een transactiemelding is als de inhoudsverwezenlijking van een levering. Klik op **[!UICONTROL Open email designer]** of **[!UICONTROL Edit email body]** en selecteer sjablooninhoud of importeer uw HTML-code.

![](assets/template-content.png){zoomable="yes"}

Als u de personalisatie in de inhoud wilt toevoegen, klikt u op de sectie waaraan u de inhoud wilt toevoegen en kiest u het pictogram **[!UICONTROL Add Personalization]** .

![](assets/template-perso.png){zoomable="yes"}

U hebt toegang tot het venster **[!UICONTROL Edit personalisation]** .
Klik op het pictogram **[!UICONTROL Event context]** om de variabelen van de triggergebeurtenis toe te voegen. U kunt de context navigeren u voor uw malplaatje ([ creeert meer over de context ](#context-sample)), en klikt op de **[!UICONTROL +]** knoop om nodig variabele op te nemen.

In de onderstaande afbeelding ziet u hoe u de personalisatie van de voornaam kunt toevoegen.

![](assets/template-firstname.png){zoomable="yes"}

In ons voorbeeld voegen we de voornaam en vervolgens de achternaam toe en personaliseren we de knopkoppeling **[!UICONTROL Reset your password]** .

![](assets/template-button.png){zoomable="yes"}

### Een voorbeeld van een sjabloon bekijken

In deze fase van het maken van de sjabloon is het verstandig een voorvertoning van de sjablooninhoud weer te geven en de personalisatie te controleren.

Om dit te doen, vul in de [ contextsteekproef ](#context-sample), en klik op **[!UICONTROL Simulate content]** knoop.

![](assets/template-preview.png){zoomable="yes"}

## Een transactiebericht maken {#transactional-message}

U kunt een transactiemelding direct tot stand brengen of door een transactiemalplaatje van het berichtbericht te gebruiken. [ Leer hoe te om een transactionele berichtmalplaatje ](#transactional-template) tot stand te brengen.

Voer de onderstaande stappen uit om een transactiebericht te maken:

* Ga in de sectie **[!UICONTROL Triggered messages]** naar **[!UICONTROL Transactional messages]** . Op het tabblad **[!UICONTROL Browse]** kunt u alle gemaakte transactiemeldingen zien. Klik op de knop **[!UICONTROL Create transactional message]** om het bericht te maken.

  ![](assets/transactional-browse.png){zoomable="yes"}

* Kies in de nieuwe weergegeven pagina het kanaal van het bericht en kies de sjabloon waarmee u wilt werken. In ons voorbeeld, kiezen wij [ het malplaatje wij hier ](#transactional-template) creeerden.

  ![](assets/transactional-channel.png){zoomable="yes"}

  Klik nogmaals op de knop **[!UICONTROL Create transactional message]** om te controleren of uw bericht op het geselecteerde kanaal is gemaakt.

* U hebt nu toegang tot de configuratie van uw transactiebericht. Uw bericht erft de configuratie van het malplaatje. Deze pagina is bijna identiek aan de configuratiepagina van het transactiemalplaatje, behalve het omvat ook de configuratie van het gebeurtenistype.

  ![](assets/transactional-configuration.png){zoomable="yes"}

  Vul de configuratie van uw bericht zoals voor een malplaatje in:
   * [De eigenschappen van het transactiebericht](#transactional-properties)
   * [Het contextvoorbeeld](#context-sample)
   * [ de berichtinhoud ](#transactional-content)
en [ vorm het gebeurtenis-type ](#event-type) zoals hieronder gedetailleerd.

* Na [ het bevestigen van uw transactiebericht ](validate-transactional.md), klik op **[!UICONTROL Review and publish]** knoop om uw bericht tot stand te brengen en te publiceren.
De triggers kunnen nu de verzending van uw transactiemelding stimuleren.

### Informatie over het gebeurtenistype {#event-type}

>[!CONTEXTUALHELP]
>id="acw_transacmessages_event"
>title="Transactionele berichtengebeurtenis"
>abstract="De configuratie van het gebeurtenistype koppelt het bericht aan de trekkergebeurtenis."

De configuratie van het gebeurtenistype koppelt het bericht aan de trekkergebeurtenis.

In het Gebruikersinterface van het Web van de Campagne, kunt u selecteren en gebeurtenis-type reeds gecreeerd of direct uw gebeurtenis-type in deze configuratiepagina creëren.

![](assets/transactional-event-type.png){zoomable="yes"}

>[!CAUTION]
>
>Als u een gebeurtenistype selecteert dat momenteel door een ander transactiemelding wordt gebruikt, zal het de twee berichten teweegbrengen. Voor beste praktijken, **adviseren wij hoogst verbindend ÉÉN gebeurtenistype met slechts ÉÉN transactioneel bericht.**

## Aanbiedingen toevoegen aan je transactieberichten {#transactional-offers}

U kunt aanbiedingen opnemen in uw transactiemeldingen, zodat u relevante voorstellen aan uw eindgebruikers kunt presenteren, zelfs als het bericht gebeurtenisgestuurd is.

Deze functie is toegankelijk tijdens de bewerkingsfase van de inhoud van uw transactiebericht. Klik op de knop **[!UICONTROL Set up offers]** om deze te configureren.

Het installatieproces is gelijk aan het configureren van aanbiedingen voor levering van standaarden. [ Leer hoe te om aanbiedingen aan uw bericht ](../msg/offers.md) toe te voegen.

![](assets/transactional-offers.png){zoomable="yes"}
