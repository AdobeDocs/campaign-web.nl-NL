---
audience: end-user
title: Doelontvangers uit een bestand
description: Leer hoe u ontvangers uit een extern bestand kunt gebruiken om uw e-mailpubliek te maken
badge: label="Beta"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: d14a461d558dec06613d7f009b347e1191c3400f
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Een e-mailpubliek laden vanuit een bestand {#audience-from-file}

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

U kunt contactpersonen uploaden vanuit een extern bestand. Profielen worden niet toegevoegd aan de database, maar alle velden in het invoerbestand zijn beschikbaar voor [personalisatie](../personalization/gs-personalization.md). Ondersteunde bestandsindelingen zijn: tekst (TXT) en door komma&#39;s gescheiden waarden (CSV).

>[!CAUTION]
>
>* Deze mogelijkheid is alleen beschikbaar voor **zelfstandige e-maillevering**. Het kan niet in werkschema&#39;s, noch met SMS of de levering van de Duw worden gebruikt.
>
>* U kunt niet [controlegroepen](control-group.md) bij het laden van de doelpopulatie uit een extern bestand.


Voer de volgende stappen uit als u profielen rechtstreeks vanuit de e-mailinterface in een lokaal bestand als doel wilt instellen:

1. Open een bestaande e-maillevering, of [een nieuwe e-maillevering maken](../email/create-email.md).
1. In het venster voor het maken van de e-maillevering, vanuit het dialoogvenster **Publiek** klikt u op de **Doelgroep selecteren** en kiest u de **Selecteren uit bestand** -optie.

   ![](assets/select-from-file.png)

1. Selecteer het lokale bestand dat u wilt uploaden. De indeling moet worden uitgelijnd met de [voorbeeldbestand](#sample-file).
1. In het centrale gedeelte van het scherm kunt u bekijken en controleren hoe gegevens worden toegewezen.
1. Kies de kolom die het e-mailadres bevat in het menu **Adresveld** vervolgkeuzelijst. U kunt de kolom van de lijst van gewezen personen ook selecteren als u dergelijke informatie in het inputdossier hebt.
1. Pas de kolominstellingen aan en maak gegevens op van de beschikbare opties.
1. Klikken **Bevestigen** als de instellingen correct zijn.

Wanneer u de inhoud van het bericht maakt en aan uw wensen aanpast, kunt u velden selecteren uit het invoerbestand in het dialoogvenster [Personalisatie-editor](../personalization/gs-personalization.md).

![](assets/select-external-perso.png)


## Voorbeeldbestand {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Een publiek uit een bestand laden"
>abstract="Ondersteunde bestandsindelingen zijn TXT en CSV. Eerste regel gebruiken als kolomkop. Lijn de bestandsindeling uit met het voorbeeldbestand in de onderstaande koppeling."

Ondersteunde indelingen zijn TXT en CSV. De eerste regel is de kolomkop.

Lijn de bestandsindeling uit met het onderstaande voorbeeldbestand:

```javascript
{
lastname,firstname,city,birthdate,email,denylist
Smith,Hayden,Paris,23/05/1985,hayden.smith@example.com,0
Mars,Daniel,London,17/11/1999,danny.mars@example.com,0
Smith,Clara,Roma,08/02/1979,clara.smith@example.com,0
Durance,Allison,San Francisco,15/12/2000,allison.durance@example.com,1
}
```
