---
audience: end-user
title: De workflowactiviteit voor pushmeldingen gebruiken
description: Leer hoe u de workflowactiviteit voor pushmeldingen kunt gebruiken
badge: label="Beta"
source-git-commit: 9fb4a5057ec05877ffbadc85d1198ab24faf8972
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Pushmelding {#push-activity}

De **Pushmelding** Met leveringsactiviteit kunt u het verzenden van een pushmelding configureren in een workflow.

>[!BEGINTABS]

>[!TAB Pushmelding (Android)]

1. Na het creëren van en het vormen van een nieuw werkschema, voeg een het publieksactiviteit van de Bouwstijl toe om een bestaand publiek te selecteren of de regelbouwer te gebruiken om uw eigen vraag te bepalen.

1. Voeg een Android-kanaalactiviteit (Push Notification) toe aan uw workflow.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Selecteer uw activiteit. Selecteer in het bezorgmenu de sjablonen die u voor deze levering wilt gebruiken. Meer informatie over sjablonen

1. Klik op Levering maken om de levering van uw pushmelding te configureren. Raadpleeg deze pagina voor meer informatie over de levering van pushberichten (Android).

1. Wanneer uw levering klaar is om te worden verzonden, navigeert u terug naar uw workflow en klikt u op Start om uw workflow te starten.

1. Door gebrek, leidt het in werking stellen van een leveringswerkschema tot het stadium van de berichtvoorbereiding, zonder onmiddellijk het bericht te verzenden.

   Klik op Reviseren en verzenden in het geavanceerde menu van de Android-kanaalactiviteit (Push Notification) om het verzenden te bevestigen.

1. Klik op Verzenden vanaf het dashboard voor pushmeldingen.

>[!TAB Pushmelding (iOS)]

1. Na het creëren van en het vormen van een nieuw werkschema, voeg een het publieksactiviteit van de Bouwstijl toe om een bestaand publiek te selecteren of de regelbouwer te gebruiken om uw eigen vraag te bepalen.

1. Voeg een Push Notification (iOS)-kanaalactiviteit toe aan uw workflow.

<!--
1. Select the Type of delivery:

    * Single delivery: Choose this option if you want the push notification to be sent only once. You have the flexibility to choose whether or not to include an outbound transition from this activity.

    * Recurring delivery: Choose this option if you want the push notification to be sent multiple times based on a defined frequency. The frequency can be configured using a Scheduler activity, allowing you to schedule the push notification to be sent at regular intervals.
-->

1. Selecteer uw activiteit. Selecteer in het bezorgmenu de sjablonen die u voor deze levering wilt gebruiken. Meer informatie over sjablonen

1. Klik op Levering maken om de levering van uw pushmelding te configureren. Raadpleeg deze pagina voor meer informatie over de levering van pushberichten (iOS).

1. Wanneer uw levering klaar is om te worden verzonden, navigeert u terug naar uw workflow en klikt u op Start om uw workflow te starten.

1. Door gebrek, leidt het in werking stellen van een leveringswerkschema tot het stadium van de berichtvoorbereiding, zonder onmiddellijk het bericht te verzenden.

   Klik op Revisie en verzend vanuit het geavanceerde menu van uw Push Notification (iOS)-kanaalactiviteit om het verzenden te bevestigen.

1. Klik op Verzenden vanaf het dashboard voor pushmeldingen.

>[!ENDTABS]