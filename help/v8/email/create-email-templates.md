---
audience: end-user
product: campaign
title: Werken met inhoudssjablonen
description: Leer hoe u sjablonen maakt om inhoud opnieuw te gebruiken in e-mails van Adobe Campaign
feature: Templates
topic: Content Management
role: User
level: Beginner
badge: label="Beperkte beschikbaarheid"
source-git-commit: 5ad8e402c330b192b00b8be36cb3e29403666c9e
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Werken met inhoudssjablonen {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Uw eigen inhoud definiëren"
>abstract="Maak een volledig zelfstandig aangepaste sjabloon, zodat uw inhoud in meerdere e-mails opnieuw kan worden gebruikt."

Voor een versnelde en verbeterde ontwerpprocedure kunt u zelfstandige sjablonen maken om aangepaste inhoud eenvoudig te hergebruiken in [!DNL Adobe Campaign].

Met deze functionaliteit kunnen gebruikers die op inhoud zijn gericht, aan zelfstandige sjablonen werken, zodat marketinggebruikers deze opnieuw kunnen gebruiken en aanpassen in hun eigen e-mailcampagnes.

>[!NOTE]
>
>Alleen op dit moment **email** inhoudssjablonen worden ondersteund.

## Sjablonen openen en beheren {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Sjablooninhoud bewerken"
>abstract="Klik op de knop **Inhoud bewerken** om uw inhoud bij te werken met de e-mailontwerper."

Als u de lijst met inhoudssjablonen wilt openen, selecteert u **[!UICONTROL Content Management]** > **[!UICONTROL Content Templates]** in het linkermenu.

![](assets/content-template-list.png)

Alle sjablonen die zijn gemaakt - hetzij op basis van een e-mail met de [Opslaan als sjabloon](#save-as-template) van de **[!UICONTROL Content Templates]** menu - worden weergegeven.

<!--You can sort content templates by creation or modification date. You can also choose to display only the items that you created or modified.-->

U kunt filteren op een specifieke [map](../get-started/permissions.md#folders) de vervolgkeuzelijst gebruiken of regels toevoegen met de [querymodel](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png)

Als u sjablooninhoud wilt bewerken, klikt u op het gewenste item in de lijst. U kunt:

* Bewerk de eigenschappen ervan.

* Klik op de knop **[!UICONTROL Edit content]** om uw inhoud bij te werken met de [E-mailDesigner](get-started-email-designer.md).

![](assets/content-template-edition.png)

Als u een sjabloon wilt verwijderen, selecteert u de bijbehorende optie in het menu **[!UICONTROL More actions]** -menu.

![](assets/content-template-list-delete.png)

>[!NOTE]
>
>Wanneer een sjabloon wordt verwijderd, worden leveringen die met deze sjabloon zijn gemaakt, niet beïnvloed.

## Inhoudssjablonen maken {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Sjabloonontwerp voor inhoud"
>abstract="Sjabloonontwerp voor inhoud"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Sjabloonselectie voor inhoud"
>abstract="Sjabloonselectie voor inhoud"

U kunt inhoudssjablonen op twee manieren maken:

* Een geheel nieuw inhoudssjabloon maken met de linkerrails **[!UICONTROL Content templates]** -menu. [Meer informatie](#create-template-from-scratch)

* Sla uw e-mailinhoud op als sjabloon wanneer u een e-mailbericht ontwerpt. [Meer informatie](#save-as-template)

Nadat u de sjabloon hebt opgeslagen, kunt u deze sjabloon nu gebruiken wanneer u een bestand maakt dat op basis van een blanco formulier of een vorige e-mail is gemaakt. [email](../email/create-email.md) binnen [!DNL Adobe Campaign]. [Meer informatie](use-email-templates.md)

>[!NOTE]
>
>* Wijzigingen die zijn aangebracht in inhoudssjablonen worden niet doorgegeven aan e-mails.
>
>* En als sjablonen worden gebruikt in een e-mailbericht, hebben wijzigingen die u aanbrengt in uw e-mailinhoud geen invloed op de eerder gebruikte inhoudssjabloon.

### Een geheel nieuwe sjabloon maken {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Sjablooneigenschappen definiëren"
>abstract="Wanneer u een geheel nieuwe sjabloon maakt, definieert u de eigenschappen die u wilt ophalen eenvoudig wanneer dat nodig is."

Voer de onderstaande stappen uit om een volledig nieuwe inhoudssjabloon te maken.

1. Open de lijst met inhoudssjablonen via **[!UICONTROL Content Management]** > **[!UICONTROL Content templates]** links.

1. Selecteer **[!UICONTROL Create template]**.

   ![](assets/content-template-create.png)

1. Vul de sjabloondetails in. U kunt de map selecteren waarin u de sjabloon wilt opslaan. Standaard worden inhoudssjablonen opgeslagen in een speciaal knooppunt van de Adobe Campaign-hiërarchie: **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Templates]** > **[!UICONTROL Content templates]**. [Leer hoe u mappen maakt](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png)

   >[!NOTE]
   >
   >Momenteel alleen de **E-mail** kanaal en **HTML** type worden ondersteund.

1. Klikken **[!UICONTROL Create]** en kies uit de verschillende opties hoe u de sjabloon wilt ontwerpen:

   * [Ontwerp uw e-mail helemaal zelf](create-email-content.md) via de interface van E-mailontwerper.

   * [Code of copy-paste onbewerkte HTML](code-content.md) rechtstreeks in de e-mailontwerper.

   * [Bestaande HTML-inhoud importeren](existing-content.md) uit een bestand of een ZIP-map.

   * Bestaande inhoud uit een lijst met ingebouwde of aangepaste sjablonen gebruiken. De stappen voor het gebruik van een inhoudssjabloon in een e-mail worden beschreven in [deze sectie](use-email-templates.md).

   ![](assets/email_designer-templates.png)

1. De [E-mailDesigner](get-started-email-designer.md) worden weergegeven. Bewerk de inhoud naar wens, net als voor alle e-mailberichten, afhankelijk van de optie die u hebt geselecteerd.

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Als de sjabloon klaar is, klikt u op **[!UICONTROL Save]**.

   Klik zo nodig op de pijl naast de sjabloonnaam om terug te gaan naar de **[!UICONTROL Details]** het scherm en geeft uw malplaatje uit.

   ![](assets/content-template-save-back.png)

Deze sjabloon kan nu worden gebruikt wanneer u e-mailberichten maakt binnen [!DNL Adobe Campaign]. [Meer informatie](use-email-templates.md)

### E-mailinhoud opslaan als sjabloon {#save-as-template}

Eenmaal [ontworpen als e-mail](create-email-content.md)kunt u deze inhoud opslaan als een sjabloon voor toekomstig hergebruik. Opgeslagen sjablonen zijn beschikbaar voor alle gebruikers van uw Adobe Campaign-omgeving.

Voer de onderstaande stappen uit om e-mailinhoud als sjabloon op te slaan:

1. Klik vanuit de e-mailontwerper op de knop **[!UICONTROL More]** op de rechterbovenhoek van het scherm.

1. Selecteren **[!UICONTROL Save as content template]** in het keuzemenu.

   ![](assets/email_designer-save-template.png)

1. Voer een naam in voor deze sjabloon en sla deze op.

   ![](assets/email_designer-template-name.png)

U kunt deze sjabloon nu gebruiken om een nieuwe inhoud samen te stellen: deze is beschikbaar in het dialoogvenster **[!UICONTROL Saved templates]** tabblad van e-mailontwerper. [Meer informatie](use-email-templates.md)

![](assets/email_designer-saved-template.png)

De sjabloon wordt opgeslagen in de **[!UICONTROL Content templates]** lijst, toegankelijk via de [!DNL Adobe Campaign] speciaal menu. Het wordt een standalone inhoudsmalplaatje dat kan worden betreden, worden uitgegeven en worden geschrapt zoals om het even welk ander punt op die lijst. [Meer informatie](#access-manage-templates)

>[!NOTE]
>
>Om het even welke verandering in dat nieuwe malplaatje wordt niet verspreid aan e-mail het uit komt. Op dezelfde manier wordt de nieuwe sjabloon niet gewijzigd wanneer de oorspronkelijke inhoud in die e-mail wordt bewerkt.

<!--
Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list through the **[!UICONTROL Content Management]** > **[!UICONTROL Content Templates]** menu and select any template.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view. [Learn more](../content-management/preview-test.md)

    ![](../email/assets/content-template-stimulate.png)

1. You can send a proof to test your content and have it approved by some internal users before using it in a journey or a campaign.

    * To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in [this section](../content-management/proofs.md).
    
    * Before sending the proof, you must select the [email surface](../configuration/channel-surfaces.md) that will be used to test your content.

        ![](../email/assets/content-template-stimulate-proof-surface.png)

>[!CAUTION]
>
>Currently tracking is not supported when testing email content templates, meaning that tracking events, UTM parameters and landing page links will not be effective in the proofs that are being sent from a template. To test tracking, [use the content template](
use-email-templates.md) in an email and [send a proof](../content-management/preview-test.md#send-proofs).-->


