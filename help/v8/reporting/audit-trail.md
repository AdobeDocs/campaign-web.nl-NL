---
product: campaign
title: Audit trail
description: Leer hoe u uw exemplaar kunt controleren met het Campagne Audit Trail
feature: Audit Trail, Monitoring, Workflows
exl-id: f4b4a33f-8250-4f4e-b2dc-129c56f9ea0f
source-git-commit: 3729a6159affbbb30d2cdab91d1e42dbf9df9c86
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 1%

---

# Audit trail{#audit-trail}

In Adobe Campaign Web User Interface biedt de functie **[!UICONTROL Audit trail]** gebruikers volledige zichtbaarheid bij alle wijzigingen die zijn aangebracht aan belangrijke entiteiten in uw instantie, meestal die wijzigingen die een vloeiende bewerking van de instantie aanzienlijk beïnvloeden.

>[!IMPORTANT]
>
>* De gebruikersinterface van het Web van Adobe Campaign controleert geen veranderingen die binnen gebruikersrechten, malplaatjes, verpersoonlijking, of campagnes worden aangebracht.
>* Het spoor van de controle kan slechts door beheerders van de instantie worden beheerd.

De functie **[!UICONTROL Audit trail]** houdt voortdurend een gedetailleerd logboek bij van de acties en gebeurtenissen die in real-time binnen de Adobe Campaign-instantie plaatsvinden. Het biedt een geschikte methode aan om tot een chronologisch verslag van gegevens toegang te hebben, die vragen zoals: de status van werkschema&#39;s, de recentste individuen richten om hen te wijzigen, of de activiteiten richten die door gebruikers binnen de instantie worden uitgevoerd.

+++ Meer informatie over beschikbare entiteiten van het audittrail

* **het de controlespoor van het Schema van Source** staat u toe om activiteiten en recente wijzigingen te controleren die aan uw schema&#39;s binnen de de cliëntconsole van de Campagne V8 worden aangebracht.

  Voor gedetailleerde informatie over schema&#39;s, verwijs naar [ de Documentatie van de Campagne v8 ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **het controletraject van het Werkschema** staat u toe om spoor van activiteiten en recente veranderingen te houden die aan werkschema&#39;s, met inbegrip van hun huidige staten zoals worden aangebracht:

   * Starten
   * Pauzeren
   * Stoppen
   * Opnieuw starten
   * Opschonen wat overeenkomt met de handeling Historie leegmaken
   * Simuleer wat aan de actieBegin op simulatiemodus evenaart
   * Wakeup die gelijk is aan de handeling Voer taken uit die in behandeling zijn.
   * Onvoorwaardelijk stoppen

  Voor meer informatie over werkschema&#39;s, verwijs naar deze [ pagina ](../workflows/gs-workflows.md).

* **de controlespoor van de Optie** laat u toe om activiteiten en recente wijzigingen te controleren die aan uw opties in Campagne V8 worden aangebracht.

  Voor meer informatie over opties, verwijs naar deze [ pagina ](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **de controletrail van de Levering** staat u toe om de activiteiten en de laatste wijzigingen te controleren die aan uw leveringen worden gedaan.

  Voor meer informatie over leveringen, verwijs naar deze [ pagina ](../msg/gs-deliveries.md).

* **Externe Rekening** staat u toe om wijzigingen te controleren die aan externe rekeningen in Campagne V8 worden aangebracht, die door technische processen zoals technische werkschema&#39;s of campagnewerkschema&#39;s worden gebruikt.

  Voor meer informatie over externe rekening, verwijs naar deze [ pagina ](../administration/external-account.md).

* **Afbeelding van de Levering** laat u toe om activiteiten en recente wijzigingen te controleren die aan uw Aflevering in Campagne V8 worden aangebracht.

  Voor meer informatie over leveringsafbeelding, verwijs naar deze [ pagina ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Toepassing van het Web** staat u toe om wijzigingen te controleren die aan de vormen van het Web in Campagne V8 worden aangebracht om pagina&#39;s met input en selectievelden tot stand te brengen, en die gegevens van het gegevensbestand kunnen omvatten.

  Voor meer informatie over Webtoepassing, verwijs naar deze [ pagina ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Aanbieding** staat u toe om de activiteiten en de laatste wijzigingen te controleren die aan uw aanbiedingen worden gedaan.

  Voor meer informatie over aanbiedingen, verwijs naar deze [ pagina ](../msg/offers.md).

* **Exploitant** laat u toe om activiteiten en recente wijzigingen te controleren die aan uw Operatoren in Campagne V8 worden aangebracht.

  Voor meer informatie over exploitanten, verwijs naar deze [ pagina ](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Audittrail openen {#accessing-audit-trail}

Ga als volgt te werk om het exemplaar **[!UICONTROL Audit trail]** te openen:

1. Selecteer **[!UICONTROL Audit trail]** onder het menu **[!UICONTROL Administration]** .

   ![](assets/audit-trail-1.png)

1. Het venster **[!UICONTROL Audit trail]** wordt geopend met de lijst met entiteiten. Adobe Campaign Web User Interface controleert het maken, bewerken en verwijderen van acties voor workflows, opties, leveringen en schema&#39;s.

   Selecteer een van de entiteiten voor meer informatie over de laatste wijzigingen.

1. In het venster **[!UICONTROL Audit entity]** vindt u gedetailleerdere informatie over de gekozen entiteit, zoals:

   * **[!UICONTROL Type]**: Workflow, opties, leveringen of schema&#39;s.
   * **[!UICONTROL Entity]**: interne naam van uw activiteiten.
   * **[!UICONTROL Modified by]**: Gebruikersnaam van de laatste persoon die deze entiteit als laatste heeft gewijzigd.
   * **[!UICONTROL Action]**: De laatste actie die op deze entiteit is uitgevoerd, is gemaakt, gewijzigd of verwijderd.
   * **[!UICONTROL Modification date]**: Datum van de laatste actie die op deze entiteit is uitgevoerd.

   Het codeblok geeft u meer informatie over wat precies in uw entiteit is gewijzigd.

   ![](assets/audit-trail-2.png)
