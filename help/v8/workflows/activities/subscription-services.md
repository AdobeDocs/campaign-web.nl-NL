---
audience: end-user
title: De activiteit van de Abonnementsservices gebruiken
description: Leer hoe u de workflowactiviteit voor abonnementenservices gebruikt
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 0e5b5e916309b2a337ac86f3741bcb83237b3fad
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 16%

---

# Abonnementsdiensten {#subscription-services}

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription"
>title="Activiteit abonnementsdiensten"
>abstract="De de dienstenactiviteit van de Abonnementsdiensten staat veelvoudige profielen toe om aan of van de dienst in één enkele actie worden geabonneerd te zijn."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_general"
>title="Algemene parameters voor de abonnementsservice"
>abstract="Kies de gewenste service en kies de actie die u wilt uitvoeren (abonnement of abonnement). In-/uitschakelen **Bevestigingsbericht verzenden** optie om de bevolking te laten weten dat zij geabonneerd zijn op of niet op de geselecteerde dienst zijn geabonneerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_outboundtransition"
>title="Een uitgaande overgang genereren"
>abstract="Schakelen tussen **Een uitgaande overgang genereren** om een overgang toe te voegen na de activiteit."

>[!CONTEXTUALHELP]
>id="acw_orchestration_subscription_additionalinfo"
>title="Aanvullende informatie"
>abstract="Aanvullende informatie"

De **Abonnementsdiensten** activiteit is **Gegevensbeheer** activiteit. Hiermee kunt u een abonnement op een informatieservice maken of verwijderen voor de populatie die is opgegeven in de overgang.

## Vorm de de dienstenactiviteit van het Abonnement {#subscription-services-configuration}

Voer de volgende stappen uit om de **Abonnementsdiensten** activiteit:

1. Voeg een **Abonnementsdiensten** in uw workflow. U kunt deze activiteit gebruiken na het richten van profielen of het invoeren van een dossier met geïdentificeerde gegevens.

1. Selecteer de service waarvoor u de abonnementen wilt beheren met een van de volgende opties:

   * **[!UICONTROL Select a specific service]**: Selecteer handmatig een service met de opdracht **[!UICONTROL Service]** veld.

   * **[!UICONTROL From inbound transition]**: Gebruik de service die is opgegeven in de binnenkomende overgang. U kunt bijvoorbeeld een bestand importeren dat de service opgeeft die voor elke regel moet worden beheerd. De service waarop de bewerking moet worden uitgevoerd, wordt vervolgens dynamisch geselecteerd voor elk profiel.

   ![](../assets/workflow-subscription-service.png)

1. Selecteer de uit te voeren bewerking: **Abonneren** of **Abonnement opzeggen**.

   Als de dienst in de binnenkomende overgang wordt bepaald, kunt u kiezen hoe te om deze verrichting terug te winnen:

   * **Een specifiek bewerkingstype selecteren**: Selecteer handmatig de bewerking die u wilt uitvoeren (**Abonneren** of **Abonnement opzeggen**)

   * **Selecteer een bewerkingstype uit een pad van een binnenkomende overgang**: Selecteer de kolom met de binnenkomende gegevens die de bewerking opgeeft die voor elke record moet worden uitgevoerd. U kunt bijvoorbeeld een bestand importeren dat de bewerking opgeeft die moet worden uitgevoerd voor elke regel in een kolom &quot;operation&quot;.

     U kunt hier alleen Booleaanse velden of velden met gehele getallen selecteren. Zorg ervoor dat de gegevens met de uit te voeren bewerking overeenkomen met deze indeling. Als u bijvoorbeeld gegevens laadt uit een activiteit van het ladingsdossier, controleer of u correct het formaat van de kolom hebt geplaatst die de verrichting in **[!UICONTROL Load file]** activiteit. Een voorbeeld wordt weergegeven in [deze sectie](#uc2).

     >[!CAUTION]
     >
     >Als u deze optie selecteert, worden standaard de **Abonnementsdiensten** activiteit verwacht dat er een koppelingsdefinitie naar de **Services (nms)** tabel die is ingesteld in de workflow. Om dit te doen, zorg ervoor u een verzoeningsverbinding in hebt gevormd **Verrijkingsactiviteit** naar boven in de workflow. Er is een voorbeeld beschikbaar waarin wordt getoond hoe u deze optie gebruikt [hier](#uc2).

   ![](../assets/workflow-subscription-service-inbound.png)

1. Als u ontvangers wilt laten weten dat ze zijn geabonneerd op of geen abonnement hebben op de geselecteerde service, schakelt u het **[!UICONTROL Send a confirmation message]** optie ingeschakeld. De inhoud van dit bericht wordt bepaald in een leveringsmalplaatje verbonden aan de informatiedienst.

1. Als u gegevens van een binnenkomende overgang gebruikt, **[!UICONTROL Additional information]** weergegeven, zodat u de gegevens en de oorsprong van het abonnement voor elke record kunt opgeven. U kunt deze sectie leeg laten, in welk geval er geen datum of oorsprong wordt ingesteld wanneer de workflow wordt uitgevoerd.

   * Als de binnenkomende gegevens een kolom bevatten die de abonnementdatum van het profiel aan de dienst aangeeft, kunt u het in de **[!UICONTROL Date]** veld.

   * In de **[!UICONTROL Origin path]** , geeft u de oorsprong van het abonnement op. U kunt het aan één van de gebieden van de binnenkomende gegevens of aan een constante waarde van uw keus plaatsen door **[!UICONTROL Set a constant as origin]** -optie.

   ![](../assets/workflow-subscription-service-additional.png)

1. Om een uitgaande overgang na de activiteit toe te voegen, knevel **[!UICONTROL Generate an outbound transition]** optie ingeschakeld.

## Voorbeelden {#example}

### Een publiek abonneren op een specifieke service {#uc1}

Deze workflow hieronder laat zien hoe u een publiek kunt abonneren op een bestaande service.

![](../assets/workflow-subscription-service-uc1.png)

* A **[!UICONTROL Build audience]** activiteit is gericht op een bestaand publiek .

* A **[!UICONTROL Subscription Services]** Met activiteit kunt u de service selecteren waarop de profielen moeten worden geabonneerd.

### Meerdere lidmaatschapsstatussen bijwerken vanuit een bestand {#uc2}

In de onderstaande workflow ziet u hoe u een bestand met profielen kunt importeren en hoe u hun abonnement kunt bijwerken naar verschillende services die in het bestand zijn opgegeven.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Load file]** Deze activiteit laadt een CSV-bestand met de gegevens en definieert de structuur van de geïmporteerde kolommen. De kolommen &quot;service&quot; en &quot;operation&quot; geven de service aan die moet worden bijgewerkt en de bewerking die moet worden uitgevoerd (abonnement of abonnement).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  Zoals u misschien hebt opgemerkt, wordt de bewerking in het bestand opgegeven als ‘sub’ of ‘unsub’. Het systeem verwacht dat een waarde **Boolean** of **Integer** de bewerking herkent die moet worden uitgevoerd: 0 voor uitschrijven en 1 voor inschrijven. Aan deze eis voldoen:
   * De **Gegevenstype** voor de kolom &quot;operation&quot; wordt ingesteld op integer.
   * A **Waarde opnieuw toewijzen** moet worden uitgevoerd om de waarden &quot;sub&quot; en &quot;unsub&quot; te laten overeenkomen met de waarden &quot;1&quot; en &quot;0&quot;.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  Als in uw bestand al 0 en 1 worden gebruikt om de bewerking te identificeren, hoeft u deze waarden niet opnieuw toe te wijzen. Alleen controleren of de kolom is verwerkt als een **Boolean** of **Geheel** in de kolommen van het voorbeeldbestand.

* Een activiteit **[!UICONTROL Reconciliation]** identificeert de data van het bestand als deel van de profieldimensie van de Adobe Campaign-database. De **email** wordt het veld van het bestand aangepast aan het **email** veld van de profielbron.

  ![](../assets/workflow-subscription-service-uc2-reconciliation.png)

* An **[!UICONTROL Enrichment]** de activiteit leidt tot een verzoeningsverbinding aan de lijst van de &quot;Diensten (nms)&quot;, met eenvoudig verbind tussen de &quot;dienst&quot;kolom van het geupload dossier, en de diensten &quot;interne naam&quot;gebied in het gegevensbestand.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Subscription Services]** geeft aan welke services moeten worden bijgewerkt als afkomstig van de overgang.

  Het **[!UICONTROL Operation type]** wordt geïdentificeerd als afkomstig van het veld **operation** van het bestand. U kunt hier alleen de velden Boolean of Integer selecteren. Als de kolom van het bestand dat de uit te voeren bewerking bevat, niet in de lijst voorkomt, moet u controleren of u de kolomindeling in de activiteit **[!UICONTROL Load file]** correct hebt ingesteld, zoals eerder in dit voorbeeld wordt uitgelegd.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)
