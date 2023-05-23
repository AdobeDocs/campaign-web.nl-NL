---
audience: end-user
title: Doelontvangers uit een bestand
description: Leer hoe u ontvangers uit een extern bestand kunt gebruiken om uw e-mailpubliek te maken
badge: label="Alpha" type="Positief"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: 7893f3132689446db388613ad5ec033ca5f26bf5
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Doelontvangers uit een bestand {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Bestandselectie"
>abstract="Selecteer het lokale bestand dat u wilt uploaden. Ondersteunde indelingen zijn TXT en CSV. Lijn de bestandsindeling uit met het voorbeeldbestand dat hieronder is gekoppeld."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Kolomdefinitie"
>abstract="Controleer de indeling van de kolommen die u wilt invoegen vanuit uw lokale bestand."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parameters opmaken"
>abstract="Controleer de opmaakparameters voor het bestand."

U kunt contactpersonen uploaden vanuit een extern bestand. Deze mogelijkheid is alleen beschikbaar voor e-mailleveringen. Ondersteunde bestandsindelingen zijn: tekst (TXT) en komma-gescheiden waarde (CSV). Profielen worden niet toegevoegd aan de database, maar alle velden in het invoerbestand zijn beschikbaar voor personalisatie.

>[!NOTE]
>
>U kunt een importworkflow maken om meerdere profielen aan de database toe te voegen of bij te werken. Meer informatie


Voer de volgende stappen uit als u profielen rechtstreeks vanuit de interface wilt richten op een lokaal bestand:

1. In het venster voor het maken van de e-maillevering, vanuit het dialoogvenster **Publiek** klikt u op de **Doelgroep selecteren** en kiest u **Selecteren uit bestand** optie.

   ![](assets/select-from-file.png)

1. Selecteer het lokale bestand dat u wilt uploaden.
1. In het centrale gedeelte van het scherm kunt u bekijken en controleren hoe gegevens worden toegewezen.
1. Kies de kolom die het e-mailadres bevat in het menu **Adresveld** vervolgkeuzelijst. U kunt de kolom van de lijst van gewezen personen ook selecteren als u dergelijke informatie in het inputdossier hebt.
1. Pas de kolominstellingen aan en maak gegevens op van de beschikbare opties.
1. Klikken **Bevestigen** als de instellingen correct zijn.

Wanneer u de inhoud van het bericht maakt en aanpast, kunt u velden uit het invoerbestand selecteren in de Persoonlijke editor.

![](assets/select-external-perso.png)

## Voorbeeldbestand {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Voorbeeldbestand"
>abstract="Ondersteunde bestandsindelingen: txt, csv. Eerste regel gebruiken als kolomkop."


```json
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,dannymars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
