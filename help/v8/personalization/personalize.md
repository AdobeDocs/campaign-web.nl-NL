---
title: Uw inhoud aanpassen in campagne
description: Leer hoe u uw inhoud kunt aanpassen in de gebruikersinterface van Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
badge: label="Alpha" type="Positief"
source-git-commit: d12c3019fb47164864259ecc40225fcb04de0e6c
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Uw inhoud aanpassen{#add-personalization}

Personalisatie kan aan om het even welke levering worden toegevoegd gebruikend de uitdrukkingsredacteur.

Voor een personalisatietag wordt altijd de volgende syntaxis gebruikt: `<%=table.field%>`.Als u bijvoorbeeld de naam van de ontvanger wilt invoegen, die in de tabel met ontvangers is opgeslagen, gebruikt de personalisatietag de syntaxis &lt;%= receiver.lastName %>.

Wanneer een levering wordt voorbereid, worden deze markeringen automatisch geïnterpreteerd door Adobe Campaign en door de waarde van het gebied voor een bepaalde ontvanger vervangen. De fysieke vervanging kan dan worden bekeken wanneer het simuleren van uw inhoud.

Als u personalisatietags wilt toevoegen aan een levering, klikt u op het pictogram van het dialoogvenster Verpersoonlijking openen dat toegankelijk is vanuit tekstbewerkingsvelden, zoals de onderwerpregel of de SMS-tekst.

![](assets/perso-access.png)

De uitdrukkingsredacteur toont. De gebieden van de aanpassing worden georganiseerd in drie menu&#39;s, die links van het scherm worden gevestigd. Deze menu&#39;s geven toegang tot alle velden die beschikbaar zijn in de Adobe Campaign-database.

| Menu | Beschrijving |
|-----|------------|
| ![](assets/do-not-localize/perso-recipients-menu.png) | De **[!UICONTROL Recipient]** worden alle velden weergegeven die in de tabel met ontvangers zijn gedefinieerd, zoals de naam, de leeftijd of het adres van de ontvangers. |
| ![](assets/do-not-localize/perso-message-menu.png) | De **[!UICONTROL Message]** worden alle velden weergegeven die betrekking hebben op de leveringslogboeken, d.w.z. alle berichten die naar ontvangers of apparaten worden verzonden via alle kanalen, zoals de datum van de laatste gebeurtenis met een bepaalde ontvanger |
| ![](assets/do-not-localize/perso-delivery-menu.png) | De **[!UICONTROL Delivery]** worden alle velden weergegeven die betrekking hebben op de parameters die vereist zijn voor het uitvoeren van leveringen, zoals het leveringskanaal, label, enz. |

>[!NOTE]
>
>Standaard worden in de lijst alle velden in de geselecteerde tabel weergegeven (Ontvangers, Bericht / Aflevering). Als u velden wilt opnemen uit tabellen die zijn gekoppeld aan de geselecteerde tabel, schakelt u de optie **[!UICONTROL Display advanced attributes]** onder de lijst.

Als u een verpersoonlijkingsveld wilt toevoegen, plaatst u de cursor op de gewenste locatie in de inhoud en klikt u op + om het veld in te voegen.

![](assets/perso-insert-field.png)
