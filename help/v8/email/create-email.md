---
audience: end-user
title: Uw eerste e-mail verzenden
description: Leer hoe u uw eerste e-mail verzendt met de gebruikersinterface van het Web van de Campagne
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 8006eeb6088d7d6ef99f374b2b846978cd679c01
workflow-type: tm+mt
source-wordcount: '1568'
ht-degree: 1%

---

# Uw eerste e-mail maken {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Aan de slag met e-mails"
>abstract="U kunt een zelfstandige e-maillevering maken of een e-mailbericht maken in de context van een campagneworkflow. Leer hoe u de levering maakt, het publiek selecteert en de e-mailinhoud ontwerpt."

Leer hoe u uw eerste e-mailadres maakt waarvoor u een e-mail wilt schrijven. In dit geval plant u het verzenden van een e-mail naar leden van Silver en Gold-loyaliteit op een bepaalde datum.

Gebaseerd op een vooraf bepaald [ ontwerpmalplaatje ](../email/create-email-templates.md), kenmerkt e-mail ook gepersonaliseerde inhoud die op de attributen van het klantenprofiel wordt gebaseerd.

➡️ [Ontdek deze functie in video](#video)

## E-maillevering maken {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Een e-mailsjabloon selecteren"
>abstract="Een e-mailmalplaatje is een specifieke leveringsconfiguratie die vooraf bepaalde montages, zoals typologieregels, verpersoonlijking, of het verpletteren van parameters bevat. De malplaatjes worden bepaald in de de cliëntconsole van de Campagne."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Uw e-maileigenschappen definiëren"
>abstract="De eigenschappen zijn de gemeenschappelijke leveringsparameters die u helpen uw levering noemen en classificeren. De extra instellingen zijn optioneel. Als uw levering op een uitgebreid schema gebaseerd is dat in de Adobe Campaign v8 console wordt bepaald, zijn sommige specifieke **gebieden van de Opties van de Douane** beschikbaar."

U kunt een zelfstandige e-maillevering maken of een e-mailbericht maken in de context van een campagneworkflow. In de onderstaande stappen wordt de procedure beschreven voor een zelfstandige (one-shot) e-maillevering. Leer meer over de stappen van de leveringsverwezenlijking in Adobe Campaign in [ deze pagina ](../msg/gs-deliveries.md).

Volg onderstaande stappen om een nieuwe, zelfstandige e-maillevering te maken.

1. Blader naar het menu **[!UICONTROL Deliveries]** op de linkertrack en klik op de knop **[!UICONTROL Create delivery]** .

   ![ Schermschot die de Create leveringsknoop in het menu van Leveringen tonen ](../msg/assets/create-a-delivery.png)

1. Selecteer **[!UICONTROL Email]** als kanaal en kies een sjabloon voor e-maillevering in de lijst.

   >[!NOTE]
   >
   >Sjablonen zijn vooraf geconfigureerde leveringsinstellingen die zijn opgeslagen voor toekomstig gebruik. [Meer informatie](../msg/delivery-template.md)

   ![ Schermafbeelding die de selectie van het e-mailkanaal en het malplaatje tonen ](assets/channel-template.png){zoomable="yes"}

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.
1. Voer een label voor de levering in en configureer aanvullende opties op basis van uw behoeften:

   * **[!UICONTROL Internal name]**: wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: gebruik dit veld om uw leveringen te ordenen op basis van uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: geef een beschrijving op voor de levering.
   * **[!UICONTROL Nature]**: geef de aard van de e-mail op voor classificatiedoeleinden. <!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Als u uw schema met specifieke douanevelden hebt uitgebreid, kunt u tot hen in de **[!UICONTROL Custom options]** sectie toegang hebben.

   ![ Schermafbeelding die de configuratie van e-maileigenschappen toont ](assets/email-properties.png){zoomable="yes"}

1. Bovendien zijn geavanceerde instellingen, zoals typologische regels en doeltoewijzingen, toegankelijk via de knop **[!UICONTROL Settings]** rechtsboven in het scherm. Deze instellingen zijn vooraf geconfigureerd in de geselecteerde sjabloon, maar kunnen zo nodig worden bewerkt voor deze specifieke e-mail. [Meer informatie](../advanced-settings/delivery-settings.md)

## De doelgroep definiëren {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Selecteer een publiek voor uw levering"
>abstract="Selecteer het beste publiek voor uw marketingbericht. U kunt een bestaand publiek kiezen (al gedefinieerd in een Campagne v8-instantie of in Adobe Experience Platform), een nieuw publiek maken met de querymodelfunctie of een bestand uploaden dat uw publiek bevat. De groepen van de controle worden niet toegelaten voor **Uitgezocht van dossier** optie en vice versa."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html?lang=nl-NL" text="Het grote publiek selecteren"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html?lang=nl-NL" text="Een controlegroep instellen"

In dit geval stuurt u de e-mail naar een bestaand publiek.

De extra instructies op hoe te met publiek te werken zijn beschikbaar in [ deze sectie ](../audience/about-recipients.md).

1. Als u het publiek voor de e-mail wilt selecteren, klikt u op de knop **[!UICONTROL Select audience]** en kiest u een bestaand publiek in de lijst.

   In dit voorbeeld willen we een bestaand publiek gebruiken dat zich richt op klanten die tot de niveaus van de Silver- en Gold-loyaliteitspunten behoren.

   ![ Schermafbeelding die het proces van de publieksselectie toont ](assets/create-audience.png){zoomable="yes"}

   >[!NOTE]
   >
   >Het publiek dat in de lijst beschikbaar is, komt uit uw Campagne v8-exemplaar of uit Adobe Experience Platform als de integratie tussen Doel en Source op uw exemplaar is geconfigureerd. Dankzij deze integratie kunt u Experience Platform-segmenten naar Adobe Campaign verzenden en Campagne leveren en logbestanden bijhouden naar Adobe Experience Platform. Leer hoe te met Campagne en Adobe Experience Platform in de [ Campagne v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html?lang=nl-NL){target="_blank"} te werken.

1. Als het publiek is geselecteerd, kunt u het doel verder verfijnen door aanvullende regels toe te passen.

   ![ Schermafbeelding die het proces van de publieksverfijning toont ](assets/audience-selected.png){zoomable="yes"}

1. U kunt ook een controlegroep instellen om het gedrag van de e-mailontvangers te analyseren in vergelijking met degenen die niet als doelgroep werden gebruikt. [ leer hoe te met controlegroepen ](../audience/control-group.md) werken

## De e-mailcontent opgeven {#create-content}

Volg onderstaande stappen om uw e-mailinhoud te maken. In dit gebruiksgeval, gebruikt u een vooraf bepaalde e-mail [ leveringsmalplaatje ](../msg/delivery-template.md) om uw e-mail te ontwerpen.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. Klik op de knop **[!UICONTROL Edit content]** in het dashboard voor e-maillevering.

   ![ Schermafbeelding die de Edit inhoudsknoop tonen ](assets/email-edit-content.png){zoomable="yes"}

   Hiermee gaat u naar een speciale interface waar u de e-mailinhoud kunt configureren en toegang kunt krijgen tot de e-mailtoepassing van de Designer. [Meer informatie](edit-content.md)

   ![ Schermafbeelding die de interface van Designer E-mail toont ](assets/edit-content.png){zoomable="yes"}

1. Voer de onderwerpregel van uw e-mail in en pas deze aan met de Expressieeditor. [ Leer hoe te om uw inhoud te personaliseren ](../personalization/personalize.md)

   ![ Schermafbeelding die de configuratie van de onderwerpregel tonen ](assets/subject-line.png){zoomable="yes"}

1. Klik op de knop **[!UICONTROL Edit email body]** om de inhoud van de e-mail te ontwerpen.

   Kies de methode die u wilt gebruiken om uw e-mailinhoud te maken. In dit voorbeeld, gebruik a [ vooraf bepaald inhoudsmalplaatje ](create-email-templates.md).

   ![ Screenshot die de selectie van een vooraf bepaald inhoudsmalplaatje ](assets/select-template.png){zoomable="yes"} toont

1. Zodra u het malplaatje hebt geselecteerd, wordt het getoond in [ E-mail Designer ](create-email-content.md), waar u om het even welke noodzakelijke uitgeeft kunt maken en verpersoonlijking toevoegen.

   Als u bijvoorbeeld personalisatie wilt toevoegen aan de e-mailtitel, selecteert u het componentblok en klikt u op **[!UICONTROL Add Personalization]** .

   ![ Schermschot die het verpersoonlijkingsproces ](assets/add-perso.png){zoomable="yes"} tonen

1. Als u tevreden bent met de inhoud, slaat u het ontwerp op en sluit u het. Klik op **[!UICONTROL Save]** om terug te keren naar het scherm voor het maken van e-mail.

   ![ Schermafbeelding die sparen knoop ](assets/save-content.png){zoomable="yes"} tonen

## Het verzenden plannen {#schedule}

Wanneer een levering in de context van een werkschema wordt verzonden, moet u de **Planner** activiteit gebruiken. Leer meer in [ deze pagina ](../workflows/activities/scheduler.md). Onderstaande stappen zijn alleen van toepassing op zelfstandige leveringen.

1. Blader naar de sectie **[!UICONTROL Schedule]** van de leveringseigenschappen.

1. Activeer de schakeloptie **[!UICONTROL Enable scheduling]** .

1. Stel de gewenste datum en tijd in voor het verzenden.

   ![ Screenshot die de het plannen configuratie ](assets/schedule.png){zoomable="yes"} tonen

Zodra u de levering verzendt, begint de daadwerkelijke verzendende op de contactdatum u hebt bepaald.

Leer meer over levering het plannen in [ deze sectie ](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Een voorbeeld van een e-mail bekijken en proefdrukken verzenden {#preview-test}

Voordat u uw e-mail verzendt, kunt u een voorbeeld bekijken en testen of deze voldoet aan uw verwachtingen.

In dit geval bekijkt u een voorbeeld van de e-mail en verzendt u proefdrukken naar specifieke e-mailadressen terwijl u zich aan enkele van de beoogde profielen aanpast.

De extra informatie over hoe te voorproef e-mail en verzendt proef is beschikbaar in [ deze sectie ](../preview-test/preview-test.md).

1. Klik op **[!UICONTROL Review and send]** om uw e-mail te bekijken. Dit toont een voorproef van uw e-mail, samen met alle gevormde eigenschappen, publiek, en programma. U kunt al deze elementen bewerken door op de knop Wijzigen te klikken.

1. Klik op de knop **[!UICONTROL Simulate content]** om een voorbeeld van de e-mail te bekijken en proefdrukken te verzenden.

   ![ Schermafbeelding die de Simuleren inhoudsknoop tonen ](assets/review-email.png){zoomable="yes"}

   >[!NOTE]
   >
   >De knop **[!UICONTROL Simulate content]** is in specifieke contexten uitgeschakeld. De beperkingen zijn gedetailleerd [ in deze sectie ](#content-simulation-limitations).

1. Selecteer links het profiel of de profielen die u wilt gebruiken voor een voorbeeld van het e-mailbericht.

   In het rechterdeelvenster ziet u een voorbeeld van de e-mail op basis van het geselecteerde profiel. Als u meerdere profielen hebt toegevoegd, kunt u tussen de profielen schakelen om een voorbeeld van de bijbehorende e-mail te bekijken.

   ![ Schermafbeelding die de e-mailvoorproef toont die op geselecteerde profielen ](assets/preview.png){zoomable="yes"} wordt gebaseerd

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using multiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Als u proefdrukken wilt verzenden, klikt u op de knop **[!UICONTROL Send proofs]** en kiest u de gewenste modus.

   In dit voorbeeld gebruikt u de modus **[!UICONTROL Substitute from main target]** , waarin proefdrukken naar specifieke e-mailadressen worden verzonden en waarin enkele profielen worden nagemaakt waarop de e-mail betrekking heeft.

   ![ Schermschot die de proef tonen die wijzeselectie verzendt ](assets/proof-mode.png){zoomable="yes"}

1. Klik op **[!UICONTROL Add address]** en geef het e-mailadres of de e-mailadressen op waar de proefdrukken worden gemaakt.

   Selecteer voor elk e-mailadres het profiel dat u wilt beleven. U kunt Adobe Campaign ook een willekeurig profiel van het doel laten selecteren.

   ![ Schermafbeelding die de toevoeging van e-mailadressen voor proefdrukken tonen ](assets/proof-test-profile.png){zoomable="yes"}

1. Klik op **[!UICONTROL Send proof]** en bevestig het verzenden.

   De proef wordt verzonden naar de gespecificeerde e-mailadressen gebruikend het geselecteerde profiel met **[Proef x]** prefix.

   ![ Screenshot die de bevestiging van bewijs toont die ](assets/proof-sent.png){zoomable="yes"} verzendt

   U kunt de status van de verzendende en de verzonden proefdrukken op elk gewenst moment controleren door op de knop **[!UICONTROL View proofs]** in het scherm Inhoud simuleren te klikken.

### Beperkingen op het simuleren van inhoud {#content-simulation-limitations}

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_multilingual"
>title="Inhoud simuleren wordt niet ondersteund"
>abstract="De **Simuleer inhoud** knoop is gehandicapt omdat de meertalige levering slechts één scène bevat."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_reconcilied_deliveries"
>title="Inhoud simuleren wordt niet ondersteund"
>abstract="De **Simuleer inhoud** knoop is gehandicapt omdat het niet compatibel is met verzochte leveringen in deze fase."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_ffda"
>title="Inhoud simuleren wordt niet ondersteund"
>abstract="De **Simuleer inhoud** knoop wordt onbruikbaar gemaakt omdat niet gesteund in de Volledige Verbond van de Onderneming van de Campagne wijze van de Toegang (FFDA)."

>[!CONTEXTUALHELP]
>id="acw_simulation_limitation_no_file"
>title="Inhoud simuleren wordt niet ondersteund"
>abstract="De **Simuleer inhoud** knoop is gehandicapt omdat geen inhoud is geupload."

In sommige gevallen kunt u geen inhoudsimulatie uitvoeren en is de knop **[!UICONTROL Simulate content]** uitgeschakeld.

In de volgende gevallen wordt de simulatie van inhoud niet ondersteund:

<!--* When a multilingual delivery contains only one locale,-->
* met onderling samenhangende leveringen,
* Wanneer uw de plaatsingsmodel van de Campagne [ Volledige Federatieve Toegang van de Onderneming van Adobe Campaign (FFDA) ](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/config/architecture/ffda/enterprise-deployment){target="_blank"} is
* Wanneer er geen bestand is geüpload.

## E-mail verzenden en controleren {#prepare-send}

Nadat u uw e-mail hebt bekeken en getest, kunt u de voorbereiding starten en verzenden.

1. Klik op **[!UICONTROL Prepare]** om het voorbereiden van de e-mail te starten. [ Leer hoe te om een e-mail ](../monitor/prepare-send.md) voor te bereiden

   ![ Schermafbeelding die de knop Voorbereiden tonen ](assets/preparation.png){zoomable="yes"}

1. Als uw e-mail gereed is om te worden verzonden, klikt u op de knop **[!UICONTROL Send]** (of **[!UICONTROL Send as scheduled]** als u de verzending hebt gepland) en bevestigt u de verzending.

1. Tijdens het verzendende proces, kunt u zijn vooruitgang volgen en statistieken in real time direct in dit scherm bekijken.

   ![ Schermschot die e-mail tonen die vooruitgang verzenden ](assets/sending-email.png){zoomable="yes"}

   <!--
    ![Screenshot showing the email sent confirmation](assets/sent-email.png){zoomable="yes"}-->

   U kunt ook gedetailleerde informatie over het verzenden bekijken door op de knop **[!UICONTROL Logs]** te klikken. [ Leer hoe te om leveringslogboeken te controleren ](../monitor/delivery-logs.md)

1. Nadat u het e-mailbericht hebt verzonden, kunt u specifieke rapporten openen voor verdere analyse door op de knop **[!UICONTROL Reporting]** te klikken.

![ Schermafbeelding die de knoop van de Rapportering ](assets/reports.png){zoomable="yes"} tonen

## Hoe kan ik-video {#video}

Leer hoe u een volledig nieuwe e-maillevering maakt, het publiek definieert, de inhoud ontwerpt, voorvertoning simuleert en een proefdruk verzendt.

>[!VIDEO](https://video.tv.adobe.com/v/3425866/?quality=12)