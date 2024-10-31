---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: 344d38239df96d570a93aff9674d38b6fd375830
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 8%

---

# Aanvullende informatie  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie "
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

De veranderingen en de verbeteringen beschikbaar met vorige versies worden vermeld [ in deze pagina ](release-notes-24.md).

## Release oktober 1924 {#24-10-release}

**de datum van de Versie**: 29 okt, 2024

De volgende functies en verbeteringen zijn beschikbaar vanaf de release in oktober.

### Functies

<table>
<thead>
<tr>
<th><strong>Externe accounts</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U hebt nu de mogelijkheid om externe accounts direct via de Adobe Campaign Web User Interface in te stellen en te beheren. Met deze nieuwe functie kunt u eenvoudig verschillende typen externe accounts configureren, zoals het stuiteren van e-mailberichten (POP3) of uitvoeringsinstanties.</p>
<p>Raadpleeg de <a href="../administration/external-account.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>


<table>
<thead>
<tr>
<th><strong>Transactieberichten</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Transactieberichten (Message Center) zijn nu beschikbaar in de webgebruikersinterface van Campagne. Deze invoegtoepassing is ontworpen voor het activeren van berichten die worden gegenereerd op basis van gebeurtenissen die worden geactiveerd via informatiesystemen en kan zijn: factuur, orderbevestiging, bevestiging van verzending, wijziging van het wachtwoord, kennisgeving van onbeschikbaarheid van het product, rekeningoverzicht, aanmaak van websiteaccount, enz.</p>
<p>Raadpleeg de <a href="../transactional-messaging/transactional.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<!--table>
<thead>
<tr>
<th><strong>External deliveries</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>You can now define External deliveries, and External delivery templates, in Campaign web user interface. With this mode, messages are generated in an input file which can be shared with your external provider. The External delivery mode is the default mode for the direct mail channel.</p>
</td>
</tr>
</tbody>
</table-->


### Verbeteringen

* **de activiteiten van het Werkschema** - u kunt een activiteit en al zijn kindknopen van een overgang aan een andere binnen een werkschema nu bewegen. Een specifieke **knoop van de Beweging** is beschikbaar in de de eigenschappen van de activiteit ruit om dit uit te voeren. [Meer informatie](../workflows/orchestrate-activities.md#move)

* **de verrijkingsactiviteit van het Werkschema**

   * U kunt een Alias en een Etiket nu bepalen wanneer het creëren van een nieuw gebied in de **Verrijking** activiteit. [Meer informatie](../workflows/activities/enrichment.md#collection-settings)
   * U kunt aanbiedingen voor elk profiel in de **Verrijking** activiteit nu toevoegen. [Meer informatie](../workflows/activities/enrichment.md##add-offers)

* **Distributie van waarden** - wanneer de toegang tot van de lijst van gebieden voor verpersoonlijking, kunt u nu controleren hoe de waarden voor elk gebied worden verdeeld. Een specifiek popup venster toont het aantal en het percentage voor elke waarde. [Meer informatie](../query/build-query.md#distribution-values-query)

* **Versie en systeeminfo** - u kunt tot details over uw instantieversies, zowel voor de cliëntconsole als het Gebruikersinterface van het Web nu toegang hebben. In deze nieuwe sectie worden ook alle ingebouwde pakketten weergegeven die in uw omgeving zijn geïnstalleerd. [Meer informatie](../get-started/user-interface.md#user-interface-about)

* **Lijsten** - u kunt de waarden van een lijst nu gemakkelijk opnieuw in orde brengen. [Meer informatie](../get-started/work-with-folders.md)

* **Levering** - de variabele van de Levering is nu toegankelijk van verpersoonlijkingsgebieden. [Meer informatie](../personalization/conditions.md#use-variables-for-conditional-content-variables-conditional)