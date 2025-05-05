---
audience: end-user
title: De e-mailinhoud bewerken
description: Leer hoe u de e-mailinhoud bewerkt in de gebruikersinterface van het Campagne Web
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: df5883f8178bc5287145c587b06dd5664400ed90
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# E-mailinhoud configureren {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="De e-mailcontent opgeven"
>abstract="Het **geeft inhoud** scherm uit staat u toe om basiselementen van uw bericht, zoals het afzenderadres en onderwerpregel te bepalen, extra acties uit te voeren zoals toevoegend gehechtheid of aanbiedingen, en tot E-mail Designer toegang te hebben om uw bericht een gepolijst blik te geven."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="E-maileigenschappen instellen"
>abstract="De **Basisdetails** sectie staat u toe om het adres van de afzender en antwoord-aan adres bij te werken, en de onderwerpregel te bepalen gebruikend de Redacteur van de Uitdrukking."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Bestanden bijvoegen bij uw e-mail"
>abstract="Selecteer een of meerdere bestanden die u in het bericht wilt invoegen. Om prestatieproblemen te voorkomen, wordt aanbevolen niet meer dan één bijlage per e-mail op te nemen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Tekstspatiëring bewerken"
>abstract="Door gebrek, wordt het volgen toegelaten voor de levering, die betekent alle verbindingen inbegrepen in de berichtinhoud worden gevolgd. U kunt deze optie hier uitschakelen."
>additional-url="https://experienceleague.adobe.com/nl/docs/campaign-web/v8/content/email-design/design-content/message-tracking" text="Koppelingen toevoegen en berichten bijhouden"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_multilingual"
>title="Talen toevoegen"
>abstract="Op dit tabblad vindt u een lijst met talen waarin de levering wordt verzonden. U kunt meer talen toevoegen door op de knop Taal toevoegen te klikken of door een andere taal via dit tabblad te dupliceren."

Met het e-mailscherm **[!UICONTROL Edit content]** kunt u:

* Definieer de basiselementen van uw bericht, zoals het adres van de afzender en de onderwerpregel
* Extra handelingen uitvoeren, zoals bijlagen toevoegen of aanbiedingen instellen
* Heb toegang tot [ E-mail Designer ](get-started-email-designer.md#start-authoring) beginnen de juiste inhoud van uw e-mail te bouwen
* Voeg taalvarianten aan uw leveringen toe.

>[!NOTE]
>
>Alle bewerkbare tekstvelden van dit scherm kunnen worden ingevuld met verpersoonlijkingsvelden. [ Leer hoe te om inhoud ](../personalization/personalize.md) te personaliseren

## De levering configureren

Volg onderstaande stappen om de inhoud van een e-mail te configureren of te bewerken.

1. Klik de **[!UICONTROL Edit content]** knoop van het [ e-mailleveringsdashboard ](../email/create-email.md) scherm.

   ![ Schermafbeelding die de Edit inhoudsknoop op het dashboard van de e-maillevering toont.](assets/email-edit-content-button.png){zoomable="yes"}

1. Het e-mailinhoudsopgavescherm wordt geopend.

   ![ Schermafbeelding die het dashboard van de e-mailinhoudsuitgave toont.](assets/email-edit-content-dashboard.png){zoomable="yes"}

   >[!NOTE]
   >
   >Als u een nieuwe e-mail configureert, zijn de velden **[!UICONTROL From name]** en **[!UICONTROL From email]** al ingevuld.

1. Het veld **[!UICONTROL From name]** wordt gedefinieerd in de e-mailsjabloon. Als u deze wilt wijzigen, gebruikt u een naam die gemakkelijk kan worden herkend door de ontvangers, zoals de naam van uw merk, om de openingssnelheid van uw leveringen te verhogen.

   >[!NOTE]
   >
   >Als u de ervaring van de ontvanger verder wilt verbeteren, kunt u de naam van een persoon toevoegen, bijvoorbeeld &#39;Oefen van luminantie&#39;.

1. Het adresveld **[!UICONTROL From email]** wordt ook gedefinieerd in de e-mailsjabloon. Zorg ervoor dat het adresdomein overeenkomt met het subdomein dat u aan Adobe hebt gedelegeerd.

   >[!NOTE]
   >
   >U kunt het deel vóór &#39;@&#39; wijzigen, maar niet het domeinadres.

1. Vouw de sectie **[!UICONTROL Reply-to fields]** uit. De naam en het adres van de afzender worden door gebrek gebruikt voor antwoorden. Adobe raadt echter aan een bestaand reëel adres te gebruiken, zoals de klantenservice van uw merk. In dit geval, als een ontvanger een antwoord verzendt, zal het team van de klantenzorg het kunnen behandelen.

   ![ Schermafbeelding die de sectie Reageren op velden in de e-mailinhoudeditor weergeeft.](assets/email-edit-content-reply-to.png){zoomable="yes"}

1. Geef de e-mail op **[!UICONTROL Subject line]** . Typ direct uw onderwerp in het specifieke gebied, of open de Redacteur van de Uitdrukking om [ verpersoonlijking ](../personalization/personalize.md) toe te voegen gebruikend diverse attributen, uitdrukkingsfragmenten, of aanbiedingen.

1. Als u een bestand bij de e-mail wilt voegen, klikt u op de knop **[!UICONTROL Add attachment]** en selecteert u een of meer bestanden.

   >[!NOTE]
   >
   >Om prestatieproblemen te voorkomen, wordt aanbevolen niet meer dan één bijlage per e-mail op te nemen.

   <!--limitation on size + number of files?-->

1. Als u aanbiedingen met uw e-mail wilt verzenden, selecteert u deze met de knop **[!UICONTROL Set up offers]** .

   Vervolgens kunt u deze bestanden in de e-mail invoegen met behulp van personalisatievelden. [ Leer hoe te om aanbiedingen te verzenden ](../msg/offers.md)

## De tekst van de e-mail bewerken

1. Klik de **[!UICONTROL Edit email body]** knoop om de inhoud van e-mail te structureren en te ontwerpen gebruikend [ E-mail Designer ](get-started-email-designer.md#start-authoring).

   >[!NOTE]
   >
   >U kunt de muisaanwijzer ook boven de voorvertoning van de e-mail plaatsen en **[!UICONTROL Open email designer]** selecteren.


   In deze secties vindt u aanvullende informatie over het ontwerpen van e-mailinhoud:

   * [E-mails van auteur helemaal opnieuw](create-email-content.md)
   * [Stijl uw inhoud](get-started-email-style.md)

1. Standaard is het bijhouden van gegevens ingeschakeld voor levering. U kunt deze optie uitschakelen in de sectie **[!UICONTROL Optional features]** . [ Leer hoe te om verbindingen toe te voegen en het volgen te beheren ](message-tracking.md)

1. Nadat de inhoud van uw e-mail is gedefinieerd, controleert u met de knop **[!UICONTROL Simulate content]** hoe het bericht wordt weergegeven voordat u het verzendt. [ Leer hoe te om uw e-mail ](../preview-test/preview-test.md) voor te vertonen en te testen.

## Een meertalige levering configureren

In de webgebruikersinterface van Campagne kunt u uw e-mailleveringen instellen als meertalig, zodat u berichten kunt verzenden op basis van de voorkeurstaal van een profiel. Wanneer geen voorkeur wordt bepaald, wordt het bericht verzonden in de standaardtaal.

Bij een meertalige aflevering is het taalbeheer gebaseerd op varianten. Elke variant vertegenwoordigt één taal.

Tijdens de levering creeert, kunt u het aantal varianten toevoegen die aan het aantal nodig talen in het bericht beantwoorden. U kunt ook de standaardtaal definiëren wanneer u nieuwe talen toevoegt.

### Een taalvariant toevoegen

Ga als volgt te werk om taalvarianten te maken:

1. Klik op de knop **[!UICONTROL Add language]** in de bovenste sectie van het configuratiescherm voor e-mail.

   >[!IMPORTANT]
   >
   >De knop **[!UICONTROL Add language]** is alleen beschikbaar als de doeldimensie het schema Taal bevat. Meer over schema&#39;s en de dimensies van het Doel leren, gelieve te verwijzen naar de [ gedetailleerde documentatie ](https://experienceleague.adobe.com/nl/docs/campaign-web/v8/audiences/targeting-dimensions){target=_blank}.

   ![](assets/edit-content_2.png){zoomable="yes"}


1. Selecteer de taal die u wilt toevoegen in de vervolgkeuzelijst **[!UICONTROL Language]** . Wanneer u de eerste taal toevoegt, wordt deze als standaard ingesteld en is de huidige inhoud de standaardtaal. Wanneer u nieuwe talen toevoegt, is de inhoud gebaseerd op de standaardinhoud.

   >[!NOTE]
   >
   >De talen die beschikbaar zijn via deze lijst, zijn afhankelijk van de waarden die zijn gedefinieerd door het taalkenmerk (waarden zoals systeem, gebruiker, dbenum, enz.) Leer meer over opsommingsbeheer in deze [ sectie ](https://experienceleague.adobe.com/nl/docs/campaign-web/v8/conf/enumerations){target=_blank}.


   ![](assets/edit-content_3.png){zoomable="yes"}

   Bijvoorbeeld hier, voor het Engels (VS):

   ![](assets/edit-content_8.png){zoomable="yes"}


1. Herhaal dit proces om andere talen toe te voegen. In het deelvenster **[!UICONTROL Language]** wordt de lijst met gekozen talen, het aantal verschillende talen en ook de standaardtaal weergegeven.

   Als u bijvoorbeeld Engels, Frans en Zweeds hebt gekozen, kunt u deze drie talen zien, zoals hieronder wordt getoond:

   ![](assets/edit-content_9.png){zoomable="yes"}

   U kunt op de uitvouwknop naar de rechterbovenhoek klikken om elke taal te verwijderen.

### De e-mailinhoud voor elke variant definiëren

Als de talen eenmaal zijn ingesteld, definieert u de inhoud van de e-mail die naar de profielen wordt verzonden met deze voorkeurstaal.

Voer de volgende stappen uit om een e-mailinhoud te definiëren:

1. Open [ E-mail Designer ](get-started-email-designer.md#start-authoring) door op de **[!UICONTROL Edit email body]** knoop te klikken.

   >[!NOTE]
   >
   >U kunt de muisaanwijzer ook boven de voorvertoning van de e-mail plaatsen en **[!UICONTROL Open email designer]** selecteren.

   ![](assets/edit-content_11.png){zoomable="yes"}


1. U kunt een voorvertoning van de levering weergeven door op de knop **[!UICONTROL Simulate content]** te klikken en het profiel en de taal te kiezen waarin de e-mail wordt weergegeven.

1. In het venster Inhoud simuleren kunt u van profiel wisselen om een voorvertoning weer te geven van de inhoud van de e-mail die overeenkomt met de taal die voor dat profiel is ingesteld.

   ![](assets/edit-content_5.png){zoomable="yes"}

### Taalvarianten dupliceren of verwijderen

U kunt op de uitvouwknop in de rechterbovenhoek klikken en op de knop **[!UICONTROL Delete all variants]** klikken om alle talen te verwijderen.

![](assets/edit-content_13.png){zoomable="yes"}

Als u een taalvariant wilt verwijderen, klikt u op de drie stippen aan de rechterkant van het tabblad en selecteert u Verwijderen.

Als u een taalvariant wilt dupliceren, klikt u op de drie stippen aan de rechterkant van het tabblad en selecteert u Dupliceren. Als u een andere taal dan de standaardtaal wilt dupliceren, wordt de gedupliceerde inhoud gebaseerd op de taal die u hebt gedupliceerd.


1. Nadat de inhoud van uw e-mail is gedefinieerd, controleert u met de knop **[!UICONTROL Simulate content]** hoe het bericht wordt weergegeven voordat u het verzendt. [ Leer hoe te om uw e-mail ](../preview-test/preview-test.md) voor te vertonen en te testen.