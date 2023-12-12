---
audience: end-user
title: Bouw uw eerste vraag gebruikend de vraagmodeler
description: Leer hoe u uw eerste query bouwt in Adobe Campaign Web query modeler.
source-git-commit: a974221fa5b46ea9463c98724b1f49a7edb0adb7
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 0%

---

# Uw eerste query samenstellen {#build-query}

Om te beginnen bouwend een vraag, heb toegang tot de vraagmodeler van de plaats van uw keus, afhankelijk van de actie u wilt uitvoeren. Het Query-model wordt geopend met een leeg canvas. Klik + knoop om de eerste knoop van uw vraag toe te voegen.

![](assets/query-add-component.png)

U kunt twee typen elementen toevoegen:

* Door componenten te filteren (aangepaste voorwaarde, publiek selecteren, vooraf gedefinieerd filter) kunt u uw eigen regels maken en een publiek of een vooraf gedefinieerd filter selecteren om de query te verfijnen.

  Voorbeeld *Ontvangers die zich hebben geabonneerd op de nieuwsbrief &#39;Sport&#39;*. *Ontvangers in New York*, *Ontvangers in San Francisco*

* De exploitanten van de groep (EN, OF, BEHALVE) staan u toe om het filtreren componenten in het diagram te groeperen om uw behoeften aan te passen.

  Voorbeeld: *Ontvangers die zich hebben geabonneerd op de nieuwsbrief &quot;Sport&quot;**EN**die in New York wonen **OF**San Francisco*.

U vindt hieronder gedetailleerde stappen voor het toevoegen en combineren van filtercomponenten en groepoperatoren.

## Filtercomponenten toevoegen

Door componenten te filteren kunt u de query verfijnen door:

* **Aangepaste voorwaarden**: Filter uw query door uw eigen voorwaarde te maken met kenmerken uit de database en geavanceerde expressies.
* **Soorten publiek**: Filter de query met een bestaand publiek.
* **Vooraf gedefinieerd filter**: Filter de query met behulp van bestaande vooraf gedefinieerde filters.

### Een aangepaste voorwaarde configureren

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_customcondition"
>title="Aangepaste voorwaarde"
>abstract="Aangepaste voorwaarde"

Voer de volgende stappen uit om de query te filteren met behulp van een aangepaste voorwaarde:

1. Klik op de +-knop op het gewenste knooppunt en selecteer **[!UICONTROL Custom condition]**.
1. Het deelvenster Eigenschappen voor aangepaste voorwaarde wordt aan de rechterkant geopend. Selecteer in het veld Kenmerk het kenmerk in de database dat u wilt gebruiken om de voorwaarde te maken.

   De beschikbare kenmerken vertegenwoordigen alle velden uit uw Campagne-database, inclusief velden uit tabellen die zijn gekoppeld aan de tabel Ontvangers.

   ![](assets/query-custom-condition-fields.png)

   >[!NOTE]
   >
   >Met de knop Uitdrukking bewerken kunt u de editor voor de Campagne-webexpressie gebruiken om handmatig een expressie te definiëren met behulp van velden uit de database en hulpfuncties.

1. Selecteer in de vervolgkeuzelijst de operator die u wilt toepassen.

   +++Lijst met beschikbare operatoren

   >[!NOTE]
   >
   >Beschikbare operatoren in de vervolgkeuzelijst zijn afhankelijk van het gegevenstype van het geselecteerde kenmerk.

   | Operator | Doel | Voorbeeld |
   |  ---  |  ---  |  ---  |
   | Gelijk aan | Retourneert een resultaat dat identiek is aan de gegevens die zijn ingevoerd in de tweede kolom Waarde. | Achternaam (@lastName) gelijk aan &#39;Jones&#39; retourneert alleen ontvangers met als achternaam Jones. |
   | Niet gelijk aan | Retourneert alle waarden die niet identiek zijn aan de ingevoerde waarde. | Taal (@taal) gelijk aan &#39;Engels&#39; |
   | Groter dan | Retourneert een waarde die groter is dan de ingevoerde waarde. | Leeftijd (@leeftijd) groter dan 50</strong>alle waarden boven &quot;50&quot;, d.w.z. &quot;51&quot;, &quot;52&quot; enz. |
   | Minder dan | Retourneert een waarde die kleiner is dan de ingevoerde waarde. | Aanmaakdatum (@created) vóór &#39;DaysAgo(100)&#39;</strong>, worden alle ontvangers geretourneerd die minder dan 100 dagen geleden zijn gemaakt. |
   | Groter dan of gelijk aan | Retourneert alle waarden die gelijk zijn aan of groter zijn dan de ingevoerde waarde. | Leeftijd (@leeftijd) groter dan of gelijk aan &#39;30&#39;</strong>, worden alle ontvangers vanaf 30 jaar geretourneerd. |
   | Kleiner dan of gelijk aan | Retourneert alle waarden die gelijk zijn aan of lager zijn dan de ingevoerde waarde. | Leeftijd (@leeftijd) kleiner dan of gelijk aan &#39;60&#39;</strong>, worden alle ontvangers vanaf 60 jaar geretourneerd. |
   | Opgenomen in | Retourneert resultaten die zijn opgenomen in de aangegeven waarden. Deze waarden moeten door een komma worden gescheiden. | De geboortedatum (@geboortedatum) is opgenomen in &quot;12/10/1979,12/10/1984&quot; en retourneert de tussen deze data geboren ontvangers. |
   | Niet in | Werkt zoals is opgenomen in operator. Hier, willen wij ontvangers uitsluiten die op de ingegane waarden worden gebaseerd. | Geboortedatum (@geboortedatum) is niet opgenomen in &quot;10-12-1979,12-10-1984&quot;. Anders dan in het vorige voorbeeld worden ontvangers die binnen deze datums geboren zijn, niet geretourneerd. |
   | Is leeg | In dit geval komt het resultaat dat we zoeken overeen met een lege waarde in de tweede kolom Waarde. | Mobiele (@mobilePhone) is leeg en retourneert alle ontvangers die geen mobiel nummer hebben. |
   | Is niet leeg | Werkt in omgekeerde volgorde naar de operator Is leeg. Het is niet nodig gegevens in te voeren in de tweede kolom Waarde. | E-mail (@email) is niet leeg. |
   | Begint met | Retourneert de resultaten die beginnen met de ingevoerde waarde. | Account # (@account) begint met &#39;32010&#39;. |
   | Begint niet met | Retourneert de resultaten die niet beginnen met de ingevoerde waarde. | Account # (@account) begint niet met &#39;20&#39; |
   | Bevat | Retourneert de resultaten die ten minste de ingevoerde waarde bevatten. | E-maildomein (@domein) bevat &#39;mail&#39;</strong>, worden alle domeinnamen geretourneerd die &#39;mail&#39; bevatten. Het domein &#39;gmail.com&#39; wordt dus ook geretourneerd. |
   | Bevat niet | Retourneert resultaten die niet de ingevoerde waarde bevatten. | E-maildomein (@domain) bevat geen &#39;vo&#39;</strong>. In dit geval worden domeinnamen die &#39;vo&#39; bevatten, niet geretourneerd. De domeinnaam voila.fr wordt niet weergegeven in de resultaten. |
   | leuk | Net als de Contains-operator. Hiermee kunt u een jokerteken % in de waarde invoegen. | Achternaam (@lastName) zoals &#39;Jon%s&#39;. Hier wordt het jokerteken gebruikt als een joker om de naam Jones te vinden, mocht de operator de ontbrekende letter tussen de &#39;n&#39; en &#39;s&#39; vergeten hebben. |
   | Niet leuk | Net als de Contains-operator. Hiermee kunt u een jokerteken % in de waarde invoegen. | Achternaam (@lastName) houdt niet van &#39;Smi%h&#39;. Hier worden de ontvangers met de achternaam &#39;Smi%h&#39; niet geretourneerd. |

+++

1. Selecteer in het veld Waarde de verwachte waarde.

   U kunt de uitdrukkingsredacteur van het Web van de gebruiksCampagne ook manueel om een uitdrukking te bepalen gebruikend gebieden van het gegevensbestand en hulpfuncties. Klik hiertoe op de knop Expressie bewerken.

   *Voorbeeld: query die alle profielen van 21 jaar of ouder retourneert*

   ![](assets/query-custom-condition.png)

<!--
querying linked tables
collect additional information on the targeted population, e.g. contract numbers, subscriptions to newsletters or origin.
Select the type of data you want to add. This can be data belonging to the filtering dimension or data stored in linked tables. Select the table which contains the information you want to collect and click Next.

aggregates: Define a calculation mode for the field to be added, such as an aggregate for example.-->

### Een publiek selecteren

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_selectaudience"
>title="Doelgroep selecteren"
>abstract="Doelgroep selecteren"

Voer de volgende stappen uit om uw query te filteren op een bestaand publiek:

1. Klik op de +-knop op het gewenste knooppunt en selecteer **[!UICONTROL Select audience]**.

1. Het deelvenster Eigenschappen voor geselecteerd publiek wordt aan de rechterkant geopend. Selecteer het publiek dat u wilt gebruiken om uw query te filteren.

   *Voorbeeld: query die alle profielen retourneert die behoren tot het &quot;Festival Goers&quot;-publiek*

   ![](assets/query-audience.png)

### Een vooraf gedefinieerd filter gebruiken

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_predefinedfilter"
>title="Vooraf gedefinieerd filter"
>abstract="Vooraf gedefinieerd filter"

Voer de volgende stappen uit om de query te filteren met een vooraf gedefinieerd filter:

1. Klik op de +-knop op het gewenste knooppunt en selecteer **[!UICONTROL Predefined filter]**.

1. Het deelvenster Eigenschappen voor geselecteerd publiek wordt aan de rechterkant geopend. Selecteer een vooraf gedefinieerd filter in de lijst met aangepaste filters of uit favorieten.

   *Voorbeeld: query die alle profielen retourneert die overeenkomen met het vooraf gedefinieerde filter &quot;Inactieve klanten&quot;.*

   ![](assets/query-predefined-filter.png)

## Filtercomponenten combineren met operatoren

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_group"
>title="Groep"
>abstract="Groep"

Wanneer het toevoegen van een het filtreren component aan uw vraag, wordt een nieuwe overgang automatisch gecreeerd op het vraagcanvas, en de nieuwe het filtreren component wordt verbonden met eerste door EN exploitant. Dit betekent dat de resultaten van zowel de het filtreren componenten in de vraagresultaten worden gecombineerd.

In dit voorbeeld wordt een nieuwe filtercomponent van het publiekstype toegevoegd aan het canvas. Deze wordt automatisch toegevoegd aan een nieuwe overgang en gekoppeld aan de vooraf gedefinieerde filtertypevoorwaarde met de operator AND. In dit geval, omvat de vraagresultaten ontvangers die door de &quot;Madridians&quot;vooraf bepaalde filter EN worden gericht die tot het publiek van de &quot;Bezoekers van de Korting&quot;behoren.

![](assets/query-operator.png)

Als u de operator wilt wijzigen die wordt gebruikt om filtervoorwaarden aan elkaar te koppelen, klikt u erop en selecteert u de gewenste operator in het vak U kunt de operator wijzigen door erop te klikken en de gewenste operator te selecteren in het deelvenster Groep dat aan de rechterkant wordt geopend.

![](assets/query-operator-change.png)

Beschikbare operatoren zijn:

* AND (Intersection): combineert resultaten van alle het filtreren componenten in de uitgaande overgangen.
* OR (Union): omvat resultaten van minstens één van de filtercomponenten in de uitgaande overgangen.
* EXCEPT (Uitsluiting): sluit resultaten uit van alle filtercomponenten in de uitgaande overgang.

## Uw query controleren en valideren

>[!CONTEXTUALHELP]
>id="acw_orchestration_querymodeler_ruleproperties"
>title="Eigenschappen van Rule"
>abstract="Eigenschappen van Rule"

Zodra u uw vraag in het canvas hebt gebouwd, kunt u het controleren gebruikend de de eigenschappen van de Regel ruit die op de rechterkant wordt gevestigd. De beschikbare bewerkingen zijn als volgt:

* **Resultaten weergeven:** geeft de gegevens weer die het resultaat zijn van de query.
* **Codeweergave**: geeft een op code gebaseerde versie van de query weer in SQL.
* **Berekenen**: werkt en toont het aantal verslagen bij die door uw vraag worden bedoeld.
* **Filter selecteren of opslaan**: kies een bestaand vooraf gedefinieerd filter dat u op het canvas wilt gebruiken, of sla uw query op als een vooraf gedefinieerd filter voor toekomstig hergebruik. [Leer hoe u met vooraf gedefinieerde filters werkt](../get-started/predefined-filters.md)

  >[!IMPORTANT]
  >
  >Selecteer een vooraf gedefinieerd filter in het deelvenster Eigenschappen regel om de query die in het canvas is gemaakt te vervangen door het geselecteerde filter.
