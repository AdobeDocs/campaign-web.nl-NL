---
audience: end-user
title: Inhoud-experimenten maken
description: Leer hoe u experimenten met inhoud maakt in Adobe Campaign Web
exl-id: 476aaaef-c4b2-4007-a050-9b88460435a6
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---

# Inhoud-experimenten maken {#content-experiment}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Inhoudsexperimenten - A/B-tests"
>abstract="U kunt nu meerdere leveringsvarianten definiëren om te testen welke het beste presteert. Wijzig de inhoud, het onderwerp of de afzender in e-mailelementen om de beste resultaten te bepalen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=nl-NL" text="Zie opmerkingen bij releases"

## Informatie over contentexperimenten {#about-content-experiment}

Met contentexperimenten in Adobe Campaign Web kunt u meerdere leveringsvarianten voor A/B-tests definiëren om te meten welke het beste voor uw doelpubliek presteert. U kunt de leveringsinhoud, het onderwerp, of de afzender variëren om verschillende versies te testen en te bepalen welke variant de beste resultaten veroorzaakt.

U kunt A/B tests op diverse e-mailelementen uitvoeren zoals:

* **Onderwerpregel van het Onderwerp**: test verschillende e-mailonderwerpregel om te zien welke het hoogste open tarief produceert
* **naam van de Afzender**: experiment met verschillende afzendercombinaties
* **de lichaamsinhoud van de e-mail**: creeer veelvoudige inhoudsversies om te identificeren welke aandrijving de beste klik-door tarief drijft

>[!NOTE]
>
>* Experimenten met inhoud zijn momenteel alleen beschikbaar voor e-mailkanalen.
>* A/B het testen wordt niet gesteund voor transactionele berichten.
>* Maximaal 3 behandelingen (varianten) per experiment.

## Een inhoudexperiment maken {#create-content-experiment}

Voer de volgende stappen uit om een inhoudexperiment toe te voegen aan uw e-maillevering:

1. Maak een e-maillevering of open een bestaande conceptlevering. [&#x200B; Leer hoe te om een e-mail &#x200B;](create-email.md) tot stand te brengen

1. Klik op de knop **[!UICONTROL Create experiment]** in de sectie **[!UICONTROL Content]** vanaf de pagina met eigenschappen voor e-maillevering.

   ![&#x200B; Schermafbeelding die de Create experimenteerknop in e-maileigenschappen toont &#x200B;](assets/ab-testing-1.png){zoomable="yes"}

## De experimentele instellingen configureren {#configure-experiment}

Configureer uw experiment met behulp van de volgende secties:

![&#x200B; Schermafbeelding die de Experimentele montages &#x200B;](assets/ab-testing-2.png){zoomable="yes"} toont

### Instellingen voor publiek {#audience-settings}

Bepaal het percentage van uw doelpopulatie dat de experimentele varianten zal ontvangen.

Voer een waarde in om de publieksgrootte in te stellen. Dit is het aantal ontvangers dat tijdens de testfase een van de experimentele varianten zal ontvangen.

* **Minimum**: 1%
* **Maximum**: 100%
* **Gebrek**: 10%

Het resterende publiek (standaard 90%) ontvangt de winnende variant zodra het experiment is voltooid en een winnaar wordt bepaald.

Met bijvoorbeeld een doelpubliek van 10.000 ontvangers en een doelgrootte van 10% worden 1.000 ontvangers willekeurig geselecteerd om deel te nemen aan het experiment. De overige 9000 ontvangers zullen de winnende variant ontvangen nadat het experiment is beëindigd.

### Winningsstrategie {#winning-strategy}

Selecteer metrisch die zal worden gebruikt om de het winnen variant te bepalen:

* **[!UICONTROL Best open rate]** (standaardwaarde): de variant met het hoogste percentage e-mailberichten wordt geopend
* **[!UICONTROL Best click-through rate]**: de variant met het hoogste percentage klikken in de e-mail wint
* **[!UICONTROL Weakest unsubscription rate]**: de variant met het laagste percentage niet-geabonneerde wins

Het systeem volgt deze metriek tijdens het experiment automatisch en berekent welke variant het best volgens uw geselecteerd criterium presteert.

### Verzendmethode voor Winner {#sending-method}

Bepaal hoe lang het experiment moet lopen en selecteer de verzendende methode:

1. Voer de waarde voor de duur in uren in. Het experiment zal gedurende deze periode lopen alvorens de winnende variant te bepalen.

   * **Minimum**: 3 uren
   * **Maximum**: 240 uren (10 dagen)
   * **Gebrek**: 24 uren

   >[!NOTE]
   >
   >Zorg ervoor dat de duur van het experiment lang genoeg is om zinvolle gegevens te verzamelen. Een korte duur kan niet voldoende statistische significantie opleveren, vooral voor metriek zoals klikdoorsnelheid die langer kan duren om zich te accumuleren.

1. Kies hoe de winnende variant naar de resterende populatie moet worden verzonden:

   * **[!UICONTROL Automatic sending]** geactiveerd: het systeem stuurt de winnende variant automatisch naar het resterende publiek zodra het experiment is beëindigd.
   * **[!UICONTROL Automatic sending]** gedeactiveerd: u moet handmatig op de knop **[!UICONTROL Send]** klikken om de winnende variant te verzenden nadat u de resultaten van het experiment hebt bekeken.

Als geen enkele variant aan het eind van het experiment significant betere resultaten bereikt dan de andere, stuurt het systeem de eerste variant naar de resterende populatie. Zie deze [&#x200B; sectie &#x200B;](#send-deliveries).

## De inhoudsbehandelingen definiëren {#define-content}

Nadat u de instellingen voor het experiment hebt opgeslagen, wordt standaard een eerste behandeling gemaakt. U moet nu andere behandelingen (maximaal drie) toevoegen en de specifieke inhoud ervan definiëren.

1. Klik op **[!UICONTROL Edit content]** in de leveringseigenschappen. De behandelingen worden links weergegeven.

   ![&#x200B; Schermafbeelding die het paneel van inhoudexperimenten toont &#x200B;](assets/ab-testing-3.png){zoomable="yes"}

1. Klik op de knop **[!UICONTROL Add treatment]** en definieer de naam ervan. Herhaal deze bewerking voor alle behandelingen die u wilt toevoegen. Vervolgens kunt u de naam wijzigen, de naam dupliceren en verwijderen.

1. Klik op elke behandeling en pas de volgende items aan:

   * **naam van de Afzender**: Pas aan wie e-mail van schijnt te zijn
   * **Onderwerpregel**: Schrijf een unieke onderwerpregel voor elke behandeling
   * **E-maillichaam**: Ontwerp verschillende inhoudsversies gebruikend e-mail Designer

   ![&#x200B; Schermafbeelding die verscheidene behandelingen tonen &#x200B;](assets/ab-testing-4.png){zoomable="yes"}

1. Geef een voorvertoning van elke behandeling weer door op de behandeling te klikken en vervolgens op **[!UICONTROL Simulate content]** te klikken.

## Start het experiment en controleer de resultaten {#validate-start}

Nadat u al uw inhoudsbehandelingen hebt gedefinieerd, kunt u het experiment valideren en starten.

1. Klik in de leveringseigenschappen op **[!UICONTROL Review and send]** en klik vervolgens op **[!UICONTROL Prepare]** .

1. Klik vervolgens op **[!UICONTROL Start experimentation]** om de A/B-test te starten.

   ![&#x200B; Schermafbeelding die de knoop van het begin experimenteren &#x200B;](assets/ab-testing-5.png){zoomable="yes"} tonen

1. Wanneer uw experiment is uitgevoerd, controleert u de verschillende meetgegevens die worden weergegeven in het dashboard voor levering.

Tijdens het experiment kunt u op **[!UICONTROL Stop sending]** klikken om het experiment te beëindigen. U kunt ook besluiten om handmatig te verzenden vóór het einde van het experiment door op **[!UICONTROL Select and send to winner]** te klikken.

>[!NOTE]
>
>De resultaten worden in bijna real-time bijgewerkt wanneer de ontvangers met uw e-mail communiceren. Vroege resultaten zijn echter wellicht niet statistisch significant. U wordt aangeraden te wachten tot de duur van het experiment is voltooid voordat u definitieve beslissingen neemt.

## De leveringen verzenden {#send-deliveries}

Verzenden kan automatisch of handmatig worden uitgevoerd, afhankelijk van wat u hebt gekozen in de instellingen van **[!UICONTROL Winner sending method]** . Zie deze [&#x200B; sectie &#x200B;](#sending-method).

### Automatisch verzenden {#automatic-sending}

Voor automatisch verzenden analyseert het systeem de resultaten op basis van uw winnende strategie en bepaalt het de winnende behandeling. De winnende behandeling wordt automatisch naar het resterende publiek verzonden. Als er geen duidelijke winnaar is gevonden, wordt de eerste variant gekozen.

### Handmatig verzenden {#manual-sending}

Als u handmatig verzenden hebt geconfigureerd, controleert u de resultaten wanneer het experiment eindigt en klikt u op **[!UICONTROL Send]** om de winnende behandeling te verzenden. Als er geen duidelijke winnaar uit de bus komt, wordt de eerste behandeling standaard geselecteerd, maar u kunt een andere kiezen.

## Uiteindelijke resultaten weergeven {#final-results}

Nadat het experiment is voltooid en de levering volledig is verzonden, hebt u toegang tot uitgebreide rapporten:

1. Klik op **[!UICONTROL Reports]** van het leveringdashboard.

1. Navigeer naar het rapporttabblad **[!UICONTROL Experiments]** om de belangrijkste prestatiegegevens voor elke behandeling weer te geven.

## Best practices {#best-practices}

Houd rekening met de volgende aanbevelingen wanneer u experimenten met inhoud maakt:

* **Test één element tegelijkertijd**: Voor duidelijkste resultaten, test variaties van één enkel element (b.v., onderwerpregel slechts, of inhoud slechts) eerder dan veelvoudige elementen gelijktijdig.

* **kies aangewezen duur**: Toestaan genoeg tijd voor statistische betekenis:
   * Voor open-snelheidstests is 12-24 uur meestal voldoende
   * Voor doorkliksnelheidstests: 24-48 uur of meer nodig
   * Grotere doelgroepen hebben mogelijk minder tijd nodig; kleinere doelgroepen hebben mogelijk langer nodig

* **Grootte uw publiek geschikt**:
   * Zorg ervoor dat het aantal deelnemers aan het experiment (het percentage dat aan het testen is toegewezen) groot genoeg is voor betekenisvolle resultaten
   * Algemene richtlijn: minimum van 1.000 ontvangers per behandeling voor betrouwbare resultaten

* **Test regelmatig maar niet bovenmatig**: Voer experimenten op belangrijke campagnes uit, maar vermijd het testen elk enkel verzendt om middelen op impactful besluiten te concentreren.

* **Document uw lessen**: houd verslagen van proefresultaten om toekomstige campagnestrategieën te informeren.

## Verwante onderwerpen {#related-topics}

* [Uw eerste e-mail maken](create-email.md)
* [E-mailinhoud configureren](edit-content.md)
* [Een e-mail voorvertonen en verzenden](../monitor/prepare-send.md)
* [E-mailleveringsrapporten](../reporting/email-report.md)
