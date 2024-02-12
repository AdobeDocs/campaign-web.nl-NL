---
audience: end-user
title: De e-mailinhoud bewerken
description: Leer hoe u de e-mailinhoud bewerkt in de gebruikersinterface van het Campagne Web
exl-id: b6316551-bebc-40e0-b75c-4408ce4d6c57
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# E-mailinhoud configureren {#edit-content}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="De e-mailcontent opgeven"
>abstract="De **Inhoud bewerken** in het scherm kunt u basiselementen van uw bericht definiëren, zoals het adres van de afzender en de onderwerpregel, aanvullende handelingen uitvoeren, zoals het toevoegen van bijlagen of aanbiedingen, en de e-mailontwerper openen om uw bericht een gepolijst uiterlijk te geven."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_header"
>title="E-maileigenschappen instellen"
>abstract="De **Basisdetails** kunt u het adres en het antwoord van de afzender bijwerken en de onderwerpregel definiëren met de Expressieeditor."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_attachment"
>title="Bestanden bijvoegen bij uw e-mail"
>abstract="Selecteer een of meerdere bestanden die u in uw bericht wilt invoegen. Om prestatieproblemen te voorkomen, wordt aanbevolen niet meer dan één bijlage per e-mail op te nemen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_options"
>title="Tekstspatiëring bewerken"
>abstract="Door gebrek, wordt het volgen toegelaten voor de levering, die betekent alle verbindingen inbegrepen in de berichtinhoud worden gevolgd. U kunt deze optie hier uitschakelen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/msg/email/content/design-content/message-tracking.html" text="Koppelingen toevoegen en berichten bijhouden"

De e-mail **[!UICONTROL Edit content]** scherm kunt u:

* Definieer de basiselementen van uw bericht, zoals het adres van de afzender en de onderwerpregel
* Extra handelingen uitvoeren, zoals bijlagen toevoegen of aanbiedingen instellen
* Toegang krijgen tot de [E-mailDesigner](get-started-email-designer.md#start-authoring) om de juiste inhoud van uw e-mail te gaan samenstellen

>[!NOTE]
>
>Alle bewerkbare tekstvelden van dit scherm kunnen worden ingevuld met verpersoonlijkingsvelden. [Leer hoe u inhoud kunt aanpassen](../personalization/personalize.md)

Volg onderstaande stappen om de inhoud van een e-mail te configureren of te bewerken.

1. Klik op de knop **[!UICONTROL Edit content]** van de knop [dashboard voor e-maillevering](../email/create-email.md) scherm.

   ![](assets/email-edit-content-button.png){zoomable=&quot;yes&quot;}

1. Het e-mailinhoudsopgavescherm wordt geopend.

   ![](assets/email-edit-content-dashboard.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Als u een nieuwe e-mail configureert, **[!UICONTROL From name]** en **[!UICONTROL From email]** velden zijn al ingevuld.

1. De **[!UICONTROL From name]** wordt gedefinieerd in de e-mailsjabloon. Als u deze wilt wijzigen, gebruikt u een naam die gemakkelijk kan worden herkend door de ontvangers, zoals de naam van uw merk, om de openingssnelheid van uw leveringen te verhogen.

   >[!NOTE]
   >
   >Als u de ervaring van de ontvanger verder wilt verbeteren, kunt u de naam van een persoon toevoegen, bijvoorbeeld &quot;Oefen van luminantie&quot;.

1. De **[!UICONTROL From email]** Het adresveld wordt ook gedefinieerd in de e-mailsjabloon. Zorg ervoor het adresdomein het zelfde als subdomein is dat u aan Adobe delegeerde.

   >[!NOTE]
   >
   >U kunt het deel vóór &#39;@&#39; wijzigen, maar niet het domeinadres.

1. Breid uit **[!UICONTROL Reply-to fields]** sectie. De naam en het adres van de afzender worden door gebrek gebruikt voor antwoorden. Adobe raadt echter aan een bestaand reëel adres te gebruiken, zoals de klantenservice van uw merk. In dit geval, als een ontvanger een antwoord verzendt, zal de klantenzorg het kunnen behandelen.

   ![](assets/email-edit-content-reply-to.png){zoomable=&quot;yes&quot;}

1. De e-mail definiëren **[!UICONTROL Subject line]**. Typ het onderwerp rechtstreeks in het desbetreffende veld of open de Expressieeditor om het toe te voegen [personalisatie](../personalization/personalize.md) het gebruiken van diverse attributen en inhoudsblokken, of aanbiedingen.

1. Als u een bestand bij de e-mail wilt voegen, klikt u op de knop **[!UICONTROL Add attachment]** Selecteer vervolgens een of meerdere bestanden.

   >[!NOTE]
   >
   >    Om prestatieproblemen te voorkomen, wordt aanbevolen niet meer dan één bijlage per e-mail op te nemen.

   <!--limitation on size + number of files?-->

1. Als u aanbiedingen met uw e-mail wilt verzenden, selecteert u deze met de **[!UICONTROL Set up offers]** knop.

   U kunt ze vervolgens in de e-mail invoegen met behulp van personalisatievelden. [Meer informatie over het verzenden van voorstellen](../msg/offers.md)

1. Klik op de knop **[!UICONTROL Edit email body]** om de inhoud van de e-mail te structureren en te ontwerpen met de [E-mailDesigner](get-started-email-designer.md#start-authoring). In deze secties vindt u aanvullende informatie over het ontwerpen van e-mailinhoud:

   * [E-mails van auteur helemaal opnieuw](create-email-content.md)
   * [Stijl uw inhoud](get-started-email-style.md)

   >[!NOTE]
   >
   >U kunt de muisaanwijzer ook boven de e-mailvoorvertoning plaatsen en **[!UICONTROL Open email designer]**.

1. Standaard is het bijhouden van gegevens ingeschakeld voor levering. U kunt deze optie uitschakelen in het dialoogvenster **[!UICONTROL Optional features]** sectie. [Leer hoe u koppelingen kunt toevoegen en bijhouden](message-tracking.md)

1. Als de inhoud van uw e-mail eenmaal is gedefinieerd, gebruikt u de opdracht **[!UICONTROL Simulate content]** om te controleren hoe het toont alvorens het te verzenden. [Leer hoe u een voorbeeld van uw e-mail kunt bekijken en deze kunt testen](../preview-test/preview-test.md)

