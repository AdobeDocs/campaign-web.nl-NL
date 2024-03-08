---
audience: end-user
title: Uw eerste e-mail verzenden
description: Leer hoe u uw eerste e-mail verzendt met de gebruikersinterface van het Web van de Campagne
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: efb5d5d9ea3b3559c57d6a0b2a250f075dabf831
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 1%

---


# Uw eerste e-mail maken {#first-email}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card3"
>title="Aan de slag met e-mails"
>abstract="U kunt een zelfstandige e-maillevering maken of een e-mailbericht maken in de context van een campagneworkflow. Leer hoe u de levering maakt, het publiek selecteert en de e-mailinhoud ontwerpt."

Leer hoe u uw eerste e-mailadres maakt waarvoor u een e-mail wilt schrijven. In dit geval plant u het verzenden van een e-mail naar leden van Silver en Gold-loyaliteit op een bepaalde datum.

Gebaseerd op een vooraf gedefinieerde [ontwerpsjabloon](../email/create-email-templates.md)Bovendien bevat de e-mail ook gepersonaliseerde inhoud op basis van de kenmerken van het klantprofiel.

## E-maillevering maken {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Een e-mailsjabloon selecteren"
>abstract="Een e-mailmalplaatje is een specifieke leveringsconfiguratie die vooraf bepaalde montages, zoals typologieregels, verpersoonlijking of het verpletteren van parameters bevat. De malplaatjes worden bepaald in de de cliëntconsole van de Campagne."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="Uw e-maileigenschappen definiëren"
>abstract="De eigenschappen zijn de gemeenschappelijke leveringsparameters die u helpen om uw levering te noemen en te classificeren. De extra instellingen zijn optioneel. Als uw levering is gebaseerd op een uitgebreid schema dat is gedefinieerd in de Adobe Campaign v8-console, zijn er enkele specifieke **Aangepaste opties** zijn beschikbaar."

U kunt een zelfstandige e-maillevering maken of een e-mailbericht maken in de context van een campagneworkflow. In de onderstaande stappen wordt de procedure beschreven voor een zelfstandige (one-shot) e-maillevering. Meer informatie over het maken van aanbiedingen in Adobe Campaign vindt u in [deze pagina](../msg/gs-deliveries.md).

Volg onderstaande stappen om een nieuwe, zelfstandige e-maillevering te maken.

1. Bladeren naar de **[!UICONTROL Deliveries]** op de linkerspoorstaaf en klik op  **[!UICONTROL Create delivery]** knop.

   ![](../msg/assets/create-a-delivery.png)

1. Selecteren **[!UICONTROL Email]** als het kanaal en kies een sjabloon voor e-maillevering in de lijst.

   >[!NOTE]
   >
   >Sjablonen zijn vooraf geconfigureerde leveringsinstellingen die zijn opgeslagen voor toekomstig gebruik. [Meer informatie](../msg/delivery-template.md)

   ![](assets/channel-template.png){zoomable=&quot;yes&quot;}

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.
1. Voer een label voor de levering in en configureer aanvullende opties op basis van uw behoeften:

   * **[!UICONTROL Internal name]**: wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: gebruik dit veld om uw leveringen te ordenen op basis van uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: geef een beschrijving voor de levering.
   * **[!UICONTROL Nature]**: specificeer de aard van de e-mail voor classificatiedoeleinden.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Als u uw schema met specifieke douanevelden hebt uitgebreid, kunt u tot hen in toegang hebben **[!UICONTROL Custom options]** sectie.

   ![](assets/email-properties.png){zoomable=&quot;yes&quot;}

1. Bovendien zijn geavanceerde instellingen, zoals typologische regels en doeltoewijzingen, toegankelijk via de **[!UICONTROL Settings]** op de knop rechtsboven in het scherm. Deze instellingen zijn vooraf geconfigureerd in de geselecteerde sjabloon, maar kunnen zo nodig worden bewerkt voor deze specifieke e-mail. [Meer informatie](../advanced-settings/delivery-settings.md)

## De doelgroep definiëren {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="Selecteer een publiek voor uw levering"
>abstract="Selecteer het beste publiek voor uw marketingbericht. U kunt een bestaand publiek kiezen (al gedefinieerd in een Campagne v8-instantie of in Adobe Experience Platform), een nieuw publiek maken met de querymodelfunctie of een bestand uploaden dat uw publiek bevat. Besturingsgroepen zijn niet ingeschakeld voor de **Selecteren uit bestand** en omgekeerd."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/add-audience.html" text="Het grote publiek selecteren"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/target-audiences/control-group.html" text="Een controlegroep instellen"

In dit geval stuurt u de e-mail naar een bestaand publiek.

Aanvullende instructies over het werken met het publiek zijn beschikbaar in [deze sectie](../audience/about-recipients.md).

1. Als u het publiek voor de e-mail wilt selecteren, klikt u op de knop **[!UICONTROL Select audience]** en kiest u een bestaand publiek in de lijst.

   In dit voorbeeld willen we een bestaand publiek gebruiken dat zich richt op klanten die behoren tot het niveau van de zilveren- en goudloyaliteitspunten.

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >De soorten publiek die beschikbaar zijn in de lijst komen uit uw Campagne v8-instantie of uit Adobe Experience Platform als de integratie Doel/Bron op uw instantie is geconfigureerd. Dankzij deze integratie kunt u segmenten van het Experience Platform naar Adobe Campaign verzenden en de bezorging en het bijhouden van logbestanden van de campagne naar Adobe Experience Platform verzenden. Meer informatie over het werken met Campagne en Adobe Experience Platform in de [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep/ac-aep.html){target="_blank"}.

1. Als het publiek is geselecteerd, kunt u het doel verder verfijnen door aanvullende regels toe te passen.

   ![](assets/audience-selected.png){zoomable=&quot;yes&quot;}

1. U kunt ook een controlegroep instellen om het gedrag van de e-mailontvangers te analyseren in vergelijking met degenen die niet als doelgroep werden gebruikt. [Leer hoe u met besturingsgroepen werkt](../audience/control-group.md)

## De e-mailcontent opgeven {#create-content}

Volg onderstaande stappen om uw e-mailinhoud te maken. In dit geval gebruikt u een vooraf gedefinieerde e-mail [leveringssjabloon](../msg/delivery-template.md) om uw e-mail te ontwerpen.<!--TBC delivery template or email content template?-->

<!--Detailed instructions on how to configure the email content are available in [this section](../email/edit-content.md).-->

1. Klik op het dashboard voor e-maillevering op de knop **[!UICONTROL Edit content]** knop.

   ![](assets/email-edit-content.png){zoomable=&quot;yes&quot;}

   Hiermee gaat u naar een speciale interface waar u de e-mailinhoud kunt configureren en toegang kunt krijgen tot de e-mailontwerper. [Meer informatie](edit-content.md)

   ![](assets/edit-content.png){zoomable=&quot;yes&quot;}

1. Voer de onderwerpregel van uw e-mail in en pas deze aan met de Expressieeditor. [Leer hoe u uw inhoud kunt aanpassen](../personalization/personalize.md)

   ![](assets/subject-line.png){zoomable=&quot;yes&quot;}

1. Als u de inhoud van de e-mail wilt ontwerpen, klikt u op de knop **[!UICONTROL Edit email body]** knop.

   Kies de methode die u wilt gebruiken om uw e-mailinhoud te maken. In dit voorbeeld gebruikt u een [vooraf gedefinieerde inhoudssjabloon](create-email-templates.md).

   ![](assets/select-template.png){zoomable=&quot;yes&quot;}

1. Nadat u de sjabloon hebt geselecteerd, wordt deze weergegeven in het dialoogvenster [E-mailDesigner](create-email-content.md), waar u eventueel noodzakelijke bewerkingen kunt uitvoeren en personalisatie kunt toevoegen.

   Als u bijvoorbeeld personalisatie wilt toevoegen aan de e-mailtitel, selecteert u het componentblok en klikt u op **[!UICONTROL Add Personalization]**.

   ![](assets/add-perso.png){zoomable=&quot;yes&quot;}

1. Als u tevreden bent met de inhoud, slaat u het ontwerp op en sluit u het. Klikken **[!UICONTROL Save]** om terug te keren naar het scherm voor het maken van e-mail.

   ![](assets/save-content.png){zoomable=&quot;yes&quot;}

## Het verzenden plannen {#schedule}

Wanneer een levering in de context van een werkschema wordt verzonden, moet u gebruiken **Planner** activiteit. Meer informatie in [deze pagina](../workflows/activities/scheduler.md). Onderstaande stappen zijn alleen van toepassing op zelfstandige leveringen.

1. Bladeren naar de **[!UICONTROL Schedule]** van de leveringseigenschappen.

1. Gebruik de **[!UICONTROL Enable scheduling]** schakelen om het te activeren.

1. Stel de gewenste datum en tijd in voor het verzenden.

   ![](assets/schedule.png){zoomable=&quot;yes&quot;}

Zodra u de levering verzendt, begint de daadwerkelijke verzendende op de contactdatum u hebt bepaald.

Meer informatie over de planning van de levering in [deze sectie](../msg/gs-deliveries.md#schedule-the-delivery-sending).

## Een voorbeeld van een e-mail bekijken en proefdrukken verzenden {#preview-test}

Voordat u uw e-mail verzendt, kunt u een voorbeeld bekijken en testen of deze voldoet aan uw verwachtingen.

In dit geval bekijkt u een voorbeeld van de e-mail en verzendt u proefdrukken naar specifieke e-mailadressen terwijl u zich aan enkele van de beoogde profielen aanpast.

Aanvullende informatie over het bekijken van een voorbeeld van een e-mail en het verzenden van proefdrukken vindt u in [deze sectie](../preview-test/preview-test.md).

1. Als u uw e-mail wilt bekijken, klikt u op **[!UICONTROL Review and send]**. Dit toont een voorproef van uw e-mail, samen met alle gevormde eigenschappen, publiek en programma. U kunt al deze elementen bewerken door op de knop Wijzigen te klikken.

1. Klik op de knop **[!UICONTROL Simulate content]** knop.

   ![](assets/review-email.png){zoomable=&quot;yes&quot;}

1. Selecteer links het profiel of de profielen die u wilt gebruiken voor een voorbeeld van het e-mailbericht.

   In het rechterdeelvenster ziet u een voorbeeld van de e-mail op basis van het geselecteerde profiel. Als u meerdere profielen hebt toegevoegd, kunt u tussen de profielen schakelen om een voorbeeld van de bijbehorende e-mail te bekijken.

   ![](assets/preview.png){zoomable=&quot;yes&quot;}

   <!--Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering
    -->

1. Als u proefdrukken wilt verzenden, klikt u op de knop **[!UICONTROL Send proofs]** kiest u vervolgens de gewenste modus.

   In dit voorbeeld gebruikt u de opdracht **[!UICONTROL Substitute from main target]** -modus, die proefdrukken naar specifieke e-mailadressen verzendt en tegelijkertijd enkele profielen nastreeft die in de e-mail worden genoemd.

   ![](assets/proof-mode.png){zoomable=&quot;yes&quot;}

1. Klikken **[!UICONTROL Add address]** en geef het e-mailadres of de e-mailadressen op die de proefdrukken ontvangen.

   Selecteer voor elk e-mailadres het profiel dat u wilt beleven. U kunt Adobe Campaign ook een willekeurig profiel van het doel laten selecteren.

   ![](assets/proof-test-profile.png){zoomable=&quot;yes&quot;}

1. Klikken **[!UICONTROL Send proof]** en de verzending bevestigen.

   Proefdrukken worden naar de opgegeven e-mailadressen verzonden met het geselecteerde profiel **[Proef x]** voorvoegsel

   ![](assets/proof-sent.png){zoomable=&quot;yes&quot;}

   U kunt de status van de verzendende persoon controleren en de verzonden proefdrukken op elk gewenst moment openen door op de knop **[!UICONTROL View proofs]** in het scherm Inhoud simuleren.

## E-mail verzenden en controleren {#prepare-send}

Nadat u uw e-mail hebt bekeken en getest, kunt u de voorbereiding starten en verzenden.

1. Als u het voorbereiden van de e-mail wilt starten, klikt u op **[!UICONTROL Prepare]**. [Leer hoe u een e-mail voorbereidt](../monitor/prepare-send.md)

   ![](assets/preparation.png){zoomable=&quot;yes&quot;}

1. Als je e-mail klaar is om te worden verzonden, klik je op de knop **[!UICONTROL Send]** knop (of **[!UICONTROL Send as scheduled]** (als u de verzending hebt gepland) en bevestig de verzending.

1. Tijdens het verzendende proces, kunt u zijn vooruitgang volgen en statistieken in real time direct in dit scherm bekijken.

   ![](assets/sending-email.png){zoomable=&quot;yes&quot;}

   <!--
    ![](assets/sent-email.png){zoomable="yes"}-->

   U kunt gedetailleerde informatie over het verzenden ook toegang hebben door te klikken op **[!UICONTROL Logs]** knop. [Leer hoe u leveringslogboeken kunt controleren](../monitor/delivery-logs.md)

1. Nadat u het e-mailbericht hebt verzonden, kunt u specifieke rapporten voor verdere analyse openen door op de knop **[!UICONTROL Reporting]** knop.

![](assets/reports.png){zoomable=&quot;yes&quot;}
