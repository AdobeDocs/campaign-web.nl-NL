---
audience: end-user
title: De workflowactiviteit voor het uitpakken van bestanden gebruiken
description: Leer hoe u de workflowactiviteit voor het uitpakken van bestanden kunt gebruiken
exl-id: fa50ab5b-2539-4517-9d7b-93315f1e505c
source-git-commit: 5b42671173e7fd7f024eb7eb03a0836eae7ef622
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 1%

---

# Bestand extraheren {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Bestand extraheren"
>abstract="De **Bestand uitpakken** kunt u gegevens uit Adobe Campaign exporteren in de vorm van een extern bestand. De gegevens kunnen vervolgens via een bestandsactiviteit voor gegevensoverdracht worden geëxporteerd naar een serverlocatie zoals SFTP, Cloud-opslag of uw campagneserver."

De **Bestand uitpakken** activiteit is **Gegevensbeheer** activiteit. Met deze activiteit kunt u gegevens uit Adobe Campaign exporteren in de vorm van een extern bestand. De gegevens kunnen vervolgens via een bestandsactiviteit voor gegevensoverdracht worden geëxporteerd naar een serverlocatie zoals SFTP, Cloud-opslag of uw campagneserver.

Om te vormen **Bestand uitpakken** activiteit, voeg een **Bestand uitpakken** Voer vervolgens de onderstaande stappen uit in uw werkstroom.

## Het uit te pakken bestand configureren {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Te extraheren bestand"
>abstract="Selecteer het bestand dat u wilt extraheren."

De **[!UICONTROL File to extract]** kunt u de bestandseigenschappen en de gegevens configureren die moeten worden opgenomen.

![](../assets/extract-file-file.png)

1. In de **[!UICONTROL File name]** voert u de gewenste naam in voor het bestand dat u wilt extraheren.

   U kunt de naam van het bestand aanpassen met behulp van gebeurtenisvariabelen, -voorwaarden en datum-/tijdfuncties. Om dit te doen, klik **[!UICONTROL Open personalization dialog]** pictogram om de uitdrukkingsredacteur te openen. [Leer hoe u met gebeurtenisvariabelen en de expressie-editor werkt](../event-variables.md)

1. Geef de kolommen op die in het geëxtraheerde bestand moeten worden weergegeven. Ga als volgt te werk om dit te doen:

   1. Klik op de knop **[!UICONTROL Add output column]**.
   1. Kies het kenmerk dat u in de kolom wilt weergeven en bevestig het vervolgens. Welke kenmerken beschikbaar zijn, is afhankelijk van de doeldimensie van de workflow.
   1. Nadat de kolom is toegevoegd, kunt u de kolominhoud wijzigen **[!UICONTROL Label]** en de bijbehorende **[!UICONTROL Attribute]**.
   1. Als u een transformatie wilt toepassen op de waarden van de kolom, selecteert u deze in de vervolgkeuzelijst. U kunt bijvoorbeeld alle waarden in de geselecteerde kolom in hoofdletters zetten.

1. Herhaal deze stappen om zoveel kolommen toe te voegen als nodig is in het extractiebestand. Gebruik de pijlen omhoog en omlaag om de positie van een kolom te wijzigen.

1. Als u alle dubbele rijen uit het geëxtraheerde bestand wilt verwijderen, schakelt u het **[!UICONTROL Remove duplicate rows(Listing)]** -optie.

1. Als u het geëxtraheerde bestand wilt sorteren op basis van een kenmerk, schakelt u het **[!UICONTROL Enable Sorting]** Kies vervolgens het kenmerk waarop u het bestand wilt sorteren, samen met de gewenste sorteermethode (oplopend of aflopend). U kunt op om het even welk attribuut van de huidige het richten afmeting sorteren, ongeacht of het aan de kolommen van het dossier of niet is toegevoegd.

## De geëxtraheerde bestandsindeling configureren {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Bestemmingsindeling"
>abstract="Selecteer de verschillende opties om te configureren hoe het geëxtraheerde bestand wordt opgemaakt."

De **[!UICONTROL Destination]** in de indelingssectie kunt u configureren hoe het geëxtraheerde bestand wordt opgemaakt.

1. Kies de optie **[!UICONTROL Output format]** voor het uitgepakte bestand: **Tekst**, **Tekst met vaste waarden met kolommen**, **CSV (Excel)** of **XML**.

1. Klik op de knop **[!UICONTROL Extraction format]** voor toegang tot specifieke opties voor de geselecteerde indeling. Vouw de sectie uit als hieronder voor meer informatie.

+++ Beschikbare opties voor de indeling voor uitnemen

   * **[!UICONTROL Use first line as column header]** (Text / CSV (Excel)): Schakel deze optie in als u de eerste kolom als koptekst wilt gebruiken.
   * **[!UICONTROL Column separator]** (Tekstopmaak): geef het teken op dat u als kolomscheidingsteken wilt gebruiken in het uitvoerbestand.
   * **[!UICONTROL String delimiter]** (Tekstopmaak): geef op hoe tekenreeksen in het uitvoerbestand moeten worden gescheiden.
   * **[!UICONTROL End of line]** (Tekstopmaak): geef op hoe het einde van regels in het uitvoerbestand moet worden afgebakend.
   * **[!UICONTROL Encoding]**: Kies de codering van het uitvoerbestand.
   * **[!UICONTROL Date format and separators]**: Geef op hoe datums moeten worden opgemaakt in het uitvoerbestand.
   * **[!UICONTROL Number format]**: Geef op hoe getallen moeten worden opgemaakt in het uitvoerbestand.
   * **[!UICONTROL Export labels instead of internal values of enumerations]**: Schakel deze optie in als u opsommingswaarden exporteert en u de kolomlabels wilt ophalen. Deze zijn eenvoudiger te begrijpen en geen interne id&#39;s.

+++

   ![](../assets/extract-file-format.png)

## Een nabewerkingsfase toevoegen {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Post-verwerking"
>abstract="Definieer een stap voor nabewerking die u wilt toepassen, zoals comprimeren of coderen."

De **[!UICONTROL Export modification script]** Hiermee kunt u een verwerkingsstadium toepassen dat wordt uitgevoerd tijdens het ophalen van gegevens, zoals comprimeren of coderen. Om dit te doen, klik **[!UICONTROL Edit script]** knop.

De uitdrukkingsredacteur opent, die u toestaat om het bevel in te gaan om op het dossier van toepassing te zijn. Het linkerdeelvenster bevat vooraf gedefinieerde syntaxis waarmee u het script kunt samenstellen. [Leer hoe u met gebeurtenisvariabelen en de expressie-editor werkt](../event-variables.md)

![](../assets/extract-file-script.png)

## Aanvullende opties {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Uitgaande overgang"
>abstract="Schakelen tussen **Een uitgaande overgang genereren** optie om een uitgaande overgang toe te voegen na de huidige activiteit."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Procesfouten"
>abstract="Schakelen tussen **Procesfouten** om een uitgaande overgang toe te voegen die fouten bevat."

Nadat de extractie van het uitvoerbestand is geconfigureerd, zijn aanvullende opties beschikbaar met betrekking tot overgangen en foutbeheer:

* **[!UICONTROL Generate outbound transition]**: Schakel deze optie in of uit om een uitgaande overgang toe te voegen en het label te configureren.
* **[!UICONTROL Do not generate a file if the inbound transition is empty]**: Schakel deze optie in en uit om het uitpakken van het bestand over te slaan als de binnenkomende overgang geen gegevens bevat.
* **[!UICONTROL Process error]**: Schakel deze optie in om een uitgaande overgang toe te voegen als er een fout optreedt tijdens het uitpakken van het bestand.

## Voorbeeld {#example}

In het volgende voorbeeld gebruiken we een **publiek opbouwen** activiteit gevolgd door een **Bestand uitpakken** activiteit om alle doelprofielen in een CSV-bestand te extraheren.

![](../assets/extract-file-example.png)

* De **[!UICONTROL File name]** wordt gevormd om de datum van de extractie te omvatten.

  ![](../assets/extract-file-example-name.png)

* Er worden kolommen toegevoegd om de voor- en achternaam van de profielen, de id&#39;s van de klant en de aanmaakdatums in de database weer te geven.

  ![](../assets/extract-file-example-columns.png)
