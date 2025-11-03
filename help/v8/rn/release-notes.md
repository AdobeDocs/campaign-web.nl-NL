---
title: Opmerkingen bij de release Campagne v8 Web User Interface
description: Ontdek nieuwe eigenschappen die met de recentste versie van de Gebruikersinterface van het Web van de Campagne komen
exl-id: a0d2ab24-1854-4ad6-8a8c-b55488b20bf9
source-git-commit: cf576041294efc1c699fee4cb5ffb7ad68b78953
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 7%

---

# Aanvullende informatie  {#latest-release}

>[!CONTEXTUALHELP]
>id="acw_homepage_learning_card2"
>title="Aanvullende informatie "
>abstract="De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Opmerkingen bij de release Campagne worden daarom meerdere keren per maand bijgewerkt met de nieuwste functies, verbeteringen en correcties. We raden u aan deze regelmatig te controleren."

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

De veranderingen en de verbeteringen beschikbaar met vorige versies worden vermeld in [ 2024 ](release-notes-24.md) en [ 2025 ](release-notes-25.md) pagina&#39;s.

## Release oktober 1925 {#25-10-updates}

_3 Nov., 2025_

<table>
<thead>
<tr>
<th><strong>Meertalige mogelijkheden voor transactioneel berichtenverkeer, pushberichten en sms (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>U kunt nu meerdere transactieberichten, pushberichten en SMS-berichten in verschillende talen verzenden in de Adobe Campaign Web User Interface. Met de functie Meertalige levering kunt u de standaardtaal van uw levering kiezen en de verschillende talen waarin de levering kan worden verzonden. U kunt deze leveringen ook voorvertonen in de talen die u hebt gekozen.</p>
<p>Opmerking: deze mogelijkheid is alleen beschikbaar voor een aantal organisaties (Beperkte beschikbaarheid) en wordt in een toekomstige release globaal geïmplementeerd.</p>
<p>Raadpleeg de <a href="../msg/multilingual.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<!--
* Enable OOTB File Upload for Multi-lingual Push Notification Deliveries. 
-->

<table>
<thead>
<tr>
<th><strong>Profielverrijking in Transactionele Berichten (LA)</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Met deze functie kunt u transactieberichten personaliseren door Adobe Campaign-databasevelden aan de inhoud van het bericht te koppelen. U kunt doeltoewijzingen, verrijkingskolommen, en een verzoeningssleutel selecteren om nauwkeurige, real-time verpersoonlijking te verzekeren terwijl het handhaven van prestatiesdrempels.</p>
<p>Opmerking: deze mogelijkheid is alleen beschikbaar voor een aantal organisaties (Beperkte beschikbaarheid) en wordt in een toekomstige release globaal geïmplementeerd. Deze functie is momenteel alleen beschikbaar voor e-mails.</p>
<p>Raadpleeg de <a href="../transactional-messaging/profile-enrichment.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Integratie met Adobe GenStudio</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Om de marketingefficiëntie te verbeteren en de consistentie van uw merk te behouden, kunt u nu probleemloos GenStudio for Performance Marketing-ervaringen integreren met Campagne. Zo kunt u GenStudio-content voor AI-kracht samen met de geavanceerde orkestmogelijkheden van Campaign maken.<p>
<p>Raadpleeg de <a href="../integrations/genstudio.md">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Ondersteuning voor de modus Donker in de e-mailontwerper</strong><br/></th> 
</tr>
</thead>
<tbody>
<tr>
<td>
<p>De e-mailweergave van Designer biedt nu de mogelijkheid om over te schakelen naar de weergave in de donkere modus, waarin u aanvullende specifieke aangepaste instellingen kunt definiëren. De uiteindelijke rendering is afhankelijk van de e-mailclient van de ontvanger. Niet alle e-mailclients ondersteunen de donkere modus.</p>
<p>Raadpleeg de <a href="../email/accessible-content.md#dark-mode">gedetailleerde documentatie</a> voor meer informatie.</p>
</td>
</tr>
</tbody>
</table>

<!-- table>
<thead>
<tr>
<th><strong>Continuous delivery activity</strong><br/></th> not ready
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Continuous delivery activity</p>
<p>For more information, refer to the detailed documentation.</p>
</td>
</tr>
</tbody>
</table-->

### Verbeteringen {#25-10-improvements}

* In leveringen die in de cliëntConsole worden gecreeerd, wijst de **sectie van het publiek** nu erop of een dynamische voorwaarde voor proefdoelstellingen is bepaald. <!-- [Learn more](../msg/gs-deliveries.md#access)-->

* U kunt nu schakelen tussen de nieuwe en de oude builder voor regels wanneer u een voorwaarde instelt met behulp van de mogelijkheid voor voorwaardelijke inhoud via e-mail Designer. <!-- [Learn more](../personalization/conditions.md#condition-condition-builder)-->

* U kunt nu verzamelingskoppelingen, zoals aankopen, selecteren in de schermdefinitie van het schema Ontvangers. Hiermee worden de gerelateerde gegevens op profielschermen weergegeven via een speciaal tabblad. <!-- [Learn more](../administration/schemas.md#collection-lists)-->

* Als campagnebeheerder kunt u nu verbindingen instellen met Salesforce CRM en Microsoft Dynamics.
  [Meer informatie](../administration/external-crm.md)

<!--
* Stop button for deliveries not linked to release and no info
-->

