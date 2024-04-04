---
audience: end-user
title: Een e-mailpubliek laden vanuit een bestand
description: Leer hoe u profielen uit een extern bestand kunt laden om uw e-mailpubliek te maken
exl-id: e6e0dd01-5573-4261-aace-fd173827c383
source-git-commit: b166d06215e06d6426ab9ce9a757fcc041810df9
workflow-type: tm+mt
source-wordcount: '640'
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

Met de Adobe Campaign Web User Interface kunt u profielen die zijn opgeslagen in een extern bestand als doel instellen. Nadat de profielen zijn geladen, kunnen alle velden in het invoerbestand worden gebruikt om de levering aan te passen [Leer hoe u uw inhoud kunt aanpassen](../personalization/personalize.md).

Profielen uit het invoerbestand worden niet toegevoegd aan de database. Ze worden geladen en zijn alleen beschikbaar voor deze specifieke zelfstandige e-maillevering.

>[!NOTE]
>
>Op deze pagina wordt beschreven hoe u externe profielen uit een bestand kunt laden wanneer u een zelfstandige e-maillevering maakt. Als u gegevens uit een bestand wilt laden in de context van een workflow, raadpleegt u [deze pagina](../workflows/activities/load-file.md).

## Lees hier meer {#must-read}

* Deze mogelijkheid is beschikbaar voor **e-mailleveringen** alleen.
* Ondersteunde bestandsindelingen zijn: tekst (TXT) en door komma&#39;s gescheiden waarden (CSV).
* U kunt niet [controlegroepen](control-group.md) bij het laden van de doelpopulatie uit een extern bestand.

## Het invoerbestand selecteren en configureren {#upload}

Voer de volgende stappen uit om profielen te kiezen uit een bestand in uw e-mails:

1. Open een bestaande e-maillevering, of [een nieuwe e-maillevering maken](../email/create-email.md).
1. In de **Publiek** klikt u op de **Doelgroep selecteren** en kies vervolgens **Selecteren uit bestand**.

   ![](assets/select-from-file.png){zoomable=&quot;yes&quot;}

1. Selecteer het lokale bestand dat u wilt laden. De bestandsindeling moet worden uitgelijnd met de [voorbeeldbestand](#sample-file).
1. In het centrale gedeelte van het scherm kunt u bekijken en controleren hoe gegevens worden toegewezen.

   ![](assets/select-from-file-map.png)

1. Geef de kolom op die het e-mailadres bevat van het dialoogvenster **Adresveld** vervolgkeuzelijst. U kunt de kolom van de lijst van gewezen personen ook selecteren als u dergelijke informatie in het inputdossier hebt.
1. Pas de kolominstellingen aan en hoe u de gegevens opmaakt op basis van de beschikbare opties.
1. Klikken **Bevestigen** als de instellingen correct zijn.

Wanneer u de inhoud van het bericht maakt, kunt u de weergave aanpassen door velden uit het invoerbestand te gebruiken. [Leer hoe u inhoud kunt aanpassen](../personalization/personalize.md)

![](assets/select-external-perso.png){zoomable=&quot;yes&quot;}

## Voorbeeldbestand {#sample-file}

>[!CONTEXTUALHELP]
>id="acw_audience_fromfile_samplefile"
>title="Een publiek uit een bestand laden"
>abstract="Ondersteunde bestandsindelingen zijn TXT en CSV. Eerste regel gebruiken als kolomkop. Lijn de bestandsindeling uit met het voorbeeldbestand in de onderstaande koppeling."

Wanneer u een extern bestand laadt naar doelprofielen in uw leveringen, moet u ervoor zorgen dat het invoerbestand overeenkomt met de onderstaande aanbevelingen:

* Ondersteunde indelingen zijn TXT en CSV.
* De eerste regel in het bestand is de kolomkop.
* Lijn de bestandsindeling uit met het onderstaande voorbeeldbestand:

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

Met Campagne Web kunt u proefdrukken weergeven en verzenden wanneer u een publiek gebruikt dat vanuit een bestand is geüpload. Ga als volgt te werk om dit te doen:

1. Klik op de knop **[!UICONTROL Simulate content button]** vanuit het bewerkingsscherm voor de inhoud van de levering en klik op de knop **[!UICONTROL Add test profile(s)]** knop.

1. De profielen in de geüploade bestandsweergave. Selecteer de profielen die u wilt gebruiken voor de voorvertoning van uw inhoud en klik op **[!UICONTROL Select]**.

1. Een voorvertoning van de leveringsinhoud wordt weergegeven in het rechterdeelvenster van het scherm. Gepersonaliseerde elementen worden vervangen door de gegevens van het profiel dat in het linkerdeelvenster is geselecteerd. [Meer informatie over de voorvertoning van inhoud voor levering](../preview-test/preview-content.md)

   ![](assets/file-upload-preview.png){zoomable=&quot;yes&quot;}

1. Als u proefdrukken wilt verzenden, klikt u op de knop **[!UICONTROL Send proof]** knop.

1. Klik op de knop **[!UICONTROL Upload proof profiles]** en selecteert u het .txt- of .csv-bestand met de proefdrukontvangers.

   >[!CAUTION]
   >
   >Zorg ervoor dat de bestandsindeling overeenkomt met de indeling die wordt gebruikt voor het uploaden van uw publiek. Bij indelingsfouten wordt een waarschuwing weergegeven.

1. Als de proefdrukprofielen zijn toegevoegd en u klaar bent om de proefdrukken te verzenden, klikt u op de knop **[!UICONTROL Send proof]** en bevestig de verzendende.

   ![](assets/file-upload-test.png){zoomable=&quot;yes&quot;}

1. U kunt de verzending van de proef controleren met de **[!UICONTROL View proofs]** op elk gewenst moment. [Meer informatie over proefdrukcontrole](../preview-test/test-deliveries.md#access-test-deliveries)
