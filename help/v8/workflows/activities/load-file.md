---
audience: end-user
title: De werkstroomactiviteit voor het laden van bestanden gebruiken
description: Leer hoe u de workflowactiviteit Bestand laden gebruikt
badge: label="Beperkte beschikbaarheid"
source-git-commit: 88daf84e617595a80c5cd3fd536969618f0fdcf5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 1%

---

# Bestand laden {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Bestandsactiviteit laden"
>abstract="De **Bestand laden** activiteit is **Gegevensbeheer** activiteit. Gebruik deze activiteit om met gegevens te werken die in een extern dossier worden opgeslagen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Voorbeeldbestand"
>abstract="Voorbeeldbestand"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Naam van het bestand"
>abstract="Naam van het bestand"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Doeldatabase"
>abstract="Doeldatabase"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Afwijzen van beheer voor het laden van bestandsactiviteiten"
>abstract="Afwijzen van beheer voor het laden van bestandsactiviteiten"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Uitgaande overgang van beheer afwijzen"
>abstract="Uitgaande overgang van beheer afwijzen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Uitgaande overgang van beheer afwijzen voor afwijzing"
>abstract="Uitgaande overgang van beheer afwijzen voor afwijzing"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Opmaak voor het laden van bestandsactiviteit"
>abstract="Opmaak voor het laden van bestandsactiviteit"


De **Bestand laden** activiteit is **Gegevensbeheer** activiteit. Gebruik deze activiteit om met profielen en gegevens te werken die in een extern dossier worden opgeslagen. Profielen en gegevens worden niet toegevoegd aan de database, maar alle velden in het invoerbestand zijn beschikbaar voor [personalisatie](../../personalization/gs-personalization.md)of om profielen of een andere tabel bij te werken.


>[!NOTE]
>Ondersteunde bestandsindelingen zijn: tekst (TXT) en door komma&#39;s gescheiden waarden (CSV).


Deze activiteit kan worden gebruikt met een [Verzoening](reconciliation.md) activiteit om niet-geïdentificeerde gegevens aan bestaande middelen te koppelen. Bijvoorbeeld de **Bestand laden** activiteit kan vóór een **Verzoening** activiteit als u niet-standaardgegevens in het gegevensbestand invoert.


## De activiteit van het bestand laden configureren {#load-configuration}

Voer de volgende stappen uit om de **Bestand laden** activiteit:


1. Sleep een **Bestand laden** in uw workflow. Klik op de knop **Selecteren uit bestand** knop.
1. Selecteer het lokale bestand dat u wilt gebruiken. De indeling moet hiermee worden uitgelijnd [voorbeeldbestand](../../audience/file-audience.md#sample-file).
1. In het centrale gedeelte van het scherm kunt u bekijken en controleren hoe gegevens worden toegewezen.
1. Pas de kolominstellingen aan en maak gegevens op van de beschikbare opties.
1. Klikken **Bevestigen** als de instellingen correct zijn.

## Voorbeeld{#load-example}

Er is een voorbeeld van het laden van een extern bestand beschikbaar in het dialoogvenster **Verzoening** activiteit in [deze sectie](reconciliation.md#example).