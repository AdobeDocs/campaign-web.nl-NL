---
audience: end-user
title: De workflowactiviteit voor het uitpakken van bestanden gebruiken
description: Leer hoe u de workflowactiviteit voor het uitpakken van bestanden kunt gebruiken
exl-id: fa50ab5b-2539-4517-9d7b-93315f1e505c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 1%

---

# Bestand extraheren {#extract-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile"
>title="Bestand extraheren"
>abstract="De **het dossier van het Extraheren** activiteit staat u toe om gegevens van Adobe Campaign in de vorm van een extern dossier uit te voeren. De gegevens kunnen vervolgens naar een serverlocatie worden geëxporteerd, zoals SFTP, Cloud-opslag of uw campagneserver met behulp van bestandsactiviteit voor gegevensoverdracht."

De **activiteit van het 0&rbrace; dossier van de Extraheren &lbrace;is het beheer van a** Gegevens **activiteit.** Met deze activiteit kunt u gegevens uit Adobe Campaign exporteren in de vorm van een extern bestand. De gegevens kunnen vervolgens naar een serverlocatie worden geëxporteerd, zoals SFTP, Cloud-opslag of uw campagneserver met behulp van bestandsactiviteit voor gegevensoverdracht.

Om het **dossier** activiteit van het Extraheren te vormen, voeg een **dossier** activiteit van het Extraheren in uw werkschema toe, dan volg de hieronder stappen.

## Het uit te pakken bestand configureren {#extract-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_file"
>title="Te extraheren bestand"
>abstract="Selecteer het bestand dat u wilt extraheren."

In de sectie **[!UICONTROL File to extract]** kunt u de bestandseigenschappen en de gegevens configureren die moeten worden opgenomen.

![&#x200B; Screenshot die de configuratieopties voor het te halen dossier toont.](../assets/extract-file-file.png)

1. Voer in het veld **[!UICONTROL File name]** de gewenste naam in voor het bestand dat u wilt extraheren.

   U kunt de naam van het bestand aanpassen met behulp van gebeurtenisvariabelen, -voorwaarden en datum-/tijdfuncties. Klik hiertoe op het pictogram **[!UICONTROL Open personalization dialog]** om de expressie-editor te openen. [&#x200B; Leer hoe te met gebeurtenisvariabelen en de uitdrukkingsredacteur &#x200B;](../event-variables.md) te werken.

1. Geef de kolommen op die in het geëxtraheerde bestand moeten worden weergegeven. Ga als volgt te werk om dit te doen:

   1. Klik op **[!UICONTROL Add output column]** .
   1. Kies het kenmerk dat u in de kolom wilt weergeven en bevestig het vervolgens. Welke kenmerken beschikbaar zijn, is afhankelijk van de doeldimensie van de workflow. [&#x200B; Leer hoe te om attributen te selecteren en hen toe te voegen aan favorieten &#x200B;](../../get-started/attributes.md).
   1. Nadat de kolom is toegevoegd, kunt u de **[!UICONTROL Label]** ervan wijzigen en de bijbehorende **[!UICONTROL Attribute]** wijzigen.
   1. Als u een transformatie wilt toepassen op de waarden van de kolom, selecteert u deze in de vervolgkeuzelijst. U kunt bijvoorbeeld alle waarden in de geselecteerde kolom in hoofdletters zetten.

1. Herhaal deze stappen om zoveel kolommen toe te voegen als nodig is in het extractiebestand. Gebruik de pijlen omhoog en omlaag om de positie van een kolom te wijzigen.

1. Schakel de optie **[!UICONTROL Remove duplicate rows (Listing)]** in als u alle dubbele rijen uit het geëxtraheerde bestand wilt verwijderen.

1. Als u het geëxtraheerde bestand wilt sorteren op basis van een kenmerk, schakelt u de optie **[!UICONTROL Enable Sorting]** in en kiest u het kenmerk waarop u het bestand wilt sorteren, samen met de gewenste sorteermethode (oplopend of aflopend). U kunt op om het even welk attribuut van de huidige het richten afmeting sorteren, ongeacht of het aan de kolommen van het dossier of niet is toegevoegd.

## De geëxtraheerde bestandsindeling configureren {#file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_destinationformat"
>title="Bestemmingsindeling"
>abstract="Selecteer de verschillende opties om te configureren hoe het geëxtraheerde bestand wordt opgemaakt."

Met de indelingssectie **[!UICONTROL Destination]** kunt u configureren hoe het geëxtraheerde bestand wordt opgemaakt.

1. Kies **[!UICONTROL Output format]** voor het gehaalde dossier: **Tekst**, **Tekst gebruikend kolommen met vaste breedte**, **CSV (Excel)**, of **XML**.

1. Klik op de knop **[!UICONTROL Extraction format]** voor toegang tot specifieke opties voor de geselecteerde indeling. Vouw de onderstaande sectie uit voor meer informatie.

+++ Beschikbare opties voor de indeling voor uitnemen

   * **[!UICONTROL Use first line as column header]** (Tekst / CSV (Excel) formaat): knevel deze optie aan om de eerste kolom als kopbal te gebruiken.
   * **[!UICONTROL Column separator]** (Tekstopmaak): geef het teken op dat u als kolomscheidingsteken wilt gebruiken in het uitvoerbestand.
   * **[!UICONTROL String delimiter]** (Tekstopmaak): geef op hoe tekenreeksen in het uitvoerbestand moeten worden gescheiden.
   * **[!UICONTROL End of line]** (Tekstopmaak): geef op hoe het einde van regels in het uitvoerbestand moet worden afgebakend.
   * **[!UICONTROL Encoding]** - Kies de codering van het uitvoerbestand.
   * **[!UICONTROL Date format and separators]**: geef op hoe datums moeten worden opgemaakt in het uitvoerbestand.
   * **[!UICONTROL Number format]**: geef op hoe getallen moeten worden opgemaakt in het uitvoerbestand.
   * **[!UICONTROL Export labels instead of internal values of enumerations]**: Schakel deze optie in als u opsommingswaarden exporteert en de kolomlabels wilt ophalen. Deze zijn eenvoudiger te begrijpen en geen interne id&#39;s.

+++

   ![&#x200B; Screenshot die de configuratieopties voor het te halen dossier toont.](../assets/extract-file-format.png)

## Een nabewerkingsfase toevoegen {#script}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_postprocessing"
>title="Nabewerking"
>abstract="Definieer een stap voor nabewerking die u wilt toepassen, zoals zipping of encryptie."

Met **[!UICONTROL Export modification script]** kunt u een verwerkingsstadium toepassen dat wordt uitgevoerd tijdens het ophalen van gegevens, zoals comprimeren of coderen. Klik hiertoe op de knop **[!UICONTROL Edit script]** .

De uitdrukkingsredacteur opent, die u toestaat om het bevel in te gaan om op het dossier van toepassing te zijn. Het linkerdeelvenster bevat vooraf gedefinieerde syntaxis waarmee u het script kunt samenstellen. [&#x200B; Leer hoe te met gebeurtenisvariabelen en de uitdrukkingsredacteur &#x200B;](../event-variables.md) te werken.

![&#x200B; Screenshot die de manuscripteditor voor post-verwerking toont.](../assets/extract-file-script.png)

## Aanvullende opties {#additiona-options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_outbound"
>title="Uitgaande overgang"
>abstract="Wisselen **produceert een uitgaande overgang** optie om een uitgaande overgang na de huidige activiteit toe te voegen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_extractfile_error"
>title="Procesfouten"
>abstract="Wissel de **optie van de Fouten van het Proces** om een uitgaande overgang toe te voegen die fouten bevat."

Nadat de extractie van het uitvoerbestand is geconfigureerd, zijn aanvullende opties beschikbaar met betrekking tot overgangen en foutbeheer:

* **[!UICONTROL Generate outbound transition]**: Schakel deze optie in om een uitgaande overgang toe te voegen en het label te configureren.
* **[!UICONTROL Do not generate a file if the inbound transition is empty]**: Schakel deze optie in om het uitpakken van het bestand over te slaan als de binnenkomende overgang geen gegevens bevat.
* **[!UICONTROL Process error]**: Schakel deze optie in om een uitgaande overgang toe te voegen als er een fout optreedt tijdens het uitpakken van het bestand.

## Voorbeeld {#example}

In het volgende voorbeeld, bouwt a **publiek** activiteit wordt gevolgd door een **dossier** activiteit van het Extraheren om alle gerichte profielen in een Csv- dossier te halen.

![&#x200B; Schermafbeelding die een voorbeeldwerkschema met een het publieksactiviteit toont van de Bouwstijl die door een het dossieractiviteit van de Uittreksel wordt gevolgd.](../assets/extract-file-example.png)

* Het veld **[!UICONTROL File name]** is geconfigureerd om de datum van de extractie op te nemen.

  ![&#x200B; Scherenshot die de configuratie van het dossier toont - noem met de inbegrepen datum.](../assets/extract-file-example-name.png)

* Er worden kolommen toegevoegd om de voor- en achternaam van de profielen, de id&#39;s van de klant en de aanmaakdatums in de database weer te geven.

  ![&#x200B; Screenshot die de configuratie van kolommen in het gehaalde dossier tonen.](../assets/extract-file-example-columns.png)