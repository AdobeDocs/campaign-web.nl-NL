---
audience: end-user
title: Soorten publiek maken
description: Leer hoe u een publiek kunt maken op Adobe Campaign Web
badge: label="Beta"
source-git-commit: ffd668b220284c2e948d1757740dbf67b27e32bd
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---


# Soorten publiek maken {#create-audiences}

>[!CONTEXTUALHELP]
>id="acw_audiences_list"
>title="Doelgroepen"
>abstract="Vanuit dit scherm kunt u soorten publiek maken en combineren tot een visueel canvas. Diverse workflowactiviteiten toevoegen, zoals **Splitsen** of **Uitsluiten** nieuwe en verfijnde doelgroepen te creëren."

>[!CONTEXTUALHELP]
>id="acw_audiences_create_settings"
>title="Instellingen voor publiek"
>abstract="Voer de naam van het publiek en aanvullende opties in en klik op de knop **Publiek maken** knop."

Met Campagne Web kunt u nieuwe soorten publiek maken tot een visueel workflowcanvas. U kunt workflowactiviteiten niet alleen helemaal vanaf het begin gebruiken om een eenvoudig publiek te maken, maar ook om het publiek te verfijnen. U kunt bijvoorbeeld meerdere soorten publiek in één publiek opnemen, het publiek verrijken met externe kenmerken of een bepaald publiek opsplitsen in meerdere.

Zodra u uw werkschema hebt gecreeerd, worden de resulterende publiek automatisch opgeslagen binnen het gegevensbestand van de Campagne naast uw bestaande degenen. Deze doelgroepen kunnen zich dan richten op campagnes of op zelfstandige leveringen.

De belangrijkste stappen om een publiek tot stand te brengen zijn als volgt:

1. Maak een publieksworkflow.
1. Vorm een het publieksactiviteit van de Bouwstijl om het gegevensbestand te vragen dat op uw behoeften wordt gebaseerd.
1. Workflowactiviteiten toevoegen om het publiek te verfijnen (optioneel).
1. Configureer een publieksactiviteit Opslaan.
1. Voer de workflow uit om de resulterende groep(en) in de database op te slaan.


## Uw eerste publiek maken {#create}

Voer de volgende stappen uit om een publiek te maken:

1. Ga naar de **[!UICONTROL Audiences]** en klik op de knop **[!UICONTROL Create Audience]** in de rechterbovenhoek.
1. Geef een label voor uw publiek op.
1. Breid uit **[!UICONTROL Additional options]** om geavanceerde publieksparameters te configureren.

   Standaard worden soorten publiek gemaakt in de **[!UICONTROL Profiles and Targets]** / **[!UICONTROL Lists]** verkenner-menu. U kunt de standaardopslaglocatie wijzigen met de **[!UICONTROL Folder]** veld.

   ![](assets/audiences-settings.png)

1. Als u de publieksinstellingen hebt geconfigureerd, klikt u op de knop **[!UICONTROL Create Audience]** knop.

1. Er wordt een werkstroomcanvas weergegeven met twee standaardactiviteiten:

   * **[!UICONTROL Build audience]**: Dit is het beginpunt van uw workflow, zodat u een publiek kunt maken en dit kunt gebruiken als basis voor uw workflow. [Leer hoe te om een het publieksactiviteit van de Bouwstijl te vormen](../workflows/activities/build-audience.md)

   * **[!UICONTROL Save audience]**: Dit is de laatste stap in uw workflow, zodat u de resultaten kunt opslaan als een nieuw publiek. [Leer hoe u een activiteit voor het opslaan van het publiek configureert](../workflows/activities/save-audience.md)

1. Als u na de **[!UICONTROL Build audience]** activiteit, voegt zo veel activiteiten toe zoals vereist in uw werkschema. Voor meer informatie over hoe vormen de werkschemaactiviteiten, naar [werkstroomdocumentatie](../workflows/activities/about-activities.md).

   >[!NOTE]
   >
   >Kanaalactiviteiten zijn niet beschikbaar voor gebruik in publieksworkflows.

   ![](assets/audience-creation-canvas.png)

1. Wanneer uw workflow gereed is, klikt u op **[!UICONTROL Start]** om het uit te voeren.

1. De workflow wordt opgeslagen in het dialoogvenster **[!UICONTROL Workflows]** en de resulterende doelgroep(en) toegankelijk zijn in de **[!UICONTROL Audiences]** lijst. [Leer hoe u het publiek kunt bewaken en beheren](access-audiences.md)

## Voorbeeld van een publiek werkstroom {#example}

In het onderstaande voorbeeld ziet u een publieksworkflow die is geconfigureerd voor vrouwelijke klanten die in New York wonen en die twee nieuwe doelgroepen creëert, afhankelijk van hun interesse in Yoga of Running tandwielen. De twee doelgroepen worden verrijkt met aanvullende informatie over de aankopen van de klanten.

SCREENSHOT TOEVOEGEN

1. De activiteiten van het publiek Build richten zich op alle Vrouwelijke profielen die in New York wonen.
1. De verrijkingsactiviteit verrijkt het publiek met attributen van de lijst van Aankopen.
1. De gesplitste activiteit verdeelt de werkstroom in twee wegen die op de centra van de klanten van belang worden gebaseerd.
1. De sparen publieksactiviteiten aan het eind van elke weg om elk publiek in het gegevensbestand te bewaren.
