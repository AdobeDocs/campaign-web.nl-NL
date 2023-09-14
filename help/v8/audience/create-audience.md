---
audience: end-user
title: Soorten publiek maken
description: Leer hoe u een publiek kunt maken op Adobe Campaign Web
badge: label="Beta"
source-git-commit: f9693c08e1f0a5b5644e8026b7dfe788ee6499c4
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---


# Soorten publiek maken {#create-audiences}

Met Campagne Web kunt u workflows maken waarin u bestaande soorten publiek kunt combineren tot een visueel canvas. Door verschillende workflowactiviteiten op te nemen, zoals Splitsen of Excluse, kunt u nieuwe en verfijnde doelgroepen genereren.

Zodra u uw werkschema hebt gecreeerd, worden de resulterende publiek automatisch opgeslagen binnen het Web van de Campagne naast uw bestaande degenen. Deze doelgroepen kunnen zich dan richten op campagnes of op zelfstandige leveringen.

## Uw eerste publiek maken {#create}

Voer de volgende stappen uit om een publiek te maken:

1. Ga naar de **[!UICONTROL Audiences]** en klik op de knop **[!UICONTROL Create Audience]** in de rechterbovenhoek.
1. Geef een label voor uw publiek op.
1. Breid uit **[!UICONTROL Additional options]** om geavanceerde publieksparameters te configureren.

   Standaard worden soorten publiek gemaakt in de **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** verkenner-menu. U kunt de standaardopslaglocatie wijzigen met de **[!UICONTROL Folder]** veld.

   ![](assets/audiences-settings.png)

1. Als u de publieksinstellingen hebt geconfigureerd, klikt u op de knop **[!UICONTROL Create Audience]** knop.

1. Er wordt een werkstroomcanvas weergegeven met twee standaardactiviteiten:

   * **[!UICONTROL Build audience]**: Dit is het beginpunt van uw workflow, zodat u een publiek kunt maken en dit kunt gebruiken als basis voor uw workflow.
   * **[!UICONTROL Save audience]**: Dit is de laatste stap in uw workflow, zodat u de resultaten kunt opslaan als een nieuw publiek.

1. Pas uw workflow aan door zoveel activiteiten toe te voegen als nodig is. Voor meer informatie over hoe vormen de werkschemaactiviteiten, naar [werkstroomdocumentatie](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanaalactiviteiten zijn niet beschikbaar voor gebruik in publieksworkflows.

   ![](assets/audience-creation-canvas.png)

1. Wanneer uw workflow gereed is, klikt u op **[!UICONTROL Start]** om het uit te voeren.

1. De workflow wordt opgeslagen in het dialoogvenster **[!UICONTROL Workflows]** en de resulterende doelgroep(en) toegankelijk zijn in de **[!UICONTROL Audiences]** lijst. [Leer hoe u het publiek kunt bewaken en beheren](access-audiences.md)
