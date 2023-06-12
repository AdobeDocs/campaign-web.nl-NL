---
title: Aan de slag met dynamische inhoud
description: Leer hoe u uw inhoud dynamisch kunt maken met behulp van verpersoonlijking, voorwaardelijke inhoud en ingebouwde inhoudsblokken.
audience: automating
content-type: reference
topic-tags: workflow-general-operation
context-tags: workflow,overview;workflow,main
feature: Workflows
role: Data Architect
level: Intermediate
source-git-commit: bf5ff77b695a5a8584bad7784597bf1521bcb23e
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Aan de slag met dynamische inhoud

Het leveren van relevante inhoud aan uw klanten is zeer belangrijk om ervoor te zorgen dat u tot een verscheidenheid van klanten en u hun interesse richt zodat uw marketing inhoud wordt gelezen.

Om optimaal te profiteren van elke marketingcampagne, biedt Adobe Campaign u een manier om een aangepaste ervaring voor verschillende groepen en individuen te creëren door aangepaste dynamische inhoud te leveren die aan klanten op hun niveau spreekt door de informatie die u over hen hebt verzameld te benutten.

* **Je berichten personaliseren** aan elke specifieke ontvanger door profielgegevens zoals hun voornaam, belangen, waar zij wonen, wat zij hebben gekocht, en nog veel meer te gebruiken.

  U kunt om het even welk gebied selecteren beschikbaar in het gegevensbestand van de verpersoonlijkingsredacteur met betrekking tot de ontvanger, het bericht of de levering. Deze verpersoonlijkingsattributen kunnen in de onderwerpregel of het lichaam van uw berichten worden opgenomen. De volgende syntaxis voegt de plaats van de ontvanger in uw inhoud in: &lt;%= receiving.location.city %>.

  ![](assets/perso-subject-line.png){width="800" align="center"}

* **Voorwaardelijke inhoud maken** om uw leveringen aan elke ontvanger aan te passen en slechts de inhoud te tonen die voor een bepaalde klant relevant is die op de informatie wordt gebaseerd u over hen hebt. Hierdoor kunt u specifieke tekstblokken en/of afbeeldingen op basis van voorwaarden weergeven. U kunt bijvoorbeeld een e-mailbanner op basis van het abonnement van de ontvangers aanpassen aan een specifieke service.

  ![](assets/condition-sample.png){width="800" align="center"}

* **Verpersoonlijkingsblokken gebruiken** om tijd en hefboomwerking gemakkelijk opnieuw te gebruiken gepersonaliseerde inhoud in uw berichten te besparen. De campagne wordt geleverd met een reeks verpersoonlijkingsblokken die een specifieke rendering bevatten die u in uw leveringen kunt invoegen. U kunt bijvoorbeeld een logo, een wensbericht of een koppeling naar de spiegelpagina van een e-mailbericht toevoegen. Inhoudsblokken zijn beschikbaar bij een speciale vermelding in de verpersoonlijkingseditor.

  ![](assets/content-blocks.png){width="800" align="center"}

## De expressie-editor openen {#access}

Adobe Campaign V8 Web verstrekt een uitdrukkingsredacteur waar u kunt selecteren, rangschikken, aanpassen en bevestigen alle gegevens om een aangepaste ervaring voor uw inhoud tot stand te brengen. De expressie-editor is beschikbaar voor alle kanalen, in alle velden met de **[!UICONTROL Open personalization dialog]** -pictogram, zoals het veld voor de onderwerpregel, of e-mailkoppelingen en componenten voor tekst/knopinhoud.

Hier volgen enkele voorbeelden van hoe u toegang krijgt tot de expressieeditor, afhankelijk van de inhoud die u dynamisch wilt maken:

* *De uitdrukkingsredacteur van het de naamgebied van de Afzender toegang hebben*

  ![](assets/expression-editor-access.png){width="800" align="center"}

* *De expressie-editor openen vanuit een e-mailtekstcomponent*

  ![](assets/expression-editor-access-email.png){width="800" align="center"}

* *Expressieeditor openen via een koppeling in een e-mailbericht*

  ![](assets/perso-link-insert-icon.png){width="800" align="center"}

>[!NOTE]
>
>Naast de expressie-editor kunt u ook een speciale, voorwaardelijke inhoudsontwikkelaar gebruiken bij het ontwerpen van een e-mail. [Meer informatie over het maken van voorwaardelijke inhoud in e-mails](conditions.md)

## Laten we dieper duiken

Nu u inzicht hebt in hoe te om uw inhoud dynamisch te maken, is het tijd om dieper in deze documentatiesecties te duiken beginnen met het werken met de eigenschap.

<table style="table-layout:fixed"><tr style="border: 0;">
<td>
<a href="personalize.md">
<img alt="Inhoud personaliseren" src="assets/do-not-localize/dynamic-personalization.jpg">
</a>
<div>
<a href="personalize.md"><strong>Aanpassing toevoegen</strong></a>
</div>
<p>
</td>
<td>
<a href="conditions.md">
<img alt="Lood" src="assets/do-not-localize/dynamic-conditional.jpg">
</a>
<div><a href="conditions.md"><strong>Voorwaardelijke inhoud toevoegen</strong>
</div>
<p>
</td>
<td>
<a href="content-blocks.md">
<img alt="Onfrequent" src="assets/do-not-localize/dynamic-content-blocks.jpg">
</a>
<div>
<a href="content-blocks.md"><strong>Ingebouwde inhoudsblokken toevoegen</strong></a>
</div>
<p></td>
</tr></table>
