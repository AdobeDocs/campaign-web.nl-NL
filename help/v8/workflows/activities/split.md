---
audience: end-user
title: De werkstroomactiviteit Splitsen gebruiken
description: Leer hoe u de activiteit van de gesplitste workflow gebruikt
badge: label="Alfa"
source-git-commit: 1527d9474e7b3d42d8c6db00f67cbfe927c1348c
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---


# Splitsen {#split}

De **Splitsen** activiteit is **Doelstelling** activiteit die u toestaat om inkomende populaties in veelvoudige subsets te segmenteren die op verschillende selectiecriteria, zoals het filtreren regels of populatiegrootte worden gebaseerd.

## Configuratie {#general}

Voer de volgende stappen uit om de **Splitsen** activiteit:

1. Voeg een **Splitsen** activiteit aan uw werkschema.

1. Het deelvenster voor activiteitenconfiguratie wordt geopend met een standaardsubset. Klik op de knop **Segment toevoegen** om zoveel subsets toe te voegen als gewenst om de binnenkomende populatie te segmenteren.

   ![](../assets/workflow-split.png)

   >[!IMPORTANT]
   >
   >Wanneer de gesplitste activiteit wordt uitgevoerd, wordt de populatie gesegmenteerd over de verschillende subsets in de volgorde waarin ze aan de activiteit worden toegevoegd. Als de eerste subset bijvoorbeeld 70% van de oorspronkelijke populatie herstelt, past de volgende toegevoegde subset zijn selectiecriteria alleen toe op de resterende 30%, enzovoort.
   >
   > Voordat u de subsets configureert, moet u ervoor zorgen dat u deze in de juiste volgorde hebt toegevoegd. De positie van deze subsets kan namelijk niet worden gewijzigd.

1. Nadat subsets zijn toegevoegd, toont de activiteit evenveel uitvoerovergangen als er subsets zijn. We raden u ten zeerste aan het label van elke subset te wijzigen om deze gemakkelijk te identificeren in het werkstroomcanvas.

1. Vorm hoe elke ondergroep de inkomende bevolking zou moeten filtreren. Ga als volgt te werk om dit te doen:

   1. Open de subset om de eigenschappen ervan weer te geven.

   1. Als u een filtervoorwaarde op de subset wilt toepassen, klikt u op **[!UICONTROL Create filter]** en vorm de gewenste het filtreren regel. Neem bijvoorbeeld profielen op van de binnenkomende populatie waarvan het e-mailadres voorkomt in de database.

   1. Schakel het selectievakje **[!UICONTROL Enable limit]** en geeft het aantal of de percentages van de populatie aan die moeten worden opgenomen.

      >[!NOTE]
      >
      >Wanneer u een populatielimiet voor een subset instelt, kunt u de geselecteerde profielen op basis van een specifiek profielkenmerk in oplopende of aflopende volgorde rangschikken. Om dit te doen, knevel op **[!UICONTROL Enable sorting]** optie. U kunt bijvoorbeeld een subset beperken tot alleen de bovenste 50 profielen met het hoogste aankoopbedrag.

   ![](../assets/workflow-split-subset.png)

1. Zodra u alle subsets hebt gevormd, kunt u de resterende populatie selecteren die geen van de subsets aanpast en hen in een extra uitgaande overgang omvat. Om dit te doen, knevel op **[!UICONTROL Generate complement]** optie.

   ![](../assets/workflow-split-complement.png)

De activiteit wordt nu gevormd. Bij de uitvoering van de workflow wordt de populatie opgedeeld in de verschillende subsets, in de volgorde waarin ze aan de activiteit zijn toegevoegd.

## Voorbeeld

In het volgende voorbeeld wordt **[!UICONTROL Split]** De activiteit wordt gebruikt om een publiek in verschillende subsets te segmenteren die op het communicatiekanaal worden gebaseerd dat wij willen gebruiken:

* **Subset 1 &quot;push&quot;**: Deze subset bestaat uit alle profielen die onze mobiele toepassing hebben geïnstalleerd.
* **Subset 2 &quot;sms&quot;**: Gebruikers van mobiele telefoons: Voor de resterende populatie die niet in Subset 1 viel, past subset 2 een het filtreren regel op uitgezochte profielen met mobiele telefoons in het gegevensbestand toe.
* **Overgang aanvullen**: Deze overgang legt alle resterende profielen vast die niet overeenkomen met Subset 1 of Subset 2. Het bevat met name profielen die de mobiele toepassing niet hebben geïnstalleerd en geen mobiele telefoon hebben, zoals gebruikers die de mobiele app niet hebben geïnstalleerd of die geen geregistreerd mobiel nummer hebben.

![](../assets/workflow-split-example.png)
