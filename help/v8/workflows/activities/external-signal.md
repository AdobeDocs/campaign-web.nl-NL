---
audience: end-user
title: De externe signaalactiviteit gebruiken
description: Leer hoe u de activiteit van de externe signaalworkflow kunt gebruiken
source-git-commit: 575219c7bcef303e211f504d13227183933924cc
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Extern signaal {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Extern signaal"
>abstract="De **Extern signaal** Met activiteit kunt u de uitvoering van een workflow starten vanuit een andere workflow of een API-aanroep."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Externe signaalparameters"
>abstract="Externe signaalparameters"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Eindtriggers"
>abstract="Eindtriggers"

De **Extern signaal** activiteit is **Stroomregeling** activiteit. Hiermee kunt u de uitvoering van een workflow starten vanuit een andere workflow of vanuit een API-aanroep.

>[!NOTE]
>
>Deze pagina bevat de belangrijkste stappen voor het configureren van een **[!UICONTROL External Signal]** activiteit in het Gebruikersinterface van het Web van de Campagne en brengt het van een ander werkschema of een API vraag teweeg. Gedetailleerde informatie over het activeren van een workflow en de aanbevolen procedures en over het werken met campagne-API&#39;s vindt u in het dialoogvenster [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Voer de volgende stappen uit om de **Extern signaal** activiteit en de uitvoering ervan in gang zetten:

1. Een **Extern signaal** in uw workflow.

1. Voltooi de configuratie van uw workflow en start de uitvoering ervan. De **[!UICONTROL External Signal]** activiteit wordt weergegeven als &quot;In behandeling&quot;, wachtend op activering.

   ![](../assets/external-signal-pending.png)

1. Haal de onderstaande gegevens op:

   * De **interne naam werkstroom**, die naast het label wordt weergegeven.

     +++Voorbeeld

     ![](../assets/external-signal-workflow-name.png)

+++

   * De **Naam van externe signaalactiviteit**, die wordt weergegeven in de **[!UICONTROL Execution options]**.

     +++Voorbeeld

     ![](../assets/external-signal-name.png)

+++

1. Als u de workflow wilt activeren, moet u de opdracht `PostEvent` JavaScript-functie. Met deze functie kunt u variabelen doorgeven met de waarden van uw keuze en deze gebruiken in de getriggerde workflow.

   De `PostEvent` Deze functie kan worden uitgevoerd vanuit een andere workflow of via een API-aanroep.

   * Om een **[!UICONTROL External signal]** activiteit vanuit een werkstroom, de PostEvent-functie uitvoeren vanuit de **[!UICONTROL Initialization script]** venster, dat toegankelijk is vanuit de activiteit **[!UICONTROL Execution options]**. Voor de **[!UICONTROL JavaScript code]** activiteit, voert de functie uit vanuit het script van de activiteit.

     De syntaxis is als volgt:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Voorbeeld

   In dit voorbeeld, brengen wij de &quot;signaal1&quot;Externe signaalactiviteit teweeg die aan het werkschema is toegevoegd de waarvan interne naam &quot;WKF12345&quot;is. We geven ook een variabele door met de naam &#39;customID&#39;, met de waarde &#39;123456&#39;.

   ![](../assets/external-signal-sample.png)

+++

   * Om een **[!UICONTROL External signal]** activiteit van een API vraag, volg de stappen in de documentatie van de Campagne API worden beschreven. [Leer hoe u de statische code gebruikt `PostEvent` methode](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html)
