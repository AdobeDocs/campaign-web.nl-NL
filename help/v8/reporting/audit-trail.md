---
product: campaign
title: Audit trail
description: Leer hoe u uw exemplaar kunt controleren met het Campagne Audit Trail
feature: Audit Trail, Monitoring, Workflows
source-git-commit: 93ac61808049da6f0d800a19f2baf97946d8612c
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 2%

---

# Audit trail{#audit-trail}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn1"
>title="Audit trail"
>abstract="De nieuwe controletrailfunctie biedt een gedetailleerd en chronologisch overzicht van alle acties en gebeurtenissen die in real-time aan uw Adobe Campaign-instantie zijn uitgevoerd."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"


In Adobe Campaign Web User Interface, **[!UICONTROL Audit trail]** biedt gebruikers volledige zichtbaarheid in alle wijzigingen die zijn aangebracht aan belangrijke entiteiten in uw instantie, meestal die entiteiten die een vloeiende bewerking van de instantie aanzienlijk beïnvloeden.

>[!IMPORTANT]
>
>* De gebruikersinterface van het Web van Adobe Campaign controleert geen veranderingen die binnen gebruikersrechten, malplaatjes, verpersoonlijking, of campagnes worden aangebracht.
>* Het spoor van de controle kan slechts door beheerders van de instantie worden beheerd.

**[!UICONTROL Audit trail]** Deze functie houdt voortdurend een gedetailleerd logboek bij van de acties en gebeurtenissen die in real-time binnen de Adobe Campaign-instantie plaatsvinden. Het biedt een geschikte methode aan om tot een chronologisch verslag van gegevens toegang te hebben, die vragen zoals: de status van werkschema&#39;s, de recentste individuen richten om hen te wijzigen, of de activiteiten richten die door gebruikers binnen de instantie worden uitgevoerd.

+++ Meer informatie over beschikbare entiteiten van het audittrail

* **Bronschema voor audittrail** staat u toe om activiteiten en recente wijzigingen te controleren die aan uw schema&#39;s binnen de de cliëntconsole van de Campagne V8 worden aangebracht.

  Raadpleeg voor meer informatie over schema&#39;s [Campagne v8 Documentatie](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/developer/shemas-forms/schemas).

* **Workflowaudittrail** kunt u activiteiten en recente wijzigingen in workflows bijhouden, waaronder de huidige statussen, zoals:

   * Starten
   * Pauzeren
   * Stoppen
   * Opnieuw starten
   * Opschonen wat overeenkomt met de handeling Historie leegmaken
   * Simuleer wat aan de actieBegin op simulatiemodus evenaart
   * Wakeup die gelijk is aan de handeling Voer taken uit die in behandeling zijn.
   * Onvoorwaardelijk stoppen

  Raadpleeg deze voor meer informatie over workflows [page](../workflows/gs-workflows.md).

* **Optie audittrail** kunt u activiteiten en recente wijzigingen in uw opties in Campagne V8 controleren.

  Raadpleeg deze voor meer informatie over opties [page](https://experienceleague.adobe.com/en/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options).

* **Afleveringsaudittrail** kunt u de activiteiten en de laatste wijzigingen die u hebt aangebracht in uw leveringen controleren.

  Raadpleeg de volgende secties voor meer informatie over leveringen [page](../msg/gs-deliveries.md).

* **Externe account** kunt u wijzigingen controleren die in externe rekeningen in Campagne V8 worden aangebracht, die door technische processen zoals technische werkschema&#39;s of campagnewerkschema&#39;s worden gebruikt.

  Voor meer informatie over externe account raadpleegt u deze [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/config/configuration/external-accounts).

* **Aflevering toewijzen** kunt u activiteiten en recente wijzigingen in uw leveringstoewijzing in Campagne V8 controleren.

  Raadpleeg deze voor meer informatie over leveringstoewijzing [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/audience/add-profiles/target-mappings).

* **Webtoepassing** Hiermee kunt u wijzigingen controleren die in webformulieren zijn aangebracht in Campagne V8 waarmee pagina&#39;s met invoer- en selectievelden worden gemaakt en die gegevens uit de database kunnen bevatten.

  Raadpleeg deze voor meer informatie over webtoepassingen [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/content/webapps).

* **Voorstel** Hiermee kunt u de activiteiten en de laatste wijzigingen in uw voorstellen controleren.

  Raadpleeg deze voor meer informatie over aanbiedingen [page](../msg/offers.md).

* **Operator** kunt u activiteiten en recente wijzigingen die in Campagne V8 aan uw Operatoren zijn aangebracht, controleren.

  Raadpleeg de volgende secties voor meer informatie over operatoren [page](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/offers/interaction-settings/interaction-operators).

+++

## Audittrail openen {#accessing-audit-trail}

Toegang krijgen tot de **[!UICONTROL Audit trail]**:

1. Onder de **[!UICONTROL Administration]** menu, selecteert u **[!UICONTROL Audit trail]** .

   ![](assets/audit-trail-1.png)

1. De **[!UICONTROL Audit trail]** wordt geopend met de lijst van uw entiteiten. Adobe Campaign Web User Interface controleert het maken, bewerken en verwijderen van acties voor workflows, opties, leveringen en schema&#39;s.

   Selecteer een van de entiteiten voor meer informatie over de laatste wijzigingen.

1. De **[!UICONTROL Audit entity]** het venster geeft u meer gedetailleerde informatie over de gekozen entiteit zoals:

   * **[!UICONTROL Type]** : Workflow, opties, leveringen of schema&#39;s.
   * **[!UICONTROL Entity]** : Interne naam van uw activiteiten.
   * **[!UICONTROL Modified by]** : Gebruikersnaam van de laatste persoon die deze entiteit als laatste heeft gewijzigd.
   * **[!UICONTROL Action]** : De laatste actie die op deze entiteit is uitgevoerd, is gemaakt, gewijzigd of verwijderd.
   * **[!UICONTROL Modification date]** : Datum van de laatste actie die op deze entiteit is uitgevoerd.

   Het codeblok geeft u meer informatie over wat precies in uw entiteit is gewijzigd.

   ![](assets/audit-trail-2.png)

