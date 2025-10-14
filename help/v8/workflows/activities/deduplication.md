---
audience: end-user
title: De deduplicatieworkflowactiviteit gebruiken
description: Leer hoe u de deduplicatieworkflowactiviteit kunt gebruiken
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 6%

---

# Deduplicatie {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Velden om duplicaten te identificeren"
>abstract="In de **Gebieden om duplicaten** sectie te identificeren, klik **voegt attribuut** knoop toe om de gebieden te specificeren waarvoor de identieke waarden duplicaten toestaan om, zoals e-mailadres, voornaam, en achternaam worden geïdentificeerd. De volgorde van de velden geeft aan welke velden eerst moeten worden verwerkt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Deduplicatieactiviteit"
>abstract="De **Deduplicatie** activiteit schrapt duplicaten in de resultaten van binnenkomende activiteiten. Het wordt meestal gebruikt na gerichte activiteiten en vóór activiteiten die gerichte gegevens gebruiken."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Een complement genereren"
>abstract="U kunt een extra uitgaande overgang produceren met de resterende bevolking uitgesloten als duplicaten. Om dit te doen, op **van een knevel te voorzien produceert complement** optie."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Instellingen voor deduplicatie"
>abstract="Als u duplicaten van binnenkomende gegevens wilt verwijderen, definieert u de deduplicatiemethode in de onderstaande velden. Standaard wordt slechts één record bewaard. Selecteer de deduplicatiemodus op basis van een expressie of een kenmerk. Standaard wordt de record die buiten de duplicaten moet blijven, willekeurig geselecteerd."

De **Deduplicatie** activiteit is a **richtend** activiteit. Deze activiteit schrapt duplicaten in de resultaten van binnenkomende activiteiten, zoals gedupliceerde profielen in de ontvankelijke lijst. De **Deduplicatie** activiteit wordt over het algemeen gebruikt na het richten van activiteiten en vóór activiteiten die gerichte gegevens gebruiken.

## De deduplicatieactiviteit configureren {#deduplication-configuration}

Voer de volgende stappen uit om de **Deduplication** -activiteit te configureren:

![&#x200B; de configuratieproces van de deduplicatie van het Werkschema &#x200B;](../assets/workflow-deduplication.png)

1. Voeg de activiteit van de a **Deduplicatie** aan uw werkschema toe.

1. In de **Gebieden om duplicaten** sectie te identificeren, klik **voegt attribuut** knoop toe om de gebieden te specificeren waarvoor de identieke waarden duplicaten toestaan om, zoals e-mailadres, voornaam, en achternaam worden geïdentificeerd. De volgorde van de velden geeft aan welke velden eerst moeten worden verwerkt. [&#x200B; Leer hoe te om attributen te selecteren en hen toe te voegen aan favorieten &#x200B;](../../get-started/attributes.md).

1. In de **montages van de Deduplicatie** sectie, selecteer het aantal unieke **Duplicaten om** te houden. De standaardwaarde voor dit veld is 1. Met de waarde 0 blijven alle duplicaten behouden.

   Bijvoorbeeld, als de verslagen A en B als duplicaten van verslag Y worden beschouwd, en verslag C als duplicaat van verslag Z wordt beschouwd:

   * Als de waarde van het veld 1 is: alleen de records Y en Z blijven behouden.
   * Als de waarde van het veld 0 is: alle records blijven behouden.
   * Als de waarde van het veld 2 is: de records C en Z worden bewaard en twee records van A, B en Y worden, toevallig of afhankelijk van de geselecteerde deduplicatiemethode, bewaard.

1. Selecteer de **methode van de Deduplicatie** aan gebruik:

   * **Willekeurige selectie**: Selecteert willekeurig het verslag om uit de duplicaten te houden.
   * **Gebruikend een uitdrukking**: Houdt de verslagen waarin de waarde van de ingegaan uitdrukking kleinste of grootste is.
   * **Niet-lege waarden**: Houdt de verslagen waarvoor de uitdrukking niet leeg is.
   * **na een lijst van waarden**: Bepaalt een waardeprioriteit voor één of meerdere gebieden. Om de waarden te bepalen, klik **Attribuut** om een gebied te selecteren of een uitdrukking tot stand te brengen, dan de waarden in de aangewezen lijst toe te voegen. Om een nieuw gebied te bepalen, klik **voeg** knoop toe die boven de lijst van waarden wordt gevestigd.

1. Controleer **aanvult** optie om de resterende bevolking te exploiteren. Het complement bestaat uit alle duplicaten. Vervolgens wordt een aanvullende overgang toegevoegd aan de activiteit.

## Voorbeeld {#deduplication-example}

In het volgende voorbeeld gebruikt u een deduplicatie-activiteit om duplicaten uit te sluiten van het doel voordat u een levering verzendt. De geïdentificeerde gedupliceerde profielen worden toegevoegd aan een specifiek publiek dat indien nodig opnieuw kan worden gebruikt. Kies het **E-mail** adres om de duplicaten te identificeren. Houd 1 ingang en selecteer de **Willekeurige** deduplicatiemethode.

![&#x200B; Voorbeeld van deduplicatieactiviteit in een werkschema &#x200B;](../assets/workflow-deduplication-example.png)