---
title: Testprofielen maken in campagne
description: Leer testprofielen maken en beheren in Adobe Campaign
feature: Audiences, Profiles, Seed Address, Proofs
role: User
level: Beginner
exl-id: d372713d-3024-46a1-b62e-f271b8ac829f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 1%

---

# Testprofielen maken en beheren {#create-test-profiles}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_menu"
>title="Testprofielen maken"
>abstract="Testprofielen zijn aanvullende ontvangers waarmee u de personalisatie en rendering kunt voorvertonen en testen voordat u uw berichten verzendt. U kunt een testprofiel selecteren wanneer u een voorbeeld van de inhoud van een bericht weergeeft en proefdrukken naar de testprofielen verzenden om de inhoud en instellingen van uw bericht te controleren en te valideren."

Testprofielen worden gebruikt om proefdrukken te verzenden en uw berichtinhoud en montages te bevestigen. Deze profielen zijn extra ontvangers waarmee u de personalisatie en rendering kunt voorvertonen en testen voordat u uw berichten verzendt. U kunt een testprofiel selecteren wanneer u een voorbeeld van de inhoud van een bericht weergeeft en proefdrukken naar de testprofielen verzenden om de inhoud en instellingen van uw bericht te controleren en te valideren.

➡️ [ ontdekt deze eigenschap in video ](#video)

<!--Learn more about test profiles in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html?lang=nl-NL){target="_blank"}.-->

De stappen om proeven naar testprofielen te verzenden zijn gedetailleerd in [ deze sectie ](../preview-test/test-deliveries.md#test-profiles).

>[!NOTE]
>
>* De profielen van de test worden gecreeerd als zaadadressen in de console van de Cliënt.
>
>* Testprofielen worden automatisch uitgesloten van rapporten over de volgende leveringsstatistieken: **[!UICONTROL Clicks]**, **[!UICONTROL Opens]**, **[!UICONTROL Unsubscriptions]** .

## Testprofielen openen en beheren {#access-test-profiles}

Als u de lijst met testprofielen wilt openen, selecteert u **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** in het linkermenu en klikt u op de tab **[!UICONTROL Test profiles]** .

![ de mening van de profiellijst van de Test ](assets/test-profile-list.png){zoomable="yes"}

* U kunt op een specifieke [ omslag ](../get-started/permissions.md#folders) filtreren gebruikend de drop-down lijst of regels toevoegen gebruikend de [ vraagmodelaar ](../query/query-modeler-overview.md).

  ![ de filters van de profiellijst van de Test ](assets/test-profile-list-filters.png){zoomable="yes"}

* U kunt elk testprofiel dupliceren en zo nodig bijwerken. De stappen om een testprofiel uit te geven zijn het zelfde als wanneer [ creërend een testprofiel ](#create-test-profile).

* Als u een testprofiel wilt verwijderen, selecteert u de bijbehorende optie in het menu **[!UICONTROL More actions]** .

  ![ de optie van het de testprofiel van de Schrapping ](assets/test-profile-list-delete.png){zoomable="yes"}

* Als u een testprofiel wilt bewerken, klikt u op het gewenste item in de lijst. De stappen om een testprofiel uit te geven zijn het zelfde als wanneer [ creërend een testprofiel ](#create-test-profile).

U hebt ook toegang tot testprofielen via de **[!UICONTROL Explorer]** -weergave, via het knooppunt **[!UICONTROL Resources]** > **[!UICONTROL Campaign Management]** > **[!UICONTROL Seed addresses]** .

Daarna kunt u naar mappen of submappen bladeren, deze maken en beheren, en de bijbehorende machtigingen controleren. [ Leer hoe te om omslagen ](../get-started/permissions.md#folders) tot stand te brengen

![ de omslagmening van de Profielen van de Test ](assets/test-profiles-folders.png){zoomable="yes"}

Van de **[!UICONTROL Explorer]** mening, kunt u ook filtreren, schrappen, uitgeven, en [&#128279;](#create-test-profile) testprofielen creëren.

## Een testprofiel maken {#create-test-profile}

>[!CONTEXTUALHELP]
>id="acw_recipients_testprofiles_additionaldata"
>title="Testprofielen Aanvullende gegevens"
>abstract="Voer de aanpassingsgegevens in die worden gebruikt voor de leveringen die in de gegevensbeheerworkflows zijn gemaakt en waaraan u een specifieke waarde wilt toewijzen."

Voer de volgende stappen uit om een testprofiel te maken:

1. Blader naar **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** en selecteer de tab **[!UICONTROL Test profiles]** .

1. Klik op de knop **[!UICONTROL Create test profile]**.

   ![ creeer de knoop van het testprofiel ](assets/test-profile-create.png){zoomable="yes"}

1. Vul zo nodig de gegevens van het testprofiel in. <!--Most of the fields are the same as when creating profiles. [Learn more]-->

   ![ vorm van de profieldetails van de Test ](assets/test-profile-details.png){zoomable="yes"}

   >[!NOTE]
   >
   >Het veld **[!UICONTROL Label]** wordt automatisch ingevuld met de door u gedefinieerde voornaam en achternaam.

1. Testprofielen worden standaard opgeslagen in de map **[!UICONTROL Seed addresses]** . U kunt dit wijzigen door naar de gewenste locatie te bladeren. [ Leer hoe te met omslagen ](../get-started/permissions.md#folders) te werken

   <!--![](assets/test-profile-folder.png){zoomable="yes"}-->

<!--
You do not need to enter all fields of each tab when creating a seed address. Missing personalization elements are entered randomly during delivery analysis. (Not valid?)
-->

1. Voer in de sectie **[!UICONTROL Contact information]** het e-mailadres en andere relevante gegevens in. Het e-mailadres wordt tussen haakjes weergegeven na het label voor het testprofiel.

   ![ de informatiesectie van het Contact ](assets/test-profile-address.png){zoomable="yes"}

1. Als u het selectievakje **[!UICONTROL No longer contact (by any channel)]** inschakelt, wordt het testprofiel op lijst van gewezen personen weergegeven. Deze ontvanger is niet langer gericht op enig kanaal (e-mail, SMS, enz.).

1. Voer op het tabblad **[!UICONTROL Additional data]** de aanpassingsgegevens in die worden gebruikt voor de leveringen die in de workflows voor gegevensbeheer zijn gemaakt en waaraan u een specifieke waarde wilt toewijzen. [ leer meer over werkschema&#39;s ](../workflows/gs-workflows.md)

   ![ Extra gegevens tabel ](assets/test-profile-additional-data.png){zoomable="yes"}

   Controleer of er aanvullende doelgegevens zijn gedefinieerd met een alias, beginnend met &#39;@&#39; in de **[!UICONTROL Enrichment]** -werkstroomactiviteit. Anders, kunt u niet het met uw zaadadressen in de leveringsactiviteit behoorlijk gebruiken. [ leer meer over de activiteit van de Verrijking ](../workflows/activities/enrichment.md)

1. Klik op de knop **[!UICONTROL Save]**.

Het testprofiel dat u zojuist hebt gemaakt, kan nu worden gebruikt om een proefdruk te verzenden. [Meer informatie](../preview-test/test-deliveries.md#test-profiles)

<!--Use test profiles in Direct mail? cf v7/v8-->

## Hoe kan ik-video {#video}

Leer om testprofielen tot stand te brengen en te beheren gebruikend het Web van de Campagne gebruikersinterface.

>[!VIDEO](https://video.tv.adobe.com/v/3442844?quality=12)