---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
badge: label="Alpha" type="Positief"
source-git-commit: 880f02c460d75c50347fb5716fbcdf7cd3908422
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---


# Orchestraten {#orchestrate}

Zodra u [een workflow hebben gemaakt](create-workflow.md)Of u nu het workflowmenu of een campagne gebruikt, u kunt de verschillende taken die het uitvoert gaan ordenen. Hiervoor wordt een visueel canvas verschaft, zodat u een workflowdiagram kunt maken. Binnen dit diagram, kunt u diverse activiteiten toevoegen en hen in een opeenvolgende orde verbinden.

In dit stadium van de configuratie, wordt het diagram getoond met een beginpictogram, dat het begin van uw werkschema vertegenwoordigt. Als u de eerste activiteit wilt toevoegen, klikt u op de knop + die is verbonden met het startpictogram.

Er wordt een lijst met activiteiten weergegeven die aan het diagram kunnen worden toegevoegd. De beschikbare activiteiten zijn afhankelijk van uw positie binnen het werkstroomdiagram. Wanneer u bijvoorbeeld uw eerste activiteit toevoegt, kunt u de workflow starten door zich te richten op een publiek, het workflowpad te splitsen of een wachtactiviteit in te stellen om de uitvoering van de workflow uit te stellen. Anderzijds, na een het publieksactiviteit van de Bouwstijl, kunt u uw doel met het richten van activiteiten verfijnen, een levering naar uw publiek met kanaalactiviteiten verzenden, of het werkschemaproces met debietcontroleactiviteiten organiseren.

![](assets/workflow-start.png)

Zodra een activiteit aan het diagram is toegevoegd, verschijnt een juiste ruit, toestaand u om de onlangs toegevoegde activiteit met specifieke montages te vormen. Gedetailleerde informatie over hoe te om elke activiteit te vormen is beschikbaar in [deze sectie](activities/about-activities.md).

![](assets/workflow-configure-activities.png)

Herhaal dit proces om zoveel activiteiten toe te voegen als u wilt afhankelijk van de taken die u de workflow wilt uitvoeren. U kunt ook een nieuwe activiteit invoegen tussen twee activiteiten. Om dit te doen, klik + knoop op de overgang tussen de activiteiten, selecteer de gewenste activiteit en vorm het in de juiste ruit.

Als u een activiteit wilt verwijderen, selecteert u deze op het canvas en klikt u op het pictogram Verwijderen in de activiteitseigenschappen.

>[!TIP]
>
>U kunt de naam van de overgangen tussen elke activiteit aanpassen. U doet dit door de overgang te selecteren en het label ervan te wijzigen in het rechterdeelvenster.

Hier volgt een voorbeeld van een workflow die is ontworpen om een e-mail naar alle klanten (andere dan VIP klanten) te sturen met een e-mail die geïnteresseerd is in koffiecomputers.

![](assets/workflow-example.png)

Hiervoor zijn de volgende activiteiten toegevoegd:

* A **[!UICONTROL Fork]** activiteit die de werkstroom in drie wegen (één voor elke reeks klant) verdeelt;
* **[!UICONTROL Build audience]** activiteiten om de drie categorieën klanten te bereiken:

   * Klanten met een e-mail,
   * Klanten die behoren tot het reeds bestaande publiek &quot;Interrested in Coffee Machine(s)&quot;,
   * Klanten die tot het reeds bestaande &quot;VIP of beloning&quot; publiek behoren.

* A **[!UICONTROL Combine]** activiteiten die klanten met een e-mail en degenen die geïnteresseerd zijn in koffiemachines verenigen;
* A **[!UICONTROL Combine]** activiteiten die VIP klanten uitsluiten;
* An **[!UICONTROL Email delivery]** activiteit die een e-mail naar de resulterende klanten verzendt.

Nadat u de workflow hebt voltooid, voegt u **[!UICONTROL End]** activiteit aan het einde van het diagram. Met deze activiteit kunt u visueel het einde van een werkstroom markeren en heeft dit geen invloed op de functionaliteit.

Nadat u het werkstroomdiagram hebt ontworpen, kunt u de werkstroom uitvoeren en de voortgang van de verschillende taken volgen. [Leer hoe u een workflow kunt starten en de uitvoering ervan kunt controleren](start-monitor-workflows.md)