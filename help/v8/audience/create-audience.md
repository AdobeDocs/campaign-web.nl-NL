---
audience: end-user
title: Soorten publiek maken
description: Leer hoe u een publiek kunt maken op Adobe Campaign Web
badge: label="Beta"
source-git-commit: b2cd72ce06e1b18689be4c40c80f3abde85f922e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Soorten publiek maken {#create-audiences}

Met Campagne Web kunt u workflows maken waarin u bestaande soorten publiek kunt combineren tot een visueel canvas en verschillende activiteiten (splitsen, uitsluiten...) kunt gebruiken om nieuwe soorten publiek te maken.

Als dit eenmaal is gedaan, worden de resulterende doelgroepen opgeslagen in Campagne Web, samen met het bestaande publiek, en kunnen ze worden gebruikt in zelfstandige leveringen of campagnes voor het doelpubliek.

## Uw eerste publiek maken {#create}

Voer de volgende stappen uit om een publiek te maken:

1. Ga naar de **[!UICONTROL Audiences]** menu en klik op **[!UICONTROL Create Audience]** in de rechterbovenhoek
1. Geef een label voor het publiek op.
1. Vouw de sectie Aanvullende opties uit om de parameters voor de doelgroep te configureren.

   >[!NOTE]
   >
   >Standaard wordt een publiek gemaakt in het menu Profielen en doelen / Lijsten. U kunt de standaardopslaglocatie wijzigen in het dialoogvenster **[!UICONTROL Folder]** veld.

1. Als de publieksinstellingen zijn geconfigureerd, klikt u op **[!UICONTROL Create Audience]** knop.

1. Er wordt een werkstroomcanvas weergegeven met twee standaardactiviteiten:

   * **[!UICONTROL Build audience]**: het beginpunt van de workflow. Met deze activiteit kunt u een of meer soorten publiek selecteren als basis voor uw workflow.
   * **[!UICONTROL Save audience]**: de laatste stap van uw workflow. Met deze activiteit kunt u het resultaat van uw workflow opslaan in een nieuw publiek.

1. Configureer uw workflow door zoveel activiteiten toe te voegen als u nodig hebt. Voor meer informatie over hoe vormen de diverse activiteiten, verwijs naar [werkstroomdocumentatie](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanaalactiviteiten zijn niet beschikbaar voor gebruik in publieksworkflows.

   ![](assets/audience-creation-canvas.png)

1. Wanneer uw workflow gereed is, klikt u op **[!UICONTROL Start]** om het uit te voeren.

1. De workflow wordt opgeslagen in de **[!UICONTROL Workflows]** en de resulterende doelgroep(en) in de **[!UICONTROL Audiences]** lijst. [Leer hoe u het publiek kunt bewaken en beheren](access-audiences.md)
