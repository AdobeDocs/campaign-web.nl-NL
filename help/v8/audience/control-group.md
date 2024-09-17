---
audience: end-user
title: Een controlegroep instellen
description: Leer hoe te om een controlegroep voor uw berichten in het gebruikersinterface van het Web van de Campagne te plaatsen
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
source-git-commit: 3879f217f3a6a1cae0d6c924733d2ef1fd4ab9e7
workflow-type: tm+mt
source-wordcount: '786'
ht-degree: 8%

---

# Een controlegroep instellen {#control-group}

Een controlegroep is een subpopulatie die van de levering is uitgesloten. U kunt een controlegroep bepalen vermijden verzendend berichten naar een gedeelte van uw publiek, en post-levering gedrag met het belangrijkste doel vergelijken. Met deze optie kunt u de impact van uw campagne meten.

➡️ [ ontdekt deze eigenschap in video ](create-audience.md#video)

## Controlegroep inschakelen{#add-a-control-group}

Om een controlegroep toe te voegen, laat de optie toe wanneer het bepalen van het publiek van uw levering. De controlegroep kan willekeurig uit de hoofdtarget worden geëxtraheerd, en/of uit een specifieke populatie worden geselecteerd. Dit betekent dat u een controlegroep op twee manieren kunt definiëren:

* Extraheer een aantal profielen uit het hoofddoel.
* Sluit enkele profielen uit van een lijst of op basis van criteria die zijn gedefinieerd in een query.

U kunt beide methoden combineren bij het definiëren van een besturingsgroep.

Alle profielen die deel uitmaken van de controlegroep bij de voorbereidingsstap voor levering worden verwijderd van het hoofddoel. Ze ontvangen het bericht niet.

>[!CAUTION]
>
>U kunt geen controlegroepen gebruiken wanneer het laden van de doelbevolking [ van een extern dossier ](file-audience.md).

Om een controlegroep aan een levering toe te voegen, activeer de **[!UICONTROL Enable control group]** knevel, van de **sectie van het Publiek** van het scherm van de leveringsverwezenlijking.

![ laat de optie van de controlegroep ](assets/control-group1.png) toe


## Extraheren uit doel {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extractiemodus"
>abstract="Een controlegroep is een reeks profielen die van de levering worden uitgesloten. Als u een controlegroep wilt definiëren, kunt u kiezen of u op willekeurige wijze of op basis van een sortering een percentage of een vast aantal profielen uit de targetpopulatie wilt extraheren."


### Een controlegroep samenstellen {#build-extract-target}

Als u een controlegroep wilt definiëren, kunt u kiezen of u willekeurig of op basis van een sortering, een percentage of een vast aantal profielen wilt extraheren uit de doelpopulatie. Als u verkiest toevoegend een extra-bevolking, kies de **Geen extractie** optie en selecteer de extra bevolking [ zoals hier gedetailleerd ](#extra-population).

Definieer eerst de manier waarop de profielen uit het doel worden geëxtraheerd: willekeurig of op basis van een sortering.

Onder de **groep van de Controle** sectie, kies een **wijze van de Uitwinning**:

* **Willekeurig**: wanneer het voorbereiden van de levering, haalt Adobe Campaign willekeurig een aantal profielen uit die aan het percentage of aan het maximumaantal beantwoorden dat als groottelimiet wordt geplaatst.

* **die door attributen (s)** wordt gerangschikt: deze optie laat u toe om een reeks profielen uit te sluiten die op specifieke attributen worden gebaseerd (s) in een specifieke sorteervolgorde(s).


Dan gebruik de **de grens van de Grootte** sectie om het aantal profielen te plaatsen dat u uit het belangrijkste doel moet halen. Dit kan een onbewerkt getal zijn (bijvoorbeeld 50 profielen om uit te sluiten) of een percentage van het oorspronkelijke publiek (bijvoorbeeld 5% van het hoofddoel).


### Monster van controlegroep{#control-group-sample}

Bijvoorbeeld, om een controlegroep met de 100 nieuwe jongste profielen tot stand te brengen, volg deze stappen:

1. Selecteer het **gebied van de Leeftijd** als sorterend criterium. Verlaat de **Overlopende** soortoptie.
1. Voeg het **gebied van de Datum van de Verwezenlijking 0} {toe.** Verandering in de **Aflopende** soortoptie.
1. Bepaal 100 als drempel in de **grens van de Grootte** sectie.

   ![](assets/control-group2.png){zoomable="yes"}

Deze 100 nieuwe jongste profielen worden dan van het hoofddoel uitgesloten.

### Controleer uw controlegroep {#check-control-group}

U kunt de logboeken bekijken om de uitgesloten profielen te controleren en te identificeren. Laten we het voorbeeld nemen van een willekeurige uitsluiting op vijf profielen.

![](assets/control-group4.png){zoomable="yes"}

Na de voorbereiding van de levering kunt u bekijken hoe de uitsluitingen werden toegepast:

* In leveringsdashboard, vóór het verzenden, controleer **om** KPI uit te sluiten.

  ![](assets/control-group5.png){zoomable="yes"}

* In de leveringslogboeken, toont het lusje van Logs de uitsluitingsstap.

  ![](assets/control-group-sample-logs.png){zoomable="yes"}
<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png){zoomable="yes"}
-->

* De **Uitsluiting veroorzaakt** lusje toont het aantal uitgesloten profiel voor elke typologieregel.

  ![](assets/control-group7.png){zoomable="yes"}

Voor meer informatie over leveringslogboeken, verwijs naar deze [ sectie ](../monitor/delivery-logs.md).

## Een extra populatie toevoegen {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Extra populatie"
>abstract="Een controlegroep is een reeks profielen die van de levering worden uitgesloten. U kunt een specifieke populatie van het leveringspubliek uitsluiten door een bestaand publiek te selecteren, of door een vraag te bepalen."

Een andere manier om een controlegroep te bepalen is een specifieke bevolking in een bestaand publiek te selecteren of door een vraag te bepalen.

Van de **Extra bevolking** sectie van het **de definitiescherm van de Groep van de Controle**, klik de **[!UICONTROL Select Audience]** knoop.

![](assets/control-group3.png){zoomable="yes"}

* Om een bestaand publiek te gebruiken, klik **Uitgezochte publiek**. Lees meer in [deze sectie](add-audience.md).

* Om een nieuwe vraag te bepalen, creeer **uw eigen** en bepaal de uitsluitingscriteria gebruikend de vraagmodeler. Lees meer in [deze sectie](../query/query-modeler-overview.md).

De profielen inbegrepen in het publiek of die het resultaat van de vraag aanpassen zijn **uitgesloten** van het leveringsdoel: zij ontvangen geen bericht.

## De resultaten vergelijken{#control-group-results}

Zodra de levering wordt verzonden, kunt u de verzendende logboeken halen om gedrag tussen de profielen te vergelijken die niet de mededeling en het efficiënte doel ontvingen. U kunt de leveringslogboeken ook gebruiken om een nieuwe het richten te bouwen.

Om te zien welke profielen van het doel werden verwijderd, controleer de **Logboeken van de Levering**. Leer meer [ in deze sectie ](#check-control-group).
