---
title: Paginaspecifieke inhoud definiëren
description: Leer hoe u landende pagina-specifieke inhoud ontwerpt in Campagne Web
feature: Landing Pages
source-git-commit: 26c41105a4c04b72e0aedf05a4b3268b0e475d40
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 1%

---

# Paginaspecifieke inhoud definiëren {#lp-content}

>[!CONTEXTUALHELP]
>id="ac_lp_components"
>title="Inhoudscomponenten gebruiken"
>abstract="Inhoudscomponenten zijn lege plaatsaanduidingen voor inhoud die u kunt gebruiken om de lay-out van een bestemmingspagina te maken. Gebruik de formuliercomponent om specifieke inhoud te definiëren waarmee gebruikers hun keuzes kunnen selecteren en verzenden."

U kunt de inhoud van elke pagina van de bestemmingspagina bewerken.


De eerste pagina, die onmiddellijk aan de gebruikers wordt getoond nadat zij de verbinding aan uw landende pagina klikken, is reeds vooraf ingevuld met [paginaspecifieke formuliercomponent landen](#use-form-component) voor de geselecteerde sjabloon<!-- to enable users to select and submit their choices-->.

De inhoud van de **[!UICONTROL Confirmation]**, **[!UICONTROL Error]** en **[!UICONTROL Expiration]** pagina&#39;s worden ook vooraf ingevuld. Bewerk deze indien nodig.

U kunt ook [stijlen voor de landingspagina](#lp-form-styles).

Voor het verder ontwerpen van de inhoud van de bestemmingspagina kunt u dezelfde componenten gebruiken als voor een e-mail. [Meer informatie](../email/content-components.md#add-content-components)

## De formuliercomponent gebruiken {#use-form-component}

>[!CONTEXTUALHELP]
>id="ac_lp_formfield"
>title="De velden voor formuliercomponenten instellen"
>abstract="Bepaal hoe de ontvangers hun keuzes vanaf de bestemmingspagina zien en verzenden."

>[!CONTEXTUALHELP]
>id="acw_landingpages_calltoaction"
>title="Wat gebeurt er als u op de knop klikt"
>abstract="Bepaal wat er gebeurt wanneer gebruikers het formulier voor de landingspagina indienen."

Als u specifieke inhoud wilt definiëren waarmee gebruikers hun keuzes op de bestemmingspagina kunnen selecteren en verzenden, bewerkt u de **[!UICONTROL Form]** component. Volg de onderstaande stappen om dit te doen.

1. Specifieke landingspagina&#39;s **[!UICONTROL Form]** wordt al weergegeven op het canvas voor de geselecteerde sjabloon.

   >[!NOTE]
   >
   >De **[!UICONTROL Form]** kan slechts eenmaal op dezelfde pagina worden gebruikt.

1. Selecteer het. De **[!UICONTROL Form content]** wordt weergegeven in het rechterpalet, zodat u de verschillende velden van het formulier kunt bewerken.

   ![](assets/lp-form-component.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >Schakel over naar de **[!UICONTROL Styles]** kunt u op elk gewenst moment de stijlen van de inhoud van uw formuliercomponent bewerken. [Meer informatie](#lp-form-styles)

1. Vouw het eerste tekstveld, indien van toepassing, uit of voeg er een toe met behulp van het gereedschap **[!UICONTROL Add]** knop. Van de **[!UICONTROL Text field 1]** kunt u het veldtype, het databaseveld dat moet worden bijgewerkt, het label en de tekst bewerken die in het veld wordt weergegeven voordat gebruikers een waarde invoeren.

   ![](assets/lp-form-text-field.png){zoomable=&quot;yes&quot;}

1. Schakel indien nodig de optie **[!UICONTROL Make form field mandatory]** in. In dat geval kan de landingspagina alleen worden verzonden als de gebruiker dit veld heeft ingevuld.

   >[!NOTE]
   >
   >Als een verplicht veld niet is ingevuld, wordt een foutbericht weergegeven wanneer de gebruiker de pagina verzendt.

1. Vouw het eventuele selectievakje uit of voeg er een toe met het gereedschap **[!UICONTROL Add]** knop. Selecteer deze optie als u een service of een veld uit de database wilt bijwerken.

   ![](assets/lp-form-checkbox.png){zoomable=&quot;yes&quot;}

   Als u **[!UICONTROL Subscription & services]** selecteert u een service in de lijst en kiest u een van de twee onderstaande opties:

   * **[!UICONTROL Subscribe in if checked]**: Gebruikers moeten het selectievakje voor toestemming (opt-in) inschakelen.
   * **[!UICONTROL Unsubscribe if checked]**: Gebruikers moeten het selectievakje inschakelen om hun toestemming te verwijderen (opt-out).

   Als u **[!UICONTROL Field]** selecteert u een veld in de lijst met kenmerken en kiest u een van de volgende twee opties:

   * **[!UICONTROL Yes if checked]**<!--TBC-->

   * **[!UICONTROL No if checked]**<!--TBC-->

1. U kunt zoveel velden verwijderen en toevoegen (zoals tekstvelden, keuzerondjes, selectievakjes, vervolgkeuzelijst, enzovoort) indien nodig.

1. Klik op Alle toegevoegde of bijgewerkte velden **[!UICONTROL Call to action]** om de bijbehorende sectie uit te vouwen. Hiermee kunt u het gedrag van de knop in het dialoogvenster **[!UICONTROL Form]** component.

   ![](assets/lp-call-to-action.png){zoomable=&quot;yes&quot;}

1. Bepaal wat er gebeurt wanneer u op de knop klikt:

   * **[!UICONTROL Confirmation page]**: De gebruiker wordt omgeleid naar de **[!UICONTROL Confirmation]** paginaset voor de huidige openingspagina.

   * **[!UICONTROL Redirect URL]**: Voer de URL in van de pagina waarnaar de gebruikers worden omgeleid.

1. Als u aanvullende updates wilt uitvoeren wanneer u het formulier verzendt, selecteert u **[!UICONTROL Additional updates]** en selecteer het item dat u wilt bijwerken:
   * Een abonnementsservice: in dat geval definieert u of u gebruikers wilt aanmelden of afmelden bij het verzenden van het formulier.
   * Het e-mailadres dat wordt gebruikt bij het invullen van het formulier.
   * Alle kanalen - bij het verzenden van het formulier worden gebruikers (afhankelijk van de geselecteerde sjabloon) in- of uitgeschakeld voor alle communicatie van uw merk op alle kanalen
   * Een veld in de database - selecteer een veld in de lijst met kenmerken en bepaal of het bij het verzenden van het formulier moet worden ingesteld op Waar of Onwaar.

   ![](assets/lp-form-additionnal-updates.png){zoomable=&quot;yes&quot;}

1. Sla uw inhoud op om terug te gaan naar de [eigenschappen van bestemmingspagina](create-lp.md#create-landing-page).

## Landingspagina-formulierstijlen definiëren {#lp-form-styles}

1. Als u de stijlen van de inhoud van een formuliercomponent wilt wijzigen, schakelt u op elk gewenst moment over naar de **[!UICONTROL Styles]** tab.

1. De **[!UICONTROL Text field]** wordt standaard uitgevouwen. Hiermee kunt u de weergave van de tekstvelden bewerken, zoals het lettertype van het label, de positie van het label, de achtergrondkleur van het veld of de veldrand.

   ![](assets/lp-text-styles.png){zoomable=&quot;yes&quot;}

1. Breid uit **[!UICONTROL Checkbox]** om de vormgeving van de selectievakjes en de bijbehorende tekst te definiëren. U kunt bijvoorbeeld de lettertypefamilie en -grootte of de randkleur van het selectievakje aanpassen.

   ![](assets/lp-checkbox-style.png){zoomable=&quot;yes&quot;}

1. Andere secties uitbreiden en bewerken die overeenkomen met andere velden die u hebt toegevoegd (keuzerondje, vervolgkeuzelijst, datum en tijd, enz.) naar uw formulier.

1. Breid uit **[!UICONTROL Call to action]** om de weergave van de knop in het deelformulier te wijzigen. U kunt bijvoorbeeld het lettertype wijzigen, een rand toevoegen, de labelkleur bewerken op de muisaanwijzer of de uitlijning van de knop aanpassen.

   ![](assets/lp-call-to-action-style.png){zoomable=&quot;yes&quot;}

   U kunt een voorvertoning van bepaalde instellingen, zoals de kleur van knoplabels op de muisaanwijzer, weergeven met de opdracht **[!UICONTROL Simulate content]** knop. [Meer informatie](create-lp.md#test-landing-page)

1. Sla uw wijzigingen op.
