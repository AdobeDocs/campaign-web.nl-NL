---
product: campaign
title: Leveringssjablonen gebruiken
description: Leer hoe je afleveringssjablonen maakt en gebruikt in Campaign Web
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
exl-id: cd3d4c2d-7bb2-4574-aeb8-6aac0683ec59
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '1053'
ht-degree: 2%

---

# Leveringssjablonen gebruiken {#work-with-delivery-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="Afleveringssjablonen"
>abstract="Voor een versneld en verbeterd ontwerpproces kunt u leveringssjablonen maken om aangepaste inhoud en instellingen in al uw campagnes eenvoudig te hergebruiken. Met deze functionaliteit kunt u de creatieve vormgeving standaardiseren, zodat u sneller campagnes kunt uitvoeren en lanceren."

Voor een versneld en verbeterd ontwerpproces, kun je leveringssjablonen maken om eenvoudig aangepaste content en instellingen te hergebruiken in al je campagnes. Met deze functionaliteit kunt u de creatieve vormgeving standaardiseren, zodat u sneller campagnes kunt uitvoeren en lanceren.

Een sjabloon kan het volgende bevatten:

* De **omslag** en **uitvoeringsomslag** van het malplaatje. De map is de locatie waar de leveringssjabloon wordt opgeslagen. De uitvoeringsmap is de map waarin op basis van deze sjabloon gemaakte leveringen worden opgeslagen.
* [ Typologies ](../advanced-settings/delivery-settings.md#typology),
* Het adres van de afzender,
* Een [ publiek ](../audience/about-recipients.md), met inbegrip van [ controlegroepen ](../audience/control-group.md),
* Aangepaste [ inhoud ](../email/edit-content.md),
* [ Gepersonaliseerde gebieden ](../personalization/personalize.md) en [ voorwaardelijke inhoud ](../personalization/conditions.md),
* Verbindingen met [ spiegelpagina ](../email/mirror-page.md) en unsubscription [ verbindingen ](../email/message-tracking.md),
* Andere leveringseigenschappen, zoals middelgeldigheid, retry parameters, of quarantaine montages.

>[!NOTE]
>
>De malplaatjes van de levering zijn verschillend van [ inhoudsmalplaatjes ](../email/create-email-templates.md), die u toestaan slechts de inhoud van uw e-mail opnieuw te gebruiken en te beginnen inhoud met één van de steekproef e-mailmalplaatjes te bouwen die uit-van-de-doos worden verstrekt.


## Leveringssjablonen openen en beheren {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="Werken met leveringssjablonen"
>abstract="Gebruik leveringssjablonen om leveringsinstellingen te maken en op te slaan voor toekomstig gebruik in uw campagnes. U kunt leveringsmalplaatjes van kras tot stand brengen, een bestaand malplaatje dupliceren, of een levering in een malplaatje omzetten."


Om tot de lijst van het inhoudsmalplaatje toegang te hebben, selecteer **[!UICONTROL Campaign Management]** > **[!UICONTROL Deliveries]** van het linkermenu, en doorblader aan de **Malplaatjes** tabel.

![](assets/templates-tab.png){zoomable="yes"}

Alle malplaatjes die [ werden gecreeerd ](#create-a-delivery-template) op het huidige milieu worden getoond.

U kunt inhoudssjablonen filteren op kanalen en mappen. U kunt geavanceerde filters ook instellen door een regel te maken met behulp van leveringskenmerken. [ Leer meer op de vraagmodelaar ](../audience/../query/query-modeler-overview.md)

![](assets/templates-filters.png){zoomable="yes"}

Als u een sjabloon wilt bewerken, klikt u op het gewenste item in de lijst. Hierna:

* U kunt de inhoud, eigenschappen, het publiek en alle aanbiedingen die eraan zijn gekoppeld, wijzigen.
* U kunt de sjabloon ook testen. [Meer informatie](#test-template)

![](assets/templates-edition.png){zoomable="yes"}

Om [ te schrappen of te dupliceren ](#copy-an-existing-template) een malplaatje, selecteer de overeenkomstige actie van het **[!UICONTROL More actions]** menu, of van de **[!UICONTROL Templates]** lijst of van het scherm van de malplaatjeuitgave.

![](assets/templates-more-actions.png){zoomable="yes"}

>[!NOTE]
>
>Wanneer een sjabloon wordt bewerkt of verwijderd, hebben leveringen die met deze sjabloon zijn gemaakt, geen invloed op deze sjabloon.

## Een leveringssjabloon maken {#create-a-delivery-template}

Als u een leveringssjabloon wilt maken, kunt u:

* Dupliceer een bestaand malplaatje - [ Leer meer ](#copy-an-existing-template)
* Zet een bestaande levering in een malplaatje om - [ leer meer ](#convert-an-existing-delivery)
* Creeer een leveringsmalplaatje van kras - [ Leer meer ](#create-a-new-template)

### Een bestaande leveringssjabloon dupliceren {#copy-an-existing-template}

De campagne wordt geleverd met een reeks ingebouwde sjablonen voor elk kanaal: e-mail, push, SMS. De gemakkelijkste manier om een leveringsmalplaatje tot stand te brengen is een ingebouwde malplaatje te dupliceren en aan te passen.

>[!NOTE]
>
>U kunt ook elke aangepaste sjabloon dupliceren.

Voer de onderstaande stappen uit om een leveringssjabloon te dupliceren:

1. Blader naar het **lusje van Malplaatjes**, van het **Levert** linkermenu. [Meer informatie](#access-manage-templates)
1. Klik op **[!UICONTROL More actions]** rechts van de gewenste sjabloonnaam en selecteer **[!UICONTROL Duplicate]** .

   U kunt ook een sjabloon in de lijst selecteren en deze optie selecteren in het scherm Sjablooneditie.

1. Herhaal duplicatie.

   ![](assets/templates-duplicate-confirm.png){zoomable="yes"}

1. Het nieuwe sjabloondashboard wordt in het centrale scherm geopend. Bewerk indien nodig de sjablooninstellingen.

   ![](assets/templates-duplicated-item.png){zoomable="yes"}

1. Klik op de knop **[!UICONTROL Review]** om uw sjabloon op te slaan en te bekijken. U kunt nog steeds alle instellingen bewerken, verwijderen en dupliceren.

   ![](assets/templates-review-screen.png){zoomable="yes"}

1. Test indien nodig de rendering van de sjabloon. [Meer informatie](#test-template)

Het nieuwe malplaatje wordt toegevoegd aan de [**lijst van Malplaatjes** ](#access-manage-templates). U kunt deze nu selecteren wanneer u een nieuwe levering maakt.

### Een levering converteren naar een sjabloon {#convert-an-existing-delivery}

Elke levering kan worden omgezet in een sjabloon voor toekomstige herhaalde leveringsacties.

Volg onderstaande stappen om een levering als een sjabloon op te slaan:

1. Blader naar het menu **[!UICONTROL Campaign management]** > **[!UICONTROL Deliveries]** .
1. Klik op het tabblad **[!UICONTROL Browse]** op de knop **[!UICONTROL More actions]** rechts van de gewenste leveringsnaam en selecteer **[!UICONTROL Copy as a template]** .

   ![](assets/templates-convert-delivery.png){zoomable="yes"}

   U kunt ook een sjabloon selecteren in de lijst en deze optie selecteren in het scherm Sjablooneditie.

1. Herhaal dit.

1. Het nieuwe sjabloondashboard wordt in het centrale scherm geopend. Bewerk de sjablooninstellingen naar wens.

1. Klik op de knop **[!UICONTROL Review]** om uw sjabloon op te slaan en te bekijken. U kunt nog steeds alle instellingen bewerken, verwijderen en dupliceren.

1. Test indien nodig de rendering van de sjabloon. [Meer informatie](#test-template)

Het nieuwe malplaatje wordt toegevoegd aan de [**lijst van Malplaatjes** ](#access-manage-templates). U kunt deze nu selecteren wanneer u een nieuwe levering maakt.

### Een nieuwe leveringssjabloon maken {#create-a-new-template}

>[!NOTE]
>
>Om configuratiefouten te vermijden, adviseert de Adobe dat u [ een ingebouwd malplaatje ](#copy-an-existing-template) dupliceert en zijn eigenschappen eerder dan tot een nieuw malplaatje leidt.

Volg onderstaande stappen om een leveringssjabloon helemaal zelf te configureren:

1. Blader naar het **lusje van Malplaatjes**, van **levert** linkermenu. [Meer informatie](#access-manage-templates)
1. Klik op de knop **[!UICONTROL Create template]**.

   ![](assets/templates-create-button.png){zoomable="yes"}

1. Selecteer het kanaal dat u voor uw sjabloon wilt gebruiken.
1. De ingebouwde leveringsmalplaatje voor dat kanaal wordt gebruikt door gebrek om u te helpen uw eigen malplaatje bouwen. Gebruik de toegewezen knop rechts van het geselecteerde kanaal om indien nodig een andere sjabloon te selecteren.

   ![](assets/templates-channel-browse.png){zoomable="yes"}

1. Klik nogmaals op de knop **[!UICONTROL Create template]** .

1. Bepaal de malplaatjeeigenschappen, [ publiek ](../audience/add-audience.md) en inhoud afhankelijk van het geselecteerde kanaal.

   >[!NOTE]
   >
   >Meer informatie over leveringskanalen en het ontwerpen van de inhoud in de volgende secties vindt u:
   >
   > * [E-mailkanaal](../email/create-email.md)
   > * [ het berichtkanaal van de duw ](../push/gs-push.md)
   > * [Sms-kanaal](../sms/create-sms.md)

1. Voor e-mailsjablonen kunt u bovendien geavanceerde instellingen, zoals typologische regels en doeltoewijzingen, gebruiken via de knop **[!UICONTROL Settings]** rechtsboven in het scherm. [Meer informatie](../advanced-settings/delivery-settings.md)

1. Klik op de knop **[!UICONTROL Review]** om de sjabloon op te slaan en te bekijken. U kunt nog steeds alle instellingen bewerken, verwijderen en dupliceren.

1. Test indien nodig de rendering van de sjabloon. [Meer informatie](#test-template)

Het nieuwe malplaatje wordt toegevoegd aan de [**lijst van Malplaatjes** ](#access-manage-templates). U kunt deze nu selecteren wanneer u een nieuwe levering maakt.

## Een leveringssjabloon testen {#test-template}

U kunt de rendering van elke leveringssjabloon testen, ongeacht of deze van nul is gemaakt of van bestaande inhoud. Volg de onderstaande stappen om dit te doen.

1. Blader naar het **lusje van Malplaatjes** door **[!UICONTROL Campaign management]** > **[!UICONTROL Deliveries]** menu en selecteer om het even welk malplaatje. [Meer informatie](#access-manage-templates)

1. Klik op de knop **[!UICONTROL Simulate content]** rechtsboven in het scherm.

   ![](assets/templates-simulate-button.png){zoomable="yes"}

1. Selecteer een of meer testprofielen om de weergave van uw e-mail te controleren. U kunt ook echte profielen selecteren in uw database. [ leer meer op testprofielen ](../audience/test-profiles.md)

1. Schakel tussen de verschillende profielen om een persoonlijke weergave van het bericht te krijgen op basis van het geselecteerde profiel. U kunt ook het zoomniveau aanpassen en de weergave voor bureaublad of mobiel kiezen.

[Meer informatie over het voorvertonen van inhoud](../preview-test/preview-content.md)

   ![](assets/templates-stimulate.png){zoomable="yes"}

1. Sluit het venster om terug te keren naar het scherm van de malplaatjeuitgave.

>[!NOTE]
>
>U kunt geen rendering via e-mail gebruiken of proefdrukken verzenden in een leveringssjabloon.


