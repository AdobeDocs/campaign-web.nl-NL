---
title: Uw inhoud aanpassen in campagne
description: Leer hoe u uw inhoud kunt aanpassen in de gebruikersinterface van Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positief"
source-git-commit: 17a6b7af67cfc9ded7f98c9497a5242cbb9e5d47
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 0%

---


# Uw inhoud aanpassen {#add-personalization}

Personalisatie kan aan om het even welke levering worden toegevoegd gebruikend de uitdrukkingsredacteur, die op elke gebieden met **[!UICONTROL Open personalization dialog]** -pictogram, zoals het veld voor de onderwerpregel, of e-mailkoppelingen en componenten voor tekst/knopinhoud. [Leer waar u dynamische inhoud wilt toevoegen](gs-personalization.md/#access)

## Personalisatiesyntaxis {#syntax}

Voor een personalisatietag wordt altijd de volgende syntaxis gebruikt: `<%=table.field%>`. Als u bijvoorbeeld de naam van de ontvanger wilt invoegen, die is opgeslagen in de tabel met ontvangers, gebruikt de personalisatietag de syntaxis &lt;%= receiver.lastName %>.

Wanneer een levering wordt voorbereid, worden deze markeringen automatisch geïnterpreteerd door Adobe Campaign en door de waarde van het gebied voor een bepaalde ontvanger vervangen. De fysieke vervanging kan dan worden bekeken wanneer het simuleren van uw inhoud.

## Aanpersonalisatietags toevoegen {#add}

Als u personalisatietags wilt toevoegen aan een levering, opent u de expressieeditor met de **[!UICONTROL Open personalization dialog]** pictogram dat toegankelijk is vanuit tekstbewerkingsvelden, zoals de onderwerpregel of de SMS-tekst. [Leer waar u dynamische inhoud wilt toevoegen](gs-personalization.md/#access)

![](assets/perso-access.png)

De uitdrukkingsredacteur toont. De gebieden van de aanpassing worden georganiseerd in drie menu&#39;s, die links van het scherm worden gevestigd. Deze menu&#39;s geven toegang tot alle velden die beschikbaar zijn in de Adobe Campaign-database.

![](assets/perso-insert-field.png)

| Menu | Beschrijving |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | De **[!UICONTROL Recipient]** worden alle velden weergegeven die in de tabel met ontvangers zijn gedefinieerd, zoals de naam, de leeftijd of het adres van de ontvangers. |
| ![](assets/do-not-localize/perso-message-menu.png) | De **[!UICONTROL Message]** worden alle velden weergegeven die betrekking hebben op de leveringslogboeken, d.w.z. alle berichten die naar ontvangers of apparaten worden verzonden via alle kanalen, zoals de datum van de laatste gebeurtenis met een bepaalde ontvanger |
| ![](assets/do-not-localize/perso-delivery-menu.png) | De **[!UICONTROL Delivery]** worden alle velden weergegeven die betrekking hebben op de parameters die vereist zijn voor het uitvoeren van leveringen, zoals het leveringskanaal, label, enz. |

>[!NOTE]
>
>Standaard worden in elk menu alle velden in de geselecteerde tabel weergegeven (Ontvangers, Bericht / Aflevering). Als u velden wilt opnemen uit tabellen die zijn gekoppeld aan de geselecteerde tabel, schakelt u de optie **[!UICONTROL Display advanced attributes]** onder de lijst.

Als u een verpersoonlijkingsveld wilt toevoegen, plaatst u de cursor op de gewenste locatie in de inhoud en klikt u op + om het veld in te voegen.

Wanneer de inhoud gereed is, kunt u deze opslaan en de rendering van de personalisatie testen door de inhoud te simuleren. In het onderstaande voorbeeld personaliseren we een SMS-bericht met de voornamen van de beoogde profielen.

*Voeg de personalisatiemarkering in de berichtinhoud toe*

![](assets/perso-preview1.png)

*Simuleer de weergave van de personalisatie voor een bepaald testprofiel*

![](assets/perso-preview2.png)
