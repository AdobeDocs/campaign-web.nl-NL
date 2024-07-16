---
audience: end-user
title: De externe signaalactiviteit gebruiken
description: Leer hoe u de activiteit van de externe signaalworkflow kunt gebruiken
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: 93f6347828c72535c1a005ecd6ca18596a180098
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Extern signaal {#external-signal}

<!--External Signal End-->

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal"
>title="Extern signaal"
>abstract="De **Externe signaal** activiteit laat u de uitvoering van een werkschema van een ander werkschema of een API vraag teweegbrengen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_externalsignal_parameters"
>title="Externe signaalparameters"
>abstract="Externe signaalparameters"

>[!CONTEXTUALHELP]
>id="acw_orchestration_end_trigger"
>title="Eindtriggers"
>abstract="Eindtriggers"

De **Externe signaal** activiteit is de controle **activiteit van de a** Stroom. Hiermee kunt u de uitvoering van een workflow starten vanuit een andere workflow of vanuit een API-aanroep.

>[!NOTE]
>
>Deze pagina presenteert de belangrijkste stappen om een **[!UICONTROL External Signal]** activiteit in het Gebruikersinterface van het Web van de Campagne te vormen en het van een andere werkschema of een API vraag teweeg te brengen. De gedetailleerde informatie over hoe te om een werkschema en zijn beste praktijken teweeg te brengen, en hoe te met Campagne APIs te werken is beschikbaar in de [ Campagne v8 (cliëntconsole) documentatie ](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example)

Volg deze stappen om de **Externe signaal** activiteit te vormen en zijn uitvoering teweeg te brengen:

1. Voeg een **Externe signaal** activiteit in uw werkschema toe.

1. Voltooi de configuratie van uw workflow en start de uitvoering ervan. De activiteit **[!UICONTROL External Signal]** wordt weergegeven als &quot;In behandeling&quot;, in afwachting van activering.

   ![](../assets/external-signal-pending.png)

1. Haal de onderstaande gegevens op:

   * De **interne naam van het werkschema**, die naast zijn etiket toont.

     +++Voorbeeld

     ![](../assets/external-signal-workflow-name.png)

+++

   * De **Externe naam van de signaalactiviteit**, die in het werkschema **[!UICONTROL Execution options]** toont.

     +++Voorbeeld

     ![](../assets/external-signal-name.png)

+++

1. Als u de workflow wilt activeren, moet u de functie `PostEvent` JavaScript uitvoeren. Met deze functie kunt u variabelen doorgeven met de waarden van uw keuze en deze gebruiken in de getriggerde workflow.

   De functie `PostEvent` kan worden uitgevoerd vanuit een andere workflow of vanuit een API-aanroep.

   * Als u een **[!UICONTROL External signal]** -activiteit wilt activeren vanuit een werkstroom, voert u de PostEvent-functie uit vanuit het deelvenster **[!UICONTROL Initialization script]** , dat toegankelijk is vanuit de activiteit **[!UICONTROL Execution options]** . Voor de **[!UICONTROL JavaScript code]** activiteit, voer de functie van het manuscript van de activiteit uit.

     De syntaxis is als volgt:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Voorbeeld

   In dit voorbeeld, brengen wij de &quot;signaal1&quot;Externe signaalactiviteit teweeg die aan het werkschema is toegevoegd de waarvan interne naam &quot;WKF12345&quot;is. We geven ook een variabele door met de naam &#39;customID&#39;, met de waarde &#39;123456&#39;.

   ![](../assets/external-signal-sample.png)

+++

   * Als u een **[!UICONTROL External signal]** -activiteit wilt activeren vanaf een API-aanroep, voert u de stappen uit die in de API-documentatie voor campagne worden beschreven. [ Leer hoe te om de statische `PostEvent` methode ](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html) te gebruiken
