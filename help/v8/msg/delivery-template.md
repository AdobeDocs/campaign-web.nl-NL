---
product: campaign
title: Leveringssjablonen gebruiken
description: Leer hoe te om leveringsmalplaatjes in het Web van de Campagne te creëren en te gebruiken
feature: Email, Push, SMS, Direct Mail, Cross Channel Orchestration
role: User
level: Beginner
badge: label="Beperkte beschikbaarheid"
exl-id: cd3d4c2d-7bb2-4574-aeb8-6aac0683ec59
source-git-commit: f8f29849bbd3e97b4168a0bac175a3cdc3e651df
workflow-type: tm+mt
source-wordcount: '1055'
ht-degree: 2%

---

# Leveringssjablonen gebruiken {#work-with-delivery-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_for_campaign"
>title="Afleveringssjablonen"
>abstract="Voor een versneld en verbeterd ontwerpproces kunt u leveringssjablonen maken om aangepaste inhoud en instellingen in al uw campagnes eenvoudig te hergebruiken. Met deze functie kunt u de creatieve vormgeving standaardiseren, zodat u sneller campagnes kunt uitvoeren en lanceren."

Voor een versneld en verbeterd ontwerpproces kunt u leveringssjablonen maken om aangepaste inhoud en instellingen in al uw campagnes eenvoudig te hergebruiken. Met deze functie kunt u de creatieve vormgeving standaardiseren, zodat u sneller campagnes kunt uitvoeren en lanceren.

Een sjabloon kan het volgende bevatten:

* De **map** en **uitvoeringsmap** van de template. De map is de locatie waar de leveringssjabloon is opgeslagen. De uitvoeringsmap is de map waarin leveringen worden opgeslagen die op basis van deze sjabloon zijn gemaakt.
* [Typologieën](../advanced-settings/delivery-settings.md#typology),
* Het adres van de afzender,
* An [publiek](../audience/about-recipients.md), inclusief [controlegroepen](../audience/control-group.md),
* Aangepast [content](../email/edit-content.md),
* [Persoonlijke velden](../personalization/personalize.md) en [voorwaardelijke inhoud](../personalization/conditions.md),
* Koppelingen naar [spiegelpagina](../email/mirror-page.md) en uit-abonnement [koppelingen](../email/message-tracking.md),
* Andere leveringseigenschappen, zoals middelgeldigheid, retry parameters, of quarantaine montages.

>[!NOTE]
>
>Afleveringssjablonen verschillen van [inhoudssjablonen](../email/create-email-templates.md), waarmee u alleen de inhoud van uw e-mails kunt hergebruiken en inhoud kunt gaan samenstellen met een van de voorbeeldsjablonen die u offline hebt ontvangen.


## Leveringssjablonen openen en beheren {#access-manage-templates}

>[!CONTEXTUALHELP]
>id="acw_delivery_templates"
>title="Werken met leveringssjablonen"
>abstract="Gebruik leveringssjablonen om leveringsinstellingen te maken en op te slaan voor toekomstig gebruik in uw campagnes. U kunt leveringsmalplaatjes van kras tot stand brengen, een bestaand malplaatje dupliceren, of een levering in een malplaatje omzetten."


Als u de lijst met inhoudssjablonen wilt openen, selecteert u **[!UICONTROL Campaign Management]** > **[!UICONTROL Deliveries]** van het linkermenu, en doorblader aan **Sjablonen** tab.

![](assets/templates-tab.png)

Alle sjablonen die [gemaakt](#create-a-delivery-template) op de huidige omgeving worden weergegeven.

U kunt inhoudssjablonen filteren op kanalen en mappen. U kunt geavanceerde filters ook instellen door een regel te maken met behulp van leveringskenmerken. [Meer informatie over querymodellen](../audience/../query/query-modeler-overview.md)

![](assets/templates-filters.png)

Als u een sjabloon wilt bewerken, klikt u op het gewenste item in de lijst. Hierna:

* U kunt de inhoud, eigenschappen, het publiek en alle aanbiedingen die eraan zijn gekoppeld, wijzigen.
* U kunt de sjabloon ook testen. [Meer informatie](#test-template)

![](assets/templates-edition.png)

Om te schrappen of [dupliceren](#copy-an-existing-template) een sjabloon, selecteert u de bijbehorende actie in het menu **[!UICONTROL More actions]** in het menu **[!UICONTROL Templates]** lijst of van een scherm van de malplaatjeuitgave.

![](assets/templates-more-actions.png)

>[!NOTE]
>
>Wanneer een sjabloon wordt bewerkt of verwijderd, hebben leveringen die met deze sjabloon zijn gemaakt, geen invloed op deze sjabloon.

## Een leveringssjabloon maken {#create-a-delivery-template}

Als u een leveringssjabloon wilt maken, kunt u:

* Een bestaande sjabloon dupliceren - [Meer informatie](#copy-an-existing-template)
* Een bestaande levering converteren naar een sjabloon - [Meer informatie](#convert-an-existing-delivery)
* Een volledig nieuwe leveringssjabloon maken - [Meer informatie](#create-a-new-template)

### Een bestaande leveringssjabloon dupliceren {#copy-an-existing-template}

De campagne wordt geleverd met een reeks ingebouwde sjablonen voor elk kanaal: e-mail, push, SMS. De gemakkelijkste manier om een leveringsmalplaatje tot stand te brengen is een ingebouwde malplaatje te dupliceren en aan te passen.

>[!NOTE]
>
>U kunt ook elke aangepaste sjabloon dupliceren.

Voer de onderstaande stappen uit om een leveringssjabloon te dupliceren:

1. Bladeren naar de **Sjablonen** tabblad, van de **Leveringen** links. [Meer informatie](#access-manage-templates)
1. Klik op de knop **[!UICONTROL More actions]** rechts van de gewenste sjabloonnaam en selecteert u  **[!UICONTROL Duplicate]**.

   U kunt ook een sjabloon selecteren in de lijst en deze optie selecteren in het scherm Sjablooneditie.

1. Herhaal dit.

   ![](assets/templates-duplicate-confirm.png)

1. Het nieuwe sjabloondashboard wordt in het centrale scherm geopend. Bewerk de sjablooninstellingen naar wens.

   ![](assets/templates-duplicated-item.png)

1. Klik op de knop **[!UICONTROL Review]** om de sjabloon op te slaan en te bekijken. U kunt nog steeds alle instellingen bewerken, verwijderen en dupliceren.

   ![](assets/templates-review-screen.png)

1. Test indien nodig de rendering van de sjabloon. [Meer informatie](#test-template)

De nieuwe sjabloon wordt toegevoegd aan de [**Sjablonen** list](#access-manage-templates). U kunt deze nu selecteren wanneer u een nieuwe levering maakt.

### Een levering converteren naar een sjabloon {#convert-an-existing-delivery}

Elke levering kan worden omgezet in een sjabloon voor toekomstige herhaalde leveringsacties.

Volg onderstaande stappen om een levering als een sjabloon op te slaan:

1. Bladeren naar de **[!UICONTROL Campaign management]** > **[!UICONTROL Deliveries]** -menu.
1. Van de **[!UICONTROL Browse]** klikt u op de knop **[!UICONTROL More actions]** rechts van de gewenste levernaam en selecteert u **[!UICONTROL Copy as a template]**.

   ![](assets/templates-convert-delivery.png)

   U kunt ook een sjabloon selecteren in de lijst en deze optie selecteren in het scherm Sjablooneditie.

1. Herhaal dit.

1. Het nieuwe sjabloondashboard wordt in het centrale scherm geopend. Bewerk de sjablooninstellingen naar wens.

1. Klik op de knop **[!UICONTROL Review]** om de sjabloon op te slaan en te bekijken. U kunt nog steeds alle instellingen bewerken, verwijderen en dupliceren.

1. Test indien nodig de rendering van de sjabloon. [Meer informatie](#test-template)

De nieuwe sjabloon wordt toegevoegd aan de [**Sjablonen** list](#access-manage-templates). U kunt deze nu selecteren wanneer u een nieuwe levering maakt.

### Een nieuwe leveringssjabloon maken {#create-a-new-template}

>[!NOTE]
>
>Om configuratiefouten te vermijden, adviseert de Adobe dat u [een ingebouwde sjabloon dupliceren](#copy-an-existing-template) en pas de eigenschappen aan in plaats van een nieuwe sjabloon te maken.

Voer de onderstaande stappen uit om een volledig nieuwe leveringssjabloon te configureren:

1. Bladeren naar de **Sjablonen** tabblad, van de **Leveringen** links. [Meer informatie](#access-manage-templates)
1. Klik op de knop **[!UICONTROL Create template]**.

   ![](assets/templates-create-button.png)

1. Selecteer het kanaal dat u voor uw sjabloon wilt gebruiken.
1. De ingebouwde leveringsmalplaatje voor dat kanaal wordt gebruikt door gebrek om u te helpen uw eigen malplaatje bouwen. Gebruik de toegewezen knop rechts van het geselecteerde kanaal om indien nodig een andere sjabloon te selecteren.

   ![](assets/templates-channel-browse.png)

1. Klik op de knop **[!UICONTROL Create template]** nogmaals.

1. Definieer de sjablooneigenschappen. [publiek](../audience/add-audience.md) en inhoud, afhankelijk van het geselecteerde kanaal.

   >[!NOTE]
   >
   >Meer informatie over leveringskanalen en het ontwerpen van de inhoud in de volgende secties vindt u:
   >
   > * [E-mailkanaal](../email/create-email.md)
   > * [Push-meldingskanaal](../push/gs-push.md)
   > * [Sms-kanaal](../sms/create-sms.md)

1. Voor e-mailsjablonen kunt u bovendien geavanceerde instellingen, zoals typologische regels en doeltoewijzingen, gebruiken via de **[!UICONTROL Settings]** op de knop rechtsboven in het scherm. [Meer informatie](../advanced-settings/delivery-settings.md)

1. Klik op de knop **[!UICONTROL Review]** om de sjabloon op te slaan en te bekijken. U kunt nog steeds alle instellingen bewerken, verwijderen en dupliceren.

1. Test indien nodig de rendering van de sjabloon. [Meer informatie](#test-template)

De nieuwe sjabloon wordt toegevoegd aan de [**Sjablonen** list](#access-manage-templates). U kunt deze nu selecteren wanneer u een nieuwe levering maakt.

## Een leveringssjabloon testen {#test-template}

U kunt de rendering van elke leveringssjabloon testen, ongeacht of deze van nul is gemaakt of van bestaande inhoud. Volg de onderstaande stappen om dit te doen.

1. Bladeren naar de **Sjablonen** door de **[!UICONTROL Campaign management]** > **[!UICONTROL Deliveries]** en selecteert u een sjabloon. [Meer informatie](#access-manage-templates)

1. Klik op de knop **[!UICONTROL Simulate content]** op de rechterbovenhoek van het scherm.

   ![](assets/templates-simulate-button.png)

1. Selecteer een of meer testprofielen om de weergave van uw e-mail te controleren. U kunt ook echte profielen selecteren in uw database. [Meer informatie over testprofielen](../audience/test-profiles.md)

1. Schakel tussen de verschillende profielen om een persoonlijke weergave van het bericht te krijgen op basis van het geselecteerde profiel. U kunt ook het zoomniveau aanpassen en de weergave voor bureaublad of mobiel kiezen.

[Meer informatie over het voorvertonen van inhoud](../preview-test/preview-content.md)

   ![](assets/templates-stimulate.png)

1. Sluit het venster om terug te keren naar het scherm van de malplaatjeuitgave.

>[!NOTE]
>
>U kunt geen e-mailrendering gebruiken of tests verzenden in een leveringssjabloon.


