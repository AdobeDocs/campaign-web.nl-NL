---
audience: end-user
title: Visuele fragmenten toevoegen aan uw e-mails
description: Leer hoe u visuele fragmenten toevoegt aan uw e-mails
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 2d6b885642fbb6e1545f899219db05c156b069c4
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# Visuele fragmenten toevoegen aan uw e-mails {#use-visual-fragments}

U kunt een visueel fragment in een [ e-maillevering ](get-started-email-designer.md), of in a [ inhoudsmalplaatje ](use-email-templates.md) gebruiken. De stappen worden hieronder beschreven. Leer hoe te om fragmenten in [ tot stand te brengen en te beheren deze sectie ](fragments.md).

>[!AVAILABILITY]
>
>Dit vermogen is in Beperkte Beschikbaarheid (LA). Het is beperkt tot klanten die **van Adobe Campaign Standard aan Adobe Campaign v8** migreren, en kan niet op een ander milieu worden opgesteld.

## Een fragment gebruiken {#use-fragment}

Voer de onderstaande stappen uit om een fragment in te voegen in een e-mailinhoud:

1. Open om het even welke e-mail of malplaatjeinhoud gebruikend [ E-mail Designer ](get-started-email-designer.md).

1. Selecteer het pictogram **[!UICONTROL Fragments]** van de linkerspoorstaaf.

   ![](assets/fragments-in-designer.png)

1. De lijst met alle visuele fragmenten die in de huidige sandbox zijn gemaakt, wordt weergegeven. U kunt:

   * Zoek naar een specifiek fragment door zijn etiket te beginnen typen.
   * Sorteer fragmenten in oplopende of aflopende volgorde.
   * De manier wijzigen waarop de fragmenten worden weergegeven (kaarten of lijstweergave).

   >[!NOTE]
   >
   >Fragmenten worden gesorteerd op aanmaakdatum: recent toegevoegde visuele fragmenten worden als eerste weergegeven in de lijst.

   Als sommige fragmenten werden gewijzigd of werden toegevoegd terwijl u uw inhoud uitgeeft, klik **verfrissen** pictogram om de lijst met de recentste veranderingen bij te werken.

1. Sleep een fragment uit de lijst naar het gebied waar u het wilt invoegen. Net als bij andere componenten kunt u het fragment in de inhoud verplaatsen.

1. Selecteer het fragment om de opties ervan in het rechterdeelvenster weer te geven.

   ![](assets/fragment-right-pane.png)

   Via het tabblad **[!UICONTROL Settings]** kunt u:

   * Kies de apparaten waarop het fragment moet worden weergegeven.
   * Klik **uitgeven inhoud** knoop om de inhoud van dit fragment te openen. [Meer informatie](../email/fragments.md#edit-fragments)

     U kunt het fragment verder aanpassen met het tabblad **[!UICONTROL Styles]** .

1. Indien nodig, kunt u de overerving met het oorspronkelijke fragment verbreken. [ Leer meer ](#break-inheritance)
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
