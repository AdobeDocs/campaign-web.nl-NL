---
audience: end-user
title: Visuele fragmenten toevoegen aan uw e-mails
description: Leer hoe u visuele fragmenten toevoegt aan uw e-mails
badge: label="Beperkte beschikbaarheid"
exl-id: 6d6f38f9-9d3e-47cb-beb8-177b5a5d8306
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 1%

---

# Visuele fragmenten toevoegen aan uw e-mails {#use-visual-fragments}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Visuele fragmenten e-mailen"
>abstract="U kunt nu visuele fragmenten maken en gebruiken. Dit zijn vooraf gedefinieerde visuele blokken die u kunt hergebruiken in meerdere e-mailleveringen of in inhoudssjablonen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"

>[!AVAILABILITY]
>
>Voor deze functie is een update van Campagne v8.6.4 vereist. Leer meer in de [ notities van de de consoleversie van de Cliënt van de Campagne v8 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/releases/release-notes).

In het Webinterface van de Campagne, **Visuele fragmenten** zijn vooraf bepaalde visuele blokken die u over veelvoudige [ e-mailleveringen ](../email/get-started-email-designer.md), of in [ inhoudsmalplaatjes ](../email/use-email-templates.md) kunt hergebruiken. Leer hoe te om inhoudsfragmenten in [ tot stand te brengen en te beheren deze sectie ](fragments.md).

![](assets/do-not-localize/fragments.gif)

## Een visueel fragment gebruiken {#use-fragment}

>[!CONTEXTUALHELP]
>id="acw_fragments_details"
>title="Fragmenten, opties"
>abstract="Dit deelvenster bevat opties voor het geselecteerde fragment. Hiermee kunt u kiezen op welke apparaten het fragment moet worden weergegeven en de inhoud van dit fragment openen. Gebruik het tabblad **[!UICONTROL Styles]** om het fragment verder aan te passen. U kunt de overerving ook verbreken met het originele visuele fragment."

<!-- pas vu dans l'UI-->

Voer de onderstaande stappen uit om een visueel fragment in te voegen in een e-mailinhoud:

1. Open om het even welke e-mail of malplaatjeinhoud gebruikend [ E-mail Designer ](../email/get-started-email-designer.md).

1. Selecteer het pictogram **[!UICONTROL Fragments]** van de linkerspoorstaaf.

   ![](assets/fragments-in-designer.png)

1. De lijst met alle visuele fragmenten die in de huidige sandbox zijn gemaakt, wordt weergegeven. U kunt:

   * Zoek naar een specifiek fragment door zijn etiket te beginnen typen.
   * Sorteer fragmenten in oplopende of aflopende volgorde.
   * De manier wijzigen waarop de fragmenten worden weergegeven (kaarten of lijstweergave).

   >[!NOTE]
   >
   >Fragmenten worden gesorteerd op aanmaakdatum: recent toegevoegde fragmenten worden als eerste weergegeven in de lijst.

   Als sommige visuele fragmenten werden gewijzigd of werden toegevoegd terwijl u uw inhoud uitgeeft, klik **verfrissen** pictogram om de lijst met de recentste veranderingen bij te werken.

1. Sleep een visueel fragment uit de lijst naar het gebied waar u het wilt invoegen. Net als bij andere componenten kunt u het fragment in de inhoud verplaatsen.

1. Selecteer het fragment om de opties ervan in het rechterdeelvenster weer te geven.

   ![](assets/fragment-right-pane.png)

   Via het tabblad **[!UICONTROL Settings]** kunt u:

   * Kies de apparaten waarop het fragment moet worden weergegeven.
   * Klik **uitgeven inhoud** knoop om de inhoud van dit fragment te openen. [Meer informatie](../content/fragments.md#edit-fragments)

     U kunt het fragment verder aanpassen met het tabblad **[!UICONTROL Styles]** .

1. Indien nodig kunt u de overerving verbreken met het originele visuele fragment. [Meer informatie](#break-inheritance)

   U kunt het fragment ook uit de inhoud verwijderen of dupliceren. Deze handelingen kunnen rechtstreeks worden uitgevoerd vanuit het contextmenu dat boven op het fragment wordt weergegeven.

1. Voeg zoveel visuele fragmenten toe als u wilt en **[!UICONTROL Save]** uw wijzigingen.

### Visueel fragment in alleen-lezen modus {#fragment-readonly}

Toegangsrechten kunnen worden toegepast op visuele fragmenten.

Als u geen het uitgeven toestemmingen voor een bepaald visueel fragment hebt, wordt het inhoudsmalplaatje getoond op **read-only wijze**. In dit geval wordt de knop **[!UICONTROL Edit content]** vervangen door de knop **[!UICONTROL View content]** , zodat u het fragment kunt bekijken zonder wijzigingen aan te brengen.

![](assets/fragment-readonly.png){zoomable="yes"}

Zoals hieronder wordt getoond, worden alle eigenschapspictogrammen gedeactiveerd, die interactie beperken tot het bekijken slechts.

![](assets/fragment-readonly-view.png){zoomable="yes"}

## Overerving onderbreken {#break-inheritance}

Wanneer u een visueel fragment bewerkt, worden de wijzigingen gesynchroniseerd. Ze worden automatisch doorgegeven aan alle e-mailleveringen en inhoudssjablonen die dat fragment bevatten.

Wanneer fragmenten aan een e-mail- of inhoudssjabloon worden toegevoegd, worden ze standaard gesynchroniseerd.

U kunt de overerving echter wel verbreken van het oorspronkelijke fragment. In dat geval wordt de inhoud van het fragment naar het huidige ontwerp gekopieerd en worden de wijzigingen niet meer gesynchroniseerd.

Volg onderstaande stappen om overerving te onderbreken:

1. Selecteer het visuele fragment.

1. Klik op het ontgrendelingspictogram op de contextafhankelijke werkbalk.

   ![](assets/fragment-break-inheritance.png)

1. Dat fragment wordt een zelfstandig element dat niet meer aan het oorspronkelijke fragment is gekoppeld. Bewerk de inhoud als elke andere inhoudscomponent in de inhoud. [Meer informatie](../email/content-components.md)
