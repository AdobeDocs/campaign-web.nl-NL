---
audience: end-user
title: Inhoudsfragmenten maken
description: Leer hoe u maakt met inhoudsfragmenten
exl-id: d155d102-a5bc-4b9b-b29c-24fde4d95ceb
source-git-commit: 2d6b885642fbb6e1545f899219db05c156b069c4
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Inhoudsfragmenten maken {#fragments}

>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Uw eigen fragmenten definiëren"
>abstract="Een fragment is een herbruikbare component waarnaar in een of meer e-mails in verschillende campagnes kan worden verwezen. Deze mogelijkheid wordt gebruikt om vooraf meerdere blokken met aangepaste inhoud samen te stellen die door marketinggebruikers kunnen worden gebruikt om snel e-mailinhoud samen te stellen in een verbeterd ontwerpproces."

>[!CONTEXTUALHELP]
>id="acw_fragments_save"
>title="Fragmenten opslaan"
>abstract="Fragmenten opslaan"

>[!CONTEXTUALHELP]
>id="acw_fragments_create"
>title="Uw eigen fragmenten definiëren"
>abstract="Een fragment is een herbruikbare component waarnaar in een of meer e-mails in verschillende campagnes kan worden verwezen."

>[!CONTEXTUALHELP]
>id="acw_fragments_properties"
>title="Eigenschappen van Fragmenten"
>abstract="Eigenschappen van Fragmenten"

>[!CONTEXTUALHELP]
>id="acw_fragments_type"
>title="Type fragment"
>abstract="Selecteer het type fragment. Momenteel zijn alleen visuele fragmenten voor e-mails beschikbaar."

>[!CONTEXTUALHELP]
>id="acw_fragments_list"
>title="Uw eigen fragmenten definiëren"
>abstract="Een fragment is een herbruikbare component waarnaar in een of meer e-mails in verschillende campagnes kan worden verwezen. U kunt ook fragmenten in uw e-mailsjablonen gebruiken. Momenteel zijn alleen visuele fragmenten beschikbaar."

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmentdetails"
>abstract="Fragmentdetails"

>[!CONTEXTUALHELP]
>id="acw_create_fragment"
>title="Uw eigen fragmenten definiëren"
>abstract="Een fragment is een herbruikbare component waarnaar in een of meer e-mails in verschillende campagnes kan worden verwezen."

Een fragment is een herbruikbare component waarnaar in een of meer e-mails in verschillende campagnes kan worden verwezen. Wanneer u een fragment wijzigt, wordt alle inhoud die het fragment gebruikt, bijgewerkt.

Met deze functionaliteit kunt u meerdere blokken met aangepaste inhoud vooraf samenstellen. Deze blokken kunnen door marketinggebruikers worden gebruikt om snel e-mailinhoud samen te stellen in een verbeterd ontwerpproces.

![](assets/fragments.gif)

U kunt zo veel mogelijk gebruikmaken van fragmenten:

* Maak uw eigen visuele fragmenten, zoals hieronder wordt beschreven.
* Gebruik ze zo vaak als nodig is in uw inhoud, via de e-mail-Designer. Zie [ visuele fragmenten aan uw e-mails ](../email/use-visual-fragments.md) toevoegen.

>[!AVAILABILITY]
>
>Dit vermogen is in Beperkte Beschikbaarheid (LA). Het is beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kan niet op een ander milieu worden opgesteld.

## Een visueel fragment maken {#create-fragments}

U kunt op twee manieren fragmenten maken:

* Maak een geheel nieuw fragment met het menu dat u toewijst aan **[!UICONTROL Fragments]** . [ leer hoe ](#create-from-scratch)

* Sla bij het ontwerpen van inhoud een deel van de inhoud op als fragment. [ leer hoe ](#save-as-fragment)

Als het fragment eenmaal is opgeslagen, kan het worden gebruikt in een e-mail- of e-mailsjabloon. Of het nu om een geheel nieuw fragment of om bestaande inhoud gaat, u kunt dit fragment nu gebruiken bij het maken van inhoud in Campagne. Zie [ visuele fragmenten ](../email/use-visual-fragments.md) toevoegen.

### Een geheel nieuw fragment maken {#create-from-scratch}

Voer de onderstaande stappen uit om een geheel nieuw fragment te maken.

1. [ heb toegang tot de fragmentlijst ](#access-manage-fragments) door **[!UICONTROL Content Management]** > **[!UICONTROL Fragments]** linkermenu.

   ![](assets/fragments-list.png)

1. Selecteer **[!UICONTROL Create fragment]**.

1. Voer het label van het fragment in.

   ![](assets/fragment-create.png)

1. Indien nodig kunt u aanvullende opties definiëren, zoals de interne naam van het fragment, de map en een beschrijving.

   >[!NOTE]
   >
   >Momenteel kunt u alleen visuele fragmenten maken.

1. Klik **creeer** knoop om de inhoud van uw fragment te vormen.

1. De [ e-mail Designer ](../email/get-started-email-designer.md) vertoningen. Bewerk uw inhoud naar wens, net als voor alle e-mailberichten in een campagne. U kunt afbeeldingen, koppelingen, personalisatievelden en dynamische inhoud toevoegen.

   ![](assets/fragment-designer.png)

1. Klik op **[!UICONTROL Save & close]** als het fragment gereed is. Het wordt toegevoegd aan de [ fragmentlijst ](#access-manage-fragments).

Dit fragment is nu klaar om te worden gebruikt wanneer het bouwen van om het even welk [ e-mail ](../email/get-started-email-designer.md) of [ inhoudsmalplaatje ](use-email-templates.md) binnen Campagne. [ leer hoe ](../email/use-visual-fragments.md)


### Inhoud opslaan als fragment {#save-as-fragment}

Alle e-mailinhoud kan worden opgeslagen als fragment en later opnieuw worden gebruikt. Wanneer het ontwerpen van a [ inhoudsmalplaatje ](use-email-templates.md) of een [ e-mail ](../email/get-started-email-designer.md) levering, kunt u een gedeelte van uw inhoud als visueel fragment bewaren. Hiervoor voert u de volgende stappen uit:

1. In [ E-mail Designer ](../email/get-started-email-designer.md), klik de **Meer** knoop op hoogste recht van het scherm.

1. Selecteer **[!UICONTROL Save as fragment]** in de vervolgkeuzelijst.

   ![](assets/fragment-save-as.png)

1. Het scherm **[!UICONTROL Save as fragment]** wordt weergegeven. Hier selecteert u de elementen die u in het fragment wilt opnemen, inclusief personalisatievelden en dynamische inhoud.

   >[!CAUTION]
   >
   >U kunt alleen secties selecteren die aan elkaar grenzen. U kunt geen lege structuur of een ander fragment selecteren.

   ![](assets/fragment-save-as-screen.png)

1. Klik op **[!UICONTROL Create]**. Vul de fragmentnaam in en sla deze op.

   ![](assets/fragment-save-confirm.png)

   Deze inhoud is nu een standalone fragment, dat aan de [ fragmentlijst ](#manage-fragments) wordt toegevoegd, en toegankelijk van het specifieke menu. U kunt dit fragment nu gebruiken wanneer het bouwen van om het even welk [ e-mail ](../email/get-started-email-designer.md) of [ inhoudsmalplaatje ](use-email-templates.md) binnen Campagne. [ leer hoe ](../email/use-visual-fragments.md)

>[!NOTE]
>
>Wijzigingen in dat nieuwe fragment worden niet doorgegeven aan het e-mailbericht of de sjabloon waaruit het fragment afkomstig is. Op dezelfde manier wordt het nieuwe fragment niet gewijzigd wanneer de oorspronkelijke inhoud wordt bewerkt in het e-mailbericht of de sjabloon.

## Uw fragmenten beheren {#manage-fragments}

U kunt een fragment uit de fragmentlijst bewerken, bijwerken, dupliceren of verwijderen.

### Een fragment bewerken en bijwerken {#edit-fragments}

Voer de onderstaande stappen uit om een fragment te bewerken.

1. Klik op de naam van het fragment dat u wilt bewerken in de lijst **[!UICONTROL Fragments]** .
1. Klik **uitgeven inhoud** knoop om de inhoud van dit fragment te openen.

   ![](assets/fragment-edit-content.png)

1. Breng de gewenste wijzigingen aan en sla uw wijzigingen op.

>[!CAUTION]
>
>Elke wijziging in een fragment wordt doorgegeven aan de e-mailleveringen of sjablonen die deze gebruiken.


### Een fragment verwijderen {#delete-fragments}

Ga als volgt te werk om een fragment te verwijderen:

1. Blader naar de fragmentlijst en klik op de knop **[!UICONTROL More actions]** naast het fragment dat u wilt verwijderen.
1. Klik **Schrapping** en bevestig.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Wanneer u een inhoudsfragment verwijdert, worden de e-mailleveringen en sjablonen waarin dit fragment wordt gebruikt, bijgewerkt: het fragment wordt uit de e-mailinhoud verwijderd, maar er wordt nog steeds naar verwezen. Om de fragmentinhoud in die leveringen en malplaatjes te houden, moet u overerving breken alvorens het fragment te schrappen, [ zoals die in deze sectie ](use-visual-fragments.md#break-inheritance) wordt gedetaillerd.
>

### Een fragment dupliceren {#duplicate-fragments}

U kunt eenvoudig een fragment dupliceren om een nieuw fragment te maken. Ga als volgt te werk om een bestaand fragment te dupliceren:

1. Blader naar de fragmentlijst en klik op de knop **[!UICONTROL More actions]** naast het fragment dat u wilt verwijderen.
1. Klik **Dupliceren** en bevestigen.
1. Voer het label van het nieuwe fragment in en sla uw wijzigingen op.

   Het fragment wordt toegevoegd aan de lijst met fragmenten. U kunt het uitgeven en het vormen zoals nodig.
