---
audience: end-user
title: Werken met workflowactiviteiten
description: Meer informatie over workflowactiviteiten
badge: label="Alpha" type="Positief"
exl-id: 6ba3bcfd-84eb-476c-837d-5aa473b820cd
source-git-commit: 92444d4ee324f64a35f4cca0b40907bdf453732c
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 1%

---


# Workflowactiviteiten {#workflow-activities}

## Targetingactiviteiten {#targeting}

inhoud-TBD

<!--à reformuler-->Met deze activiteiten kunt u een of meer doelen maken door sets te definiëren en deze sets te splitsen of te combineren met behulp van doorsnede-, samenvoegings- of uitsluitingsbewerkingen.


## Stroombeheeractiviteiten {#flow-control}

inhoud-TBD

<!--à reformuler-->Met deze activiteiten kunt u een of meer doelen maken door sets te definiëren en deze sets te splitsen of te combineren met behulp van doorsnede-, samenvoegings- of uitsluitingsbewerkingen.

De activiteiten van de debietcontrole worden gebruikt om de werkschemaactiviteiten te coördineren.

## Data-managementactiviteiten {#data-management}

overzicht: waarvoor ze worden gebruikt, zodat u met hen kunt werken

lijst beschikbare activiteiten + korte beschrijving + verwijzing naar sectie

### Verrijking {#enrichment}

>[!CONTEXTUALHELP]
>id="acw_orchestration_enrichment_data"
>title="Verrijkingsactiviteit"
>abstract="Met de verrijkingsactiviteit kunt u de doelgegevens verbeteren met aanvullende informatie uit de database. Het wordt vaak gebruikt in een werkstroom na het richten van activiteiten.<br/>Zodra de verrijkingsgegevens aan het werkschema zijn toegevoegd, kan het in de activiteiten worden gebruikt die na de activiteit van de Verrijking worden toegevoegd om klanten in verschillende groepen te segmenteren die op hun gedrag, voorkeur, en behoeften worden gebaseerd, of om gepersonaliseerde marketing berichten en campagnes te creëren die eerder met uw doelpubliek zullen resoneren."

Met de verrijkingsactiviteit kunt u de doelgegevens verbeteren met aanvullende informatie uit de database. Het wordt vaak gebruikt in een werkstroom na het richten van activiteiten.

Verrijkingsgegevens kunnen worden verkregen:

* **Van dezelfde werktabel** als doelversie in uw workflow:

   *Stel een groep klanten in en voeg het veld Geboortedatum toe aan de huidige tabel*

* **Van een andere werktabel**:

   *Selecteer een groep klanten en voeg de velden Bedrag en Type product uit de tabel Aankoop toe*.

Zodra de verrijkingsgegevens aan het werkschema zijn toegevoegd, kan het dan in de activiteiten worden gebruikt die na de activiteit van de Verrijking worden toegevoegd om klanten in verschillende groepen te segmenteren die op hun gedrag, voorkeur, en behoeften worden gebaseerd, of om gepersonaliseerde marketing berichten en campagnes te creëren die eerder met uw doelpubliek zullen resoneren.

U kunt bijvoorbeeld informatie over aankopen van klanten toevoegen aan de werkstroomwerktabel en deze gegevens gebruiken om de e-mails aan te passen aan de laatste aankoop of het bedrag dat aan deze aankopen is besteed.

Voer de volgende stappen uit om een verrijkingsactiviteit toe te voegen aan uw workflow:

1. activiteit toevoegen
1. kenmerk selecteren dat moet worden gebruikt als verrijkingsgegevens

   Optie Geavanceerde velden weergeven i-knop

   opmerking: kenmerken van de doeldimensie

1. Selecteer hoe de gegevens worden verzameld
1. aantal records dat moet worden opgehaald als u een verzameling van meerdere records wilt ophalen
1. Filters toepassen en regel bouwen

   Selecteer een bestaand filter om het filter op te slaan, zodat u de weergaveresultaten van het filter visueel of in de codeweergave kunt hergebruiken

1. records sorteren met een kenmerk

hefboomwerking verrijkingsgegevens in campagne

waar we de verrijkingsgegevens kunnen gebruiken : e-mail, andere gebruiksgevallen personaliseren?
