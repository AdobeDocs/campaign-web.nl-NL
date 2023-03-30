---
title: Uw inhoud aanpassen in campagne
description: Leer hoe u uw inhoud kunt aanpassen in de gebruikersinterface van Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
exl-id: d1fd20c1-6835-4727-b20e-6e365a7aaa04
source-git-commit: b85bf75da466502e4579a061c02a2c4ce4361cd5
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# Uw inhoud aanpassen{#add-personalization}

![](../assets/do-not-localize/badge.png)

U kunt de inhoud van het bericht aanpassen door:

* Dynamisch invoegen **personalisatievelden**

   De gebieden van de verpersoonlijking worden gebruikt voor verpersoonlijking op het eerste niveau van uw berichten. U kunt om het even welk gebied selecteren beschikbaar in het gegevensbestand van de verpersoonlijkingsredacteur. Voor een levering, kunt u om het even welk gebied selecteren met betrekking tot de ontvanger, het bericht of de levering. Deze verpersoonlijkingsattributen kunnen in de onderwerpregel of het lichaam van uw berichten worden opgenomen.

   ![](assets/perso-subject-line.png)

   De volgende syntaxis voegt de plaats van de ontvanger in uw inhoud in: &lt;%= receiving.location.city %>.

* Vooraf gedefinieerde invoegen **inhoudsblokken**

   De campagne wordt geleverd met een reeks verpersoonlijkingsblokken die een specifieke rendering bevatten die u in uw leveringen kunt invoegen. U kunt bijvoorbeeld een logo, een wensbericht of een koppeling naar de spiegelpagina van het bericht toevoegen. Inhoudsblokken zijn beschikbaar bij een speciale vermelding in de personalisatie-editor.

   ![](assets/perso-content-blocks.png)
<!--
* Create **conditional content**

    Configure conditional content to add dynamic personalization based on the recipient’s profile for example. Text blocks and/or images are inserted when a particular condition is true.
-->

## De onderwerpregel van de e-mail aanpassen {#personalize-subject-line}

Om verpersoonlijking in toe te voegen **[!UICONTROL Subject line]** Voer in het veld van het bericht de onderstaande stappen uit:

1. Klik op de knop **Dialoogvenster voor aanpassen openen** pictogram rechts van **Onderwerpregel** veld.
1. Voer de inhoud van de onderwerpregel in en selecteer de personalisatiekenmerken die u wilt toevoegen.
1. Klikken **Bevestigen** om te valideren. De personalisatiekenmerken worden toegevoegd aan de onderwerpregel.

![](assets/perso-subject.png)

## Uw e-mailinhoud aanpassen {#personalize-emails}

Als u de e-mailinhoud wilt aanpassen, opent u het bericht in de e-mailontwerper en:

1. Klik in een tekstblok.
1. Selecteer in de contextafhankelijke werkbalk **Aanpassing toevoegen**.

   ![](assets/perso-add-to-content.png)

1. Voeg de naam van de ontvanger in de verpersoonlijkingseditor in en bevestig deze.

   ![](assets/perso-add-name.png)

   Het personalisatiekenmerk wordt toegevoegd aan de e-mailinhoud.

   U kunt de inhoud simuleren om de rendering te controleren. [Meer informatie](../preview-test/preview-content.md)

   ![](assets/perso-rendering.png)

Als u een inhoudsblok aan uw e-mail wilt toevoegen, voert u dezelfde stappen uit en selecteert u een inhoudsblok van het laatste pictogram:

![](assets/perso-insert-block.png)

Nadat het inhoudsblok is ingevoegd, wordt het toegevoegd aan de e-mailinhoud, zoals hieronder wordt weergegeven. Het wordt automatisch aangepast aan het ontvankelijke profiel wanneer de verpersoonlijking, bij de leveringsvoorbereidingsstap wordt geproduceerd.

![](assets/perso-content-block-in-email.png)


Ingebouwde inhoudsblokken zijn:

* **[!UICONTROL Enabled by Adobe Campaign]**: voegt het logo &quot;Enabled by Adobe Campaign&quot; in.
* **[!UICONTROL Formatting function for proper nouns]**: genereert de **[!UICONTROL toSmartCase]** De functie Javascript, die de eerste letter van elk woord in hoofdletters verandert.
* **[!UICONTROL Greetings]**: voegt begroetingen met de volledige naam van de ontvanger in, gevolgd door een komma. Voorbeeld: &quot;Hallo JanDoe,&quot;.
* **[!UICONTROL Insert logo]**: voegt een logo in dat in de instantie-instellingen is gedefinieerd.
* **[!UICONTROL Link to mirror page]**: voegt een koppeling in naar de [spiegelpagina](../content/mirror-page.md). Standaardindeling is: &quot;Klik hier als je dit bericht niet juist kunt weergeven.&quot;
* **[!UICONTROL Mirror page URL]**: voegt de URL van de spiegelpagina in, waardoor de leveringsontwerpers de koppeling kunnen controleren.
* **[!UICONTROL Offer acceptance URL in unitary mode]**: voegt een URL in waarmee een aanbieding kan worden ingesteld op **[!UICONTROL Accepted]**. (Dit blok is beschikbaar als de module van de Interactie wordt toegelaten)
* **[!UICONTROL Registration confirmation]**: voegt een koppeling in waarmee u het abonnement kunt bevestigen.
* **[!UICONTROL Registration link]**: voegt een abonnementkoppeling in. Deze koppeling wordt gedefinieerd in de instantie-instellingen. De standaardinhoud is: &quot;Klik hier om te registreren.&quot;
* **[!UICONTROL Registration link (with referrer)]**: voegt een abonnementkoppeling in, waarmee de bezoeker en de levering kunnen worden geïdentificeerd. Deze koppeling wordt gedefinieerd in de instantie-instellingen.
* **[!UICONTROL Registration page URL]**: voegt een abonnement-URL in
* **[!UICONTROL Style of content emails]** en **[!UICONTROL Notification style]**: genereren code waarmee een e-mailbericht wordt opgemaakt met vooraf gedefinieerde HTML-stijlen.
* **[!UICONTROL Unsubscription link]**: voegt een koppeling in waarmee u zich kunt afmelden bij alle leveringen (lijst van gewezen personen). De standaard gekoppelde inhoud is: &quot;U ontvangt dit bericht omdat u contact hebt gehad met ***uw organisatienaam*** of een gelieerde. Als u geen berichten meer wilt ontvangen van ***uw organisatienaam*** klik hier.&quot;



## Koppelingen in e-mails aanpassen {#personalize-links}

Een **link**:

1. Selecteer een tekstblok of een afbeelding.
1. Selecteer in de contextafhankelijke werkbalk **Koppeling invoegen**.

   ![](assets/perso-link.png)

1. Voer het koppelingslabel in en gebruik de **Koppeling invoegen** om de koppeling aan te passen.

   ![](assets/perso-link-insert-icon.png)

1. Gebruik de verpersoonlijkingsredacteur om de verbinding te bepalen en te personaliseren, en te bevestigen.

   ![](assets/perso-link-edit.png)


## Je aanbiedingen aanpassen {#personalize-offers}

U kunt tot de verpersoonlijkingsredacteur ook toegang hebben wanneer het toevoegen van tekst-type inhoud aan uw aanbiedingen&#39; vertegenwoordiging. Meer informatie in [deze sectie](../content/offers.md).
