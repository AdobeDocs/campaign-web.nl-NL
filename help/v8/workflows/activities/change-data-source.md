---
audience: end-user
title: De werkstroomactiviteit van de gegevensbronworkflow wijzigen gebruiken
description: Leer hoe u de werkstroomactiviteit van de gegevensbronworkflow wijzigen gebruikt
exl-id: 4dd28746-7bc7-49fc-91ac-3312af02ef45
source-git-commit: 1ed20f88d9a11dcac7aa4a3aa93e3058b18c04ff
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 2%

---

# Databron wijzigen {#change-data-source}

>[!CONTEXTUALHELP]
>id="acw_orchestration_change_data_source"
>title="Databron wijzigen"
>abstract="De **gegevensbron van de Verandering** activiteit staat u toe om een verschillende gegevensbron voor de het Werken lijst van uw werkschema te selecteren."

De **gegevensbron van de Verandering** activiteit is a **richtend** activiteit. Met deze activiteit kunt u de gegevensbron wijzigen die wordt gebruikt door de werkstroomlijst. Dit biedt meer flexibiliteit door u toe te staan om gegevens over uw verschillende gegevensbestanden te beheren en prestaties te verbeteren.

In werkschema&#39;s, wordt het gegeven dat van één activiteit aan een andere door overgangen wordt vervoerd opgeslagen in een tijdelijke **het Werken lijst**. Standaard worden werktabellen gemaakt in dezelfde database als de bron van de verwerkte gegevens. Als u bijvoorbeeld een query uitvoert op de tabel &quot;Profielen&quot; die is opgeslagen in de Cloud-database, wordt een tabel voor werken gemaakt in dezelfde Cloud-database.

In sommige gevallen zijn gegevens niet beschikbaar in de huidige database of zijn ze niet efficiënt genoeg om eenheidsbewerkingen uit te voeren. Daarom moet u de workflow mogelijk dwingen een andere database te gebruiken om dergelijke bewerkingen uit te voeren door een **[!UICONTROL Change data source]** -activiteit toe te voegen.

De gedetailleerde informatie over de architectuur van de Campagne is beschikbaar in [&#x200B; Campagne v8 (cliëntconsole) documentatie &#x200B;](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/architecture/architecture.html).

>[!IMPORTANT]
>
>De activiteiten **[!UICONTROL Change Dimension]** en **[!UICONTROL Change Data source]** mogen niet in één rij worden toegevoegd. Als u beide activiteiten opeenvolgend wilt gebruiken, neemt u er een **[!UICONTROL Enrichment]** activiteit tussen op. Dit zorgt voor een correcte uitvoering en voorkomt mogelijke conflicten of fouten.

>[!NOTE]
>
>De **activiteit van de Gegevens van de Verandering Source** kan een maximum van één miljoen verslagen per uitvoering verwerken. Neem contact op met uw Adobe-vertegenwoordiger als u deze limiet wilt verhogen.

<!--

Let's say you want to send VIP customers a unique offer code that they can redeem on your online store. To do this, you need to:

1. Query VIP customers on the "Profiles" table located on the Cloud database,
1. Retrieve an offer code for each targeted profile through API calls,
1. Update each profile with the assigned offer code,
1. Send an email to the profiles with their offer code.

In this situation, it is recommended to execute the offer code assignment operation on the local database, which is better suited for unitary operations. To do this, you need to add a **[!UICONTROL Change data source]** activity before the operation in order to execute it on the Campaign local database.

Before executing the operation, the working table is copied to the local database so that the operation can run there. Once done, the system detects that the profiles that we want to update are on another location. The data is therefore automatically copied back to the Cloud database where the "Profiles" table is located.
-->

## Vorm de de gegevensbronactiviteit van de Verandering {#configure}

Volg deze stappen om de **gegevensbron van de Verandering** activiteit te vormen:

![&#x200B; Schermafbeelding die toont hoe te om de de gegevensbronactiviteit van de Verandering aan een werkschema toe te voegen.](../assets/workflow-change-data-source-add.png)

1. Voeg de gegevensbron van de a **Verandering** activiteit aan uw werkschema toe.

1. Definieer de gegevensbron waar u de werktabel wilt verplaatsen:

   * **[!UICONTROL Default Campaign database (PostgreSQL)]**: de lokale standaarddatabase voor campagne gebruiken.
   * **[!UICONTROL FDA external account]**: gebruik externe Cloud-databases die zijn verbonden met Adobe Campaign via de Federated Data Access-functie.

     >[!AVAILABILITY]
     >
     >De configuratie van de campagne en de verbinding aan externe systemen worden beperkt tot geavanceerde gebruikers en slechts beschikbaar bij de cliëntconsole. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/fda.html){target="_blank"}

1. Configureer uw workflow om de gewenste bewerkingen uit te voeren met de nieuwe gegevensbron.

<!--
## Example {#example}

The workflow below illustrates the use case detailed earlier, sending VIP customers offer codes that they can redeem on our online store.

-->