---
audience: end-user
title: De deduplicatieworkflowactiviteit gebruiken
description: Leer hoe u de deduplicatieworkflowactiviteit kunt gebruiken
badge: label="Beta"
source-git-commit: 0c6369c8099831dca1e0d38dbed818f3c7ab1867
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 12%

---


# Deduplicatie {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Vorkactiviteit"
>abstract="Met de deduplicatieactiviteit kunt u..."

Met de activiteit Deduplicatie kunt u duplicaten in het resultaat of de resultaten van de binnenkomende activiteiten verwijderen.

De deduplicatieactiviteit wordt over het algemeen gebruikt na gerichte activiteiten en vóór activiteiten die het gebruik van gerichte gegevens mogelijk maken.

## Configuratie

Voer de volgende stappen uit om de **Planner** activiteit:

1. Voeg een **Deduplicatie** activiteit aan uw werkschema.

1. In de **Velden om duplicaten te identificeren** klikt u op de **Kenmerk toevoegen** om aan te geven voor welke velden de identieke waarden het mogelijk maken de duplicaten te identificeren: e-mailadres, voornaam, achternaam, enz. In de volgorde van de velden kunt u opgeven welke velden eerst moeten worden verwerkt.

1. Selecteer het aantal unieke **Duplicaten om te behouden**. De standaardwaarde voor dit veld is 1. Met de waarde 0 kunt u alle duplicaten behouden.

<!--
    For example, if records A and B are considered duplicates of record Y, and a record C is considered as a duplicate of record Z:

    * If the value of the field is 1: only the Y and Z records are kept.
    * If the value of the field is 0: all the records are kept.
    * If the value of the field is 2: records C and Z are kept and two records from A, B, and Y are kept, by chance or depending on the deduplication method selected thereafter.

-->

1. Selecteer de **Deduplicatiemethode** te gebruiken:

   * **Willekeurige selectie**: hiermee selecteert u willekeurig de record die u uit de duplicaten wilt verwijderen.
   * **Expressies gebruiken**: hiermee kunt u de records bijhouden waarin de waarde van de ingevoerde expressie het kleinst of het grootst is. ++ expression ++ Soort
   * **Na een lijst met waarden**: hiermee kunt u een waardeprioriteit voor een of meer velden definiëren. Klik op **Kenmerk** als u een veld wilt selecteren of een expressie wilt maken, voegt u de waarde(n) toe aan de desbetreffende tabel. Klik op de knop Toevoegen boven de lijst met waarden om een nieuw veld te definiëren. ++ sorteren

1. Controleer de **Complement genereren** als u de overblijvende bevolking wilt uitbuiten. Het complement bestaat uit alle duplicaten. Er wordt dan een aanvullende overgang toegevoegd aan de activiteit.
