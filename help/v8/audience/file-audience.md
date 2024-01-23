---
audience: end-user
title: Doelontvangers uit een bestand
description: Leer hoe u ontvangers uit een extern bestand kunt gebruiken om uw e-mailpubliek te maken
badge: label="Beperkte beschikbaarheid"
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: a3476e46c29723af8246683a005543cfd605e7df
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 1%

---

# Een e-mailpubliek laden vanuit een bestand {#audience-from-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_select"
>title="Bestandselectie"
>abstract="Selecteer het lokale bestand dat u wilt uploaden. Ondersteunde indelingen zijn TXT en CSV. Lijn de bestandsindeling uit met het voorbeeldbestand dat hieronder is gekoppeld."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_columns"
>title="Kolomdefinitie"
>abstract="Controleer de indeling van de kolommen in het externe bestand."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_formatting"
>title="Parameters opmaken"
>abstract="Geef op hoe het externe bestand wordt opgemaakt om ervoor te zorgen dat de gegevens correct worden geïmporteerd."

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_preview"
>title="Een voorbeeld van uw bestand bekijken"
>abstract="Controleer de voorvertoning van de kolommen van het externe bestand. Dit scherm toont slechts tot 30 verslagen."

U kunt doelprofielen opgeven die zijn opgeslagen in een extern bestand. Profielen worden niet toegevoegd aan de database, maar alle velden in het invoerbestand zijn beschikbaar voor [personalisatie](../personalization/gs-personalization.md). Ondersteunde bestandsindelingen zijn: tekst (TXT) en door komma&#39;s gescheiden waarden (CSV). In dit artikel wordt beschreven hoe u een extern profiel kunt laden wanneer u een zelfstandige e-maillevering maakt. Als u gegevens uit een bestand in een workflow wilt laden, raadpleegt u [deze pagina](../workflows/activities/load-file.md).

>[!CAUTION]
>
>* Deze mogelijkheid is alleen beschikbaar voor **e-mailleveringen**. Deze kan niet worden gebruikt met SMS of Push-berichten.
>
>* U kunt niet [controlegroepen](control-group.md) bij het laden van de doelpopulatie uit een extern bestand.
>
>* Profielen worden niet toegevoegd aan de database en alleen geladen en beschikbaar voor deze specifieke zelfstandige e-maillevering.

## Uw bestand selecteren en configureren {#upload}

Voer de volgende stappen uit als u profielen rechtstreeks vanuit de e-mailinterface in een lokaal bestand als doel wilt instellen:

1. Open een bestaande e-maillevering, of [een nieuwe e-maillevering maken](../email/create-email.md).
1. In het venster voor het maken van de e-maillevering, vanuit het dialoogvenster **Publiek** klikt u op de **Doelgroep selecteren** en kiest u de **Selecteren uit bestand** -optie.

   ![](assets/select-from-file.png)

1. Selecteer het lokale bestand dat u wilt gebruiken. De indeling moet worden uitgelijnd met de [voorbeeldbestand](#sample-file).
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

## Uw e-mail voorvertonen en testen {#test}

Met Campagne Web kunt u teste-mails voorvertonen en verzenden wanneer u een publiek gebruikt dat vanuit een bestand is geüpload. Ga als volgt te werk om dit te doen:

1. Klik op de knop **[!UICONTROL Simulate content button]** vanuit het bewerkingsscherm voor de inhoud van de levering en klik op de knop **[!UICONTROL Add test profile(s)]** knop.

1. De profielen in de geüploade bestandsweergave. Selecteer de profielen die u wilt gebruiken voor de voorvertoning van uw inhoud en klik op **[!UICONTROL Select]**.

1. Een voorvertoning van de leveringsinhoud wordt weergegeven in het rechterdeelvenster van het scherm. Gepersonaliseerde elementen worden vervangen door de gegevens van het profiel dat in het linkerdeelvenster is geselecteerd. [Meer informatie over de voorvertoning van inhoud voor levering](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png)

1. Als u e-mailberichten wilt verzenden, klikt u op de knop **[!UICONTROL Test]** knop.

1. Klik op de knop **[!UICONTROL Upload proof profiles]** en selecteert u het .txt- of .csv-bestand met de proefdrukontvangers.

   >[!CAUTION]
   >
   >Zorg ervoor dat de bestandsindeling overeenkomt met de indeling die wordt gebruikt voor het uploaden van uw publiek. Bij indelingsfouten wordt een waarschuwing weergegeven.

1. Als de proefontvangers zijn toegevoegd en u klaar bent om de proefdrukken te verzenden, klikt u op de knop **[!UICONTROL Send test email]** en bevestig de verzendende.

   ![](assets/file-upload-test.png)

1. U kunt de verzending van de teste-mail controleren met de **[!UICONTROL View test email log]** op elk gewenst moment. [Meer informatie over e-mailcontrole tijdens tests](../preview-test/test-deliveries.md#access-test-deliveries)
