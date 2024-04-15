---
audience: end-user
title: De werkstroomactiviteit voor het laden van bestanden gebruiken
description: Leer hoe u de workflowactiviteit Bestand laden gebruikt
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: 935fba929c26d6d7b3057ee7c24148215a04e45e
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

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

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Doelbestand voor laden van bestandsactiviteit"
>abstract="Doelbestand voor laden van bestandsactiviteit"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Waarde opnieuw toewijzen voor activiteit van bestand laden"
>abstract="Waarde opnieuw toewijzen voor activiteit van bestand laden"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Bestand laden, opdracht"
>abstract="Het toestaan van arbitraire bevel voor preprocessing is een veiligheidszorg, maak veiligheidsoptie XtkSecurity_Disable_Preproc onbruikbaar om het gebruik van een vooraf bepaalde lijst van bevelen te dwingen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Bestand verwijderen na importeren"
>abstract="Schakelen tussen **Bestand verwijderen na importeren** om het oorspronkelijke bestand van de server te verwijderen nadat het bestand is geïmporteerd."

De **Bestand laden** activiteit is **Gegevensbeheer** activiteit. Gebruik deze activiteit om met profielen en gegevens te werken die in een extern dossier worden opgeslagen. Profielen en gegevens worden niet toegevoegd aan de database, maar alle velden in het invoerbestand zijn beschikbaar voor [personalisatie](../../personalization/gs-personalization.md)of om profielen of een andere tabel bij te werken.

>[!NOTE]
>Ondersteunde bestandsindelingen zijn: tekst (TXT) en door komma&#39;s gescheiden waarden (CSV).

Deze activiteit kan worden gebruikt met een [Verzoening](reconciliation.md) activiteit om niet-geïdentificeerde gegevens aan bestaande middelen te koppelen. Bijvoorbeeld de **Bestand laden** activiteit kan vóór een **Verzoening** activiteit als u niet-standaardgegevens in het gegevensbestand invoert.

## De activiteit van het bestand laden configureren {#load-configuration}

Voer de volgende stappen uit om de **Bestand laden** activiteit:

1. Voeg een **Bestand laden** in uw workflow. Klik op de knop **Selecteren uit bestand** knop.

1. Selecteer het lokale bestand dat u wilt gebruiken. De indeling moet hiermee worden uitgelijnd [voorbeeldbestand](../../audience/file-audience.md#sample-file).

1. In het centrale gedeelte van het scherm kunt u bekijken en controleren hoe gegevens worden toegewezen.

   ![](../assets/load-file.png)

1. Gebruik de **Kolommen** in het linkerdeelvenster om het gegevenstype en de breedte voor elke kolom aan te passen.

1. In de **Opmaak** onder de kolomconfiguratie, specificeer hoe het externe dossier wordt geformatteerd om ervoor te zorgen dat de gegevens correct worden ingevoerd.

1. Klikken **Bevestigen** als de instellingen correct zijn.

## Voorbeeld{#load-example}

Een voorbeeld van een extern bestand dat wordt geladen en dat wordt gebruikt voor de **Verzoening** activiteit is beschikbaar in [deze sectie](reconciliation.md#reconciliation-example).
