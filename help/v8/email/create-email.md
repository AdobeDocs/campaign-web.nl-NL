---
audience: end-user
title: Uw eerste e-mail maken
description: Campagne v8 Webdocumentatie
source-git-commit: cdddef89cda4fa39cee38e9d0171a6ea395537c7
workflow-type: tm+mt
source-wordcount: '911'
ht-degree: 1%

---

# Uw eerste e-mail verzenden {#first-email}

>[!NOTE]
>
>Deze documentatie is in opbouw en wordt regelmatig bijgewerkt. De definitieve versie van deze inhoud zal in Januari 2023 klaar zijn.

In dit geval wordt uitgelegd hoe u uw eerste e-mail maakt

In dit voorbeeld plannen we de verzending van een e-mail op een specifieke datum naar klanten met zilveren en gouden loyaliteit. Deze e-mail wordt ontworpen met behulp van een vooraf gedefinieerde HTML-sjabloon uit een ZIP-bestand en bevat personalisatie met profielkenmerken.

![](assets/delivery-list.png)

## E-mail maken {#create-email}

1. Een nieuwe levering maken via de **[!UICONTROL Deliveries]** -menu.
1. Selecteer **[!UICONTROL Email]** kanaal en de sjabloon die u wilt gebruiken en klik vervolgens op **[!UICONTROL Create]**.

   >[!NOTE]
   >
   >informatie over sjablonen. info controleren in V7 doc

   ![](assets/channel-template.png)

1. Verstrek een etiket voor de levering en vorm extra opties afhankelijk van uw behoeften:

   * Interne naam:
   * Map:
   * Leveringscode:
   * Beschrijving:
   * Aard:

   controleren welke montages in het malplaatje worden bepaald en hen vermelden (beschrijving? map?, natuur?)

   ![](assets/email-properties.png)

   >[!NOTE]
   >
   >info over de knop voor leveringsinstellingen + koppeling naar doc

## E-mailinhoud maken {#create-content}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Maak uw eerste e-mailinhoud met de e-mailontwerper."
>abstract="Uw eerste e-mailinhoud maken"

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_content"
>title="E-mailinhoud maken"
>abstract="TBC"

1. Klik op de knop **[!UICONTROL Edit content]** om de inhoud van uw e-mail te maken.

   In dit scherm kunt u de e-mailinhoud configureren en ontwerpen met de e-mailontwerper.

   ![](assets/edit-content.png)

   >[!NOTE]
   >
   >De Van naam en van e-mailinformatie worden vooraf bepaald in het geselecteerde e-mailmalplaatje.
   >
   >E-mailtracking is standaard ingeschakeld voor het openen en klikken. Als u deze opties wilt uitschakelen, heft u de selectie op in de sectie Optionele functies.

1. Geef het onderwerp van uw e-mail op met de Expressieeditor. [Leer hoe u uw inhoud kunt aanpassen](../personalization/personalize.md)

   In dit voorbeeld willen we de onderwerpregel personaliseren met de voornaam van het profiel.

   ![](assets/subject-line.png)

1. Voeg zo nodig een bijgevoegd bestand toe aan uw e-mail. Leer hoe u e-mailinhoud kunt bewerken

1. Klik op de knop **[!UICONTROL Edit email body]** om de inhoud van uw e-mail te maken en te ontwerpen.

   Kies de methode die u wilt gebruiken om uw e-mailinhoud te maken. In dit voorbeeld willen we bestaande HTML-inhoud importeren.

   ![](assets/import-html.png)

1. Selecteer het HTML- of ZIP-bestand dat u wilt importeren en klik op **[!UICONTROL Next]**.

   Als uw map elementen bevat, kiest u de instantie en map waarin deze moeten worden opgeslagen en klikt u op **[!UICONTROL Import]**. (+ koppeling naar document over middelen?)

   ![](assets/import-folder.png)

1. Nadat de inhoud is geïmporteerd, wordt deze weergegeven in de e-mailontwerper, zodat u deze desgewenst kunt bewerken en een persoonlijke voorkeur kunt toevoegen.

   In dit voorbeeld willen we personalisatie toevoegen aan de titel van de e-mail. Om dit te doen, selecteer het componentenblok dan klik **[!UICONTROL Add Personalization]**.

   ![](assets/add-perso.png)

1. Als de inhoud gereed is, slaat u deze op en klikt u op de pijl om terug te keren naar het scherm voor het maken van e-mail.

   ![](assets/save-content.png)

## De doelgroep definiëren {#define-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience"
>title="De doelgroep definiëren"
>abstract="TBC"

1. Klik op de knop **[!UICONTROL Select audience]** kiest u een bestaand publiek of maakt u een nieuw publiek.

   In dit voorbeeld willen we een bestaand publiek gebruiken dat zich richt op klanten die behoren tot het niveau van de zilveren- en goudloyaliteitspunten.

   ![](assets/create-audience.png)

   >[!NOTE]
   >
   >Het publiek dat in de lijst beschikbaar is, is afkomstig uit uw Campagne V8-instantie of uit Adobe Experience Platform als de integratie Doel/Bronnen op uw instantie is geïmplementeerd. Leer hoe u het e-mailpubliek kunt selecteren

1. Nadat u het publiek hebt geselecteerd, kunt u de regels indien nodig bewerken. U kunt ook een controlegroep instellen om het gedrag van de e-mailontvangers te analyseren in vergelijking met het gedrag van profielen die niet als doelprofielen werden gebruikt. Leer hoe u met besturingsgroepen werkt

## Plan de verzending {#schedule}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_schedule"
>title="Plan de verzending"
>abstract="TBC"

Als u het verzenden van de e-mail wilt plannen, klikt u op Inschakelen en geeft u de gewenste datum en tijd op.

= bevestig vóór verzendoptie: wat gebeurt er op de geplande datum : kennisgeving om de verzending van het bericht te bevestigen?

![](assets/schedule.png)

## E-mail voorvertonen en testen {#preview-test}

Zodra uw e-mail klaar is, kunt u een voorbeeld bekijken en testen voordat u de verzending start.

1. Klik op **[!UICONTROL Review to send]**. Een voorbeeld van uw e-mailvertoningen, samen met alle gevormde eigenschappen, publiek en programma. U kunt al deze elementen bewerken met de knop Wijzigen.

   ![](assets/review-email.png)

1. Klik op de knop **[!UICONTROL Simulate content]** om een voorbeeld van de e-mail te bekijken en proefdrukken te verzenden.

1. Selecteer in het linkergedeelte de profielen die u wilt gebruiken voor een voorvertoning van het e-mailbericht. U kunt doelprofielen of specifieke testprofielen gebruiken.

1. Een voorbeeld van de e-mail wordt weergegeven in het rechtergebied op basis van het geselecteerde profiel. Als u meerdere profielen hebt toegevoegd, kunt u tussen de profielen schakelen om een voorbeeld van de bijbehorende e-mail te bekijken.

   ![](assets/preview.png)

   >[!NOTE]
   >
   >Daarnaast worden de **[!UICONTROL Render email]** kunt u een voorbeeld van de e-mail bekijken met meerdere apparaten of e-mailproviders. Leer hoe u een voorbeeld van het renderen van e-mail kunt bekijken

1. Als u proefdrukken van uw e-mail wilt verzenden, klikt u op de knop **[!UICONTROL Test]** selecteert u vervolgens de profielen die de proefdruk ontvangen. In dit voorbeeld willen we de proefdrukken naar een specifiek testprofiel verzenden.

   ![](assets/proof-test-profile.png)

   >[!NOTE]
   >
   >U kunt uw berichten ook testen door u voor te doen met bepaalde profielen en het proefdrukbericht naar het e-mailadres van uw keuze te sturen. Leer hoe u Vervangend kunt gebruiken vanuit de doelmodus

1. Klikken **[!UICONTROL Send test email ]** bevestig vervolgens de verzending.

   Nadat de proefdrukken zijn verzonden, kunt u de status controleren door op de knop **[!UICONTROL View test email log]** knop.

## E-mail verzenden en controleren {#prepare-send}

Nadat u uw e-mail hebt bekeken en getest, kunt u de voorbereiding starten en verzenden.

1. Klikken **[!UICONTROL Prepare]** om de voorbereiding van het bericht te starten.

   U kunt de voortgang van de voorbereiding in real time volgen, samen met statistieken. Zodra de voorbereiding wordt voltooid, kunt u tot gedetailleerde logboeken voor verdere analyse toegang hebben. Leer hoe u leveringen kunt controleren

   ![](assets/preparation.png)

1. Klik op **[!UICONTROL Send]** bevestig vervolgens de verzending.

   U kunt het verzenden in real time, samen met statistieken volgen. Daarnaast worden de **[!UICONTROL Logs]** toegang tot gedetailleerde informatie over het verzenden van e-mail. Leer hoe u leveringen kunt controleren

   ![](assets/logs.png)

1. Nadat u het e-mailbericht hebt verzonden, kunt u speciale rapporten openen voor verdere analysedoeleinden.

   ![](assets/reports.png)
