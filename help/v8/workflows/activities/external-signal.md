---
audience: end-user
title: De externe signaalactiviteit gebruiken
description: Leer hoe u de activiteit van de externe signaalworkflow kunt gebruiken
exl-id: e4244ecc-5e37-41a6-a4dd-6e32da6d5512
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '374'
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

De **Externe signaal** activiteit is de controle **activiteit van de a** Stroom. Hiermee kunt u de uitvoering van een workflow starten vanuit een andere workflow of een API-aanroep.

>[!NOTE]
>
>Deze pagina verklaart de belangrijkste stappen om een **[!UICONTROL External Signal]** activiteit in het Gebruikersinterface van het Web van de Campagne te vormen en het van een andere werkschema of een API vraag teweeg te brengen. De gedetailleerde informatie over hoe te om een werkschema, beste praktijken teweeg te brengen, en hoe te met Campagne APIs te werken is beschikbaar in de [&#x200B; Campagne v8 (cliëntconsole) documentatie &#x200B;](https://experienceleague.adobe.com/en/docs/campaign/automation/workflows/advanced-management/javascript-in-workflows#trigger-example).

Volg deze stappen om de **Externe signaal** activiteit te vormen en zijn uitvoering teweeg te brengen:

1. Voeg een **Externe signaal** activiteit in uw werkschema toe.

1. Voltooi de configuratie van uw workflow en start de uitvoering ervan. De **[!UICONTROL External Signal]** -activiteit wordt weergegeven als &quot;In behandeling&quot; en wacht op activering.

   ![&#x200B; het schermschot toont de Externe activiteit van het Signaal in een hangende staat.](../assets/external-signal-pending.png)

1. Haal de volgende gegevens op:

   * De **interne naam van het werkschema**, die naast zijn etiket toont.

     +++Voorbeeld weergeven

     ![&#x200B; het schermschot toont de interne naam van het werkschema naast zijn etiket.](../assets/external-signal-workflow-name.png)

     +++

   * De **Externe naam van de signaalactiviteit**, die in het werkschema **[!UICONTROL Execution options]** toont.

     +++Voorbeeld weergeven

     ![&#x200B; het schermschot toont de Externe naam van de activiteit van het Signaal in de opties van de Uitvoering.](../assets/external-signal-name.png)

     +++

1. Als u de workflow wilt activeren, voert u de functie `PostEvent` JavaScript uit. Deze functie laat u variabelen met de waarden van uw keus overgaan en hen in het teweeggebrachte werkschema gebruiken.

   De functie `PostEvent` kan worden uitgevoerd vanuit een andere workflow of vanuit een API-aanroep.

   * Als u een **[!UICONTROL External signal]** -activiteit wilt activeren vanuit een workflow, voert u de PostEvent-functie uit vanuit het deelvenster **[!UICONTROL Initialization script]** , dat toegankelijk is via de **[!UICONTROL Execution options]** -activiteit. Voor de **[!UICONTROL JavaScript code]** activiteit, voer de functie van het manuscript van de activiteit uit.

     De syntaxis is als volgt:

     ```
     xtk.workflow.PostEvent("<workflow-internal-name>","<signal-activity-name>","",<variables <variable-name>="<value>"/>, false);
     ```

   +++Voorbeeld weergeven

   In dit voorbeeld wordt de &quot;signaal1&quot; externe signaalactiviteit geactiveerd. Het is toegevoegd aan de workflow met de interne naam &quot;WKF12345&quot;. Een variabele met de naam &quot;customID&quot; wordt doorgegeven met de waarde &quot;123456&quot;.

   ![&#x200B; het schermafbeelding toont een voorbeeld van het teweegbrengen van de Externe activiteit van het Signaal gebruikend de functie PostEvent.](../assets/external-signal-sample.png)

   +++

   * Als u een **[!UICONTROL External signal]** -activiteit wilt activeren vanaf een API-aanroep, voert u de stappen uit die in de API-documentatie voor campagne worden beschreven. [&#x200B; Leer hoe te om de statische `PostEvent` methode &#x200B;](https://experienceleague.adobe.com/developer/campaign-api/api/sm-workflow-PostEvent.html) te gebruiken.