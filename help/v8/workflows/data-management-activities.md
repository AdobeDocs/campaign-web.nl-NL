---
audience: end-user
title: Werken met gegevensbeheeractiviteiten voor workflows
description: Leer hoe u gegevensbeheeractiviteiten kunt gebruiken in Adobe Campaign Web-workflows
badge: label="Alpha" type="Positief"
source-git-commit: 5efcdf2da104b86bf3ee37ee7162495c2d99fb48
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 1%

---

# Data-managementactiviteiten {#data-management}

overzicht: waarvoor ze worden gebruikt, zodat u met hen kunt werken

lijst beschikbare activiteiten + korte beschrijving + verwijzing naar sectie

## Verrijking {#enrichment}

De verrijkingsactiviteit wordt vaak gebruikt in een werkstroom na het richten van activiteiten. Hiermee kunt u de doelgegevens verbeteren met aanvullende informatie uit de database.

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
