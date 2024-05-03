---
audience: end-user
title: Werken met fragmenten
description: Leren werken met fragmenten
hidefromtoc: true
source-git-commit: 2abbe837197980b4eacb0b5171dc29637fd19dfc
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# Werken met fragmenten {#fragments}


>[!CONTEXTUALHELP]
>id="acw_fragments_menu"
>title="Uw eigen fragmenten definiëren"
>abstract="Een fragment is een herbruikbare component waarnaar in een of meer e-mails in verschillende campagnes kan worden verwezen."

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
* U kunt ze zo vaak gebruiken als nodig is in uw inhoud, via de e-mailontwerper. Zie [Visuele fragmenten toevoegen](../email/use-visual-fragments.md)

## Een visueel fragment maken {#create-fragments}

U kunt op twee manieren fragmenten maken:

* Een geheel nieuw fragment maken met de opdracht **[!UICONTROL Fragments]** speciaal menu. [Meer informatie](#create-from-scratch)

* Sla bij het ontwerpen van inhoud een deel van de inhoud op als fragment. [Meer informatie](#save-as-fragment)

Als het fragment eenmaal is opgeslagen, kan het worden gebruikt in een e-mail- of e-mailsjabloon. Of het nu om een geheel nieuw fragment of om bestaande inhoud gaat, u kunt dit fragment nu gebruiken bij het maken van inhoud in Campagne. Zie [Visuele fragmenten toevoegen](../email/use-visual-fragments.md).

### Een geheel nieuw fragment maken {#create-from-scratch}

Voer de onderstaande stappen uit om een geheel nieuw fragment te maken.

1. [De fragmentlijst openen](#access-manage-fragments) via de **[!UICONTROL Content Management]** > **[!UICONTROL Fragments]** links.

   ![](assets/fragments-list.png)

1. Selecteer **[!UICONTROL Create fragment]**.

1. Voer het label van het fragment in.

   ![](assets/fragment-create.png)

1. Indien nodig kunt u aanvullende opties definiëren, zoals de interne naam van het fragment, de map en een beschrijving.

   >[!NOTE]
   >
   >Momenteel kunt u alleen visuele fragmenten maken.

1. Klik op de knop **Maken** om de inhoud van het fragment te configureren.

1. De [E-mailDesigner](../email/get-started-email-designer.md) worden weergegeven. Bewerk uw inhoud naar wens, net als voor alle e-mailberichten in een campagne. U kunt afbeeldingen, koppelingen, personalisatievelden en dynamische inhoud toevoegen.

   ![](assets/fragment-designer.png)

1. Wanneer het fragment gereed is, klikt u op **[!UICONTROL Save & close]**. Het wordt toegevoegd aan de [fragmentlijst](#access-manage-fragments).

1. Klik zo nodig op de pijl naast de fragmentnaam om terug te gaan naar de map **[!UICONTROL Details]** en bewerken.

Dit fragment kan nu worden gebruikt bij het maken van [email](../email/get-started-email-designer.md) of [inhoudssjabloon](use-email-templates.md) in Campaign. [Meer informatie](../email/use-visual-fragments.md)


### Inhoud opslaan als fragment {#save-as-fragment}

Alle e-mailinhoud kan worden opgeslagen als fragment en later opnieuw worden gebruikt. Wanneer u een [inhoudssjabloon](use-email-templates.md) of een [email](../email/get-started-email-designer.md) levering, kunt u een gedeelte van uw inhoud als visueel fragment bewaren. Hiervoor voert u de volgende stappen uit:

1. In de [E-mailDesigner](../email/get-started-email-designer.md)klikt u op de knop **Meer** op de rechterbovenhoek van het scherm.

1. Selecteren **[!UICONTROL Save as fragment]** in het keuzemenu.

   ![](assets/fragment-save-as.png)

1. De **[!UICONTROL Save as fragment]** schermweergaven. Hier selecteert u de elementen die u in het fragment wilt opnemen, inclusief personalisatievelden en dynamische inhoud.

   >[!CAUTION]
   >
   >U kunt alleen secties selecteren die aan elkaar grenzen. U kunt geen lege structuur of een ander fragment selecteren.

   ![](assets/fragment-save-as-screen.png)

1. Klik op **[!UICONTROL Create]**. Vul de fragmentnaam in en sla deze op.

   ![](assets/fragment-save-confirm.png)

   Deze inhoud is nu een op zichzelf staand fragment dat aan de [fragmentlijst](#manage-fragments)en toegankelijk via het toegewezen menu. U kunt dit fragment nu gebruiken wanneer u een [email](../email/get-started-email-designer.md) of [inhoudssjabloon](use-email-templates.md) in Campaign. [Meer informatie](../email/use-visual-fragments.md)

>[!NOTE]
>
>Wijzigingen in dat nieuwe fragment worden niet doorgegeven aan het e-mailbericht of de sjabloon waaruit het fragment afkomstig is. Op dezelfde manier wordt het nieuwe fragment niet gewijzigd wanneer de oorspronkelijke inhoud wordt bewerkt in het e-mailbericht of de sjabloon.

## Uw fragmenten beheren {#manage-fragments}

U kunt een fragment uit de fragmentlijst bewerken, bijwerken, dupliceren of verwijderen.

### Een fragment bewerken en bijwerken {#edit-fragments}

Voer de onderstaande stappen uit om een fragment te bewerken.

1. Klik op de naam van het fragment dat u wilt bewerken vanuit het dialoogvenster **[!UICONTROL Fragments]** lijst.
1. Klik op de knop **Inhoud bewerken** om de inhoud van dit fragment te openen.

   ![](assets/fragment-edit-content.png)

1. Breng de gewenste wijzigingen aan en sla uw wijzigingen op.

>[!CAUTION]
>
>Elke wijziging in een fragment wordt doorgegeven aan de e-mailleveringen of sjablonen die deze gebruiken.


### Een fragment verwijderen {#delete-fragments}

Ga als volgt te werk om een fragment te verwijderen:

1. Blader naar de fragmentlijst en klik op de knop **[!UICONTROL More actions]** naast het te verwijderen fragment.
1. Klikken **Verwijderen** en bevestigen.

   ![](assets/fragment-list-more-actions.png)

>[!CAUTION]
>
>Wanneer u een inhoudsfragment verwijdert, worden de e-mailleveringen en sjablonen waarin dit fragment wordt gebruikt, bijgewerkt en wordt het fragment uit de inhoud van het bericht verwijderd. Indien nodig kunt u de overerving verbreken. [Meer informatie](use-visual-fragments.md#break-inheritance)
>

### Een fragment dupliceren {#duplicate-fragments}

U kunt eenvoudig een fragment dupliceren om een nieuw fragment te maken. Ga als volgt te werk om een bestaand fragment te dupliceren:

1. Blader naar de fragmentlijst en klik op de knop **[!UICONTROL More actions]** naast het te verwijderen fragment.
1. Klikken **Dupliceren** en bevestigen.
1. Voer het label van het nieuwe fragment in en sla uw wijzigingen op.

   Het fragment wordt toegevoegd aan de lijst met fragmenten. U kunt het uitgeven en het vormen zoals nodig.
