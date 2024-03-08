---
audience: end-user
title: De deduplicatieworkflowactiviteit gebruiken
description: Leer hoe u de deduplicatieworkflowactiviteit kunt gebruiken
exl-id: 8efdc140-6cae-430d-b585-ff581993ff60
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 17%

---

# Deduplicatie {#deduplication}

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_fields"
>title="Velden om duplicaten te identificeren"
>abstract="In de **Velden om duplicaten te identificeren** klikt u op de **Kenmerk toevoegen** om de velden op te geven waarvoor de identieke waarden het mogelijk maken duplicaten te identificeren, zoals: e-mailadres, voornaam, achternaam, enz. In de volgorde van de velden kunt u opgeven welke velden eerst moeten worden verwerkt."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication"
>title="Deduplicatieactiviteit"
>abstract="De **Deduplicatie** Met activiteit kunt u duplicaten uit de resultaten van de binnenkomende activiteiten verwijderen. Het wordt meestal gebruikt na doelgerichte activiteiten en vóór activiteiten die het gebruik van gerichte gegevens mogelijk maken."

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_complement"
>title="Een complement genereren"
>abstract="U kunt een extra uitgaande overgang met de resterende bevolking produceren, die als duplicaat werd uitgesloten. Om dit te doen, knevel op **Complement genereren** option"

>[!CONTEXTUALHELP]
>id="acw_orchestration_deduplication_settings"
>title="Instellingen voor deduplicatie"
>abstract="Als u duplicaten van binnenkomende gegevens wilt verwijderen, definieert u de deduplicatiemethode in de onderstaande velden. Standaard wordt slechts één record bewaard. U moet ook de deduplicatiemodus selecteren op basis van een expressie of een kenmerk. Standaard wordt de record die buiten de duplicaten moet blijven, willekeurig geselecteerd."

De **Deduplicatie** activiteit is **Targeting** activiteit. Met deze activiteit kunt u duplicaten verwijderen uit het resultaat of de resultaten van de binnenkomende activiteiten, bijvoorbeeld gedupliceerde profielen in de lijst met ontvangers. De **Deduplicatie** de activiteit wordt doorgaans gebruikt na doelgerichte activiteiten en vóór activiteiten die het gebruik van gerichte gegevens mogelijk maken.

## De deduplicatieactiviteit configureren{#deduplication-configuration}

Voer de volgende stappen uit om de **Deduplicatie** activiteit:

![](../assets/workflow-deduplication.png)

1. Voeg een **Deduplicatie** activiteit aan uw werkschema.

1. In de **Velden om duplicaten te identificeren** klikt u op de **Kenmerk toevoegen** om de velden op te geven waarvoor de identieke waarden het mogelijk maken duplicaten te identificeren, zoals: e-mailadres, voornaam, achternaam, enz. In de volgorde van de velden kunt u opgeven welke velden eerst moeten worden verwerkt.

1. In de **Instellingen voor deduplicatie** selecteert u het aantal unieke **Duplicaten om te behouden**. De standaardwaarde voor dit veld is 1. Met de waarde 0 kunt u alle duplicaten behouden.

   Stel bijvoorbeeld dat records A en B worden beschouwd als duplicaten van record Y en dat een record C wordt beschouwd als duplicaat van record Z:

   * Als de waarde van het veld 1 is: alleen de records Y en Z blijven behouden.
   * Als de waarde van het veld 0 is: alle records blijven behouden.
   * Als de waarde van het veld 2 is: de records C en Z blijven behouden en twee records van A, B en Y blijven behouden, bij toeval of afhankelijk van de daarna geselecteerde deduplicatiemethode.

1. Selecteer de **Deduplicatiemethode** te gebruiken:

   * **Willekeurige selectie**: hiermee selecteert u willekeurig de record die u uit de duplicaten wilt verwijderen.
   * **Expressies gebruiken**: hiermee kunt u de records bijhouden waarin de waarde van de ingevoerde expressie het kleinst of het grootst is.
   * **Na een lijst met waarden**: hiermee kunt u een waardeprioriteit voor een of meer velden definiëren. Klik op **Kenmerk** als u een veld wilt selecteren of een expressie wilt maken, voegt u de waarde(n) toe aan de desbetreffende tabel. Klik op de knop Toevoegen boven de lijst met waarden om een nieuw veld te definiëren.

1. Controleer de **Complement genereren** als u de overblijvende bevolking wilt uitbuiten. Het complement bestaat uit alle duplicaten. Er wordt dan een aanvullende overgang toegevoegd aan de activiteit.

## Voorbeeld{#deduplication-example}

In het volgende voorbeeld gebruikt u een deduplicatie-activiteit om duplicaten uit te sluiten van het doel voordat u een levering verzendt. De geïdentificeerde gedupliceerde profielen worden toegevoegd aan een specifiek publiek dat indien nodig opnieuw kan worden gebruikt. Kies de optie **E-mail** adres om de duplicaten te identificeren. 1 item behouden en selecteer de optie **Willekeurig** deduplicatiemethode.

![](../assets/workflow-deduplication-example.png)
