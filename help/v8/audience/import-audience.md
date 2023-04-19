---
audience: end-user
title: Ontvangers uit een bestand importeren
description: Leer hoe u ontvangers kunt importeren uit een extern bestand
badge: label="Alpha" type="Positief"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: f103fe804deccc83638a3e56a03f6e715e68e550
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Ontvangers uit een bestand importeren {#audience-from-file}

U kunt contacten van de leveringsinterface toevoegen of bijwerken, door een tekstdossier (TXT) of een komma-gescheiden waardedossier (CSV) te uploaden. Zij zullen dan aan het gegevensbestand worden toegevoegd.

>[!NOTE]
>
>U kunt ook een importworkflow maken om meerdere profielen toe te voegen of bij te werken.


Voer de volgende stappen uit om profielen uit een lokaal bestand rechtstreeks vanuit de interface toe te voegen:

1. Klik in het venster voor het maken van de aflevering op de knop **Doelgroep selecteren** en selecteert u de **Selecteren uit bestand** optie.
1. Selecteer het lokale bestand dat u wilt uploaden.
1. Definieer de kolominstellingen en hoe u gegevens wilt opmaken. U kunt een kolom overslaan met de opdracht **Kolom negeren** schakelen.
1. Geef een voorvertoning weer van hoe gegevens worden toegewezen in het centrale gedeelte van het scherm.
1. Klikken **Bevestigen** als de instellingen correct zijn.

Wanneer u de inhoud van het bericht maakt en aanpast, kunt u velden uit het invoerbestand selecteren in de Persoonlijke editor.

## Voorbeeldbestand {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Voorbeeldbestand"
>abstract="Ondersteunde bestandsindelingen: txt, csv, xls. Eerste regel gebruiken als kolomkop."


```json
{
lastname,firstname,birthdate,email,crmID
Smith,Hayden,23/05/1989,hayden.smith@example.com,124365
Mars,Daniel,17/11/1987,dannymars@example.com,123545
Smith,Clara,08/02/1989,clara.smith@example.com,124567
Durance,Allison,15/12/1978,allison.durance@example.com,120987
}
```
