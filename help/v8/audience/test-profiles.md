---
title: Testprofielen maken in campagne
description: Leer testprofielen maken en beheren in Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
adge: label="LA"
source-git-commit: 6610095b2af486bf64a1d875b5fb793cbfdc391d
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 3%

---

# Testprofielen maken en beheren {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Testprofielen maken"
>abstract="Testprofielen worden gemaakt als beginadressen. Het zijn extra ontvangers in de database die worden gebruikt om fictieve profielen als doel in te stellen die niet voldoen aan de gedefinieerde doelcriteria."

Testprofielen worden gemaakt als beginadressen. Het zijn extra ontvangers in de database die worden gebruikt om fictieve profielen als doel in te stellen die niet voldoen aan de gedefinieerde doelcriteria. Hiermee kunt u de personalisatie en rendering voorvertonen en testen voordat u de levering verzendt, door ze proefdrukken te sturen.

<!--Learn more on test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}.-->

De stappen om testberichten naar zaadadressen te verzenden zijn gedetailleerd in [deze sectie](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>De profielen van de test worden automatisch uitgesloten van rapporten over de volgende leveringsstatistieken: **[!UICONTROL Clicks]**, **[!UICONTROL Opens]**, **[!UICONTROL Unsubscriptions]**.

## Testprofielen openen en beheren {#access-test-profiles}

Als u de lijst met inhoudssjablonen wilt openen, selecteert u **[!UICONTROL Customer Management]** > **[!UICONTROL Profiles]** in het linkermenu en selecteert u de **[!UICONTROL Test profiles]** tab.

U kunt filteren op een specifieke [map](../get-started/permissions.md#folders) de vervolgkeuzelijst gebruiken of regels toevoegen met de [querymodel](../query/query-modeler-overview.md).

Als u een testprofiel wilt bewerken, klikt u op het gewenste item in de lijst.

Als u een testprofiel wilt verwijderen, selecteert u de bijbehorende optie in het menu **[!UICONTROL More actions]** -menu.

## Een testprofiel maken {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Testprofielen Aanvullende gegevens"
>abstract="Voer de aanpassingsgegevens in die worden gebruikt voor de leveringen die in de gegevensbeheerworkflows zijn gemaakt en waaraan u een specifieke waarde wilt toewijzen."

Voer de onderstaande stappen uit om een testprofiel te maken.

1. Bladeren naar **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]**.

1. Selecteer het tabblad **[!UICONTROL Test profiles]**. 

   ![](assets/test-profile-list.png)

1. Klik op de knop **[!UICONTROL Create test profile]**.

1. Vul de gegevens van het testprofiel in. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![](assets/test-profile-details.png)

   >[!NOTE]
   >
   >Het label van het adres wordt automatisch ingevuld met de voornaam en achternaam die u hebt gedefinieerd.

1. Standaard worden testprofielen opgeslagen in het dialoogvenster **[!UICONTROL Seed addresses]** map. U kunt dit wijzigen door naar de gewenste locatie te bladeren. [Meer informatie](#seed-addresses-folders)

   ![](assets/test-profile-folder.png)

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. In de **[!UICONTROL Contact information]** en voert u het e-mailadres en andere relevante gegevens in. Het e-mailadres wordt tussen haakjes weergegeven na het label voor het testprofiel.

   ![](assets/test-profile-address.png)

1. Als u **[!UICONTROL No longer contact (by any channel)]** schakelt, is het profiel op lijst van gewezen personen. Deze ontvanger is niet langer gericht op enig kanaal (e-mail, SMS, enz.).

1. In de **[!UICONTROL Additional data]** voert u de aanpassingsgegevens in die worden gebruikt voor de leveringen die worden gemaakt in de workflows voor gegevensbeheer en waaraan u een specifieke waarde wilt toewijzen. [Meer informatie over workflows](../workflows/gs-workflows.md)

   ![](assets/test-profile-additional-data.png)

   Zorg ervoor dat aanvullende doelgegevens zijn gedefinieerd met een alias die begint met &#39;@&#39; in het dialoogvenster **[!UICONTROL Enrichment]** workflowactiviteit. Anders, kunt u niet het met uw zaadadressen in de leveringsactiviteit behoorlijk gebruiken. [Meer informatie over verrijkingsactiviteiten](../workflows/activities/enrichment.md)

1. Klik op de knop **[!UICONTROL Save]**.

Het testprofiel dat u zojuist hebt gemaakt, kan nu worden gebruikt om een test te verzenden. [Meer informatie](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Zaadadresmappen beheren {#seed-addresses-folders}

Zaadadressen worden opgeslagen in een speciaal knooppunt van de Adobe Campaign-hiërarchie: **[!UICONTROL Explorer]** > **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]**.

Als u testprofielen wilt ordenen, kunt u submappen maken in de vervolgkeuzelijst Meer acties. [Leer hoe u mappen maakt](../get-started/permissions.md#folders)

![](assets/test-profile-sub-folders.png)

U kunt ook een testprofiel maken van elke **[!UICONTROL Seed addresses]** map of submap. Vul alle details in zoals u het van het **[!UICONTROL Customer Management]** > **[!UICONTROL Profiles]** -menu. [Meer informatie](#create-test-profile)

Als u testprofielen wilt bewerken, klikt u op het label van het profiel in het menu **[!UICONTROL Test profiles]** of uit de map waarin deze is opgeslagen.


