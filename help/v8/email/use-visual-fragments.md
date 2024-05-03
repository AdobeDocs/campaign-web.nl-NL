---
audience: end-user
title: Visuele fragmenten toevoegen aan uw e-mails
description: Leer hoe u visuele fragmenten toevoegt aan uw e-mails
hide: true
hidefromtoc: true
source-git-commit: 341e2a5ab073405d3be19068f85b9ea917b32a69
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 1%

---

# Visuele fragmenten toevoegen aan uw e-mails {#use-visual-fragments}

U kunt een visueel fragment gebruiken in een [e-maillevering](get-started-email-designer.md)of in een [inhoudssjabloon](use-email-templates.md). De stappen worden hieronder beschreven.


>[!NOTE]
>
>Leer hoe u fragmenten maakt en beheert in [deze sectie](fragments.md).


## Een fragment gebruiken {#use-fragment}

Voer de onderstaande stappen uit om een fragment in te voegen in een e-mailinhoud:

1. Open e-mail- of sjablooninhoud met de [E-mailDesigner](get-started-email-designer.md).

1. Selecteer de **[!UICONTROL Fragments]** pictogram van de linkerrails.

   ![](assets/fragments-in-designer.png)

1. De lijst met alle visuele fragmenten die in de huidige sandbox zijn gemaakt, wordt weergegeven. U kunt:

   * Zoek naar een specifiek fragment door zijn etiket te beginnen typen.
   * Sorteer fragmenten in oplopende of aflopende volgorde.
   * De manier wijzigen waarop de fragmenten worden weergegeven (kaarten of lijstweergave).

   >[!NOTE]
   >
   >Fragmenten worden gesorteerd op aanmaakdatum: recent toegevoegde visuele fragmenten worden als eerste weergegeven in de lijst.

   Als sommige fragmenten zijn gewijzigd of toegevoegd terwijl u de inhoud bewerkt, klikt u op de knop **Vernieuwen** pictogram om de lijst bij te werken met de meest recente wijzigingen.

1. Sleep een fragment uit de lijst naar het gebied waar u het wilt invoegen. Net als bij andere componenten kunt u het fragment in de inhoud verplaatsen.

1. Selecteer het fragment om de opties ervan in het rechterdeelvenster weer te geven.

   ![](assets/fragment-right-pane.png)

   Van de **[!UICONTROL Settings]** kunt u:

   * Kies de apparaten waarop het fragment moet worden weergegeven.
   * Open het fragment op een nieuw tabblad om het zo nodig te bewerken. [Meer informatie](../email/fragments.md#edit-fragments)

   U kunt het fragment verder aanpassen met de opdracht **[!UICONTROL Styles]** tab.

1. Indien nodig, kunt u de overerving met het oorspronkelijke fragment verbreken. [Meer informatie](#break-inheritance)
U kunt het fragment ook uit de inhoud verwijderen of dupliceren. Deze handelingen kunnen rechtstreeks worden uitgevoerd vanuit het contextmenu dat boven op het fragment wordt weergegeven.

1. Voeg zoveel fragmenten toe als u wilt en **[!UICONTROL Save]** uw wijzigingen.

## Overerving onderbreken {#break-inheritance}

Wanneer u een visueel fragment bewerkt, worden de wijzigingen gesynchroniseerd. Ze worden automatisch doorgegeven aan alle e-mailleveringen en inhoudssjablonen die dat fragment bevatten.

Wanneer fragmenten aan een e-mail- of inhoudssjabloon worden toegevoegd, worden ze standaard gesynchroniseerd.

U kunt de overerving echter wel verbreken van het oorspronkelijke fragment. In dat geval wordt de inhoud van het fragment naar het huidige ontwerp gekopieerd en worden de wijzigingen niet meer gesynchroniseerd.

Volg onderstaande stappen om overerving te onderbreken:

1. Selecteer het fragment.

1. Klik op het ontgrendelingspictogram op de contextafhankelijke werkbalk.

   ![](assets/fragment-break-inheritance.png)

1. Dat fragment wordt een zelfstandig element dat niet meer aan het oorspronkelijke fragment is gekoppeld. Bewerk de inhoud als elke andere inhoudscomponent in de inhoud. [Meer informatie](content-components.md)
