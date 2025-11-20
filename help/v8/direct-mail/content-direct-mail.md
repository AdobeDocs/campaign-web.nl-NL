---
audience: end-user
title: Direct maillevering ontwerpen
description: Leer hoe u direct-maillevering ontwerpt met Adobe Campaign Web
exl-id: aefba651-4125-4b1e-992f-1fe90fd95e4c
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 1%

---

# Het extractiebestand ontwerpen {#design-direct-mail}

>[!CONTEXTUALHELP]
>id="acw_directmail_content"
>title="Inhoud uitpakken"
>abstract="Klik **uitgeven inhoud** knoop om te beginnen het extractiedossier te ontwerpen dat door uw directe postleverancier wordt vereist. Op deze manier kunt u de bestandseigenschappen definiëren, zoals het label en de indeling, en de kolommen opgeven die u in het bestand wilt opnemen."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_file"
>title="Bestandseigenschappen"
>abstract="Configureer de eigenschappen van het extractiebestand, zoals de naam en indeling. U kunt de bestandsnaam personaliseren met kenmerken uit de database met behulp van de expressie-editor."

>[!CONTEXTUALHELP]
>id="acw_directmail_properties_content"
>title="Inhoud"
>abstract="Geef in deze sectie de kolommen op die u wilt weergeven in het extractiebestand. Zodra gedaan, kunt u voorproef het extractiedossier gebruiken **inhoud** knoop simuleren."

Als u de inhoud wilt ontwerpen van het extractiebestand dat wordt gegenereerd door de directe verzending via e-mail, klikt u op de knop **[!UICONTROL Edit content]** op de leveringspagina en configureert u vervolgens de bestandseigenschappen en -inhoud.

## De eigenschappen van het extractiebestand configureren {#properties}

1. Geef in het veld **[!UICONTROL File name]** de gewenste naam op voor het extractiebestand. U kunt de bestandsnaam aanpassen met kenmerken uit de database. Klik hiertoe op het pictogram **[!UICONTROL Open personalization dialog]** om de expressie-editor te openen. [&#x200B; Leer hoe te om uw inhoud te personaliseren &#x200B;](../personalization/personalize.md)

1. Op het **[!UICONTROL File format]** gebied, kies het gewenste formaat voor het extractiedossier: **Tekst**, **Tekst gebruikend kolommen met vaste breedte**, **CSV (Excel)**, of **XML**.

1. Vouw de sectie **[!UICONTROL Extraction format]** uit om toegang te krijgen tot specifieke opties met betrekking tot de indeling van het extractiebestand. Welke waarden beschikbaar zijn, is afhankelijk van de geselecteerde indeling.

   +++ Beschikbare opties voor de indeling voor uitnemen

   * **[!UICONTROL Use first line as column header]** (Tekst / CSV (Excel) formaat): knevel deze optie aan om de eerste kolom als kopbal te gebruiken.
   * **[!UICONTROL Column separator]** (Tekstopmaak): geef het teken op dat u als kolomscheidingsteken wilt gebruiken in het extractiebestand.
   * **[!UICONTROL String delimiter]** (Tekstopmaak): geef op hoe tekenreeksen in het extractiebestand moeten worden gescheiden.
   * **[!UICONTROL End of line]** (Tekstopmaak): geef op hoe het einde van regels in het extractiebestand moet worden afgebakend.
   * **[!UICONTROL Encoding]**: kies de codering van het extractiebestand.
   * **[!UICONTROL Date format and separators]**: geef op hoe datums moeten worden opgemaakt in het extractiebestand.
   * **[!UICONTROL Number format]**: geef op hoe getallen moeten worden opgemaakt in het extractiebestand.
   * **[!UICONTROL Export labels instead of internal values of enumerations]**: Schakel deze optie in als u opsommingswaarden exporteert en de kolomlabels wilt ophalen. Deze zijn eenvoudiger te begrijpen en geen interne id&#39;s.

   +++

1. Schakel de optie **[!UICONTROL Requested quantity]** in of uit om het aantal ontvangers voor de levering te beperken.

   ![&#x200B; het Schermafbeelding die de configuratieopties van inhoudsdetails voor het extractiedossier toont.](assets/dm-content-details.png){zoomable="yes"}

## Kolommen van het extractiebestand configureren {#content}

Geef in de sectie **[!UICONTROL Content]** de kolommen op die u wilt weergeven in het extractiebestand. Ga als volgt te werk om dit te doen:

1. Klik op **[!UICONTROL Add Attribute]** om een nieuwe kolom te maken.
1. Kies het kenmerk dat u in de kolom wilt weergeven en bevestig het vervolgens. U kunt de expressie-editor gebruiken om het kenmerk te selecteren door op de knop **[!UICONTROL Edit expression]** te klikken. [&#x200B; leer hoe te om attributen te selecteren en hen toe te voegen aan favorieten &#x200B;](../get-started/attributes.md)

   ![&#x200B; Schermschot die de Add knoop van Attributen en opties tonen om attributen aan het extractiedossier toe te voegen.](assets/dm-add-attribute.png)

1. Nadat de kolom is toegevoegd, kunt u het label wijzigen en het bijbehorende kenmerk wijzigen met het bewerkingspictogram.
1. Herhaal deze stappen om zoveel kolommen toe te voegen als u nodig hebt voor het extractiebestand.
1. Als u het extractiebestand met een van de kolommen wilt sorteren, klikt u op het pictogram in de kolom **[!UICONTROL Sorting]** en selecteert u de gewenste sorteermethode.
1. Gebruik de pijlen omhoog en omlaag om de positie van een kolom te wijzigen.

![&#x200B; Screenshot die de opties van de attributenconfiguratie voor het extractiedossier toont.](assets/dm-content-attributes.png)

U kunt nu een voorbeeld van het extractiebestand bekijken en de levering verzenden om het extractiebestand te genereren. [&#x200B; Leer hoe te om direct-mailberichten te testen en te verzenden &#x200B;](send-direct-mail.md)