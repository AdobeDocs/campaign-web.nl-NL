---
audience: end-user
title: Het goedkeuringsproces instellen en beheren
description: Leer hoe u goedkeuringen van marketingcampagnes beheert in Campagne Web
feature: Approvals, Campaigns
exl-id: 8140f904-ec0a-44e1-981f-0e050d3c9cdb
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 1%

---

# Het goedkeuringsproces beheren {#campaign-approvals}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn6"
>title="Goedkeuringsbeheer voor campagnes"
>abstract="U kunt nu de validatie van belanghebbenden coördineren voordat u leveringen verzendt. Vereisen goedkeuring van marketingmanagers, gegevensanalisten of andere teams voor kwaliteitscontrole."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"

>[!IMPORTANT]
>
>Goedkeuringen zijn alleen beschikbaar voor leveringen die in een campagne zijn gemaakt. Dit is niet van toepassing op zelfstandige leveringen of leveringen die in workflows buiten een campagnecontext worden gemaakt.

Het goedkeuringsproces helpt meerdere belanghebbenden te coördineren en zorgt voor kwaliteitscontrole voordat leveringen worden verzonden. Gebruik goedkeuringen wanneer uw organisatie validatie van verschillende teams vereist, zoals marketingmanagers die inhoud controleren of gegevensanalisten die doelgroepen valideren.

Wanneer goedkeuringen zijn ingeschakeld, moet u inhoud of doel ter goedkeuring indienen. Aangewezen revisoren ontvangen e-mailmeldingen met het verzoek om validatie en kunnen deze rechtstreeks vanuit de interface van de webinterface goedkeuren of afwijzen. Leveringen kunnen pas worden verzonden nadat alle vereiste goedkeuringen zijn verleend. U kunt inschakelen:

* **Goedkeuring van de Inhoud**: bevestig berichtinhoud, ontwerp, en verpersoonlijking
* **goedkeuring van het Doel**: bevestig het publiek en richtend criteria
* **Bevestiging van de Levering**: vereist een definitieve bevestiging alvorens te verzenden

## Goedkeuringsinstellingen configureren {#configure-approvals}

De goedkeuringsinstellingen worden overgenomen van de campagnemalplaatje en kunnen voor afzonderlijke campagnes worden gewijzigd. Voer de volgende stappen uit om goedkeuringsinstellingen te configureren:

1. Open uw campagne of campagnemalplaatje, of creeer nieuwe, van het **[!UICONTROL Campaigns]** menu.

1. Klik op de knop **[!UICONTROL Settings]** in de rechterbovenhoek van het campagnemdashboard.

1. Configureer in de sectie **[!UICONTROL Approvals]** de volgende opties:

   ![&#x200B; Schermafbeelding die de montages van de campagnegoedkeuring toont &#x200B;](assets/approvals1.png){zoomable="yes"}

   * **[!UICONTROL Enable content approval]**: als deze optie is ingeschakeld, moet de inhoud van de levering worden goedgekeurd voordat deze wordt verzonden. Klik op het mappictogram in het veld **[!UICONTROL Reviewer]** om een operator of een operatorgroep te selecteren.

   * **[!UICONTROL Enable target approval]**: als deze optie is ingeschakeld, moet het doelpubliek van de levering worden goedgekeurd. Klik op het mappictogram in het veld **[!UICONTROL Reviewer]** om een operator of een operatorgroep te selecteren.

   * **[!UICONTROL Confirm the delivery before sending]**: vereist een laatste handmatige bevestiging voordat u gaat verzenden, zelfs nadat alle andere goedkeuringen zijn voltooid.

>[!NOTE]
>
>* Als er geen controleur is opgegeven, wordt de eigenaar van de campagne toegewezen als controleur.
>* Revisoren hebben de juiste machtigingen nodig om leveringen goed te keuren. Alleen gebruikers die zijn geïdentificeerd in de lijst met revisoren kunnen goedkeuring verlenen.

## Ter goedkeuring indienen {#submit-approval}

Nadat u de levering hebt gemaakt, voert u de volgende stappen uit om inhoud en doel ter goedkeuring te verzenden.

>[!NOTE]
>Goedkeuringen zijn beschikbaar in workflowleveringen voor campagnes en zelfstandige leveringen voor campagnes.

1. Klik op de knop **[!UICONTROL Submit content]** in het dashboard voor levering. Aangewezen revisoren kunnen deze goedkeuren of afwijzen. Zie deze [&#x200B; sectie &#x200B;](#approve-reject).

   ![&#x200B; Schermafbeelding die de Submit inhoudsknoop tonen &#x200B;](assets/approvals2.png){zoomable="yes"}

   De goedkeuringsstatus wordt gewijzigd in InDesign in de sectie **[!UICONTROL Properties]** van het leveringsdashboard. Zie deze [&#x200B; sectie &#x200B;](#rack-approvals).

1. Wanneer de inhoud is goedgekeurd, klikt u op de knop **[!UICONTROL Prepare]** om het leveringsdoel voor te bereiden. Het systeem bereidt het publiek voor en richt criteria.

1. Klik op de knop **[!UICONTROL Submit target]**. Aangewezen revisoren kunnen vervolgens goedkeuren of afwijzen. Zie deze [&#x200B; sectie &#x200B;](#approve-reject).

   ![&#x200B; Schermafbeelding die de Submit doelknoop toont &#x200B;](assets/approvals5.png){zoomable="yes"}

   De goedkeuringsstatus verandert in In behandeling. Zie deze [&#x200B; sectie &#x200B;](#rack-approvals).

1. Zodra het doel is goedgekeurd, wordt het preparaat hervat en kan de levering worden verzonden.

>[!NOTE]
>Als een goedkeuring wordt geweigerd, moet de eigenaar van de levering alle noodzakelijke wijzigingen in de inhoud of het doel aanbrengen op basis van de feedback van de controleur en deze opnieuw ter goedkeuring voorleggen.

## Goedkeuren of afwijzen {#approve-reject}

Aangewezen revisoren kunnen inhoud en doelverzendingen goedkeuren of afwijzen. Zie deze [&#x200B; sectie &#x200B;](#submit-approval).

>[!NOTE]
>Het e-mailbericht kan alleen worden verzonden als het adres van de revisor in de instantie is geconfigureerd.

1. Wanneer u het bericht e-mail ontvangt, open de levering die goedkeuring direct van de interface van het Web UI vereist.

1. Controleer de inhoud of doelinformatie.

1. Klik op **[!UICONTROL Approve content]** of **[!UICONTROL Approve target]** .

   ![&#x200B; Schermafbeelding die de Goedkeuren inhoudsknoop in het leveringsdashboard toont &#x200B;](assets/approvals3.png){zoomable="yes"}

1. Klik op **[!UICONTROL Approve]** of **[!UICONTROL Reject]** .

1. Voeg desgewenst een **[!UICONTROL Comment]** toe om uw beslissing toe te lichten.

   ![&#x200B; Schermafbeelding die de goedkeuringsdialoog tonen met goedkeuren, verwerpt knopen en gebied van de Commentaar &#x200B;](assets/approvals4.png){zoomable="yes"}

1. Bevestig uw beslissing. De goedkeuringsstatus wordt onmiddellijk bijgewerkt in het leveringsdashboard. Zie deze [&#x200B; sectie &#x200B;](#rack-approvals).

## Goedkeuringsstatus track {#track-approvals}

De goedkeuringsstatus is zichtbaar in de **[!UICONTROL Properties]** -sectie van het leveringsdashboard. De status geeft aan welke goedkeuringen wachten en welke status ze hebben:

![&#x200B; Schermafbeelding die goedkeuringsstatus tonen &#x200B;](assets/approvals5.png){zoomable="yes"}

* **[!UICONTROL Being edited]**: de inhoud of het doel is nog niet ter goedkeuring ingediend
* **[!UICONTROL Pending approval]**: de inhoud of het doel is in afwachting van revisie
* **[!UICONTROL Approved]**: de inhoud of het doel is goedgekeurd door de controleur
* **[!UICONTROL Rejected]**: de inhoud of het doel is afgewezen door de controleur

In het goedkeuringsgedeelte worden alle ingeschakelde goedkeuringen en updates in real-time weergegeven terwijl revisoren elke stap valideren of afwijzen.

## Verwante onderwerpen {#related}

* [Campagnes maken](create-campaigns.md)
* [Campagnes beheren](manage-campaigns.md)
