---
title: Opmerkingen bij de laatste release
description: Ontdek nieuwe eigenschap die met het Web van de Campagne Gebruikersinterface komt
source-git-commit: 45795b35fd2c02f7b513b0d4952504ca3f5f45c3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# Aanvullende informatie  {#latest-release}

<!--Last update: **March 19, 2024**-->

De gebruikersinterfaceversies van het Web van Adobe Campaign werken op een ononderbroken leveringsmodel dat voor een scalable, gefaseerde benadering van eigenschapplaatsing toestaat. Deze releaseopmerkingen worden daarom meerdere keren per maand bijgewerkt. Controleer ze regelmatig.

>[!AVAILABILITY]
>
>Deze versie is beschikbaar voor alle gebruikers die beginnen [Campagne (console) v8.6-release](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/release-notes.html). Meer informatie over de release en upgrades van de Adobe Campaign-clientconsole in [Campagne v8 (console)-documentatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/releases/upgrades.html){target="_blank"}.

## Release maart {#24-3-release}

**Releasedatum**: 19-20 maart 2024

### Direct Mail Channel {#24-3-dm}

**Directe post** kanaal is nu beschikbaar voor gebruik in werkschema&#39;s en als standalone leveringen. Directe post is een off-line kanaal dat u toestaat om een extractiedossiers tot stand te brengen, te personaliseren en te produceren, en het met uw directe postleveranciers te delen om post naar uw klanten te verzenden. [Meer informatie](../direct-mail/gs-direct-mail.md)

![](../assets/do-not-localize/direct-mail.gif)

### Nieuwe werkstroomactiviteit gegevensbron wijzigen {#24-3-change-data-source}

De **Gegevensbron wijzigen** Door doelactiviteit toe te wijzen, kunt u de gegevensbron wijzigen die wordt gebruikt door de werktabel van uw werkstroom. Deze activiteit verstrekt meer flexibiliteit door u toe te staan om gegevens over uw verschillende gegevensbestanden te beheren en prestaties te verbeteren. [Meer informatie](../workflows/activities/change-data-source.md)

![](../assets/do-not-localize/change-data-source.gif)

### Verbetering van workflowactiviteit splitsen {#24-3-split}

U kunt nu de opdracht **Alle subsets in dezelfde tabel genereren** in de **Splitsen** workflowactiviteit om alle subsets te groeperen in één uitvoerovergang. [Meer informatie](../workflows/activities/split.md)

### Query-modelleraar {#24-3-query-modeler}

* Het querymodel is nu beschikbaar voor gebruik in de e-mailontwerper. Hiermee kunt u voorwaarden maken wanneer u voorwaardelijke inhoud maakt. [Meer informatie](../personalization/conditions.md)
* Vooraf gedefinieerde waarden zijn nu beschikbaar voor datumtekstkenmerken wanneer u een aangepaste voorwaarde maakt. [Meer informatie](../query/build-query.md)
* Operatoren kunnen niet meer worden toegevoegd aan een nieuwe overgang in het diagram. Ze kunnen alleen aan een bestaande overgang worden toegevoegd voordat u componenten filtert om deze samen te groeperen. [Meer informatie](../query/build-query.md)
