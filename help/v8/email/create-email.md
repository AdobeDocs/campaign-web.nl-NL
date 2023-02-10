---
audience: end-user
title: Uw eerste e-mail verzenden
description: Leer hoe u uw eerste e-mail verzendt met de interface van het Web van de Campagne
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: 4332facf1b7853cb36c9de752ff48bb68e97d6e0
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 1%

---

# Uw eerste e-mail verzenden {#first-email}

![](../assets/do-not-localize/badge.png)

Leer hoe u uw eerste e-mailadres maakt waarvoor u een e-mail wilt schrijven. In dit geval plant u het verzenden van een e-mail naar leden van Silver en Gold-loyaliteit op een bepaalde datum.

Op basis van een vooraf gedefinieerde ontwerpsjabloon bevat de e-mail ook gepersonaliseerde inhoud op basis van de kenmerken van het klantprofiel.

![](assets/delivery-list.png)

## E-mail maken {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Een e-mailsjabloon selecteren"
>abstract="Een e-mailmalplaatje is een specifieke leveringsconfiguratie die vooraf bepaalde montages, zoals typologieregels, verpersoonlijking of het verpletteren van parameters bevat. De malplaatjes worden bepaald in de de cliëntconsole van de Campagne."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="E-maileigenschappen"
>abstract="De eigenschappen zijn de gemeenschappelijke leveringsparameters die u helpen om uw levering te noemen en te classificeren. Als uw levering is gebaseerd op een uitgebreid schema dat is gedefinieerd in de Adobe Campaign v8-console, zijn er enkele specifieke **Aangepaste opties** zijn beschikbaar."

1. Als u een nieuwe levering wilt maken, gaat u naar de **[!UICONTROL Deliveries]** en selecteert u **[!UICONTROL Email]** als het kanaal.

1. Selecteer de sjabloon die u wilt gebruiken en klik op **[!UICONTROL Create delivery]**.

   >[!NOTE]
   >
   >Sjablonen zijn vooraf geconfigureerde leveringsinstellingen die zijn opgeslagen voor toekomstig gebruik. Ze kunnen door beheerders in de Adobe Campaign-console worden gemaakt. [Meer informatie over het werken met leveringssjablonen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. Geef een label voor de e-mail en configureer aanvullende opties op basis van uw behoeften:

   * **[!UICONTROL Internal name]**: een unieke identificatiecode aan de levering toewijzen;
   * **[!UICONTROL Folder]**: de levering opslaan in een specifieke map,
   * **[!UICONTROL Delivery code]**: gebruik dit veld om uw leveringen te ordenen op basis van uw eigen naamgevingsconventie,
   * **[!UICONTROL Description]**: een omschrijving van de levering,
   * **[!UICONTROL Nature]**: de aard van het e-mailbericht voor classificatiedoeleinden specificeren.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Als u uw schema met specifieke douanevelden hebt uitgebreid, kunt u tot hen in toegang hebben **[!UICONTROL Custom options]** sectie.

   ![](assets/email-properties.png)

   Bovendien, kunnen de geavanceerde montages, zoals typologieregels en doelafbeeldingen, worden betreden door de knoop te klikken die naast de leveringsnaam wordt gevestigd. Deze instellingen zijn vooraf geconfigureerd in de geselecteerde sjabloon, maar kunnen zo nodig worden bewerkt voor deze specifieke e-mail.

## E-mailinhoud maken {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Leer hoe u uw e-mailinhoud ontwerpt"
>abstract="Leer hoe u de e-mailontwerper gebruikt."

In dit geval gebruikt u een vooraf gedefinieerde sjabloon om ons e-mailbericht te ontwerpen.

Gedetailleerde instructies over het configureren van de e-mailinhoud zijn beschikbaar in [deze sectie](../content/edit-content.md).

1. Klik op de knop **[!UICONTROL Edit content]** knop.

   Hiermee gaat u naar een speciale interface waar u de e-mailinhoud kunt configureren en ontwerpen met de e-mailontwerper.

   ![](assets/edit-content.png)

1. Voer de onderwerpregel van uw e-mail in en pas deze aan met de Expressieeditor. [Leer hoe u uw inhoud kunt aanpassen](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Als u de hoofdtekst van de e-mail wilt ontwerpen, klikt u op de knop **[!UICONTROL Edit email body]** knop.

   Kies de methode die u wilt gebruiken om uw e-mailinhoud te maken. In dit voorbeeld gebruikt u een vooraf gedefinieerde ontwerpsjabloon.

   ![](assets/select-template.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Nadat u de sjabloon hebt geselecteerd, wordt deze weergegeven in de e-mailontwerper, waar u eventueel noodzakelijke bewerkingen kunt uitvoeren en personalisatie kunt toevoegen.

   Als u bijvoorbeeld personalisatie wilt toevoegen aan de e-mailtitel, selecteert u het componentblok en klikt u op **[!UICONTROL Add Personalization]**.

   ![](assets/add-perso.png)

1. Als u tevreden bent met de inhoud, slaat u het ontwerp op en sluit u het. Klikken **[!UICONTROL Save]** om terug te keren naar het scherm voor het maken van e-mail.

   ![](assets/save-content.png)

## De doelgroep definiëren {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="De doelgroep definiëren"
>abstract="Selecteer het beste publiek voor uw marketingbericht. U kunt een bestaand publiek kiezen dat al is gedefinieerd in een Campagne v8-instantie of in Adobe Experience Platform, of u kunt een nieuw publiek maken met de functie voor het maken van regels."

In dit geval stuurt u de e-mail naar een bestaand publiek. Aanvullende instructies over het werken met het publiek zijn beschikbaar in [deze sectie](../audience/about-audiences.md).

1. Als u het publiek voor de e-mail wilt selecteren, klikt u op de knop **[!UICONTROL Select audience]** en kiest u een bestaand publiek in de lijst.

   In dit voorbeeld willen we een bestaand publiek gebruiken dat zich richt op klanten die behoren tot het niveau van de zilveren- en goudloyaliteitspunten.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Het publiek beschikbaar in de lijst komt van uw instantie van de Campagne v8 of van Adobe Experience Platform voort als de Bestemming/Bronintegratie op uw instantie is gevormd.
   >
   >Met de integratie Doel/Bronnen kunt u de segmenten Experience Platform naar Adobe Campaign verzenden en de bezorging en tracering van campagnes naar Adobe Experience Platform verzenden. [Leer hoe u met Campagne en Adobe Experience Platform werkt](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. Als het publiek is geselecteerd, kunt u het doel verder verfijnen door aanvullende regels toe te passen.

   U kunt ook een controlegroep instellen om het gedrag van de e-mailontvangers te analyseren in vergelijking met degenen die niet als doelgroep werden gebruikt. [Leer hoe u met besturingsgroepen werkt](../audience/control-group.md)

   ![](assets/audience-selected.png)

## Plan de verzending {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Plan de verzending"
>abstract="Bepaal de datum en de nauwkeurige tijd voor uw verzendend. Door de meest geschikte tijd voor uw marketingbericht te kiezen, kunt u de open tarieven maximaliseren."

Als u het verzenden van de e-mail wilt plannen, klikt u op **[!UICONTROL Enable]** en stelt u de gewenste datum en tijd voor verzending in.

Standaard worden de **[!UICONTROL Confirm before sending]** is ingeschakeld, zodat u de verzending moet bevestigen voordat het e-mailbericht op de geplande datum en tijd wordt verzonden. Als u het e-mailbericht automatisch wilt verzenden op de geplande datum en tijd, kunt u deze optie uitschakelen.

![](assets/schedule.png)

## E-mail voorvertonen en testen {#preview-test}

Voordat u uw e-mail verzendt, kunt u een voorbeeld bekijken en testen of deze voldoet aan uw verwachtingen.

In dit geval bekijkt u een voorbeeld van de e-mail en verzendt u testversies naar specifieke e-mailadressen terwijl u zich aan enkele van de beoogde profielen aanpast.

Aanvullende informatie over het bekijken en testen van e-mails is beschikbaar in [deze sectie](../preview-test/preview-test.md).

1. Klik op **[!UICONTROL Review and send]**. Dit toont een voorproef van uw e-mail, samen met alle gevormde eigenschappen, publiek en programma. U kunt al deze elementen bewerken door op de knop Wijzigen te klikken.

1. Klik op de knop **[!UICONTROL Simulate content]** knop.

   ![](assets/review-email.png)

1. Selecteer links het profiel of de profielen die u wilt gebruiken voor een voorbeeld van het e-mailbericht.

   In het rechterdeelvenster ziet u een voorbeeld van het e-mailbericht op basis van het geselecteerde profiel. Als u meerdere profielen hebt toegevoegd, kunt u tussen de profielen schakelen om een voorbeeld van de bijbehorende e-mail te bekijken.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Als u testversies van uw e-mail wilt verzenden, klikt u op de knop **[!UICONTROL Test]** kiest u vervolgens de gewenste modus.

   In dit voorbeeld gebruikt u de opdracht **[!UICONTROL Substitute from main target]** -modus, die testversies naar specifieke e-mailadressen verzendt en tegelijkertijd enkele profielen nastreeft die in de e-mail worden genoemd.

   ![](assets/proof-mode.png)

1. Klikken **[!UICONTROL Add address]** en vermeld het e-mailadres of de e-mailadressen die de testversies ontvangen.

   Selecteer voor elk e-mailadres het profiel dat u wilt beleven. U kunt Adobe Campaign ook een willekeurig profiel van het doel laten selecteren.

   ![](assets/proof-test-profile.png)

1. Klikken **[!UICONTROL Send test email]** en de verzending bevestigen.

   Testversies worden naar de opgegeven e-mailadressen verzonden met behulp van het geselecteerde profiel met het **[Proef x]** voorvoegsel.

   ![](assets/proof-sent.png)

   U kunt de status van de verzendende e-mail controleren en de verzonden teste-mails op elk gewenst moment openen door op de knop **[!UICONTROL View test email log]** in het scherm Inhoud simuleren.

## E-mail verzenden en controleren {#prepare-send}

Nadat u uw e-mail hebt bekeken en getest, kunt u de voorbereiding starten en verzenden.

1. Klik op **[!UICONTROL Prepare]**. [Leer hoe u een e-mail voorbereidt](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Als je e-mail klaar is om te worden verzonden, klik je op de knop **[!UICONTROL Send]** knop (of **[!UICONTROL Send as scheduled]** (als u de verzending hebt gepland) en bevestig de verzending.

1. Tijdens het verzendende proces, kunt u zijn vooruitgang volgen en statistieken in real time direct in dit scherm bekijken.

   ![](assets/sent-mail.png)

   U kunt gedetailleerde informatie over het verzenden ook toegang hebben door te klikken op **[!UICONTROL Logs]** knop. [Leer hoe u leveringslogboeken kunt controleren](../monitor/delivery-logs.md)

1. Nadat u het e-mailbericht hebt verzonden, kunt u specifieke rapporten voor verdere analyse openen door op de knop **[!UICONTROL Reporting]** knop.

![](assets/reports.png)
