---
audience: end-user
title: De activiteit van de Abonnementsservices gebruiken
description: Leer hoe u de workflowactiviteit voor abonnementenservices gebruikt
exl-id: 0e7c2e9a-3301-4988-ae0e-d901df5b84db
source-git-commit: 9cd2d3c7ac4c0ff3c9939cd43606400011fce739
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 3%

---

# Abonnementsdiensten {#subscriptipon-services}

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

     >[!NOTE]
     >
     >U kunt hier alleen Booleaanse velden of velden met gehele getallen selecteren. Zorg ervoor dat de gegevens met de uit te voeren bewerking overeenkomen met deze indeling. Als u bijvoorbeeld gegevens laadt uit een activiteit van het ladingsdossier, controleer of u correct het formaat van de kolom hebt geplaatst die de verrichting in **[!UICONTROL Load file]** activiteit. Een voorbeeld wordt weergegeven in [deze sectie](#uc2).

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

<!--
### Updating multiple subscription statuses from a file {#uc2}

The workflow below shows how to import a file containing profiles and update their subscription to several services specified in the file.

![](../assets/workflow-subscription-service-uc2.png)

* A **[!UICONTROL Load file]** activity loads a CSV file containing the data and defines the structure of the imported columns. The "service" and "operation" columns specify the service to update and the operation to perform (subscription or unsubscription).

  ```
  Lastname,firstname,city,birthdate,email,service,operation
  Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,yoga,sub
  Mars,Daniel,London,17/11/1999,danny.mars@example.com,running,sub
  Smith,Clara,Roma,08/02/1979,clara.smith@example.com,running,unsub
  Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,yoga,sub
  Durance,Alison,San Francisco,15/12/2000,allison.durance@example.com,running,unsub
  ```

  As you may have noticed, the operation is specified in the file as "sub" or "unsub". The system expects a **Boolean** or **Integer** value to recognize the operation to perform: "0" to unsubscribe and "1" to subscribe. To match this requirement, a remapping of values must be performed in the detail of the "operation" column in the sample file configuration screen.

  ![](../assets/workflow-subscription-service-uc2-mapping.png)

  If your file already uses "0" and "1" to identify the operation, you don't need to remap those values. Only make sure that the column is processed as a **Boolean** or **Integer** in the sample file columns.

* A **[!UICONTROL Reconciliation]** activity identifies the data from the file as belonging to the profile dimension of the Adobe Campaign database. The **email** field of the file is matched to the **email** field of the profile resource.

  ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* An **[!UICONTROL Enrichment]** activity creates a link to the "Services (nms)" table and creates a simple join between the "service" column of the uploaded file, and the services "internal name" field in the database.

    ![](../assets/workflow-subscription-service-uc2-enrichment.png)

* A **[!UICONTROL Deduplication]** based on the **email** field identifies duplicates. It is important to eliminate duplicates since the subscription to a service will fail for all data in case of duplicates.

  ![](../assets/workflow-subscription-service-uc2-dedup.png)
  
* A **[!UICONTROL Subscription Services]** identifies the services to update as coming from the transition, through the link created in the **[!UICONTROL Reconciliation]** activity.

  The **[!UICONTROL Operation type]** is identified as coming from the **operation** field of the file. Only Boolean or Integer fields can be selected here. If the column of your file that contains the operation to perform does not appear in the list, make sure that you have correctly set your column format in the **[!UICONTROL Load file]** activity, as explained earlier in this example.

  ![](../assets/workflow-subscription-service-uc2-subscription.png)-->
