---
audience: end-user
title: Workflows maken met Adobe Campaign Web
description: Leer hoe u workflows kunt maken met Adobe Campaign Web
exl-id: c9c41189-0150-49a4-bdb3-317fe543eb2c
source-git-commit: b9f3deb579cf786e0eafa57f42a728b3f7a002d1
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# Uw workflows starten en controleren {#start-monitor}

Nadat u de workflow hebt gemaakt en de taken hebt ontworpen die u op het canvas wilt uitvoeren, kunt u deze starten en controleren hoe deze wordt uitgevoerd.

## De workflow starten {#start}

Als u de workflow wilt starten, navigeert u naar het menu **[!UICONTROL Workflows]** of de bijbehorende campagne en klikt u op de knop **[!UICONTROL Start]** rechtsboven in het canvas.

Wanneer de workflow is gestart, wordt elke activiteit op het canvas opeenvolgend uitgevoerd tot het einde van de workflow is bereikt.

U kunt de voortgang van doelprofielen in real-time bijhouden met behulp van een visuele stroom. Hierdoor kunt u snel de status van elke activiteit en het aantal profielen identificeren dat tussen de activiteiten overgaat.

![&#x200B; Visuele vertegenwoordiging van werkschemauitvoering lopend.](assets/workflow-execution.png){zoomable="yes"}

## Workflowovergangen {#transitions}

In werkstromen, worden de gegevens die van één activiteit aan een andere door overgangen worden vervoerd opgeslagen in een tijdelijke het werklijst. Deze gegevens kunnen voor elke overgang worden weergegeven. Als u de gegevens wilt weergeven, selecteert u een overgang om de eigenschappen ervan in de rechterkant van het scherm te openen.

* Klik op **[!UICONTROL Preview schema]** om het schema van de werktabel weer te geven.
* Klik op **[!UICONTROL Preview results]** om de gegevens weer te geven die in de geselecteerde overgang worden verzonden.

![&#x200B; Voorbeeld van overgangseigenschappen en gegevensvoorproef.](assets/transition.png){zoomable="yes"}

## Activiteitenuitvoering controleren {#activities}

De visuele indicatoren in de hoger-juiste hoek van elke activiteitendoos staan u toe om hun uitvoeringsstatus te controleren:

| Visuele indicator | Beschrijving |
|------------------|-------------|
| ![](assets/activity-status-pending.png){zoomable="yes"}{width="70%"} | De activiteit wordt momenteel uitgevoerd. |
| ![](assets/activity-status-orange.png){zoomable="yes"}{width="70%"} | De activiteit vereist uw aandacht. Dit kan inhouden dat de verzending van een levering wordt bevestigd of dat de nodige actie wordt ondernomen. |
| ![](assets/activity-status-red.png){zoomable="yes"}{width="70%"} | Er is een fout opgetreden in de activiteit. Open de logbestanden van de workflow voor meer informatie om het probleem op te lossen. |
| ![](assets/activity-status-green.png){zoomable="yes"}{width="70%"} | De activiteit is uitgevoerd. |

## Logboeken en taken controleren {#logs-tasks}

Het controleren van workflowlogboeken en taken is een belangrijke stap om uw workflows te analyseren en ervoor te zorgen dat deze correct worden uitgevoerd. Logbestanden en taken zijn toegankelijk via het pictogram **[!UICONTROL Logs]** , dat beschikbaar is op de werkbalk Handeling en in het deelvenster Eigenschappen van elke activiteit.

Het menu **[!UICONTROL Logs and tasks]** bevat een geschiedenis van de uitvoering van de workflow, waarin alle handelingen van de gebruiker zijn opgenomen en fouten zijn aangetroffen. Deze geschiedenis wordt bewaard voor de duur die in de werkschema [&#x200B; wordt gespecificeerd uitvoeringsopties &#x200B;](workflow-settings.md). Tijdens deze periode worden alle berichten opgeslagen, zelfs nadat de workflow opnieuw is gestart. Als u geen berichten uit een vorige uitvoering wilt opslaan, klikt u op de knop **[!UICONTROL Purge history]** .

![&#x200B; Voorbeeld van werkschemalogboeken en takeninterface.](assets/workflow-logs.png){zoomable="yes"}

Er zijn twee soorten informatie beschikbaar:

* Het tabblad **[!UICONTROL Log]** bevat de uitvoeringsgeschiedenis van alle workflowactiviteiten. De uitgevoerde bewerkingen en uitvoeringsfouten worden chronologisch geïndexeerd.
* Het tabblad **[!UICONTROL Tasks]** bevat details over de uitvoeringsvolgorde van de activiteiten.

Op beide tabbladen kunt u de weergegeven kolommen en hun volgorde kiezen, filters toepassen en het zoekveld gebruiken om snel de gewenste informatie te zoeken.

## Opdrachten voor workflowuitvoering {#execution-commands}

De actiebalk in de rechterbovenhoek bevat opdrachten waarmee u de uitvoering van de workflow kunt beheren. U kunt:

* **[!UICONTROL Start]** / **[!UICONTROL Resume]** de uitvoering van de workflow. Als de werkstroom is gepauzeerd, wordt deze hervat. Anders wordt het programma gestart en worden de initiële activiteiten geactiveerd.
* **[!UICONTROL Pause]** de uitvoering van de workflow. De workflow neemt vervolgens de status Gepauzeerd aan. Er worden geen nieuwe activiteiten geactiveerd totdat het programma wordt hervat, maar lopende activiteiten worden niet opgeschort.
* **[!UICONTROL Stop]** een workflow die wordt uitgevoerd. De workflow neemt vervolgens de status Voltooid aan. Bewerkingen die worden uitgevoerd worden indien mogelijk onderbroken. U kunt de werkstroom niet hervatten vanaf het punt waar deze is gestopt.