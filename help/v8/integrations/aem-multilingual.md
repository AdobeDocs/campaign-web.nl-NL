---
audience: end-user
title: Meertalige e-mails maken met Adobe Experience Manager
description: Leer hoe u meertalige e-mailleveringen maakt met Adobe Experience Manager-taalkopieën in Campagne Web.
feature: Email
topic: Content Management
role: User
level: Intermediate
exl-id: 6fc6ff43-ac7f-46c7-aa1a-9489ffc45423
source-git-commit: bc43288d58145aa28e914f7a9480cb9ab90f5a54
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 1%

---

# Meertalige e-mails maken met Adobe Experience Manager {#aem-multilingual}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn3"
>title="Experience Manager-kopieën voor levende en talen"
>abstract="U hebt nu rechtstreeks toegang tot de Adobe Experience Manager-taal en live kopieën in Campagne. Inhoud in realtime vernieuwen voorkomt handmatige synchronisatie voor gestroomlijnde workflows in meerdere talen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=nl-NL" text="Zie opmerkingen bij releases"

Dankzij de Adobe Experience Manager-integratie kunt u meertalige e-mailleveringen maken met Adobe Experience Manager-taalkopieën. Zo kunt u varianten in de inhoud van verschillende talen beheren en persoonlijke e-mails aanbieden op basis van de taalvoorkeuren van de ontvanger.

## Vereisten {#prerequisites}

Voordat u een meertalige e-maillevering maakt, moet u controleren of u beschikt over:

* Toegang tot een Adobe Experience Manager-instantie die is geconfigureerd voor de integratie van de Adobe Campaign-webinterface.
* Adobe Experience Manager-inhoud met reeds gemaakte en goedgekeurde taalkopieën. Leer meer over de Tovenaar van het Exemplaar van de Taal in [&#x200B; documentatie van Adobe Experience Manager &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/sites/administering/reusing-content/translation/wizard)
* Sjabloon voor e-maillevering geconfigureerd voor ontvangst van Adobe Experience Manager-inhoud. Verwijs naar de stappen die in [&#x200B; worden gedetailleerd toelaten meertalige wijze &#x200B;](#enable-multilingual) sectie.

## Maak uw meertalige levering

Als u een meertalige e-maillevering wilt maken, moet u eerst de meertalige optie inschakelen in de leveringsinstellingen. Het systeem detecteert automatisch beschikbare taalkopieën en geeft aan welke er moeten worden toegevoegd.

### Meertalige modus inschakelen {#enable-multilingual}

Maak een nieuwe levering en schakel de meertalige optie in de geavanceerde instellingen in.

1. Klik in het menu **[!UICONTROL Deliveries]** op **[!UICONTROL Create delivery]** .

   ![](assets/lg-copy-1.png)

1. Selecteer de sjabloon **[!UICONTROL Email delivery with AEM content]** en klik op **[!UICONTROL Create delivery]** .

   ![](assets/lg-copy-2.png)

1. Ga een etiket voor de levering in en vorm uw publiek. [Meer informatie](../email/create-email.md)

1. Open de levering **[!UICONTROL Settings]** en navigeer naar de sectie **[!UICONTROL Advanced]** .

1. Schakel de optie **[!UICONTROL Enable AEM multilingual]** in.

   ![](assets/lg-copy-3.png)

1. Controleer of:

   * **[!UICONTROL Content editing mode]** wordt ingesteld op **[!UICONTROL AEM]** .
   * De juiste Adobe Experience Manager **[!UICONTROL External account]** is geselecteerd.

1. Klik op **[!UICONTROL Save and close]**.

### Inhoudsvarianten maken {#create-variants}

Selecteer de Adobe Experience Manager-inhoud en kies welke taalvarianten u wilt opnemen in de levering.

1. Klik op **[!UICONTROL Edit content]**.

1. Selecteer **[!UICONTROL Create content variant]**.

   ![](assets/lg-copy-4.png)

1. Selecteer de Adobe Experience Manager-inhoud in de lijst.

   ![](assets/lg-copy-5.png)

1. Het systeem detecteert alle taalkopieën die aan de geselecteerde inhoud zijn gekoppeld (relatie bovenliggend-onderliggend). Als de Adobe Experience Manager-inhoud bijvoorbeeld varianten in het Frans, Duits en Italiaans heeft, zijn alle varianten beschikbaar voor selectie.

   Selecteer de taalvarianten u in uw levering wilt omvatten.

   ![](assets/lg-copy-6.png)

1. Klik op **[!UICONTROL Save]**.

1. Bekijk de taalvarianten in de inhoudseditor. U kunt nu [&#x200B; elke variant individueel &#x200B;](#manage-variants) beheren of met [&#x200B; te werk gaan verzendend de levering &#x200B;](../monitor/prepare-send.md).

   ![](assets/lg-copy-7.png)

## Taalvarianten beheren {#manage-variants}

Nadat u inhoudsvarianten hebt gemaakt, kunt u deze rechtstreeks in de levering beheren:

1. Als u een standaardtaal wilt instellen, opent u het geavanceerde menu voor de gekozen variant en selecteert u **[!UICONTROL Set as default]** . De standaardtaal wordt gebruikt wanneer de taalvoorkeur van een profiel niet wordt geplaatst of geen beschikbare variant aanpast.

   Klik op **[!UICONTROL Delete]** om een willekeurige variant uit de levering te verwijderen.

   ![](assets/lg-copy-8.png)

1. Klik in het menu Geavanceerde inhoudvarianten op **[!UICONTROL Manage locales]** om andere landinstellingen aan uw levering toe te voegen.

   ![](assets/lg-copy-9.png)

1. Selecteer extra taalkopieën als u meer varianten wilt opnemen en klik op **[!UICONTROL Save]** .

   ![](assets/lg-copy-11.png)

1. Als de inhoud in Adobe Experience Manager wordt bijgewerkt, klikt u op **[!UICONTROL Refresh AEM content]** om alle varianten te synchroniseren met de meest recente versie.

   ![](assets/lg-copy-10.png)

1. Klik op **[!UICONTROL Unlink AEM content]** als u inhoud rechtstreeks in Campagne wilt bewerken of de koppeling met Adobe Experience Manager wilt verbreken.

   >[!CAUTION]
   >
   >Na het ontkoppelen kunt u de inhoud van Adobe Experience Manager niet vernieuwen of nieuwe varianten maken. De inhoud wordt onafhankelijk van Adobe Experience Manager.
