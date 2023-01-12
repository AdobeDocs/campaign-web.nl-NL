---
audience: end-user
title: Uw eerste e-mail maken
description: Campagne v8 Webdocumentatie
exl-id: afa3638b-3d48-4d2b-98b8-dedd4235ba9a
source-git-commit: bc58f1f9ebb5f73dbd23539ca14aa5c0be4c841d
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 1%

---

# Uw eerste e-mail verzenden {#first-email}

![](../assets/do-not-localize/badge.png)

In deze gebruiksaanwijzing wordt uitgelegd hoe u uw eerste e-mail kunt maken. We gaan de verzending van een e-mail op een specifieke datum plannen voor klanten met zilveren en gouden loyaliteit. Dit e-mailbericht wordt ontworpen met behulp van een vooraf gedefinieerde sjabloon en bevat personalisatie met behulp van profielkenmerken.

![](assets/delivery-list.png)

## E-mail maken {#create-email}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_template_selection"
>title="Een e-mailsjabloon selecteren"
>abstract="Een sjabloon wordt gedefinieerd in de Adobe Campaign v8-console. Dit is een specifieke leveringsconfiguratie die vooraf bepaalde parameters zoals typologieregels, verpersoonlijking of het verpletteren van parameters bevat."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_properties"
>title="E-maileigenschappen"
>abstract="De eigenschappen zijn de gemeenschappelijke leveringsparameters die u helpen om uw levering te noemen en te classificeren. Als uw levering is gebaseerd op een uitgebreid schema dat is gedefinieerd in de Adobe Campaign v8-console, zijn er enkele specifieke **Aangepaste opties** zijn beschikbaar."

1. Een nieuwe levering maken via de **[!UICONTROL Deliveries]** -menu.

1. Selecteer **[!UICONTROL Email]** kanaal en de sjabloon die u wilt gebruiken en klik vervolgens op **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >Een sjabloon is een specifieke leveringsconfiguratie die als sjabloon is opgeslagen om opnieuw te worden gebruikt. Leveringssjablonen worden geconfigureerd door beheerders in de Adobe Campaign-console. [Meer informatie over het werken met leveringssjablonen](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/create-templates.html){target="_blank"}.

   ![](assets/channel-template.png)

1. Geef een label voor de e-mail en configureer aanvullende opties op basis van uw behoeften:

   * **[!UICONTROL Internal name]**: een unieke identificatiecode aan de levering toewijzen;
   * **[!UICONTROL Folder]**: de levering opslaan in een specifieke map,
   * **[!UICONTROL Delivery code]**: gebruik dit veld om uw leveringen te ordenen op basis van uw eigen naamgevingsconventie,
   * **[!UICONTROL Description]**: een omschrijving van de levering,
   * **[!UICONTROL Nature]**: de aard van het e-mailbericht voor classificatiedoeleinden specificeren.<!--The content of the list is defined in the delivery template selected when creating the email.-->

   >[!NOTE]
   >
   >Als u uw schema met specifieke douanevelden hebt uitgebreid, kunt u tot hen van toegang hebben **[!UICONTROL Custom options]** sectie.

   ![](assets/email-properties.png)

   Geavanceerde instellingen (typologieregel, doeltoewijzingen, enz.) zijn beschikbaar bij de knoop naast de leveringsnaam. Deze zijn vooraf gedefinieerd in de geselecteerde sjabloon wanneer u de e-mail maakt. U kunt deze desgewenst bewerken.

## E-mailinhoud maken {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Leer hoe u uw e-mailinhoud ontwerpt met de e-mailontwerper."
>abstract="Leer hoe u uw inhoud ontwerpt"

In dit geval, gaan wij e-mail ontwerpen gebruikend een vooraf bepaalde malplaatje. Gedetailleerde informatie over het configureren van e-mailinhoud is beschikbaar in [deze sectie](../content/edit-content.md).

1. Klik op de knop **[!UICONTROL Edit content]** om de inhoud van uw e-mail te maken.

   In dit scherm kunt u de e-mailinhoud configureren en ontwerpen met de e-mailontwerper.

   ![](assets/edit-content.png)

1. Geef het onderwerp van uw e-mail op en pas het aan met de Expressieeditor. [Leer hoe u uw inhoud kunt aanpassen](../personalization/personalize.md)

   ![](assets/subject-line.png)

1. Klik op de knop **[!UICONTROL Edit email body]** om de inhoud van uw e-mail te maken en te ontwerpen.

   Kies de methode die u wilt gebruiken om uw e-mailinhoud te maken. In dit voorbeeld willen we een bestaande ontwerpsjabloon gebruiken.

   ![](assets/import-html.png)

<!--1. Select the HTML or ZIP file to import then click **[!UICONTROL Next]**.

    If your folder contains assets, choose the instance and folder where they should be stored then click **[!UICONTROL Import]**. (+ link to doc on assets?)

    ![](assets/import-folder.png)-->

1. Nadat u de sjabloon hebt geselecteerd, wordt deze weergegeven in de e-mailontwerper, zodat u de sjabloon indien nodig kunt bewerken en een personalisatie kunt toevoegen.

   In dit voorbeeld willen we personalisatie toevoegen aan de titel van de e-mail. Om dit te doen, selecteer het componentenblok dan klik **[!UICONTROL Add Personalization]**.

   ![](assets/add-perso.png)

1. Als de inhoud gereed is, slaat u deze op en klikt u op de pijl om terug te keren naar het scherm voor het maken van e-mail.

   ![](assets/save-content.png)

## De doelgroep definiëren {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="De doelgroep definiëren"
>abstract="Selecteer het beste publiek voor uw marketingbericht. U kunt een bestaand publiek kiezen dat al is gedefinieerd in een Campagne v8-instantie of in Adobe Experience Platform, of u kunt een nieuw publiek maken met de regelbouwer."

In dit geval sturen we de e-mail naar een bestaand publiek. Aanvullende informatie over het werken met het publiek is beschikbaar in [deze sectie](../audience/about-audiences.md).

1. Klik op de knop **[!UICONTROL Select audience]** kiest u vervolgens een bestaand publiek dat u als doel wilt instellen.

   In dit voorbeeld willen we een bestaand publiek gebruiken dat zich richt op klanten die behoren tot het niveau van de zilveren- en goudloyaliteitspunten.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Het publiek beschikbaar in de lijst komt of van uw instantie van de Campagne V8 of van Adobe Experience Platform voort als de Bestemming/Bronintegratie op uw instantie is gevormd.
   >
   >Met de integratie Doel/Bronnen kunt u de segmenten Experience Platform naar Adobe Campaign verzenden en de bezorging en tracering van campagnes naar Adobe Experience Platform verzenden. [Leer hoe u met Campagne en Adobe Experience Platform werkt](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aep.html){target="_blank"}.

1. Nadat u het publiek hebt geselecteerd, kunt u het doel verfijnen aan de hand van extra regels.

   U kunt ook een controlegroep instellen om het gedrag van de e-mailontvangers te analyseren in vergelijking met het gedrag van profielen die niet als doelprofielen werden gebruikt. [Leer hoe u met besturingsgroepen werkt](../audience/control-group.md)

## Plan de verzending {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Plan de verzending"
>abstract="Bepaal de datum en de nauwkeurige tijd voor uw verzendend. Door de meest geschikte tijd voor uw marketingbericht te kiezen, maximaliseert u de open tarieven."

Als u het verzenden van de e-mail wilt plannen, klikt u op **[!UICONTROL Enable]** en geeft u de gewenste datum en tijd voor de verzending op.

Standaard worden de **[!UICONTROL Confirm before sending]** is ingeschakeld. Dit betekent dat u het verzenden moet bevestigen om het verzenden van de e-mail op de opgegeven datum en tijd toe te staan. Schakel deze optie uit als u het e-mailbericht op de geplande datum en tijd wilt verzenden zonder dat een bevestiging nodig is.

![](assets/schedule.png)

## E-mail voorvertonen en testen {#preview-test}

Zodra uw e-mail klaar is, kunt u een voorbeeld bekijken en testen voordat u de verzending start.

In dit geval bekijken we een voorbeeld van de e-mail en sturen we een proefdruk met behulp van bestaande profielen.

Aanvullende informatie over het bekijken en testen van e-mails is beschikbaar in [deze sectie](../preview-test/preview-test.md).

1. Klik op **[!UICONTROL Review to send]**. Een voorbeeld van uw e-mailvertoningen, samen met alle gevormde eigenschappen, publiek en programma. U kunt al deze elementen bewerken met de knop Wijzigen.

1. Klik op de knop **[!UICONTROL Simulate content]** om een voorbeeld van de e-mail te bekijken en proefdrukken te verzenden.

   ![](assets/review-email.png)

1. Selecteer in het linkergedeelte het profiel of de profielen dat u wilt gebruiken voor een voorvertoning van het e-mailbericht.

1. Op basis van het geselecteerde profiel wordt in het rechterdeelvenster een voorbeeld van het e-mailbericht weergegeven. Als u meerdere profielen hebt toegevoegd, kunt u tussen de profielen schakelen om een voorbeeld van de bijbehorende e-mail te bekijken.

   ![](assets/preview.png)

   <!-- !NOTE
    >
    >Additionally, the **[!UICONTROL Render email]** button allows you to preview the email using mutiple devices or mail providers. Learn on how to preview email rendering-->

1. Als u proefdrukken van uw e-mail wilt verzenden, klikt u op de knop **[!UICONTROL Test]** selecteert u vervolgens de profielen die de proefdruk ontvangen.

   <!--TO REPLACE WITH SUBSTITUTION PROFILE-->

   In dit voorbeeld, willen wij de proeven naar een specifiek testprofiel verzenden, dat een zaadadres is dat geen deel van het doel uitmaakt. Leer hoe u met zaadadressen werkt in [Campaign Classic v7-documentatie](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/using-seed-addresses/about-seed-addresses.html){target="_blank"}.

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >U kunt uw berichten ook testen door u voor te doen met bepaalde profielen en het proefdrukbericht naar het e-mailadres van uw keuze te sturen. [Ontdek hoe u proeven verzendt](../preview-test/preview-test.md)

1. Klikken **[!UICONTROL Send test email ]** bevestig vervolgens de verzending.

   Nadat de proefdrukken zijn verzonden, kunt u de status controleren door op de knop **[!UICONTROL View test email log]** knop.

## E-mail verzenden en controleren {#prepare-send}

Nadat u uw e-mail hebt bekeken en getest, kunt u de voorbereiding starten en verzenden.

1. Klikken **[!UICONTROL Prepare]** om de voorbereiding van het bericht te starten. [Leer hoe u een e-mail voorbereidt](../monitor/prepare-send.md)

   ![](assets/preparation.png)

1. Klik op **[!UICONTROL Send]** bevestig vervolgens de verzending.

   U kunt het verzenden in real time, samen met statistieken volgen. Daarnaast worden de **[!UICONTROL Logs]** toegang tot gedetailleerde informatie over het verzenden van e-mail. [Leer hoe u leveringslogboeken kunt controleren](../monitor/delivery-logs.md)
   ![](assets/logs.png)

1. Nadat het e-mailbericht is verzonden, hebt u toegang tot uw toegewezen [rapporten](../reporting/reports.md) voor verdere analyse.

   ![](assets/reports.png)
