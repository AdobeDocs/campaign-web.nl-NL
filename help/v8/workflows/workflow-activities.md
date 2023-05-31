---
audience: end-user
title: Werken met workflowactiviteiten
description: Meer informatie over workflowactiviteiten
badge: label="Alpha" type="Positief"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: ebd119a38129f8576ad9b4e4b9301b116a255c9b
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 7%

---


# Workflowactiviteiten {#workflow-activities}

## Targetingactiviteiten {#targeting}

Met deze activiteiten kunt u een of meer doelen maken door sets te definiëren en deze sets te splitsen of te combineren met behulp van doorsnede-, samenvoegings- of uitsluitingsbewerkingen.

### publiek opbouwen {#build-audience}

Met deze activiteit kunt u een publiek definiëren. U kunt of een bestaande kandidaat van de Campagne selecteren of de regelbouwer gebruiken om uw eigen vraag te bepalen.

<!--
The **Build audience** activity can be placed at the beginning of the workflow or after any other activity. Any activity can be placed after the **Build audience**.
-->

Voer de volgende stappen uit om de **publiek opbouwen** activiteit:

1. Voeg een de publieksactiviteit van de Bouwstijl toe.
1. Definieer een label.
1. Bepaal het publiekstype: **Maak uw eigen** of **Lees publiek**.

Voer de volgende extra stappen uit om uw eigen query te maken:

1. Selecteren **Uw eigen (query) maken**.
1. Kies de optie **Doeldimensie**. Met de doeldimensie kunt u de doelgroep voor de bewerking definiëren: ontvangers, begunstigden van contracten, exploitanten, abonnees, enz. Standaard is het doel geselecteerd bij de ontvangers. Zie de [v8-documentatie](https://experienceleague.adobe.com/docs/campaign/automation/workflows/introduction/wf-type/targeting-workflows.html#targeting-and-filtering-dimensions){target="_blank"}.
1. Klikken **Doorgaan**.
1. Gebruik de bouwer van de regel om uw vraag te bepalen, de zelfde manier u creeert een publiek wanneer het ontwerpen van een nieuwe e-mail. Zie dit [sectie](../audience/segment-builder.md).

Voer de volgende stappen uit om een bestaand publiek te selecteren:

1. Selecteren **Lees publiek**.
1. Klikken **Doorgaan**.
1. Selecteer uw publiek, zoals u een publiek gebruikt bij het ontwerpen van een nieuwe e-mail. Zie dit [sectie](../audience/add-audience.md).

### Combineren {#combine}

Deze activiteit staat u toe om reeksen op binnenkomende gegevens te verwerken. U kunt dus meerdere populaties combineren, een deel ervan uitsluiten of gegevens alleen gemeenschappelijk houden voor verschillende doelen. Hier volgen de beschikbare segmentatietypen:

<!--
The **Combine** activity can be placed after any other activity, but not at the beginning of the workflow. Any activity can be placed after the **Combine**.
-->

* De **Unie** staat u toe om het resultaat van veelvoudige activiteiten in één enkel doel te hergroeperen.
* De **Intersectie** Hiermee kunt u alleen de elementen behouden die gemeenschappelijk zijn voor de verschillende binnenkomende populaties in de activiteit.
* De **Uitsluiting** kunt u elementen op basis van bepaalde criteria uitsluiten van één populatie.

Voer de volgende stappen uit om de **Combineren** activiteit:

1. Voeg uw **Combineren** activiteit aan om het even welke vorige segmentatieovergangen.
1. Selecteer het segmentatietype: samenvoegen, doorsnijden of uitsluiten.
1. Klikken **Doorgaan**.
1. In de **Stelt in om te verbinden** , controleert u alle vorige activiteiten waaraan u wilt deelnemen.

Voor de **Unie** en **Intersectie** selecteert u de **Type afstemming** om te bepalen hoe duplicaten worden verwerkt:

    * Alleen toetsen: dit is de standaardmodus. De activiteit behoudt slechts één element wanneer elementen van de verschillende binnenkomende overgangen dezelfde sleutel hebben. Deze optie kan alleen worden gebruikt als de binnenkomende populaties homogeen zijn.
    * Een selectie van kolommen: Selecteer deze optie om de lijst met kolommen te definiëren waarop de afstemming van gegevens wordt toegepast. U moet eerst de primaire set (de set met de brondata) selecteren en vervolgens de kolommen die u voor de samenvoeging wilt gebruiken.

Voor de **Intersectie** en **Uitsluiting**, kunt u de **Voltooiing genereren** als u de resterende populatie wilt verwerken. Het complement zal de samenvoeging bevatten van de resultaten van alle binnenkomende activiteiten min de doorsnede. Een extra uitgaande overgang zal dan aan de activiteit worden toegevoegd.

Voor de **Uitsluiting**, selecteert u de **Primaire set** van de binnenkomende overgangen, in **Stelt in om te verbinden** sectie. Dit is de set waaruit elementen worden uitgesloten. De andere sets komen overeen met de elementen voordat deze worden uitgesloten van de primaire set.

### Verrijking {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Verrijkingsactiviteit"
>abstract="Met de verrijkingsactiviteit kunt u de doelgegevens verbeteren met aanvullende informatie uit de database. Het wordt vaak gebruikt in een werkstroom na het richten van activiteiten.<br/>Zodra de verrijkingsgegevens aan het werkschema zijn toegevoegd, kan het in de activiteiten worden gebruikt die na de activiteit van de Verrijking worden toegevoegd om klanten in verschillende groepen te segmenteren die op hun gedrag, voorkeur, en behoeften worden gebaseerd, of om gepersonaliseerde marketing berichten en campagnes te creëren die eerder met uw doelpubliek zullen resoneren."

Met de verrijkingsactiviteit kunt u de doelgegevens verbeteren met aanvullende informatie uit de database. Het wordt vaak gebruikt in een werkstroom na het richten van activiteiten.

Verrijkingsgegevens kunnen worden verkregen:

* **Van dezelfde werktabel** als doelversie in uw workflow:

   *Stel een groep klanten in en voeg het veld Geboortedatum toe aan de huidige tabel*

* **Van een andere werktabel**:

   *Selecteer een groep klanten en voeg de velden Bedrag en Type product uit de tabel Aankoop toe*.

Zodra de verrijkingsgegevens aan het werkschema zijn toegevoegd, kan het dan in de activiteiten worden gebruikt die na de activiteit van de Verrijking worden toegevoegd om klanten in verschillende groepen te segmenteren die op hun gedrag, voorkeur, en behoeften worden gebaseerd, of om gepersonaliseerde marketing berichten en campagnes te creëren die eerder met uw doelpubliek zullen resoneren.

U kunt bijvoorbeeld informatie over aankopen van klanten toevoegen aan de werkstroomwerktabel en deze gegevens gebruiken om de e-mails aan te passen aan de laatste aankoop of het bedrag dat aan deze aankopen is besteed.

Voer de volgende stappen uit om een verrijkingsactiviteit toe te voegen aan uw workflow:

1. activiteit toevoegen
1. kenmerk selecteren dat moet worden gebruikt als verrijkingsgegevens

   Optie Geavanceerde velden weergeven i-knop

   opmerking: kenmerken van de doeldimensie

1. Selecteer hoe de gegevens worden verzameld
1. aantal records dat moet worden opgehaald als u een verzameling van meerdere records wilt ophalen
1. Filters toepassen en regel bouwen

   Selecteer een bestaand filter om het filter op te slaan, zodat u de weergaveresultaten van het filter visueel of in de codeweergave kunt hergebruiken

1. records sorteren met een kenmerk

hefboomwerking verrijkingsgegevens in campagne

waar we de verrijkingsgegevens kunnen gebruiken : e-mail, andere gebruiksgevallen personaliseren?

## Kanaalactiviteiten {#channel}

Met Adobe Campaign Web kunt u marketingcampagnes automatiseren en uitvoeren op meerdere kanalen, zoals e-mail, SMS of push. Met Adobe Campaign-workflows kunt u kanaalactiviteiten combineren tot het canvas om kanaalworkflows te maken die acties op basis van klantgedrag kunnen activeren.

U kunt bijvoorbeeld een welkomstcampagne voor e-mail maken met een reeks berichten via verschillende kanalen, zoals e-mail, SMS en push. U kunt ook een e-mail verzenden nadat een klant een aankoop heeft voltooid of een gepersonaliseerd verjaardagsbericht via SMS naar een klant sturen.

Door kanaalactiviteiten te gebruiken, kunt u uitvoerige, gepersonaliseerde campagnes tot stand brengen die klanten over veelvoudige touchpoints en aandrijvingsomzettingen in dienst nemen.

Kanaalactiviteiten zijn beschikbaar in het palet, links op het scherm, in de sectie Kanalen.

### Email {#email}

beschrijving, die het geval gebruikt u kunt uitvoeren (gemeenschappelijke andere activiteiten die u voor van na de activiteit kunt verbinden)

hoe te om de activiteit toe te voegen en te vormen

voorbeeld van een geconfigureerde activiteit binnen een workflow


Met de activiteit E-mail verzenden kunt u het verzenden van een e-mail configureren in een workflow.

<!-- Scheduled emails available?

This can be a single send email and sent just once, or it can be a recurring email.
* Single send emails are standard emails, sent once.
* Recurring emails allow you to send the same email multiple times to different targets over a defined period. You can aggregate the deliveries per period in order to get reports that correspond to your needs.

When linked to a scheduler, you can define recurring emails.-->

E-mailontvangers worden vóór de activiteit in dezelfde workflow gedefinieerd via een doelactiviteit voor het publiek.

<!--The message preparation is triggered according to the workflow execution parameters. From the message dashboard, you can select whether to request or not a manual confirmation to send the message (required by default). You can start the workflow manually or place a scheduler activity in the workflow to automate execution.-->


### Sms {#sms}

### Pushmelding (Android) {#push-android}

### Pushmelding (iOS) {#push-ios}

## Stroombeheeractiviteiten {#flow-control}

inhoud-TBD

<!--à reformuler-->Met deze activiteiten kunt u een of meer doelen maken door sets te definiëren en deze sets te splitsen of te combineren met behulp van doorsnede-, samenvoegings- of uitsluitingsbewerkingen.

De activiteiten van de debietcontrole worden gebruikt om de werkschemaactiviteiten te coördineren.

### Vertakking {#fork}

### AND-join {#join}


### Wachten {#wait}

### Einde {#end}

## Data-managementactiviteiten {#data-management}

overzicht: waarvoor ze worden gebruikt, zodat u met hen kunt werken

lijst beschikbare activiteiten + korte beschrijving + verwijzing naar sectie

