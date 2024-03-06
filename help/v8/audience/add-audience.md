---
audience: end-user
title: Bestaande doelgroep selecteren
description: Leer hoe u een publiek kunt selecteren
exl-id: 76873315-a2eb-4936-bd10-6759bf603dd0
source-git-commit: 1d639f16c470297d115443b5579547419413a3d3
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---


# Bestaande doelgroep selecteren {#add-audience}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_audience_select"
>title="Bestaande doelgroep selecteren"
>abstract="Blader in de lijst om een bestaand publiek te selecteren. Gebruik het pictogram Filters tonen om de lijst te filteren of selecteer een specifieke map."

In deze sectie wordt uitgelegd hoe u een bestaand publiek kunt selecteren wanneer u de doelpopulatie van een levering definieert. Wanneer u het hoofddoel van een levering definieert, kunt u ook:

* [Eenmalig publiek maken](one-time-audience.md) het gebruiken van de vraagmodeler.
* [Een publiek laden vanuit een extern bestand](file-audience.md) (alleen voor e-mails).

De doelgroepen in de leveringen zijn toegankelijk via de **Publiek** links. Zij komen uit veelvoudige bronnen zoals de console van de Cliënt, de het publiekswerkschema&#39;s van het Web van de Campagne of Adobe Experience Platform voort. [Leer hoe u het publiek kunt controleren en beheren](manage-audience.md)

Volg onderstaande stappen om een bestaand publiek voor uw bericht te selecteren:

1. Van de **Publiek** sectie van de medewerker van de leveringsverwezenlijking, klik **[!UICONTROL Select audience]** en kies vervolgens **[!UICONTROL Select audience]** om een bestaand publiek te gebruiken.

   ![](assets/create-audience.png){zoomable=&quot;yes&quot;}

1. In dit scherm worden alle bestaande soorten publiek voor de huidige map weergegeven.

   ![](assets/create-audience2.png){zoomable=&quot;yes&quot;}

   Blader naar de `AEP Audiences folder` in het filtergedeelte van het scherm. [Meer informatie over Adobe Experience Platform-publiek](manage-audience.md#monitor)

   ![](assets/select-audience-folder.png){zoomable=&quot;yes&quot;}

1. Met de filtersectie hebt u toegang tot filteropties om de lijst met doelgroepen te verfijnen. Om dit te doen, klik **Regels toevoegen** om tot de vraagmodeler toegang te hebben, die u geavanceerde filters voor de lijst van publiek laat tot stand brengen. [Leer hoe te om de vraagmodeler te gebruiken](../query/query-modeler-overview.md)

   U kunt bijvoorbeeld een regel definiëren om op de oorsprong van het publiek te filteren, zoals hieronder wordt getoond:

   ![](assets/filter-on-aep-audience.png){zoomable=&quot;yes&quot;}

1. Klikken **Bevestigen** om uw publiek toe te voegen als belangrijkste doel voor levering. Zodra gedaan, kunt u het publiek nog verfijnen gebruikend de vraagmodeler door te klikken **Regels bewerken** knop.

   ![](assets/refine-audience.png){zoomable=&quot;yes&quot;}

   U kunt ook een controlegroep instellen om het effect van uw campagnes te meten. De controlegroep ontvangt niet het bericht. Dit staat u toe om het gedrag van de bevolking te vergelijken die het bericht met het gedrag van contacten ontving die niet. [Meer informatie](control-group.md)
