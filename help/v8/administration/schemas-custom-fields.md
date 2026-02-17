---
title: Aangepaste velden bewerken
description: Leer hoe u aangepaste velden en hun zichtbaarheid in de interface configureert.
source-git-commit: 28f7bcf5f65671136be25c79b414f149532b749f
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Aangepaste velden bewerken {#fields}

Aangepaste velden zijn aanvullende kenmerken die via de Adobe Campaign-console aan out-of-the-box-schema&#39;s worden toegevoegd. Zij staan u toe om schema&#39;s aan te passen door nieuwe attributen aan de behoeften van uw organisatie te omvatten.

Aangepaste velden kunnen op verschillende schermen worden weergegeven, zoals profieldetails in de interface. U kunt bepalen welke velden zichtbaar zijn en hoe ze in de interface worden weergegeven.

Voor meer informatie over het scherm van de het schermdefinitie en hoe te om tot het toegang te hebben, verwijs naar [ toegang tot de sectie van de het schermdefinitie ](schemas-browse-access.md#screen-def).

Aangepaste velden toevoegen aan de lijst:

1. Blader naar het menu **[!UICONTROL Schemas]** en zoek bewerkbare schema&#39;s met de filters.

1. Selecteer de schemanaam in de lijst om het te openen en de **[!UICONTROL Screen edition]** knoop in de mening van schemadetails te klikken om tot de het schermdefinitie toegang te hebben.

1. Klik op het pictogram van de ovaal boven de **[!UICONTROL List of custom fields]** -tabel en kies **[!UICONTROL Select attributes]** om een of meerdere aangepaste velden te selecteren die in de interface moeten worden weergegeven.
   ![ het scherm van de gebieden van de Douane die editable attributen tonen ](assets/schemas-custom5.png)
1. Selecteer de aangepaste velden die u wilt toevoegen en bevestigen.

   ![ het scherm van de gebieden van de Douane die editable attributen tonen ](assets/schemas-custom2.png)

   >[!NOTE]
   >
   > U kunt ook **[!UICONTROL Fill automatically the list of custom fields]** selecteren om alle aangepaste velden die voor het schema zijn gedefinieerd, toe te voegen aan de interface.

Nadat u aangepaste velden hebt toegevoegd, kunt u deze voorvertonen, opnieuw rangschikken, de velden verplicht maken, de instellingen van de velden bewerken of in subsecties ordenen.

## Veldinstellingen configureren {#field-settings}

Als u specifieke instellingen voor elk aangepast veld wilt configureren, klikt u op het pictogram met de ellips op een veldrij in de lijst en selecteert u **[!UICONTROL Edit]** .

![ de instellingendialoog van Attributen ](assets/schemas-attribute-settings.png)

Beschikbare instellingen zijn:

* **[!UICONTROL Attribute]**: De naam van het aangepaste veld (alleen-lezen).
* **[!UICONTROL Label (custom)]**: Het label dat in de interface moet worden weergegeven. Als er geen label is opgegeven, wordt het label dat in het schema is gedefinieerd, weergegeven.
* **[!UICONTROL Visible if]**: Definieer een voorwaarde met een xtk-expressie die bepaalt wanneer het veld wordt weergegeven. Verberg dit veld bijvoorbeeld als een ander veld leeg is.
* **[!UICONTROL Mandatory]**: maak het veld verplicht in de interface.
* **[!UICONTROL Read-only]**: maak het veld alleen-lezen in de interface. Gebruikers kunnen de waarde van het veld niet bewerken.
* **[!UICONTROL Filter settings]** (voor koppelingstype velden): gebruik de querymodelfunctie om regels op te geven voor de weergave van een aangepast veld van het type koppeling. Beperk bijvoorbeeld lijstwaarden op basis van invoer van een ander veld.

  +++Voorbeeld weergeven

  U kunt ook met de syntaxis `$(<field-name>)` verwijzen naar de waarde die in uw eigen omstandigheden in andere velden is ingevoerd. Op deze manier kunt u verwijzen naar de huidige waarde van een veld zoals dat in het formulier is ingevoerd, zelfs als het nog niet in de database is opgeslagen.

  In het onderstaande voorbeeld controleert de voorwaarde of de waarde van het veld @ref overeenkomt met de waarde die is ingevoerd in het veld @refCom. Als u daarentegen `@refCom` in plaats van `$(@refCom)` gebruikt, verwijst u naar de waarde van het veld @ref zoals dit in de database bestaat.

  ![ Schermafbeelding die een voorbeeld van filtermontages voor douanegebieden toont ](assets/custom-fields-ref.png)

  +++

* **[!UICONTROL Span two columns]**: Standaard worden aangepaste velden in de interface weergegeven in twee kolommen. Schakel deze optie in om het aangepaste veld over de volledige breedte van het scherm weer te geven in plaats van over twee kolommen.

## Aangepaste velden voorvertonen {#preview}

Klik op **[!UICONTROL Preview]** om de aangepaste velden in een voorbeeldscherm weer te geven. Zo kunt u zien hoe de velden in de interface worden weergegeven, inclusief welke velden als verplicht zijn gemarkeerd.

![ Voorproef douanegebieden ](assets/schemas-custom4.png)

## Velden indelen in subsecties {#separator}

Voor betere leesbaarheid kunt u scheidingstekens toevoegen aan aangepaste velden in de interface. Voer hiertoe de volgende stappen uit:

1. Klik op het pictogram van de ovaal boven de tabel **[!UICONTROL List of custom fields]** en kies **[!UICONTROL Add separator]** .

1. Er wordt een nieuwe regel met het scheidingsteken toegevoegd aan de lijst. Klik op het ovaalpictogram op de scheidingsrij en kies **[!UICONTROL Edit]** .

1. Voer een **[!UICONTROL Label]** in voor het scheidingsteken en (optioneel) stel een **[!UICONTROL Visible if]** -voorwaarde in om te bepalen wanneer het scheidingsteken wordt weergegeven.

   ![ de eigenschappendialoog van de Scheiding ](assets/schemas-custom3.png)

1. Gebruik de pijlen omhoog en omlaag om het scheidingsteken naar de gewenste locatie te verplaatsen. Velden die onder het scheidingsteken worden weergegeven, worden erin gegroepeerd.

   In dit voorbeeld worden de velden &quot;Geïnteresseerde verzamelingen&quot; en &quot;Merk&quot; gegroepeerd in een subsectie &quot;Verzameling&quot;.

   | Configuratie van aangepaste velden | Renderen in de interface |
   |  ---  |  ---  |
   | ![ Schermschot die de configuratie van een separator ](assets/custom-fields-separator.png){zoomable="yes"} tonen | ![ Schermschot die het teruggeven van een onderafdeling in de interface tonen ](assets/custom-fields-section.png){zoomable="yes"} |
