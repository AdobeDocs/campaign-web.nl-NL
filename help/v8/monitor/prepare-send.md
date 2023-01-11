---
audience: end-user
title: Een e-mail voorbereiden en verzenden
description: Campagne v8 Webdocumentatie
exl-id: 80c16d2d-2a31-48f1-a161-ee574ec24172
source-git-commit: 1157113798f95329651e71b726d6132f9d8c7544
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 4%

---

# Uw e-mail voorbereiden en verzenden {#prepare-send}

![](../assets/do-not-localize/badge.png)

>[!CONTEXTUALHELP]
>id="acw_homepage_card5"
>title="Uw e-mail voorbereiden en verzenden"
>abstract="Ontdek hoe u uw e-mail kunt voorbereiden en meer kunt leren over het verzenden van KPI&#39;s."

<!--

	show how to prepare and send the email + the live kpis in the dashboard

like acc when preparation, target calculated then send
real time KPIs, not in AJO. similar to ACS.
exclusion logs, causes
-->

<!--
send also KPIs
-->

## De verzending voorbereiden{#prepare}

Wanneer u uw inhoud, publiek en planning hebt bepaald, bent u bereid om uw bericht voor te bereiden. Tijdens de voorbereiding, wordt de doelbevolking berekend en de berichtinhoud geproduceerd voor elk profiel inbegrepen in het doel. Zodra de voorbereiding is voltooid, zijn de berichten klaar om te worden verzonden, of onmiddellijk of op de geplande datum en tijd. De validatieregels die tijdens de analyse worden gebruikt, worden in deze [sectie](https://experienceleague.adobe.com/docs/campaign-classic/using/sending-messages/key-steps-when-creating-a-delivery/steps-validating-the-delivery.html#validation-process-with-typologies).

Volg de onderstaande stappen:

1. Klik op het bezorgdashboard op de knop **Voorbereiden** in de rechterbovenhoek en bevestig.

   ![](assets/prepare.png)

   De voortgang van de voorbereiding wordt weergegeven. Afhankelijk van de omvang van de doelpopulatie kan deze operatie enige tijd in beslag nemen.

   >[!NOTE]
   >
   >U kunt de bereiding op elk gewenst moment stoppen met de **Voorbereiding stoppen** knop. Tijdens de voorbereidingsfase worden geen berichten verzonden. U kunt dit daarom starten of stoppen zonder het risico te lopen iets te beïnvloeden.

1. Controleer de PKI&#39;s wanneer de bereiding is voltooid. Als het aantal berichten dat u wilt verzenden niet overeenkomt met uw verwachtingen, wijzigt u het publiek en start u de voorbereiding opnieuw.

   ![](assets/prepare2.png)

   Hier worden de verschillende KPI&#39;s weergegeven:

   * **Gericht**: het aantal doelgroepen
   * **Om te leveren**: het aantal berichten dat wordt verzonden
   * **Uitsluiten**: het aantal berichten dat door een typologieregel is uitgesloten

1. Klik op de knop **Logboeken** en controleert u of er geen fout optreedt. In het laatste logbericht worden foutberichten en het aantal fouten weergegeven. Zie [deze sectie](delivery-logs.md) voor meer informatie.

   ![](assets/prepare-logs.png)

Als in het preparaat een kritieke fout wordt aangetroffen waardoor de levering niet kan worden verzonden, wordt de status van het preparaat in het leveringsdashboard weergegeven als mislukt.

![](assets/prepare-error.png)

Als u na de bereiding wijzigingen in uw aflevering moet aanbrengen, moet u de voorbereiding opnieuw starten om met deze wijzigingen rekening te houden.

Zodra de voorbereiding zonder fout volledig is, is uw bericht klaar om te worden verzonden. Zie [deze sectie](#send) voor meer informatie.

## Bericht verzenden{#send}

Zodra de voorbereiding volledig is, kunt u uw bericht nu verzenden. Deze stap is alleen vereist voor berichten die direct worden verzonden. Als het bericht gepland is, wordt het verzonden op de bepaalde datum.

Voer de volgende stappen uit:

1. Klik op het bezorgdashboard op de knop **Verzenden** in de rechterbovenhoek en bevestigen.

   ![](assets/send.png)

1. De verzendvoortgang wordt weergegeven. Controleer de getoonde KPIs. U kunt ook de logbestanden controleren. Zie [deze sectie](delivery-logs.md) voor meer informatie.

   ![](assets/send2.png)

   Hier worden de verschillende KPI&#39;s weergegeven:

   * **Geleverd**: het aantal berichten dat is verzonden. Het percentage is gebaseerd op het totale aantal beoogde ontvangers.
   * **Openen**: het aantal geopende berichten. Het percentage is gebaseerd op het aantal geleverde berichten.
   * **Klikken**: het aantal ontvangers dat ten minste één keer in de e-mail heeft geklikt. Het percentage is gebaseerd op het aantal geleverde berichten.

   >[!NOTE]
   >
   >De **Openen** en **Klikken** indicatoren worden in real time bijgewerkt.

   U kunt het verzenden op elk ogenblik pauzeren en dan hervatten. Als u de levering tegenhoudt terwijl het wordt verzonden, zult u niet kunnen hervatten.
