---
audience: end-user
title: Een controlegroep instellen
description: Leer hoe te om een controlegroep voor uw berichten in het Web UI van de Campagne te plaatsen
exl-id: 02f3adec-681a-4cec-a895-41c80eb345db
badge: label="Beta"
source-git-commit: 334014d3d89c878617b8e43ea73c9ff4e957f6d7
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 12%

---

# Een controlegroep instellen {#control-group}

Een controlegroep is een subpopulatie die van de levering is uitgesloten. U kunt een controlegroep bepalen vermijden verzendend berichten naar een gedeelte van uw publiek, en post-levering gedrag met het belangrijkste doel vergelijken. Met deze optie kunt u de impact van uw campagne meten.

## Controlegroep inschakelen{#add-a-control-group}

Om een controlegroep toe te voegen, laat de optie toe wanneer het bepalen van het publiek van uw levering. De controlegroep kan willekeurig uit de hoofdtarget worden geëxtraheerd, en/of uit een specifieke populatie worden geselecteerd. Dit betekent dat u een controlegroep op twee manieren kunt definiëren:

* Een aantal profielen extraheren uit de hoofdtarget.
* Sluit enkele profielen uit van een lijst of op basis van criteria die zijn gedefinieerd in een query.

U kunt beide methoden combineren bij het definiëren van een besturingsgroep.

Alle profielen die deel uitmaken van de controlegroep bij de voorbereidingsstap voor levering worden verwijderd van het hoofddoel. Ze ontvangen het bericht niet.

>[!CAUTION]
>
>U kunt geen controlegroepen gebruiken wanneer het laden van de doelpopulatie [van een extern bestand](file-audience.md).

Als u een controlegroep wilt toevoegen aan een levering, activeert u de optie **[!UICONTROL Enable control group]** schakelen tussen **Publiek** van het scherm voor het maken van de levering.

![De optie Besturingsgroep inschakelen](assets/control-group1.png)


## Extraheren uit doel {#extract-target}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_target"
>title="Extractiemodus"
>abstract="Een controlegroep is een reeks profielen die van de levering worden uitgesloten. Als u een controlegroep wilt definiëren, kunt u kiezen of u op willekeurige wijze of op basis van een sortering een percentage of een vast aantal profielen uit de targetpopulatie wilt extraheren."


### Een controlegroep samenstellen {#build-extract-target}

Als u een controlegroep wilt definiëren, kunt u kiezen of u op willekeurige wijze of op basis van een sortering een percentage of een vast aantal profielen uit de targetpopulatie wilt extraheren. Als u liever een extra populatie toevoegt, kiest u de optie **Geen extractie** en selecteert u de extra populatie [zoals hier beschreven](#extra-population).

Definieer eerst de manier waarop de profielen uit het doel worden geëxtraheerd: willekeurig of op basis van een sortering.

Onder de **Controlegroep** in, kiest u een **Extractiemodus**:

* **Willekeurig**: bij het voorbereiden van de levering extraheert Adobe Campaign willekeurig een aantal profielen dat overeenkomt met het percentage of het maximumaantal dat is ingesteld als de maximale grootte.

* **Gerangschikt op kenmerk(en)**: met deze optie kunt u een set profielen uitsluiten op basis van specifieke kenmerken in een specifieke sorteervolgorde.


Gebruik vervolgens de **Groottebeperking** om het aantal profielen in te stellen dat u uit het hoofddoel moet extraheren. Dit kan een onbewerkt getal zijn (bijvoorbeeld 50 profielen om uit te sluiten) of een percentage van het oorspronkelijke publiek (bijvoorbeeld 5% van het hoofddoel).


### Monster van controlegroep{#control-group-sample}

Bijvoorbeeld, om een controlegroep met de 100 nieuwe jongste ontvangers tot stand te brengen, volg deze stappen:

1. Selecteer de **Leeftijd** veld als sorteercriterium. Laat de **Oplopend** sorteeroptie.
1. Voeg de **Aanmaakdatum** veld. Wijzigen in de **Aflopend** sorteeroptie.
1. Definieer 100 als de drempel in het dialoogvenster **Groottebeperking** sectie.

   ![](assets/control-group2.png)

Deze 100 nieuwe jongste ontvangers worden dan uitgesloten van het hoofddoel.

### Controleer uw controlegroep {#check-control-group}

U kunt de logboeken bekijken om de uitgesloten profielen te controleren en te identificeren. Laten we het voorbeeld nemen van een willekeurige uitsluiting op vijf profielen.

![](assets/control-group4.png)

Na de voorbereiding van de levering kunt u bekijken hoe de uitsluitingen werden toegepast:

* Controleer in het bezorgdashboard, vóór de verzending, het **Uitsluiten** KPI.

  ![](assets/control-group5.png)

* In de leveringslogboeken, toont het lusje van Logs de uitsluitingsstap.

  ![](assets/control-group-sample-logs.png)
<!--

 * The **Exclusion logs** tab displays each profile and the related exclusion **Reason**.

    ![](assets/control-group6.png)
-->

* De **Uitsluiting veroorzaakt** wordt het aantal uitgesloten profielen voor elke typeregel weergegeven.

  ![](assets/control-group7.png)

Voor meer informatie over leveringslogboeken, verwijs naar dit [sectie](../monitor/delivery-logs.md).

## Een extra populatie toevoegen {#extra-population}

>[!CONTEXTUALHELP]
>id="acw_deliveries_email_controlgroup_extra"
>title="Extra populatie"
>abstract="Een controlegroep is een reeks profielen die van de levering worden uitgesloten. U kunt een specifieke populatie van het leveringspubliek uitsluiten door een bestaand publiek te selecteren, of door een vraag te bepalen."

Een andere manier om een controlegroep te bepalen is een specifieke bevolking in een bestaand publiek te selecteren of door een vraag te bepalen.

Van de **Extra populatie** van de **Controlegroep** definitiescherm, klik **[!UICONTROL Select Audience]** knop.

![](assets/control-group3.png)

* Om een bestaand publiek te gebruiken, klik **Doelgroep selecteren**. Meer informatie in [deze sectie](add-audience.md).

* Als u een nieuwe query wilt definiëren, selecteert u **Maak uw eigen** en definieert u de uitsluitingscriteria met behulp van de regelbouwer. Meer informatie in [deze sectie](segment-builder.md).

De profielen die zijn opgenomen in het publiek of die overeenkomen met het resultaat van de query, zijn **uitgesloten** van het leveringsdoel: zij ontvangen geen bericht.

## De resultaten vergelijken{#control-group-results}

Zodra de levering wordt verzonden, kunt u de verzendende logboeken halen om gedrag tussen de profielen te vergelijken die niet de mededeling en het efficiënte doel ontvingen. U kunt de leveringslogboeken ook gebruiken om een nieuwe het richten te bouwen.

Als u wilt zien welke profielen uit het doel zijn verwijderd, controleert u de knop **Leveringslogboeken**. Meer informatie [in deze sectie](#check-control-group).


