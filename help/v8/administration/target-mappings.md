---
title: Doeltoewijzingen beheren
description: Leer hoe u doeltoewijzingen beheert.
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Doeltoewijzingen beheren {#target-mappings}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Doeltoewijzingen"
>abstract="U kunt doeltoewijzingen in het Gebruikersinterface van het Web van de Campagne nu tot stand brengen. Doeltoewijzingen bepalen hoe verschillende leveringskanalen (e-mail, SMS, pushmeldingen) worden gekoppeld aan de gegevensvelden van een schema."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_list"
>title="Doeltoewijzingen "
>abstract="Doeltoewijzingen"

## Over doeltoewijzingen {#about}

Elk communicatiekanaal gebruikt een standaarddoelafbeelding om hun ontvangers te richten. Sjablonen voor e-mail- en SMS-verzending zijn standaard bijvoorbeeld gericht op **[!UICONTROL Recipients]** . Hun doelafbeelding gebruikt daarom de gebieden van **nms:ontvankelijke** lijst. Voor de Duw berichten, is de standaarddoelafbeelding **toepassingen van de Abonnee (nms:appSubscriptionRcp)**, die met de lijst van ontvangers verbonden is.

Doeltoewijzingen zijn toegankelijk via het menu **[!UICONTROL Administration]** > **[!UICONTROL Target mappings]** . Vanuit dit scherm hebt u toegang tot details over elke doeltoewijzing of kunt u nieuwe doeltoewijzingen maken die aan uw behoeften voldoen.

![](assets/target-mappings-list.png)

Voor meer informatie over de ingebouwde doelafbeeldingen die van Adobe Campaign worden verstrekt, verwijs naar de [ de consoledocumentatie van de Cliënt van de Campagne v8 ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html) {target="_blank"}.

## Doeltoewijzing maken {#create-mapping}

>[!CONTEXTUALHELP]
>id="acw_targetmapping_properties"
>title="Eigenschappen voor doeltoewijzing"
>abstract="In de sectie **[!UICONTROL Properties]** kunt u algemene instellingen definiëren voor de doeltoewijzing en de doelpopulatie."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_mapping"
>title="Toewijzing doel"
>abstract="In de sectie **[!UICONTROL Mapping]** kunt u aangeven welke kenmerken van het schema van de doeltoewijzing moeten worden gebruikt voor de verschillende velden voor het bezorgadres."

>[!CONTEXTUALHELP]
>id="acw_targetmapping_denylist"
>title="Lijst van gewezen personen voor doeltoewijzing"
>abstract="Lijst van gewezen personen voor doeltoewijzing"

>[!CONTEXTUALHELP]
>id="acw_targetmapping_storage"
>title="Opslag doeltoewijzing"
>abstract="In de sectie **[!UICONTROL Storage]** kunt u aangeven waar logbestanden moeten worden opgeslagen."

Open het menu **[!UICONTROL Administration]** > **[!UICONTROL Target mappings]** om een nieuwe doeltoewijzing te maken. Klik op de knop **[!UICONTROL Create mapping]** en volg de stappen die in de onderstaande secties worden beschreven.

1. Voer in de sectie **[!UICONTROL Properties]** een **[!UICONTROL Label]** in voor de doeltoewijzing.

1. Vouw de sectie **[!UICONTROL Additional options]** uit om geavanceerde instellingen te definiëren, zoals de interne naam, opslagmap en beschrijving van de doeltoewijzing.

1. Selecteer de doelpopulatie. U kunt:

   * **[!UICONTROL Use the targeting dimension directly]**: selecteer de dimensie die u rechtstreeks wilt gebruiken in de lijst met beschikbare afmetingen.
   * **[!UICONTROL Use linked data]**: met deze optie kunt u beginnen met een doeldimensie (bijvoorbeeld abonnementen) en vervolgens overschakelen op de doeldimensie die u wilt gebruiken (bijvoorbeeld ontvangers).

   ![](assets/target-mappings-properties.png)

1. Als de geselecteerde afmeting niet reeds door een bestaande doelafbeelding wordt gebruikt, moeten de schema&#39;s om de logboeken op te slaan worden gecreeerd. Hiervoor zijn aanvullende opties beschikbaar in de sectie **[!UICONTROL Storage]** . Vouw de onderstaande sectie uit voor meer informatie.

   +++Opslagopties voor nieuwe doeldimensies

   1. **[!UICONTROL Namespace]**: identificeer de naamruimte die wordt gebruikt om de logbestanden te maken.
   1. **[!UICONTROL Suffix of the extension schema]** - Geef een achtervoegsel op voor het nieuwe schema.

      In het onderstaande voorbeeld is de naam van de broadlog &#39;cusbroadlogSupplier&#39;.

      ![](assets/target-mappings-new.png)

   1. **[!UICONTROL Delivery logs]**: activeer de opties in deze sectie om de verzendende logboeken te verrijken met een gebied van de segmentcode of met een gebied dat het bezorgingsIP adres bevat. U kunt bijvoorbeeld een segmentcode die tijdens de workflow is berekend, opslaan in de verzendende logboeken om het doel later te verfijnen. Hierdoor kunt u profielen met deze specifieke segmentcode als doel instellen.

   1. **[!UICONTROL Exclusions]**: geef op hoe u de uitsluitingslogboeken wilt opslaan.

   1. **[!UICONTROL Tracking logs]**: activeer de optie **[!UICONTROL Generate a schema for tracking]** om een opslagschema te genereren voor het bijhouden van logbestanden

+++

1. Gebruik de sectie **[!UICONTROL Mapping]** om te identificeren welke kenmerken van het schema van de doelafbeelding moeten worden gebruikt voor elke veld van het bezorgadres. Selecteer voor elk veld het kenmerk dat u wilt toewijzen. U kunt ook een expressie maken om het veld te identificeren. U kunt bijvoorbeeld een lagere functie toepassen op het adreskenmerk.

   ![](assets/target-mappings-mapping.png)

1. Klik op de knop **[!UICONTROL Create]** wanneer de doeltoewijzing gereed is. De systemen leiden automatisch tot de doelafbeelding en alle verwante schema&#39;s voor de logboeken.

Nadat u de doeltoewijzing hebt gemaakt, worden twee extra secties op het scherm weergegeven:

* **[!UICONTROL Denylisting]**: In deze sectie kunt u de kenmerken van het schema van de doeltoewijzing identificeren die voor lijsten van gewezen personen moeten worden gebruikt.

  ![](assets/target-mappings-denylisting.png)

* **[!UICONTROL Storage]**: in deze sectie kunt u de tabellen identificeren die u wilt gebruiken voor het opslaan van logbestanden.

  ![](assets/target-mappings-storage.png)

   * **[!UICONTROL Message schema]**: identificeert het schema dat moet worden gebruikt om de verzendende logboeken op te slaan.
   * **[!UICONTROL Messages excluded]**: in deze sectie wordt aangegeven hoe u opslag van bezorgings- en uitsluitingslogbestanden beheert.

      * **[!UICONTROL Store exclusions and messages in the same table]**
      * **[!UICONTROL Store messages only]**: geen uitsluitingen opslaan.
      * **[!UICONTROL Store exclusions and messages in separate tables]**: selecteer het schema dat u wilt gebruiken om uitsluitingslogboeken op te slaan in het **[!UICONTROL Rejection schema]** -veld.

   * **[!UICONTROL Tracking logs]**: Kies waar u trackinglogboeken en de standaardverkeersbron wilt opslaan.
   * **[!UICONTROL Additional fields]**: in deze sectie kunt u een lijst opgeven met extra velden die worden opgeslagen in de leveringslogboeken. In deze velden kunnen gegevens permanent worden opgeslagen over afzonderlijke leden van het doel (bijvoorbeeld `recipient/@firstName`) of aanvullende gegevens opslaan die tijdens de workflow zijn berekend (bijv. `[targetData/@offeCode]`)

     Selecteer **[!UICONTROL Add field]** om dit te doen. Identificeer de informatie u in het **[!UICONTROL Source]** gebied wilt opslaan, en de attributen in het verzenden logboeken te gebruiken om deze informatie in het **[!UICONTROL Destination]** gebied te bewaren.

     ![](assets/target-mappings-additional.png){width="50%" zoomable="yes"}
