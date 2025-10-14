---
product: campaign
title: Audit trail
description: Leer hoe u uw exemplaar kunt controleren met het Campagne Audit Trail
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 1%

---

# Audit trail {#audit-trail}

In Adobe Campaign Web User Interface biedt de functie **[!UICONTROL Audit trail]** gebruikers volledige zichtbaarheid bij alle wijzigingen die zijn aangebracht aan belangrijke entiteiten in uw instantie, meestal die wijzigingen die een aanzienlijke invloed hebben op de vloeiende werking van de instantie.

>[!IMPORTANT]
>
>* De gebruikersinterface van het Web van Adobe Campaign controleert geen veranderingen die binnen gebruikersrechten, malplaatjes, verpersoonlijking, of campagnes worden aangebracht.
>* Alleen beheerders van de instantie kunnen het audittrail beheren.

De functie **[!UICONTROL Audit trail]** neemt voortdurend een gedetailleerd logboek op van acties en gebeurtenissen die in real-time in de Adobe Campaign-instantie plaatsvinden. Het biedt een geschikte methode aan om tot een chronologisch verslag van gegevens toegang te hebben, die vragen zoals de status van werkschema&#39;s, de recentste individuen richten om hen te wijzigen, of de activiteiten richten die door gebruikers binnen de instantie worden uitgevoerd.

+++ Meer informatie over beschikbare entiteiten in het audittrail

* **het de controlespoor van het Schema van Source** staat u toe om activiteiten en recente wijzigingen te controleren die aan uw schema&#39;s binnen de de cliëntconsole van de Campagne v8 worden aangebracht.

  Voor gedetailleerde informatie over schema&#39;s, verwijs naar [&#x200B; de Documentatie van de Campagne v8 &#x200B;](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **het controletraject van het Werkschema** staat u toe om spoor van activiteiten en recente veranderingen te houden die aan werkschema&#39;s, met inbegrip van hun huidige staten zoals worden aangebracht:

   * Starten
   * Pauzeren
   * Stoppen
   * Opnieuw starten
   * Overbodig verwijderen; dit is gelijk aan de handeling Geschiedenis leegmaken
   * Simuleren, dat gelijk is aan de handeling Start in de simulatiemodus
   * Wakeup, dat gelijk is aan de handeling Voer taken uit die in behandeling zijn.
   * Onvoorwaardelijk stoppen

  Voor meer informatie over werkschema&#39;s, verwijs naar deze [&#x200B; pagina &#x200B;](../workflows/gs-workflows.md).

* **de controlespoor van de Optie** laat u toe om activiteiten en recente wijzigingen te controleren die aan uw opties in Campagne v8 worden aangebracht.

  Voor meer informatie over opties, verwijs naar deze [&#x200B; pagina &#x200B;](https://experienceleague.adobe.com/nl/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **de controletrail van de Levering** staat u toe om de activiteiten en de laatste wijzigingen te controleren die aan uw leveringen worden gedaan.

  Voor meer informatie over leveringen, verwijs naar deze [&#x200B; pagina &#x200B;](../msg/gs-deliveries.md).

* **Externe Rekening** staat u toe om wijzigingen te controleren die aan externe rekeningen in Campagne v8 worden aangebracht, die door technische processen zoals technische werkschema&#39;s of campagnewerkschema&#39;s worden gebruikt.

  Voor meer informatie over externe rekeningen, verwijs naar deze [&#x200B; pagina &#x200B;](../administration/external-account.md).

* **Afbeelding van de Levering** laat u toe om activiteiten en recente wijzigingen te controleren die aan uw Aflevering in Campagne v8 worden aangebracht.

  Voor meer informatie over leveringsafbeelding, verwijs naar deze [&#x200B; pagina &#x200B;](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Toepassing van het Web** staat u toe om wijzigingen te controleren die aan de vormen van het Web in Campagne v8 worden aangebracht, die worden gebruikt om pagina&#39;s met input en selectievelden tot stand te brengen, en die gegevens van het gegevensbestand kunnen omvatten.

  Voor meer informatie over Webtoepassingen, verwijs naar deze [&#x200B; pagina &#x200B;](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/content/webapps).

* **Aanbieding** staat u toe om de activiteiten en de laatste wijzigingen te controleren die aan uw aanbiedingen worden gedaan.

  Voor meer informatie over aanbiedingen, verwijs naar deze [&#x200B; pagina &#x200B;](../msg/offers.md).

* **Exploitant** laat u toe om activiteiten en recente wijzigingen te controleren die aan uw Operatoren in Campagne v8 worden aangebracht.

  Voor meer informatie over exploitanten, verwijs naar deze [&#x200B; pagina &#x200B;](https://experienceleague.adobe.com/nl/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Audittrail openen {#accessing-audit-trail}

Ga als volgt te werk om het exemplaar **[!UICONTROL Audit trail]** te openen:

1. Selecteer **[!UICONTROL Audit trail]** onder het menu **[!UICONTROL Administration]** .

   ![&#x200B; Schermschot die het menu van het Beleid met de geselecteerde het spooroptie van de Controle tonen &#x200B;](assets/audit-trail-1.png)

1. Het venster **[!UICONTROL Audit trail]** wordt geopend met de lijst met entiteiten. De gebruikersinterface van het Web van Adobe Campaign controleert creeert, geeft, en schrapt acties voor werkschema&#39;s, opties, leveringen, en schema&#39;s uit.

   Selecteer een van de entiteiten voor meer informatie over de laatste wijzigingen.

1. Het venster **[!UICONTROL Audit entity]** bevat gedetailleerde informatie over de gekozen entiteit, zoals:

   * **[!UICONTROL Type]**: Workflow, Opties, Leveringen of Schema&#39;s.
   * **[!UICONTROL Entity]**: interne naam van uw activiteiten.
   * **[!UICONTROL Modified by]**: Gebruikersnaam van de laatste persoon die deze entiteit heeft gewijzigd.
   * **[!UICONTROL Action]**: De laatste actie die op deze entiteit is uitgevoerd, is gemaakt, gewijzigd of verwijderd.
   * **[!UICONTROL Modification date]**: Datum van de laatste actie die op deze entiteit is uitgevoerd.

   Het codeblok bevat meer informatie over wat precies in uw entiteit is gewijzigd.

   ![&#x200B; Schermafbeelding die het venster van de Auditentiteit met gedetailleerde informatie over wijzigingen tonen &#x200B;](assets/audit-trail-2.png)