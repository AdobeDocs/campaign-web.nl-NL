---
title: Uw inhoud aanpassen in campagne
description: Leer hoe u uw inhoud kunt aanpassen op Adobe Campaign Web
feature: Personalization
topic: Personalization
old-role: Data Engineer
role: Developer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: 85ebbbe1e318cf0561b33d4c14250cded6ffbc65
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Uw inhoud personaliseren {#add-personalization}

>[!CONTEXTUALHELP]
>id="acw_personalization_editor_add_current_date"
>title="Huidige datum toevoegen"
>abstract="Dit menu bevat functies die gerelateerd zijn aan de datumopmaak en die u kunt gebruiken om uw inhoud aan te passen."

Personalization van leveringsinhoud is een zeer belangrijke eigenschap die u toestaat om berichten aan individuele ontvangers aan te passen, die communicatie relevanter maken en aansprekend.

In Adobe Campaign, door [&#x200B; profielgegevens &#x200B;](#data-personalization) te gebruiken, zoals de naam, de plaats, of de voorbije interactie van het profiel, en specifieke [&#x200B; variabelen van uw levering &#x200B;](#variables-personalization), past u dynamisch elementen zoals tekst, beelden, en aanbiedingen in uw mededeling aan.

De personalisatie van de levering verbetert de gebruikerservaring en verbetert de betrokkenheidspercentages, wat leidt tot hogere conversie en klanttevredenheid.

## Profielgegevens gebruiken voor personalisatie {#data-personalization}

U kunt elke levering personaliseren met profielgegevens door de uitdrukkingsredacteur te gebruiken, die in gebieden met het **[!UICONTROL Open personalization dialog]** pictogram, zoals de onderwerpregel, e-mailverbindingen, en tekst/knoop inhoudcomponenten toegankelijk is. [&#x200B; Leer hoe te om tot de uitdrukkingsredacteur &#x200B;](gs-personalization.md#access) toegang te hebben.

### Personalization-syntaxis {#syntax}

Personalization-tags volgen een specifieke syntaxis: `<%= table.field %>` . Als u bijvoorbeeld de achternaam van de ontvanger wilt invoegen in de tabel met ontvangers, gebruikt u de syntaxis `<%= recipient.lastName %>` .

Tijdens de voorbereiding van de levering, interpreteert Adobe Campaign deze markeringen en vervangt hen met de overeenkomstige gebiedswaarden voor elke ontvanger. U kunt de daadwerkelijke vervanging bekijken door uw inhoud te simuleren.

Wanneer u contactpersonen uit een extern bestand uploadt voor een zelfstandige e-maillevering, zijn alle velden in het invoerbestand beschikbaar voor personalisatie. De syntaxis is als volgt: `<%= dataSource.field %>`.

### Aanpersonalisatietags toevoegen {#add}

Voer de volgende stappen uit om personalisatietags toe te voegen aan een levering:

1. Open de expressie-editor met het pictogram **[!UICONTROL Open personalization dialog]** , dat toegankelijk is vanuit tekstbewerkingsvelden, zoals de onderwerpregel of de SMS-inhoud. [&#x200B; Leer hoe te om tot de uitdrukkingsredacteur &#x200B;](gs-personalization.md#access) toegang te hebben.

   ![&#x200B; Schermafbeelding die tonen hoe te om tot de verpersoonlijkingsdialoog toegang te hebben &#x200B;](assets/perso-access.png){zoomable="yes"}{width="800" align="center"}

1. De expressie-editor wordt geopend. De gebieden van de verpersoonlijking beschikbaar in het gegevensbestand van Adobe Campaign worden georganiseerd in verscheidene menu&#39;s op de linkerkant van het scherm:

   ![&#x200B; Schermafbeelding die het menu van het verpersoonlijkingsgebied tonen &#x200B;](assets/perso-insert-field.png){zoomable="yes"}{width="800" align="center"}

   | Menu | Beschrijving |
   |------|-------------|
   | ![&#x200B; het menupictogram van het de toepassingsmenu van Abonnees &#x200B;](assets/do-not-localize/perso-subscribers-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Subscribers application]** bevat velden die betrekking hebben op de abonnees van een toepassing, zoals de gebruikte terminal of het besturingssysteem. *Dit menu is beschikbaar voor duw slechts berichten.* |
   | ![&#x200B; het menupictogram van Ontvangers &#x200B;](assets/do-not-localize/perso-recipients-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Recipient]** bevat velden die zijn gedefinieerd in de tabel met ontvangers, zoals namen, pagina&#39;s of adressen van ontvangers. Wanneer [&#x200B; het uploaden contacten van een extern dossier &#x200B;](../audience/file-audience.md) voor een standalone e-maillevering, maakt een lijst dit menu van alle gebieden beschikbaar in het inputdossier. |
   | ![&#x200B; het menupictogram van het Bericht &#x200B;](assets/do-not-localize/perso-message-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Message]** bevat velden die betrekking hebben op de leveringslogboeken, inclusief alle berichten die naar ontvangers of apparaten via alle kanalen worden verzonden, zoals de datum van de laatste gebeurtenis met een bepaalde ontvanger. |
   | ![&#x200B; het menupictogram van de Levering &#x200B;](assets/do-not-localize/perso-delivery-menu.png){zoomable="yes"} | Het menu **[!UICONTROL Delivery]** bevat velden die betrekking hebben op de parameters die vereist zijn voor het uitvoeren van leveringen, zoals het leveringskanaal of label. |

   >[!NOTE]
   >
   >Standaard worden in elk menu alle velden in de geselecteerde tabel weergegeven (Ontvangers, Bericht / Aflevering). Als u velden wilt opnemen uit tabellen die zijn gekoppeld aan de geselecteerde tabel, schakelt u de optie **[!UICONTROL Display advanced attributes]** onder de lijst in.

1. Als u een verpersoonlijkingsveld wilt toevoegen, plaatst u de cursor op de gewenste locatie in de inhoud en klikt u op de knop `+` om deze in te voegen.

1. Wanneer de inhoud gereed is, slaat u deze op en test u de rendering van de personalisatie door uw inhoud te simuleren. In het onderstaande voorbeeld ziet u de personalisatie van een SMS-bericht met de voornamen van de ontvangers.

   ![&#x200B; Schermafbeelding die de voorproef van de verpersoonlijking van SMS met de eerste naam van de ontvanger toont &#x200B;](assets/perso-preview1.png){zoomable="yes"}{width="800" align="center"}

   ![&#x200B; Schermafbeelding die de voorproef van de verpersoonlijking van SMS met de eerste naam van de ontvanger toont &#x200B;](assets/perso-preview2.png){zoomable="yes"}{width="800" align="center"}

## Variabelen voor personalisatie gebruiken {#variables-personalization}

U gebruikt ook variabelen om uw levering aan te passen. Leer meer over [&#x200B; toevoegend variabelen aan een levering &#x200B;](../advanced-settings/delivery-settings.md#variables-delivery).

De variabele `deliveryType` wordt bijvoorbeeld gedefinieerd zoals hieronder wordt weergegeven.

![&#x200B; Screenshot die de definitie van de variabele deliveryType &#x200B;](assets/variables-deliveryType.png){zoomable="yes"} toont

Deze variabele wordt gebruikt in de inhoud van de levering met behulp van het pictogram **[!UICONTROL Add Personalization]** en de expressie `<%= variables.deliveryType %>` voor dit voorbeeld.

![&#x200B; Schermschot die het gebruik van de variabele deliveryType in verpersoonlijking tonen &#x200B;](assets/variables-perso.png){zoomable="yes"}

Controleer het gebruik van de variabele met de knop **[!UICONTROL Simulate Content]** .

![&#x200B; Schermafbeelding die de simulatie van inhoud met veranderlijke deliveryType tonen &#x200B;](assets/variables-simulate.png){zoomable="yes"}