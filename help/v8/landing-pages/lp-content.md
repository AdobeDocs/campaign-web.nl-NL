---
title: Paginaspecifieke inhoud definiëren
description: Leer hoe u landende pagina-specifieke inhoud ontwerpt in Campagne Web
feature: Landing Pages
badge: label="Beperkte beschikbaarheid"
source-git-commit: 5c3f02d4c95951693ac73de4a6e8810e1b662e53
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 1%

---

# Paginaspecifieke inhoud definiëren {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Inhoudscomponenten gebruiken"
>abstract="Inhoudscomponenten zijn lege plaatsaanduidingen voor inhoud die u kunt gebruiken om de lay-out van een bestemmingspagina te maken. Gebruik de formuliercomponent om specifieke inhoud te definiëren waarmee gebruikers hun keuzes kunnen selecteren en verzenden."

Wanneer u de inhoud van een willekeurige pagina van de bestemmingspagina bewerkt, is deze al ingevuld.

De primaire pagina is de pagina die onmiddellijk aan de gebruikers wordt getoond nadat zij de verbinding aan uw landende pagina, zoals van een e-mail of een website klikken. De primaire pagina is al voorgevuld met de [paginaspecifieke formuliercomponent landen](#use-form-component) om gebruikers in staat te stellen hun keuzes te selecteren en te verzenden. U kunt ook [paginaspecifieke stijlen plaatsen](#lp-form-styles).

Voor het verder ontwerpen van de inhoud van de bestemmingspagina kunt u dezelfde componenten gebruiken als voor een e-mail. [Meer informatie](../email/content-components.md#add-content-components)

<!--
The content of the **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** and **[!UICONTROL Expiration]** pages is also pre-filled. Edit them as needed.

Set the subscription form to the appropriate fields from the database to make sure it will work correctly.

The landing page default fields are already there for the selected template.

>[!NOTE]
>
>You can also create a click-through landing page without a **[!UICONTROL Form]** component. In that case, the landing page will be displayed to users, but they will not be required to submit any form. This can be useful if you only want to showcase a landing page without requiring any action from your recipients such as opt-in or opt out, or want to provide information that doesn't require user input.

Using the landing page content designer, you can also leverage contextual data coming from the primary page in a subpage. [Learn more](#use-primary-page-context)-->

## De formuliercomponent gebruiken {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="De velden voor formuliercomponenten instellen"
>abstract="Bepaal hoe de ontvangers hun keuzes vanaf de bestemmingspagina zien en verzenden."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Wat gebeurt er als u op de knop klikt"
>abstract="Bepaal wat er gebeurt wanneer gebruikers het formulier voor de landingspagina indienen."

Als u specifieke inhoud wilt definiëren waarmee gebruikers hun keuzes vanaf de bestemmingspagina kunnen selecteren en verzenden, gebruikt u de optie **[!UICONTROL Form]** component. Volg de onderstaande stappen om dit te doen.

1. Specifieke landingspagina&#39;s **[!UICONTROL Form]** wordt al weergegeven op het canvas voor de geselecteerde sjabloon.

   >[!NOTE]
   >
   >De **[!UICONTROL Form]** kan slechts eenmaal op dezelfde pagina worden gebruikt.

1. Selecteer het. De **[!UICONTROL Form content]** wordt weergegeven in het rechterpalet, zodat u de verschillende velden van het formulier kunt bewerken.

   ![](assets/lp-form-component.png)

   >[!NOTE]
   >
   >Schakel over naar de **[!UICONTROL Styles]** kunt u op elk gewenst moment de stijlen van de inhoud van uw formuliercomponent bewerken. [Meer informatie](#lp-form-styles)

1. Vouw het eerste tekstveld uit. Van de **[!UICONTROL Text field 1]** kunt u het veldtype, het veld uit de database, het label en de tekst bewerken die in het veld worden weergegeven voordat de gebruiker het veld invult.

   ![](assets/lp-form-text-field.png)

1. Schakel indien nodig de optie **[!UICONTROL Make form field mandatory]** in. In dat geval kan de landingspagina alleen worden verzonden als de gebruiker dit veld heeft ingevuld.

   >[!NOTE]
   >
   >Als een verplicht veld niet is ingevuld, wordt een foutbericht weergegeven wanneer de gebruiker de pagina verzendt.

1. Voeg een selectievakje toe. Selecteer deze optie als u een service of een veld uit de database wilt bijwerken.

   ![](assets/lp-form-checkbox.png)

   Definieer of dit selectievakje gebruikers in- of uitschakelt. Kies een van de twee onderstaande opties:

   * **[!UICONTROL Subscribe if checked]**: Gebruikers moeten het selectievakje voor toestemming (opt-in) inschakelen.
   * **[!UICONTROL Unsubscribe if checked]**: Gebruikers moeten het selectievakje inschakelen om hun toestemming te verwijderen (opt-out).

1. U kunt zo veel tekstvelden en/of selectievakjes verwijderen en toevoegen.

1. Nadat u alle gewenste selectievakjes en/of tekstvelden hebt toegevoegd, klikt u op **[!UICONTROL Call to action]** om de bijbehorende sectie uit te vouwen. Hiermee kunt u het gedrag van de knop in het dialoogvenster **[!UICONTROL Form]** component.

   ![](assets/lp-call-to-action.png)

1. Bepaal wat er gebeurt wanneer u op de knop klikt:

   * **[!UICONTROL Confirmation page]**: De gebruiker wordt omgeleid naar de **[!UICONTROL Confirmation]** paginaset voor de huidige openingspagina.

   * **[!UICONTROL Redirect URL]**: Voer de URL in van de pagina waarnaar de gebruikers worden omgeleid.

1. Als u aanvullende updates wilt uitvoeren wanneer u het formulier verzendt, selecteert u **[!UICONTROL Addtional updates]**, kiest u **[!UICONTROL Opt in]** of **[!UICONTROL Opt out]** en definieer of u een abonnementenlijst, het kanaal of alleen het gebruikte e-mailadres wilt bijwerken.

   ![](assets/lp-form-additionnal-updates.png)

1. Sla uw inhoud op om terug te gaan naar de [eigenschappen van bestemmingspagina](create-lp.md).

## Landingspagina-formulierstijlen definiëren {#lp-form-styles}

1. Als u de stijlen van de inhoud van een formuliercomponent wilt wijzigen, schakelt u op elk gewenst moment over naar de **[!UICONTROL Style]** tab.

   ![](assets/lp_designer-form-style.png)

1. De **[!UICONTROL Fields]** wordt standaard uitgevouwen, zodat u de weergave van het tekstveld kunt bewerken, zoals het label- en plaatsaanduidingslettertype, de positie van het label, de achtergrondkleur van het veld of de veldrand.

   ![](assets/lp_designer-form-style-fields.png)

1. Breid uit **[!UICONTROL Checkboxes]** om de vormgeving van de selectievakjes en de bijbehorende tekst te definiëren. U kunt bijvoorbeeld de lettertypefamilie of -grootte of de randkleur van het selectievakje aanpassen.

   ![](assets/lp_designer-form-style-checkboxes.png)

1. Breid uit **[!UICONTROL Buttons]** om de weergave van de knop in het deelformulier te wijzigen. U kunt bijvoorbeeld het lettertype wijzigen, een rand toevoegen, de labelkleur bewerken op de muisaanwijzer of de uitlijning van de knop aanpassen.

   ![](assets/lp_designer-form-style-buttons.png)

   U kunt een voorvertoning van bepaalde instellingen, zoals de kleur van knoplabels op de muisaanwijzer, weergeven met de opdracht **[!UICONTROL Simulate content]** knop. Meer informatie over het testen van bestemmingspagina&#39;s [hier](create-lp.md#test-landing-page).

1. Breid uit **[!UICONTROL Form layout]** om de layoutinstellingen zoals de achtergrondkleur, opvulling of marge te bewerken.

   ![](assets/lp_designer-form-style-layout.png)

<!--
1. Expand the **[!UICONTROL Form error]** section to adjust the display of the error message that displays in case a problem occurs. Check the corresponding option to preview the error text on the form.

    ![](assets/lp_designer-form-error-preview.png)-->

