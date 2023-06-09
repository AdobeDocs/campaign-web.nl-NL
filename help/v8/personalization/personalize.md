---
title: Uw inhoud aanpassen in campagne
description: Leer hoe u uw inhoud kunt aanpassen in de gebruikersinterface van Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positief"
source-git-commit: 1e5bc39adfeae4f956fc208ef9763eb020552364
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---


# Uw inhoud aanpassen {#add-personalization}

U kunt elke levering personaliseren door de uitdrukkingsredacteur te gebruiken, die in gebieden met te gebruiken **[!UICONTROL Open personalization dialog]** -pictogram, zoals de onderwerpregel, e-mailkoppelingen en tekst-/knopinhoudcomponenten. [Leer hoe u toegang krijgt tot de expressie-editor](gs-personalization.md/#access)

## Personalisatiesyntaxis {#syntax}

Voor personalisatietags wordt een specifieke syntaxis gebruikt: `<%=table.field%>`. Als u bijvoorbeeld de achternaam van de ontvanger wilt invoegen in de tabel van de ontvanger, gebruikt u de opdracht `<%= recipient.lastName %>` syntaxis.

Tijdens de voorbereiding van de levering, interpreteert Adobe Campaign automatisch deze markeringen en vervangt hen met de overeenkomstige gebiedswaarden voor elke ontvanger. U kunt de daadwerkelijke vervanging bekijken door uw inhoud te simuleren.

## Aanpersonalisatietags toevoegen {#add}

Voer de volgende stappen uit om personalisatietags toe te voegen aan een levering:

1. De expressie-editor openen met de **[!UICONTROL Open personalization dialog]** pictogram dat toegankelijk is vanuit tekstbewerkingsvelden, zoals de onderwerpregel of de SMS-tekst. [Leer hoe u toegang krijgt tot de expressie-editor](gs-personalization.md/#access)

   ![](assets/perso-access.png)

1. De expressie-editor wordt geopend. De gebieden van de verpersoonlijking beschikbaar in het gegevensbestand van Adobe Campaign worden georganiseerd in verscheidene menu&#39;s op de linkerkant van het scherm:

![](assets/perso-insert-field.png)

| Menu | Beschrijving |
|-----|------------|
| ![](assets/do-not-localize/perso-subscribers-menu.png) | De **[!UICONTROL Subscribers application]** bevat velden die betrekking hebben op de abonnees van een toepassing, zoals de gebruikte terminal of het besturingssysteem. *Dit menu is alleen beschikbaar voor pushmeldingen* |
| ![](assets/do-not-localize/perso-recipients-menu.png) | De **[!UICONTROL Recipient]** worden de velden weergegeven die zijn gedefinieerd in de tabel met ontvangers, zoals namen, pagina&#39;s of adressen van ontvangers. |
| ![](assets/do-not-localize/perso-message-menu.png) | De **[!UICONTROL Message]** menu maakt een lijst van gebieden met betrekking tot de leveringslogboeken, met inbegrip van alle berichten die naar ontvangers of apparaten over alle kanalen worden verzonden, zoals de datum van de laatste gebeurtenis met een bepaalde ontvanger |
| ![](assets/do-not-localize/perso-delivery-menu.png) | De **[!UICONTROL Delivery]** bevat velden die betrekking hebben op de parameters die vereist zijn voor het uitvoeren van leveringen, zoals het leveringskanaal of label. |

>[!NOTE]
>
>Standaard worden in elk menu alle velden in de geselecteerde tabel weergegeven (Ontvangers, Bericht / Aflevering). Als u velden wilt opnemen uit tabellen die zijn gekoppeld aan de geselecteerde tabel, schakelt u de optie **[!UICONTROL Display advanced attributes]** onder de lijst.

1. Als u een verpersoonlijkingsveld wilt toevoegen, plaatst u de cursor op de gewenste locatie in de inhoud en klikt u op de knop `+` om het in te voegen.

1. Wanneer de inhoud gereed is, kunt u deze opslaan en de rendering van de personalisatie testen door de inhoud te simuleren. In het onderstaande voorbeeld ziet u de personalisatie van een SMS-bericht met de voornamen van de ontvangers.

   *Voeg de personalisatiemarkering in de berichtinhoud toe*

   ![](assets/perso-preview1.png)

   *Simuleer de weergave van de personalisatie voor een bepaald testprofiel*

   ![](assets/perso-preview2.png)
