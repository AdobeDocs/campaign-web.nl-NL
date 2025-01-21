---
title: Uw inhoud aanpassen in campagne
description: Leer hoe u uw inhoud kunt aanpassen op Adobe Campaign Web
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 7185e1cbc8ce9dd325bebc20c0ac362d7067f3e9
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---


# Uw inhoud personaliseren {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="Huidige datum toevoegen"
>abstract="Dit menu bevat functies die gerelateerd zijn aan de datumopmaak en die u kunt gebruiken om uw inhoud aan te passen."

Personalization van leveringsinhoud is een zeer belangrijke eigenschap die u toestaat om berichten aan individuele ontvangers aan te passen, die communicatie relevanter maken en aansprekend.

In Adobe Campaign, door [ profielgegevens ](#data-personalization) te gebruiken, zoals de naam, de plaats, of de voorbije interactie van het profiel, en specifieke [ variabelen van uw levering ](#variables-personalization), kunt u elementen zoals tekst, beelden en aanbiedingen in uw mededeling dynamisch aanpassen.

De verpersoonlijking van de levering verbetert niet alleen de gebruikerservaring maar verbetert ook de tarieven van de overeenkomst, die tot hogere omzetting en klantentevredenheid leiden.

## Profielgegevens gebruiken voor personalisatie {#data-personalization}

U kunt elke levering personaliseren met profielgegevens door de uitdrukkingsredacteur te gebruiken, die in gebieden met het **[!UICONTROL Open personalization dialog]** pictogram, zoals de onderwerpregel, e-mailverbindingen, en tekst/knoop inhoudcomponenten toegankelijk is. [ Leer hoe te om tot de uitdrukkingsredacteur toegang te hebben ](gs-personalization.md/#access)

### Personalization-syntaxis {#syntax}

Personalization-tags volgen een specifieke syntaxis: `<%= table.field %>` . Als u bijvoorbeeld de achternaam van de ontvanger wilt invoegen in de tabel met ontvangers, gebruikt u de syntaxis `<%= recipient.lastName %>` .

Tijdens de voorbereiding van de levering, interpreteert Adobe Campaign automatisch deze markeringen en vervangt hen met de overeenkomstige gebiedswaarden voor elke ontvanger. U kunt de daadwerkelijke vervanging bekijken door uw inhoud te simuleren.

Wanneer u contactpersonen uit een extern bestand uploadt voor een zelfstandige e-maillevering, zijn alle velden in het invoerbestand beschikbaar voor personalisatie. De syntaxis is als volgt: `<%= dataSource.field %>`.

### Aanpersonalisatietags toevoegen {#add}

Voer de volgende stappen uit om personalisatietags toe te voegen aan een levering:

1. Open de expressie-editor met behulp van het pictogram **[!UICONTROL Open personalization dialog]** dat toegankelijk is vanuit tekstbewerkingsvelden, zoals de onderwerpregel of de SMS-inhoud. [ Leer hoe te om tot de uitdrukkingsredacteur toegang te hebben ](gs-personalization.md/#access)

   ![](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. De expressie-editor wordt geopend. De gebieden van de verpersoonlijking beschikbaar in het gegevensbestand van Adobe Campaign worden georganiseerd in verscheidene menu&#39;s op de linkerkant van het scherm:

   ![](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menu | Beschrijving |
   |-----|------------|
   | ![](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Subscribers application]** bevat velden die betrekking hebben op de abonnees van een toepassing, zoals de gebruikte terminal of het besturingssysteem. *Dit menu is beschikbaar voor duw slechts berichten* |
   | ![](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Recipient]** bevat velden die zijn gedefinieerd in de tabel met ontvangers, zoals namen, pagina&#39;s of adressen van ontvangers. Wanneer [ het uploaden contacten van een extern dossier ](../audience/file-audience.md) voor een standalone e-maillevering, maakt een lijst dit menu van alle gebieden beschikbaar in het inputdossier. |
   | ![](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Message]** bevat velden die betrekking hebben op de leveringslogboeken, inclusief alle berichten die via alle kanalen naar ontvangers of apparaten worden verzonden, zoals de datum van de laatste gebeurtenis met een bepaalde ontvanger |
   | ![](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Delivery]** bevat velden die betrekking hebben op de parameters die vereist zijn voor het uitvoeren van leveringen, zoals het leveringskanaal of label. |

   >[!NOTE]
   >
   >Standaard worden in elk menu alle velden in de geselecteerde tabel weergegeven (Ontvangers, Bericht / Aflevering). Als u velden wilt opnemen uit tabellen die zijn gekoppeld aan de geselecteerde tabel, schakelt u de optie **[!UICONTROL Display advanced attributes]** onder de lijst in.

1. Als u een verpersoonlijkingsveld wilt toevoegen, plaatst u de cursor op de gewenste locatie in de inhoud en klikt u op de knop `+` om deze in te voegen.

1. Wanneer de inhoud gereed is, kunt u deze opslaan en de rendering van de personalisatie testen door de inhoud te simuleren. In het onderstaande voorbeeld ziet u de personalisatie van een SMS-bericht met de voornamen van de ontvangers.

   ![](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Variabelen voor personalisatie gebruiken {#variables-personalization}

U kunt variabelen ook gebruiken om uw levering aan te passen.
Leer meer over [ toevoegend variabelen aan een levering ](../advanced-settings/delivery-settings.md#variables-delivery).

De variabele `deliveryType` wordt bijvoorbeeld als volgt gedefinieerd.

![](assets/variables-deliveryType.png){zoomable="yes"}

Deze variabele kan in de inhoud van de levering worden gebruikt, door het pictogram **[!UICONTROL Add Personalization]** en de expressie `<%= variables.deliveryType %>` voor ons voorbeeld te gebruiken.

![](assets/variables-perso.png){zoomable="yes"}

U kunt het gebruik van de variabele controleren met de knop **[!UICONTROL Simulate Content]** .

![](assets/variables-simulate.png){zoomable="yes"}
