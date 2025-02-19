---
title: Werken met schema's
description: Leer hoe u met schema's werkt.
source-git-commit: 1f3f3afb9b21ab37aeea73057d832cea172c00bf
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Werken met schema&#39;s {#schemas}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Werken met schema&#39;s"
>abstract="U kunt tot de details van een schema nu toegang hebben door zijn naam in de lijst te selecteren. De de gebiedsuitgave van de douane is ook toegankelijk van **geeft de knoop van het douanedetail** uit."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"



>[!CONTEXTUALHELP]
>id="acw_schema"
>title="Schemas"
>abstract="**[!DNL Adobe Campaign]** gebruikt op XML gebaseerde schema&#39;s om de fysieke en logische structuur van gegevens binnen de toepassing te bepalen. Van dit scherm, kunt u alle bestaande schema&#39;s bekijken en tot de details van een schema toegang hebben door zijn naam in de lijst te selecteren. Er zijn filters beschikbaar waarmee u de lijst kunt verfijnen, zoals alleen bewerkbare schema&#39;s weergeven."

## Over schema&#39;s {#about}

**[!DNL Adobe Campaign]** gebruikt op XML gebaseerde schema&#39;s om de fysieke en logische structuur van gegevens binnen de toepassing te bepalen. Een schema is een XML-document dat is gekoppeld aan een databasetabel die het volgende definieert:

* De SQL-tabelstructuur (tabelnaam, velden, relaties).
* De XML-gegevensstructuur (elementen, kenmerken, hiërarchie, typen, standaardwaarden, labels).

Schema&#39;s spelen een sleutelrol in:

* Toepassingsgegevens toewijzen aan databasetabellen.
* Relaties tussen gegevensobjecten definiëren.
* De structuur en eigenschappen van elk veld opgeven.

Elke entiteit in Adobe Campaign heeft een speciaal schema, dat zorgt voor consistentie en organisatie van de gegevens.

De gedetailleerde informatie over schema&#39;s is beschikbaar in de [ de consoledocumentatie van de Campagne ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas) {target="_blank"}

## De schema&#39;s van de toegang in het Gebruikersinterface van het Web {#access}

Schema&#39;s zijn toegankelijk via het menu **[!UICONTROL Administration]** > **[!UICONTROL Schemas]** .

![](assets/schemas-list.png)

Vanuit dit scherm kunt u alle bestaande schema&#39;s weergeven. Er zijn filters beschikbaar waarmee u de lijst kunt verfijnen, zoals alleen bewerkbare schema&#39;s weergeven.

Als u een schema wilt openen, selecteert u de naam ervan. Er wordt een gedetailleerde schemaweergave weergegeven.

![](assets/schema-details.png)

### Overzicht van schema {#overview}

Het tabblad **[!UICONTROL Overview]** biedt een algemene weergave van het schema:

* In de sectie **[!UICONTROL Properties]** worden belangrijke gegevens weergegeven, zoals de naam van het schema, de naamruimte en de bijbehorende tabelnaam.

* In de sectie **[!UICONTROL Schema definition]** worden details over de schemadefinitie weergegeven, zoals de primaire sleutel die wordt gebruikt voor het afstemmen van gegevens en de koppelingen naar andere tabellen.

  Klik op de knop **[!UICONTROL Schema preview]** om de verschillende velden en koppelingen waaruit het schema bestaat, weer te geven. Hierdoor kunt u de volledige structuur van een schema controleren. Als het schema is uitgebreid met aangepaste velden, kunt u alle extensies visualiseren.

* In de sectie **[!UICONTROL Content]** wordt de XML-inhoud van het schema weergegeven, zodat u kunt schakelen tussen de bron en de gegenereerde syntaxis.

### Schema-gegevens {#data}

Het tabblad **[!UICONTROL Data]** bevat informatie over de schemagegevens.

![](assets/schemas-data.png)

## Aangepaste velden bewerken {#fields}

Aangepaste velden zijn aanvullende kenmerken die via de Adobe Campaign-console aan out-of-the-box-schema&#39;s worden toegevoegd. Zij staan u toe om schema&#39;s aan te passen door nieuwe attributen aan de behoeften van uw organisatie te omvatten.

De gebieden van de douane kunnen in diverse schermen zoals profieldetails in de interface van het Web van de Campagne worden getoond. U kunt bepalen welke velden zichtbaar zijn en hoe ze in de interface worden weergegeven. Klik hiertoe op de knop **[!UICONTROL Edit custom detail]** in het menu **[!UICONTROL Schemas]** .

![](assets/schemas-custom.png)

De gedetailleerde informatie over hoe te om douanegebieden in een schema uit te geven, verwijs naar deze sectie: [ vormt douanegebieden ](../administration/custom-fields.md).
