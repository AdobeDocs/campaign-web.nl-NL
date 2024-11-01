---
audience: end-user
title: De activiteit van de afstemmingsworkflow gebruiken
description: Leer hoe u de workflowactiviteit Verzoening gebruikt
exl-id: 33f2aa76-1e75-4545-805a-016c95824e09
source-git-commit: 935fba929c26d6d7b3057ee7c24148215a04e45e
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 10%

---

# Afstemming {#reconciliation}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation"
>title="Afstemmingsactiviteit"
>abstract="De **Verzoening** activiteit is a **richtend** activiteit die u toestaat om het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in een het werklijst te bepalen. Bijvoorbeeld, kan de **Verzoening** activiteit na a **dossier** activiteit van de Lading worden geplaatst om niet-standaardgegevens in het gegevensbestand in te voeren. In dit geval, laat de **Verzoening** activiteit u het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in de externe lijst bepalen."

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

De **Verzoening** activiteit is a **richtend** activiteit die u toestaat om het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in een het werklijst te bepalen, bijvoorbeeld gegevens die van een extern dossier worden geladen.

Bijvoorbeeld, kan de **Verzoening** activiteit na a **dossier** activiteit van de Lading worden geplaatst om niet-standaardgegevens in het gegevensbestand in te voeren. In dit geval, laat de **Verzoening** activiteit u het verband tussen de gegevens in het gegevensbestand van Adobe Campaign en de gegevens in de het werklijst bepalen.

## Best practices {#reconciliation-best-practices}

Terwijl de **Verrijking** activiteit u toestaat om extra gegevens te bepalen in uw werkschema (u kunt een **Verrijking** activiteit gebruiken om gegevens te combineren die uit veelvoudige reeksen komen, of verbindingen tot stand te brengen aan een tijdelijk middel), staat de **Verzoening** activiteit u toe om ongeidentificeerde gegevens aan bestaande middelen te verbinden.

>[!NOTE]
>De afstemmingsoperatie houdt in dat de gegevens van de gekoppelde afmetingen al in de database staan.  Als u bijvoorbeeld een aankoopbestand importeert waarin wordt aangegeven welk product is gekocht, op welk moment, door welke klant, enzovoort, moeten het product en de klant al in de database aanwezig zijn.

## De afstemmingsactiviteit configureren {#reconciliation-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting"
>title="Doeldimensie"
>abstract="Selecteer de nieuwe doeldimensie. Met een dimensie kunt u de doelgroep definiëren: ontvangers, abonnees van apps, operators, abonnees, enzovoort. Standaard is de huidige doeldimensie geselecteerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_rules"
>title="Afstemmingsregels"
>abstract="Selecteer afstemmingsregels die u wilt gebruiken voor de deduplicatie. Om attributen te gebruiken, selecteer de **Eenvoudige attributen** optie en kies de bron en bestemmingsgebieden. Om uw eigen verzoeningsvoorwaarde tot stand te brengen gebruikend de vraagmodeler, selecteer de **Geavanceerde verzoeningsvoorwaarden** optie."
>additional-url="https://experienceleague.adobe.com/en/docs/campaign-web/v8/query-database/query-modeler-overview" text="Werken met de querymodelfunctie"

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_targeting_selection"
>title="Doeldimensie selecteren"
>abstract="Selecteer het richten afmeting voor uw binnenkomende gegevens met elkaar in overeenstemming te brengen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/audiences/gs-audiences-recipients.html#targeting-dimensions" text="Doelafmetingen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_keep_unreconciled_data"
>title="Niet-compatibele gegevens behouden"
>abstract="Door gebrek, worden de niet in overeenstemming gebrachte gegevens gehouden in de uitgaande overgang en beschikbaar in de werklijst voor toekomstig gebruik. Om onverenigde gegevens te verwijderen, desactiveer **houden unconiled gegevens** optie."

>[!CONTEXTUALHELP]
>id="acw_orchestration_reconciliation_attribute"
>title="Afstemmingskenmerk"
>abstract="Selecteer het kenmerk dat u wilt gebruiken om gegevens op elkaar af te stemmen en klik op Bevestigen."

Volg deze stappen om de **Verzoening** activiteit te vormen:

1. Voeg a **Verzoening** activiteit in uw werkschema toe. Deze activiteit moet worden toegevoegd na een overgang met een populatie waarvan de doeldimensie niet rechtstreeks uit Adobe Campaign afkomstig is.

1. Selecteer de nieuwe doeldimensie. Met een dimensie kunt u de doelgroep definiëren: ontvangers, abonnees van apps, operators, abonnees, enzovoort. [ Leer meer over het richten van dimensies ](../../audience/about-recipients.md#targeting-dimensions).

1. Selecteer de velden die u wilt gebruiken voor de afstemming. U kunt een of meer verzoeningscriteria gebruiken.

   1. Om attributen te gebruiken om gegevens te combineren, selecteer de **Eenvoudige attributen** optie. Het **Source** gebied maakt een lijst van de gebieden beschikbaar in de inputovergang, die moeten worden in overeenstemming gebracht. Het **gebied van de Bestemming** beantwoordt aan de gebieden van geselecteerde het richten afmeting. De gegevens worden in overeenstemming gebracht wanneer bron en bestemming gelijk zijn. Bijvoorbeeld, selecteer de **E-mail** gebieden om profielen te dedupliceren die op hun e-mailadres worden gebaseerd.

      Om andere verzoeningscriteria toe te voegen, klik **regel** toevoegen knoop. Als er meerdere samenvoegvoorwaarden zijn opgegeven, moeten deze ALLES worden gecontroleerd zodat de gegevens aan elkaar kunnen worden gekoppeld.

      ![](../assets/workflow-reconciliation-criteria.png)

   1. Om andere attributen te gebruiken om gegevens te combineren, selecteer de **Geavanceerde verzoeningsvoorwaarden** optie. U kunt dan uw eigen verzoeningsvoorwaarde tot stand brengen gebruikend de vraagmodeler. [ Leer hoe te met de vraagmodelaar ](../../query/query-modeler-overview.md) te werken.

1. U kunt gegevens filtreren om het gebruiken van te verzoenen **creeer filterknoop**. Hiermee kunt u een aangepaste voorwaarde maken met behulp van de querymodelfunctie. [ Leer hoe te met de vraagmodelaar ](../../query/query-modeler-overview.md) te werken

Door gebrek, worden de niet in overeenstemming gebrachte gegevens gehouden in de uitgaande overgang en beschikbaar in de werkbare lijst voor toekomstig gebruik. Om onverenigde gegevens te verwijderen, desactiveer **houden unconiled gegevens** optie.

## Voorbeeld {#reconciliation-example}

In het volgende voorbeeld ziet u een workflow die een doelgroep van profielen rechtstreeks maakt op basis van een geïmporteerd bestand dat nieuwe klanten bevat. De workflow bestaat uit de volgende activiteiten:

De workflow is als volgt ontworpen:

![](../assets/workflow-reconciliation-sample-1.0.png)


Het wordt gebouwd met de volgende activiteiten:

* Met een activiteit [Bestand laden](load-file.md) uploadt u een bestand met profieldata die uit een extern hulpprogramma zijn geëxtraheerd.

  Bijvoorbeeld:

  ```
  lastname;firstname;email;birthdate;
  JACKMAN;Megan;megan.jackman@testmail.com;07/08/1975;
  PHILLIPS;Edward;phillips@testmail.com;09/03/1986;
  WEAVER;Justin;justin_w@testmail.com;11/15/1990;
  MARTIN;Babe;babeth_martin@testmail.net;11/25/1964;
  REESE;Richard;rreese@testmail.com;02/08/1987;
  ```

* A **Verzoening** activiteit die de inkomende gegevens als profielen identificeert, door **e-mail** en **Datum van geboorte** gebieden als verzoeningscriteria te gebruiken.

  ![](../assets/workflow-reconciliation-sample-1.1.png)

* A [ sparen publiek ](save-audience.md) activiteit om een nieuw publiek tot stand te brengen dat op deze updates wordt gebaseerd. U kunt **sparen publiek** activiteit door een **Eind** activiteit ook vervangen als geen specifiek publiek moet worden gecreeerd of worden bijgewerkt. Ontvangersprofielen worden in elk geval bijgewerkt wanneer u de workflow uitvoert.


## Compatibiliteit {#reconciliation-compat}

De **Verzoening** activiteit bestaat niet in de console van de Cliënt. Alle **Verrijkt** activiteiten die in de console van de Cliënt met de toegelaten verzoeningsopties worden gecreeerd worden getoond als **verzoenings** activiteiten in het gebruikersinterface van het Web van de Campagne.
