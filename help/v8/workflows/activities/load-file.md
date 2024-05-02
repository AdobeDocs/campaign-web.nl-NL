---
audience: end-user
title: De werkstroomactiviteit voor het laden van bestanden gebruiken
description: Leer hoe u de workflowactiviteit Bestand laden gebruikt
exl-id: 230177e2-1926-451a-8a66-0db962ada514
source-git-commit: ba187eaebf299e5d2ee303c4e15180d35a9e6180
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 2%

---

# Bestand laden {#load-file}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile"
>title="Bestandsactiviteit laden"
>abstract="De **Bestand laden** activiteit is **Gegevensbeheer** activiteit. Gebruik deze activiteit om met gegevens te werken die in een extern dossier worden opgeslagen. Profielen en gegevens worden niet toegevoegd aan de database, maar alle velden in het invoerbestand zijn beschikbaar voor personalisatie, voor het bijwerken van profielen of een andere tabel. "

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition"
>title="Uitgaande overgang van beheer afwijzen"
>abstract="Uitgaande overgang van beheer afwijzen"

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_outboundtransition_reject"
>title="Uitgaande overgang van beheer afwijzen voor afwijzing"
>abstract="Uitgaande overgang van beheer afwijzen voor afwijzing"


De **Bestand laden** activiteit is **Gegevensbeheer** activiteit. Gebruik deze activiteit om met profielen en gegevens te werken die in een extern dossier worden opgeslagen. Profielen en gegevens worden niet toegevoegd aan de database, maar alle velden in het invoerbestand zijn beschikbaar voor [personalisatie](../../personalization/gs-personalization.md)of om profielen of een andere tabel bij te werken.

>[!NOTE]
>Ondersteunde bestandsindelingen zijn: tekst (TXT) en door komma&#39;s gescheiden waarden (CSV). U kunt bestanden laden met een maximale grootte van 50 MB.

Deze activiteit kan worden gebruikt met een [Verzoening](reconciliation.md) activiteit om niet-geïdentificeerde gegevens aan bestaande middelen te koppelen. Bijvoorbeeld de **Bestand laden** activiteit kan vóór een **Verzoening** activiteit als u niet-standaardgegevens in het gegevensbestand invoert.

## De activiteit van het bestand laden configureren {#load-configuration}

De **Bestand laden** de activiteitenconfiguratie omvat twee stappen. Eerst moet u de verwachte bestandsstructuur definiëren door een voorbeeldbestand te uploaden. Als dit is gebeurd, kunt u de oorsprong opgeven van het bestand waarvan de gegevens worden geïmporteerd. Voer de onderstaande stappen uit om de activiteit te configureren.

![](../assets/workflow-load-file.png)

### Voorbeeldbestand configureren {#sample}

>[!AVAILABILITY]
>
>Dit vermogen is in Beperkte Beschikbaarheid (LA). Het is beperkt tot klanten die op een server van de Campagne v8.7 lopen en kan niet op een andere milieu worden opgesteld.

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_samplefile"
>title="Voorbeeldbestand"
>abstract="Selecteer de verwachte bestandsstructuur door een voorbeeldbestand te uploaden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_formatting"
>title="Opmaak voor het laden van bestandsactiviteit"
>abstract="In de **Opmaak** in, geeft u op hoe het bestand wordt opgemaakt om ervoor te zorgen dat de gegevens correct worden geïmporteerd."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_valueremapping"
>title="Waarde opnieuw toewijzen voor activiteit van bestand laden"
>abstract="Gebruik deze optie om specifieke waarden van de geladen bestanden toe te wijzen aan nieuwe waarden. Als de kolom bijvoorbeeld waarden &quot;Waar&quot;/&quot;Onwaar&quot; bevat, kunt u een toewijzing toevoegen om die waarden automatisch te vervangen door &quot;0&quot;/&quot;1&quot;-tekens."

Voer de volgende stappen uit om het voorbeeldbestand te configureren dat wordt gebruikt om de verwachte bestandsstructuur te definiëren:

1. Voeg een **Bestand laden** in uw workflow.

1. Selecteer het voorbeeldbestand dat u wilt gebruiken om de verwachte bestandsstructuur te definiëren. Om dit te doen, klik **Bestand selecteren** in de **[!UICONTROL Sample file]** en selecteert u het lokale bestand dat u wilt gebruiken.

   >[!NOTE]
   >
   >De data van het voorbeeldbestand worden gebruikt voor het configureren van de activiteit, maar worden niet geïmporteerd. We raden u aan een voorbeeldbestand te gebruiken dat weinig gegevens bevat. De bestandsindeling moet hiermee worden uitgelijnd [voorbeeldbestand](../../audience/file-audience.md#sample-file).

1. Er wordt een voorbeeld van het voorbeeldbestand weergegeven met maximaal 30 regels.

1. In de **[!UICONTROL File type]** vervolgkeuzelijst, geeft u op of het bestand kolommen met begrenzingen of kolommen met vaste breedte gebruikt.

   ![](../assets/workflow-load-file-sample.png)

1. Voor bestandstypen met gescheiden kolommen gebruikt u de opdracht **Kolommen** sectie om de eigenschappen van elke kolom te vormen.

   +++Beschikbare opties voor bestandskolommen

   * **[!UICONTROL Label]**: Label dat moet worden weergegeven voor de kolom.
   * **[!UICONTROL Data type]**: Type gegevens in de kolom.
   * **[!UICONTROL Width]** (gegevenstype tekenreeks): maximum aantal tekens dat in de kolom moet worden weergegeven.
   * **[!UICONTROL Data Transformation]** (gegevenstype tekenreeks): pas transformatie toe op de waarden in de kolom.
   * **[!UICONTROL White space management]** (gegevenstype tekenreeks): geef op hoe de spaties in de kolom moeten worden beheerd.
   * **[!UICONTROL Separators]** (gegevenstypen datum, tijd, geheel getal en getal)*: geef de tekens op die u als scheidingsteken wilt gebruiken.
   * **[!UICONTROL Allow NULLs]**: Geef op hoe u lege waarden in de kolom wilt beheren. De optie Adobe Campaign default geeft een fout weer als er een lege waarde aanwezig is.
   * **[!UICONTROL Error processing]** (gegevenstype tekenreeks): geef het gedrag op bij fouten in een van de regels.
   * **[!UICONTROL Value remapping]**: Met deze optie kunt u specifieke waarden toewijzen aan nieuwe waarden. Als de kolom bijvoorbeeld waarden &quot;Waar&quot;/&quot;Onwaar&quot; bevat, kunt u een toewijzing toevoegen om die waarden automatisch te vervangen door &quot;0&quot;/&quot;1&quot;-tekens.

+++

1. In de **Opmaak** in, geeft u op hoe het bestand wordt opgemaakt om ervoor te zorgen dat de gegevens correct worden geïmporteerd.

### Doelbestand definiëren om te uploaden {#target}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetfile"
>title="Doelbestand voor laden van bestandsactiviteit"
>abstract="In de **[!UICONTROL Target file]** , geeft u op hoe u het bestand ophaalt dat u op de server wilt uploaden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_nameofthefile"
>title="Naam van het bestand"
>abstract="Geef de naam op van het veld dat u wilt uploaden op de server. Klik op de knop **[!UICONTROL Open personalization dialog]** gebruiken om de expressie-editor, inclusief gebeurtenisvariabelen, te gebruiken om de bestandsnaam te berekenen."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_targetdb"
>title="Doeldatabase"
>abstract="Als u een **[!UICONTROL Load file]** activiteit die reeds in de cliëntconsole is opstelling, een extra **[!UICONTROL Target database]** is beschikbaar als u de activiteit hebt gevormd om het dossier aan een extern gegevensbestand te uploaden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_command"
>title="Bestand laden, opdracht"
>abstract="Het toestaan van arbitraire bevel voor preprocessing is een veiligheidszorg, maak veiligheidsoptie XtkSecurity_Disable_Preproc onbruikbaar om het gebruik van een vooraf bepaalde lijst van bevelen te dwingen."

>[!CAUTION]
>
>Voordat u het doelbestand laadt, moet u controleren of het bestand voldoet aan de indeling van het voorbeeldbestand. Eventuele verschillen in bestandsindeling, kolomstructuur of aantal kolommen kunnen leiden tot fouten tijdens de uitvoering van de workflow.

1. In de **[!UICONTROL Target file]** , geeft u de actie op die moet worden uitgevoerd wanneer u het bestand ophaalt dat u op de server wilt uploaden.

   * **[!UICONTROL Upload file from local machine]**: Selecteer het bestand dat u wilt uploaden van uw computer.

   * **[!UICONTROL Specified in the transition]**: Upload het bestand dat is opgegeven in de inkomende overgang die volgt uit een eerdere activiteit, zoals **[!UICONTROL Transfer file]**.

   * **[!UICONTROL Pre-process the file]**: Upload het bestand dat u in de vorige overgang hebt opgegeven en pas er een voorbewerkingsopdracht op toe, zoals **[!UICONTROL Decompression]** of **[!UICONTROL Decrypt]**.

   * **[!UICONTROL Calculated]**: Upload het bestand waarvan de naam in het dialoogvenster **[!UICONTROL File name]** veld. Klik op de knop **[!UICONTROL Open personalization dialog]** gebruiken om de expressie-editor, inclusief gebeurtenisvariabelen, te gebruiken om de bestandsnaam te berekenen.

   ![](../assets/workflow-load-file-config.png)

   >[!NOTE]
   >
   >Als u een **[!UICONTROL Load file]** activiteit die reeds in de cliëntconsole is opstelling, een extra **[!UICONTROL Target database]** wordt weergegeven als u de activiteit hebt geconfigureerd om het bestand te uploaden naar een externe database. Hiermee kunt u opgeven of u het bestand wilt uploaden naar de campagneserver of naar de externe database.

### Aanvullende opties {#options}

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_rejectmgt"
>title="Afwijzen van beheer voor het laden van bestandsactiviteiten"
>abstract="In de **Afwijzen** in, geeft u aan hoe de activiteit zich moet gedragen in het geval van fouten. U kunt het maximale aantal toegestane fouten definiëren en de **[!UICONTROL Keep rejects in a file]** een bestand met de fouten die tijdens het importeren zijn opgetreden, op de server downloaden."

>[!CONTEXTUALHELP]
>id="acw_orchestration_loadfile_delete"
>title="Bestand verwijderen na importeren"
>abstract="Schakelen tussen **Bestand verwijderen na importeren** om het oorspronkelijke bestand van de server te verwijderen nadat het bestand is geïmporteerd."


>[!AVAILABILITY]
>
>Deze opties staan in Beperkte Beschikbaarheid (LA). Zij zijn beperkt tot klanten die op een server van de Campagne v8.7 lopen en kunnen niet op een andere milieu worden opgesteld.

1. In de **Afwijzen** in, geeft u aan hoe de activiteit zich moet gedragen in het geval van fouten:

   * In de **[!UICONTROL Dele]** veld, geeft u het maximale aantal fouten op dat is toegestaan bij het verwerken van het te laden bestand. Als de waarde bijvoorbeeld is ingesteld op &quot;20&quot;, mislukt de uitvoering van de workflow als er meer dan 20 fouten optreden bij het laden van het bestand.

   * Als u de fouten die zijn opgetreden bij het laden van het bestand wilt behouden, schakelt u het **[!UICONTROL Keep rejects in a file]** en geeft u de gewenste naam voor het bestand op in het dialoogvenster **[!UICONTROL Rejection File]** veld.

     Na het activeren van deze optie wordt een extra uitvoerovergang met de naam &quot;Complement&quot; toegevoegd na de activiteit. Eventuele fouten die tijdens het importeren optreden, worden opgeslagen in het opgegeven bestand op de server.

1. Als u het geüploade bestand van de server wilt verwijderen nadat de workflow is uitgevoerd, schakelt u het **[!UICONTROL Delete file after import]** -optie.

   ![](../assets/workflow-load-file-options.png)

1. Klikken **Bevestigen** als de instellingen correct zijn.

## Voorbeeld {#load-example}

Een voorbeeld van een extern bestand dat wordt geladen en dat wordt gebruikt voor de **Verzoening** activiteit is beschikbaar in [deze sectie](reconciliation.md#reconciliation-example).
