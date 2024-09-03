---
product: campaign
title: Toegang tot leveringen
description: Leer hoe u toegang krijgt tot uw producten en deze beheert in Campagne Web
feature: Email, Push, SMS, Cross Channel Orchestration
role: User
level: Beginner
exl-id: 3afff35c-c15f-46f8-b791-9bad5e38ea44
source-git-commit: ecff4e56bd346aadf381a1bf2077204804938f62
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Toegang tot leveringen {#work-with-deliveries}

>[!CONTEXTUALHELP]
>id="acw_deliveries_list"
>title="Leveringen"
>abstract="Een levering is een communicatie die naar een publiek op een specifiek kanaal wordt verzonden: e-mail, SMS, of Duw. In dit scherm kunt u bestaande leveringen bewerken, dupliceren en verwijderen. U kunt ook rapporten weergeven voor voltooide leveringen. Klik **creeer levering** knoop om een nieuwe levering toe te voegen."

## Toegang tot leveringen {#access}

>[!CONTEXTUALHELP]
>id="acw_deliveries_additional_target"
>title="Aanvullend doel"
>abstract="Deze regels kunnen slechts in de cliëntconsole worden veranderd."

Leveringen zijn toegankelijk via het menu **[!UICONTROL Deliveries]** aan de linkerkant. Alle die leveringen of van de cliëntconsole of de vertoning van het Gebruikersinterface van het Web in deze lijst worden gecreeerd. Vanuit dit scherm kunt u alle bestaande leveringen controleren, deze dupliceren of verwijderen of nieuwe leveringen maken.

![](assets/deliveries-list.png)

Als u een levering wilt openen, klikt u in de lijst op de naam van de levering. De levering opent, die u toestaat om diverse acties uit te voeren zoals het uitgeven van zijn parameters, het controleren van zijn uitvoering of het controleren van zijn prestaties gebruikend specifieke rapporten.

![](assets/delivery-details.png)

>[!NOTE]
>
>Als u een levering opent die in de cliëntconsole wordt gecreeerd, kan de **[!UICONTROL Additional target]** sectie voor het publiek tonen. Dit betekent dat er meerdere doelen zijn geconfigureerd voor deze levering. Deze parameters kunnen alleen in de console worden gewijzigd.
>
>![](assets/target-warning-audience.png){zoomable="yes"}

## Een levering dupliceren {#delivery-duplicate}

U kunt een kopie van een bestaande levering maken, vanuit de leveringslijst of vanaf het bezorgdashboard.

Voer de volgende stappen uit om een levering te dupliceren uit de lijst met leveringen:

1. Klik op de drie puntenknop rechts naast de naam van de levering die u wilt dupliceren.
1. Selecteer **[!UICONTROL Duplicate]** .
1. Herhaling bevestigen: het nieuwe bezorgdashboard wordt in het centrale scherm geopend.

Voer de volgende stappen uit om een levering te dupliceren vanaf het dashboard:

1. Open de levering en klik op de knop **[!UICONTROL ...More]** boven in het scherm.
1. Selecteer **[!UICONTROL Duplicate]**.
1. Herhaling bevestigen: de nieuwe levering vervangt de huidige levering in het centrale scherm.

## Een levering verwijderen {#delivery-delete}

De leveringen worden uit de leveringslijst geschrapt - hetzij van de hoofdlevering in de linkerspoorstaaf, hetzij van de leveringslijst van een campagne.

Voer de volgende stappen uit om een levering te verwijderen uit de lijst met leveringen:

1. Klik op de drie puntenknop rechts naast de naam van de levering die u wilt dupliceren.
1. Selecteer **[!UICONTROL Delete]** .
1. Verwijderen bevestigen.

![ Schrap een levering van de leveringslijst ](assets/delete-delivery-from-list.png)

Alle leveringen zijn beschikbaar in deze lijsten, maar leveringen die in een workflow zijn gemaakt, kunnen daar niet van worden verwijderd. Als u een levering wilt verwijderen die in de context van een workflow is gemaakt, moet u de leveringsactiviteit uit de workflow verwijderen.

Ga als volgt te werk om een levering uit een workflow te verwijderen:

1. Selecteer de leveringsactiviteit.
1. Klik op het pictogram **[!UICONTROL Delete]** in het rechterdeelvenster.
1. Verwijderen bevestigen. Als de levering kindknopen heeft, kunt u verkiezen om hen ook te schrappen, of hen te houden.

![ Schrap een levering in een werkschema ](assets/delete-delivery-from-wf.png)
