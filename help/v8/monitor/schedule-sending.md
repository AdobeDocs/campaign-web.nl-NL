---
audience: end-user
title: Plaats de verzending van een levering
description: Leer hoe u een levering kunt plannen
exl-id: 0738a148-d550-41c2-a8c2-6054684ba789
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Plaats de verzending van een levering {#schedule-sending}

U kunt de verzending van een levering plannen. De stappen zijn afhankelijk van het feit of het een zelfstandige (one-shot) levering is of dat u in de context van een campagneworkflow werkt.

## Zelfstandige levering

Voor standalone leveringen, bepaal de datum en de tijd direct in de levering. Zie de voorbeelden hieronder voor elk type levering: e-mail, SMS en pushmelding.

### Email {#schedule-email-standalone}

Voer de volgende stappen uit om de verzending van een e-mailbericht te plannen:

1. Activeer in de sectie **[!UICONTROL Schedule]** van de leveringseigenschappen de schakeloptie **[!UICONTROL Enable scheduling]** .

1. Stel de gewenste datum en tijd in voor het verzenden en klik op de knop **[!UICONTROL Review and send]** .

   ![ activeer het plannen en plaats datum en tijd ](assets/schedule-email-standalone.png){zoomable="yes"}

>[!NOTE]
>
>Standaard is de optie **[!UICONTROL Enable confirmation before sending]** ingeschakeld. Voor deze optie moet u de verzending bevestigen voordat de levering op de geplande datum en tijd wordt verzonden. Schakel deze optie uit als u de levering automatisch op de geplande datum en tijd wilt verzenden.
>

1. Controleer of het schema juist is en klik op de knop **[!UICONTROL Prepare]** .

![ Controle programma en bereidt levering ](assets/schedule-email-standalone-prepare.png){zoomable="yes"} voor

1. Zodra de voorbereiding is voltooid, zijn de berichten klaar om te worden verzonden. De belangrijkste metriek voor de levering wordt getoond, met inbegrip van totale doelbevolking, aantal te leveren berichten, en aantal uitgesloten ontvangers. Klik op de knop **[!UICONTROL Send as scheduled]** om te bevestigen dat de levering op de geplande datum en tijd wordt verzonden naar het hoofddoel.

![ bevestigt het verzenden zoals gepland ](assets/schedule-email-standalone-send.png){zoomable="yes"}

### Sms

Voer dezelfde stappen uit als voor e-mailleveringen als voor het plannen van de levering van SMS-berichten voor een bepaalde datum en tijd. [ zie hierboven ](#schedule-email-standalone).

![ levering van SMS van het Programma ](assets/schedule-sms-standalone.png){zoomable="yes"}

U kunt ook controleren of het schema wordt toegepast:

![ het programma van SMS van de Controle ](assets/schedule-sms-standalone-prepare.png){zoomable="yes"}

### Pushmelding

Volg dezelfde stappen als voor e-mailleveringen als voor het plannen van een zelfstandige pushlevering voor een specifieke datum en tijd. [ zie hierboven ](#schedule-email-standalone).

![ de dupmeldingslevering van het Programma ](assets/schedule-push-standalone.png){zoomable="yes"}

U kunt ook controleren of het schema wordt toegepast:

![ pushmeldingsprogramma van de Controle ](assets/schedule-push-standalone-prepare.png){zoomable="yes"}

### Zelfstandige levering in een campagne

U kunt een zelfstandige levering binnen een campagne tot stand brengen zonder een werkschema te gebruiken. Stel de datum en het tijdschema voor deze levering in, zoals hierboven beschreven. De campagne kan een eigen planning hebben, inclusief een begindatum en een einddatum. Dit schema interfereert niet met uw leveringsschema.

![ Standalone levering in een campagne ](assets/schedule-delivery-standalone.png){zoomable="yes"}

## Een levering plannen in een campagneworkflow

In de context van een campagneworkflow kunt u het beste de **[!UICONTROL Scheduler]** -activiteit gebruiken om een datum en tijd toe te passen voor het starten van de workflow, waarbij de levering wordt verzonden. [ leer meer over Planner ](../workflows/activities/scheduler.md).

![ levering van het Programma in een campagnewerkschema ](assets/schedule-workflow.png){zoomable="yes"}

Configureer de datum en tijd in de **[!UICONTROL Scheduler]** -activiteit.

![ vorm de activiteit van de Planner ](assets/schedule-workflow-scheduler.png){zoomable="yes"}

>[!NOTE]
>
>Wanneer u de **[!UICONTROL Scheduler]** -activiteit gebruikt om de verzending van de levering in een workflow te plannen, activeert u de **[!UICONTROL Enable scheduling]** -schakeloptie niet in de activiteitsinstellingen van **[!UICONTROL Delivery]** . De levering wordt automatisch verzonden.
>

Als u de schakeloptie **[!UICONTROL Enable scheduling]** activeert in de instellingen voor **[!UICONTROL Delivery]** -activiteit en daar een datum en tijd instelt, wordt de levering wacht op verzending op deze datum en tijd. Dit betekent dat als er een vertraging is tussen de startdatum van de workflow en de verzenddatum, het publiek mogelijk niet up-to-date is.