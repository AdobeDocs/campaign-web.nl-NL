---
audience: end-user
product: campaign
title: Werken met inhoudssjablonen
description: Leer hoe u sjablonen maakt om inhoud opnieuw te gebruiken in e-mails van Adobe Campaign
feature: Templates
topic: Content Management
role: User
level: Beginner
exl-id: 23818080-d7c6-4829-8117-d6b359bd76dd
source-git-commit: 371bccc8371d9ff4a9b1659510953ff7776c2459
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 0%

---

# Werken met inhoudssjablonen {#content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_menu"
>title="Contentsjablonen"
>abstract="Voor een versnelde en verbeterde ontwerpprocedure kunt u zelfstandige e-mailsjablonen maken om aangepaste inhoud eenvoudig te hergebruiken in Adobe Campaign. Deze inhoudssjablonen kunnen geheel nieuw worden ontworpen, op basis van ingebouwde of aangepaste sjablonen, op basis van bestaande inhoud of geïmporteerd in de inhoudssjablooneditor."

Voor een versnelde en verbeterde ontwerpprocedure kunt u zelfstandige sjablonen maken om aangepaste inhoud eenvoudig te hergebruiken in [!DNL Adobe Campaign]. Deze inhoudssjablonen kunnen geheel nieuw worden ontworpen, op basis van ingebouwde of aangepaste sjablonen, op basis van bestaande inhoud of geïmporteerd in de inhoudssjablooneditor.

Met deze functionaliteit kunnen gebruikers die op inhoud zijn gericht, aan zelfstandige sjablonen werken, zodat marketinggebruikers deze opnieuw kunnen gebruiken en aanpassen in hun eigen e-mailcampagnes.

>[!NOTE]
>
>Alleen op dit moment **email** inhoudssjablonen worden ondersteund.

## Sjablonen voor inhoud openen {#access-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_edition"
>title="Sjablooninhoud bewerken"
>abstract="Klik op de knop **Inhoud bewerken** om uw inhoud bij te werken met de e-mailontwerper."

Blader naar de **[!UICONTROL Content Management]** > **[!UICONTROL Content Templates]** van de linkerspoorstaaf.

![](assets/content-template-list.png){zoomable=&quot;yes&quot;}

In dit dashboard worden alle beschikbare inhoudssjablonen als een lijst weergegeven. U kunt filteren op een specifieke [map](../get-started/permissions.md#folders) de vervolgkeuzelijst gebruiken of regels toevoegen met de [querymodel](../query/query-modeler-overview.md).

![](assets/content-template-list-filters.png){zoomable=&quot;yes&quot;}

In de lijst kunt u bestaande inhoudssjablonen bewerken, dupliceren of verwijderen. Gebruik de knop in de bovenste sectie om een inhoudssjabloon te maken.


## Inhoudssjablonen maken {#create-content-templates}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_design"
>title="Sjabloonontwerp voor inhoud"
>abstract="Sjabloonontwerp voor inhoud"

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_selection"
>title="Sjabloonselectie voor inhoud"
>abstract="Sjabloonselectie voor inhoud"

Inhoudssjablonen kunnen worden gemaakt door [opslaan van een bestaande e-mail als sjabloon](#save-as-template)of uit de lijst met e-mailsjablonen via de **Inhoudssjabloon maken** knop, [zoals hieronder beschreven](#create-template-from-scratch).

Nadat u de sjabloon hebt opgeslagen, kunt u deze sjabloon nu gebruiken bij het samenstellen van [email](../email/create-email.md) binnen [!DNL Adobe Campaign]. [Meer informatie](use-email-templates.md)

>[!NOTE]
>
>* Wijzigingen die zijn aangebracht in inhoudssjablonen worden niet doorgegeven aan e-mails.
>
>* En als sjablonen worden gebruikt in een e-mailbericht, hebben wijzigingen die u aanbrengt in uw e-mailinhoud geen invloed op de eerder gebruikte inhoudssjabloon.

### Een nieuwe inhoudssjabloon maken {#create-template-from-scratch}

>[!CONTEXTUALHELP]
>id="acw_contenttemplate_properties"
>title="Sjablooneigenschappen definiëren"
>abstract="De sjablooneigenschappen voor e-mailinhoud die u wilt ophalen, kunt u eenvoudig definiëren wanneer dat nodig is."

Ga als volgt te werk om een nieuwe inhoudssjabloon te maken van het dashboard voor inhoudssjablonen:

1. Bladeren naar de lijst met inhoudssjablonen in het menu **[!UICONTROL Content Management]** > **[!UICONTROL Content templates]** linker spoor.

1. Selecteer **[!UICONTROL Create template]**.

   ![](assets/content-template-create.png){zoomable=&quot;yes&quot;}

1. Voer het sjabloonlabel en de eigenschappen in. U kunt de map selecteren waarin u de sjabloon wilt opslaan. Standaard worden inhoudssjablonen opgeslagen in een speciale map in de Adobe Campaign-hiërarchie: **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Templates]** > **[!UICONTROL Content templates]**. Meer informatie over mappen in [deze pagina](../get-started/permissions.md#folders)

   ![](assets/content-template-details.png){zoomable=&quot;yes&quot;}

1. Klikken **[!UICONTROL Create]** en kies uit de verschillende opties hoe u de sjabloon wilt ontwerpen:

   * [Ontwerp uw inhoud helemaal zelf](create-email-content.md) via de interface van E-mailontwerper.

   * [Code of copy-paste onbewerkte HTML](code-content.md) rechtstreeks in de e-mailontwerper.

   * [Bestaande HTML-inhoud importeren](existing-content.md) uit een bestand of een ZIP-map.

   * Bestaande inhoud uit een lijst met ingebouwde of aangepaste sjablonen gebruiken. De stappen voor het gebruik van een inhoudssjabloon in een e-mail worden beschreven in [deze sectie](use-email-templates.md).

   ![](assets/email_designer-templates.png){zoomable=&quot;yes&quot;}

1. In het dialoogvenster E-mailontwerper wordt weergegeven. Bewerk de inhoud naar wens, net als voor alle e-mailberichten, afhankelijk van de optie die u hebt geselecteerd. Meer informatie over het gebruik van de e-mailontwerper in [deze sectie](get-started-email-designer.md).

   <!--You can test your content if needed. [Learn how](#test-template)-->

1. Als de sjabloon klaar is, klikt u op **[!UICONTROL Save]**.

   Klik zo nodig op de pijl naast de sjabloonnaam om terug te gaan naar de **[!UICONTROL Details]** het scherm en geeft uw malplaatje uit.

   ![](assets/content-template-save-back.png){zoomable=&quot;yes&quot;}

De sjabloon is beschikbaar in het dialoogvenster **[!UICONTROL Content templates]** lijst. [Meer informatie](#access-templates)

U kunt deze sjabloon nu gebruiken om een nieuwe inhoud samen te stellen: deze is beschikbaar in het dialoogvenster **[!UICONTROL Saved templates]** tabblad van e-mailontwerper. [Meer informatie](use-email-templates.md)

### E-mailinhoud opslaan als sjabloon {#save-as-template}

Eenmaal [ontworpen als e-mail](create-email-content.md)kunt u deze inhoud opslaan als een sjabloon voor toekomstig hergebruik. Opgeslagen sjablonen zijn beschikbaar voor alle gebruikers van uw Adobe Campaign-omgeving.

Voer de onderstaande stappen uit om e-mailinhoud als sjabloon op te slaan:

1. Klik vanuit de e-mailontwerper op de knop **[!UICONTROL More]** op de rechterbovenhoek van het scherm.

1. Selecteren **[!UICONTROL Save as content template]** in het keuzemenu.

   ![](assets/email_designer-save-template.png){zoomable=&quot;yes&quot;}

1. Voer een naam in voor deze sjabloon en sla deze op.

   ![](assets/email_designer-template-name.png){zoomable=&quot;yes&quot;}

De sjabloon wordt opgeslagen en weergegeven in het dialoogvenster **[!UICONTROL Content templates]** lijst. Het wordt een standalone inhoudsmalplaatje dat kan worden betreden, worden uitgegeven en worden geschrapt zoals om het even welk ander punt op die lijst. [Meer informatie](#access-manage-templates)

U kunt deze sjabloon nu gebruiken om een nieuwe inhoud samen te stellen: deze is beschikbaar in het dialoogvenster **[!UICONTROL Saved templates]** tabblad van e-mailontwerper. [Meer informatie](use-email-templates.md)

![](assets/email_designer-saved-template.png){zoomable=&quot;yes&quot;}


>[!NOTE]
>
>Om het even welke verandering in dat nieuwe malplaatje wordt niet verspreid aan e-mail het uit komt. Op dezelfde manier wordt de nieuwe sjabloon niet gewijzigd wanneer de oorspronkelijke inhoud in die e-mail wordt bewerkt.

<!--

Test your content template {#test-template}

You can test the rendering of any email content template, whether created from scratch or from an email. To do so, follow the steps below.

1. Access the content template list.

1. Click **[!UICONTROL Edit content]** from the **[!UICONTROL Template properties]**.

1. Click **[!UICONTROL Simulate Content]** and select a test profile to check your email rendering. You can choose the desktop or mobile view.

1. You can send a proof to test your content and have it approved by some internal users before using it. To do so, click the **[!UICONTROL Send proof]** button and follow the steps described in .

-->


## Een inhoudssjabloon wijzigen {#modify-delete}

Voer de volgende stappen uit om een bestaande inhoudssjabloon bij te werken:

1. Klik in de lijst met inhoudssjablonen op het label van de sjabloon die u wilt wijzigen om deze te bewerken.

1. Klik op de knop **[!UICONTROL Edit content]** om uw inhoud bij te werken met de [E-mailDesigner](get-started-email-designer.md).

![](assets/content-template-edition.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>Wijzigingen die zijn aangebracht in inhoudssjablonen, worden niet doorgegeven aan e-mails met deze inhoudssjabloon.

## Een inhoudssjabloon verwijderen {#content-delete}

U kunt een inhoudssjabloon op twee manieren verwijderen:

* in de lijst met inhoudssjablonen klikt u op de knop voor ovaal en selecteert u **Verwijderen**

  ![Een inhoudssjabloon verwijderen uit het dashboard](assets/content-template-list-delete.png)

* in de inhoudssjabloon zelf klikt u op de knop **Meer** dan selecteert u **Verwijderen**


>[!NOTE]
>
>Het verwijderen van een inhoudssjabloon heeft geen invloed op leveringen die zijn gemaakt met deze sjabloon.


## Een inhoudssjabloon dupliceren {#content-duplicate}

U kunt een inhoudssjabloon op twee manieren dupliceren:

* in de lijst met inhoudssjablonen klikt u op de knop voor ovaal en selecteert u **Dupliceren**

* in de inhoudssjabloon zelf klikt u op de knop **Meer** dan selecteert u **Dupliceren**

In beide gevallen bevestigt u de duplicatie om de nieuwe inhoudssjabloon te maken. Het label van de nieuwe inhoudssjabloon is **Kopie van`<label of the initial campaign`**. Blader naar de sjablooninstellingen om dit label bij te werken.

