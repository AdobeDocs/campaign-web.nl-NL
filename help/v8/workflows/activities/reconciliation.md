---
audience: end-user
title: De activiteit van de afstemmingsworkflow gebruiken
description: Leer hoe u de workflowactiviteit Verzoening gebruikt
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 3%

---

# Afstemming {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Afstemmingsactiviteit"
>abstract="De **Verzoening** activiteit is a **richtend** activiteit die het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in een het werklijst bepaalt. Bijvoorbeeld, kan de **Verzoening** activiteit na a **dossier** activiteit van de Lading worden geplaatst om niet-standaardgegevens in het gegevensbestand in te voeren. In dit geval, bepaalt de **Verzoening** activiteit het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in de externe lijst."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_field"
>title="Selectieveld Afstemmen"
>abstract="Selectieveld Afstemmen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_condition"
>title="Afstemming maken, voorwaarde"
>abstract="Afstemming maken, voorwaarde"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_complement"
>title="Afstemming genereren"
>abstract="Afstemming genereren"

De **Verzoening** activiteit is a **richtend** activiteit die het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in een het werklijst bepaalt, zoals gegevens die van een extern dossier worden geladen.

Bijvoorbeeld, kan de **Verzoening** activiteit na a **dossier** activiteit van de Lading worden geplaatst om niet-standaardgegevens in het gegevensbestand in te voeren. In dit geval, bepaalt de **Verzoening** activiteit het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in de het werklijst.

## Best practices {#reconciliation-best-practices}

Terwijl de **Verrijking** activiteit extra gegevens bepaalt om in uw werkschema (bijvoorbeeld, combinerend gegevens van veelvoudige reeksen of creërend verbindingen aan een tijdelijk middel) te verwerken, de **Verzoening** activiteit verbindt niet geïdentificeerde gegevens met bestaande middelen.

>[!NOTE]
>Voor afstemmingsbewerkingen moeten de gegevens van de gekoppelde afmetingen al in de database aanwezig zijn. Als u bijvoorbeeld een bestand met aankopen importeert waarin wordt aangegeven welk product is aangeschaft, op welk tijdstip en op welke client, het product en de client al in de database moeten bestaan.

## De afstemmingsactiviteit configureren {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Doeldimensie"
>abstract="Selecteer de nieuwe doeldimensie. Een dimensie definieert de doelpopulatie: ontvangers, app-abonnees, operators, abonnees en meer. Standaard is de huidige doeldimensie geselecteerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Afstemmingsregels"
>abstract="Selecteer afstemmingsregels voor deduplicatie. Om attributen te gebruiken, selecteer de **Eenvoudige attributen** optie en kies de bron en bestemmingsgebieden. Om uw eigen verzoeningsvoorwaarde tot stand te brengen gebruikend de vraagmodeler, selecteer de **Geavanceerde verzoeningsvoorwaarden** optie."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Werken met de querymodelfunctie"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Doeldimensie selecteren"
>abstract="Selecteer het richten afmeting voor uw binnenkomende gegevens met elkaar in overeenstemming te brengen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html#targeting-dimensions" text="Doelafmetingen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Niet-compatibele gegevens behouden"
>abstract="Standaard worden niet-compatibele gegevens bewaard in de uitgaande overgang en beschikbaar in de werktabel voor toekomstig gebruik. Om unconiled gegevens te verwijderen, deactiveer **houden unconiled gegevens** optie."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Afstemmingskenmerk"
>abstract="Selecteer het kenmerk dat u wilt gebruiken om gegevens met elkaar te verzoenen en klik op Bevestigen."

Volg deze stappen om de **Verzoening** activiteit te vormen:

1. Voeg a **Verzoening** activiteit aan uw werkschema toe. Deze activiteit moet volgen op een overgang met een bevolking waarvan de doelgerichtheid niet rechtstreeks uit Adobe Campaign afkomstig is.

1. Selecteer de nieuwe doeldimensie. Een dimensie definieert de doelpopulatie: ontvangers, app-abonnees, operators, abonnees en meer. [&#x200B; Leer meer over het richten van dimensies &#x200B;](../../audience/about-recipients.md#targeting-dimensions).

1. Selecteer de velden die u wilt gebruiken voor de afstemming. U kunt een of meer verzoeningscriteria gebruiken.

   1. Om attributen te gebruiken om gegevens te combineren, selecteer de **Eenvoudige attributen** optie. Het **Source** gebied maakt een lijst van de gebieden beschikbaar in de inputovergang, die met elkaar in overeenstemming moeten worden gebracht. Het **gebied van de Bestemming** beantwoordt aan de gebieden van geselecteerde het richten afmeting. De gegevens worden in overeenstemming gebracht wanneer de bron en het doel gelijk zijn. Bijvoorbeeld, selecteer de **E-mail** gebieden om profielen te dedupliceren die op hun e-mailadres worden gebaseerd.

      Om een ander verzoeningscriterium toe te voegen, klik **regel** knoop toevoegen. Als er meerdere samenvoegvoorwaarden zijn opgegeven, moeten deze allemaal worden gecontroleerd voordat de gegevens worden gekoppeld.

      ![&#x200B; voorbeeld van verzoeningscriteria &#x200B;](../assets/workflow-reconciliation-criteria.png)

   1. Om andere attributen te gebruiken om gegevens te combineren, selecteer de **Geavanceerde verzoeningsvoorwaarden** optie. U kunt dan uw eigen verzoeningsvoorwaarde tot stand brengen gebruikend de vraagmodeler. [&#x200B; Leer hoe te met de vraagmodelaar &#x200B;](../../query/query-modeler-overview.md) te werken.

1. De gegevens van de filter om het gebruiken van **te verzoenen leiden filter** knoop. Hiermee kunt u een aangepaste voorwaarde maken met behulp van de querymodelfunctie. [&#x200B; Leer hoe te met de vraagmodelaar &#x200B;](../../query/query-modeler-overview.md) te werken.

Standaard worden niet-compatibele gegevens bewaard in de uitgaande overgang en beschikbaar in de werktabel voor toekomstig gebruik. Om unconiled gegevens te verwijderen, deactiveer **houden unconiled gegevens** optie.

## Voorbeeld {#reconciliation-example}

In het volgende voorbeeld ziet u een workflow die een doelgroep van profielen rechtstreeks maakt op basis van een geïmporteerd bestand dat nieuwe klanten bevat. Het omvat de volgende activiteiten:

De workflow is als volgt ontworpen:

![&#x200B; voorbeeld van het Werkschema &#x200B;](../assets/workflow-reconciliation-sample-1.0.png)

Het wordt gebouwd met de volgende activiteiten:

* A [&#x200B; de dossieractiviteit van de Lading &#x200B;](load-file.md) uploadt een dossier dat profielgegevens bevat die uit een extern hulpmiddel worden gehaald.

  Bijvoorbeeld:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* A **de verzoening** activiteit identificeert de inkomende gegevens als profielen door **E-mail** en **Datum van geboorte** gebieden als verzoeningscriteria te gebruiken.

  ![&#x200B; het voorbeeld van de Verzoening activiteit &#x200B;](../assets/workflow-reconciliation-sample-1.1.png)

* A [&#x200B; sparen publiek &#x200B;](save-audience.md) activiteit leidt tot een nieuw publiek dat op deze updates wordt gebaseerd. U kunt **sparen publiek** activiteit met een **Eind** activiteit ook vervangen als geen specifiek publiek moet worden gecreeerd of worden bijgewerkt. Ontvangersprofielen worden in elk geval bijgewerkt wanneer u de workflow uitvoert.

## Compatibiliteit {#reconciliation-compat}

De **Verzoening** activiteit bestaat niet in de console van de Cliënt. Alle **Verrijking** activiteiten die in de console van de Cliënt met de toegelaten verzoeningsopties worden gecreeerd worden getoond als **Verzoening** activiteiten in het gebruikersinterface van het Web van de Campagne.