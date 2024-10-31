---
audience: end-user
title: De activiteit van de Abonnementsservices gebruiken
description: Leer hoe u de workflowactiviteit voor abonnementenservices gebruikt
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 5d13a654974b8a448c2bbaded46f9f6f5727682f
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 15%

---

# Abonnementsdiensten {#subscription-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Activiteit abonnementsdiensten"
>abstract="Met de activiteit Subscription services kunnen meerdere profielen in één actie worden geabonneerd op of afgemeld van een service."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Algemene parameters voor de abonnementsservice"
>abstract="Kies de gewenste service en kies de actie die u wilt uitvoeren (abonnement of abonnement). Knevel op **verzendt bevestigingsbericht** optie op om de bevolking mee te delen dat zij van de geselecteerde dienst geabonneerd of geabonneerd zijn."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Een uitgaande overgang genereren"
>abstract="Wissel **om een uitgaande overgang** optie te produceren om een overgang na de activiteit toe te voegen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="Aanvullende informatie"
>abstract="Geef de gegevens en de oorsprong van het abonnement voor elke record op. U kunt deze sectie leeg laten, in welk geval er geen datum of oorsprong wordt ingesteld tijdens het uitvoeren van de workflow. Als de binnenkomende gegevens een kolom bevatten die de abonnementsdatum van het profiel voor de service aangeeft, kunt u deze selecteren in het veld **[!UICONTROL Date]** . Definieer in het veld **[!UICONTROL Origin path]** de oorsprong van het abonnement. U kunt de eigenschap instellen op een van de velden van de binnenkomende gegevens of op een constante waarde van uw keuze door de optie **[!UICONTROL Set a constant as origin]** te selecteren."

De **activiteit van de diensten van het Abonnement van 0} is a** het Beheer van Gegevens **activiteit.** Hiermee kunt u een abonnement op een informatieservice maken of verwijderen voor de populatie die is opgegeven in de overgang.

## Vorm de de dienstenactiviteit van het Abonnement {#subscription-services-configuration}

Volg deze stappen om de **activiteit van de Diensten van het Abonnement** te vormen:

1. Voeg de diensten van het a **Abonnement** activiteit in uw werkschema toe. U kunt deze activiteit gebruiken nadat u zich hebt gericht op profielen of een bestand met geïdentificeerde gegevens hebt geïmporteerd.

1. Selecteer de service waarvoor u de abonnementen wilt beheren aan de hand van een van de volgende opties:

   * **[!UICONTROL Select a specific service]**: selecteer handmatig een service met het veld **[!UICONTROL Service]** .

   * **[!UICONTROL From inbound transition]**: gebruik de service die is opgegeven in de binnenkomende overgang. U kunt bijvoorbeeld een bestand importeren dat de service opgeeft die voor elke regel moet worden beheerd. De service waarop de bewerking moet worden uitgevoerd, wordt vervolgens dynamisch geselecteerd voor elk profiel.

   ![](../assets/workflow-subscription-service.png)

1. Selecteer de uit te voeren verrichting: **Abonneren** of **Unsubscribe**.

   Als de dienst in de binnenkomende overgang wordt bepaald, kunt u kiezen hoe te om deze verrichting terug te winnen:

   * **selecteer een specifiek verrichtingstype**: Selecteer manueel de uit te voeren verrichting (**Abonneren** of **Unsubscribe**)

   * **selecteer een verrichtingstype van een weg van binnenkomende overgang**: Selecteer de kolom van de binnenkomende gegevens die de verrichting om voor elk verslag specificeert uit te voeren. U kunt bijvoorbeeld een bestand importeren dat de bewerking aangeeft die voor elke regel moet worden uitgevoerd in een kolom &quot;bewerking&quot;.

     U kunt hier alleen Booleaanse velden of velden met gehele getallen selecteren. Zorg ervoor dat de gegevens met de uit te voeren bewerking overeenkomen met deze indeling. Als u bijvoorbeeld gegevens laadt uit een activiteit van het type Load file, controleert u of u de indeling van de kolom met de bewerking correct hebt ingesteld in de activiteit **[!UICONTROL Load file]** . Een voorbeeld wordt voorgesteld in [ deze sectie ](#uc2).

     >[!CAUTION]
     >
     >Door gebrek, als u deze optie selecteert, verwacht de **activiteit van de Abonnementendiensten** een verbindingsdefinitie aan de **Diensten (nms)** lijst opstelling in het werkschema te hebben. Om dit te doen, verzeker u een verzoeningsverbinding in een **activiteit van de Verrijking** omhoog in het werkschema hebt gevormd. Een voorbeeld dat toont hoe te om deze optie te gebruiken is beschikbaar [ hier ](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Schakel de optie **[!UICONTROL Send a confirmation message]** in als u ontvangers wilt laten weten dat ze zijn geabonneerd op of geen abonnement hebben op de geselecteerde service. De inhoud van deze melding wordt gedefinieerd in een leversjabloon die is gekoppeld aan de informatiedienst.

1. Als u gegevens uit een inkomende overgang gebruikt, wordt een **[!UICONTROL Additional information]** -sectie weergegeven waarin u de gegevens en de oorsprong van het abonnement voor elke record kunt opgeven. U kunt deze sectie leeg laten, in welk geval er geen datum of oorsprong wordt ingesteld tijdens het uitvoeren van de workflow.

   * Als de binnenkomende gegevens een kolom bevatten die de abonnementdatum van het profiel voor de service aangeeft, kunt u deze selecteren in het veld **[!UICONTROL Date]** .

   * Definieer in het veld **[!UICONTROL Origin path]** de oorsprong van het abonnement. U kunt dit instellen op een van de velden van de binnenkomende gegevens of op een constante waarde van uw keuze door de optie **[!UICONTROL Set a constant as origin]** te selecteren.

   ![](../assets/workflow-subscription-service-additional.png)

1. Als u een uitgaande overgang na de activiteit wilt toevoegen, schakelt u de optie **[!UICONTROL Generate an outbound transition]** in of uit.

## Voorbeelden {#example}

### Een doelgroep abonneren op een specifieke service {#uc1}

Deze workflow hieronder laat zien hoe u een publiek kunt abonneren op een bestaande service.

![](../assets/workflow-subscription-service-uc1.png)

* Een **[!UICONTROL Build audience]** -activiteit is gericht op een bestaand publiek.

* Met een **[!UICONTROL Subscription Services]** -activiteit kunt u de service selecteren waarop de profielen moeten worden geabonneerd.

### Meerdere lidmaatschapsstatussen bijwerken vanuit een bestand {#uc2}

In de onderstaande workflow ziet u hoe u een bestand met profielen kunt importeren en hoe u hun abonnement kunt bijwerken naar verschillende services die in het bestand zijn opgegeven.

![](../assets/workflow-subscription-service-uc2.png)

* Een **[!UICONTROL Load file]** -activiteit laadt een CSV-bestand met de gegevens en definieert de structuur van de geïmporteerde kolommen. De kolommen &quot;service&quot; en &quot;operation&quot; geven de service aan die moet worden bijgewerkt en de bewerking die moet worden uitgevoerd (abonnement of abonnement).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Zoals u misschien hebt opgemerkt, wordt de bewerking in het bestand opgegeven als ‘sub’ of ‘unsub’. Het systeem verwacht dat een waarde **Boolean** of **Integer** de bewerking herkent die moet worden uitgevoerd: 0 voor uitschrijven en 1 voor inschrijven. Aan deze vereiste voldoen:
   * Het **type van Gegevens** voor de &quot;verrichting&quot;kolom wordt geplaatst aan geheel.
   * A **opnieuw in kaart brengen van de Waarde** moet worden uitgevoerd om de &quot;sub&quot;en &quot;unsub&quot;waarden met &quot;1&quot;en &quot;0&quot;waarden aan te passen.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Als in uw bestand al 0 en 1 worden gebruikt om de bewerking te identificeren, hoeft u deze waarden niet opnieuw toe te wijzen. Zorg slechts ervoor dat de kolom als a **Van Boole** of **Geheel getal** in de kolommen van het steekproefdossier wordt verwerkt.

* Een activiteit **[!UICONTROL Reconciliation]** identificeert de data van het bestand als deel van de profieldimensie van de Adobe Campaign-database. Het **e-mail** gebied van het dossier wordt aangepast aan het **e-mail** gebied van het profielmiddel.

  ![](../assets/workflow-subscription-service-uc2-reconciliation.png)

* Een **[!UICONTROL Enrichment]** activiteit leidt tot een verzoeningsverbinding aan de lijst &quot;van de Diensten (nms)&quot;, met eenvoudige verbinding tussen de &quot;dienst&quot;kolom van het geupload dossier, en de de diensten &quot;interne naam&quot;gebied in het gegevensbestand.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Subscription Services]** identificeert de services die moeten worden bijgewerkt als zijnde afkomstig van de overgang.

  Het **[!UICONTROL Operation type]** wordt geïdentificeerd als afkomstig van het veld **operation** van het bestand. U kunt hier alleen de velden Boolean of Integer selecteren. Als de kolom van het bestand dat de uit te voeren bewerking bevat, niet in de lijst voorkomt, moet u controleren of u de kolomindeling in de activiteit **[!UICONTROL Load file]** correct hebt ingesteld, zoals eerder in dit voorbeeld wordt uitgelegd.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
