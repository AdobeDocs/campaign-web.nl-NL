---
audience: end-user
title: Middelen beheren met Adobe Experience Manager as a Cloud Service
description: Leer hoe u inhoud beheert met Adobe Experience Manager as a Cloud Service
exl-id: 43b186c8-294e-4cbe-b269-e127065515ed
source-git-commit: d58b9e9b32b85acfbd58dfcbef2000f859feb40d
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 1%

---

# Sjablonen beheren met [!DNL Adobe Experience Manager as a Cloud Service]{#aem-assets}

## Aan de slag met [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem}

Dankzij de integratie van de Adobe Campaign Web-interface met Adobe Experience Manager kunt u inhoud en formulieren voor e-mailbezorging direct binnen het Adobe Experience Manager-platform beheren.

![](assets/do-not-localize/book.png)[ leer meer over Adobe Experience Manager as a Cloud Service ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/sites/authoring/getting-started/quick-start.html?lang=en)

## Een sjabloon maken in [!DNL Adobe Experience Manager as a Cloud Service]{#create-aem-template}

1. Navigeer naar de auteurinstantie van [!DNL Adobe Experience Manager] en klik op Adobe Experience in de linkerbovenhoek van de pagina. Kies **[!UICONTROL Sites]** in het menu.

1. Toegang **[!UICONTROL Campaigns > Name of your brand > Main Area > Name of your page]**.

1. Klik op **[!UICONTROL Create]** en selecteer **[!UICONTROL Page]** in het vervolgkeuzemenu.

   ![ Schermschot die de &quot;Create&quot;knoop en &quot;Pagina&quot;optie in het dropdown menu tonen.](assets/aem_1.png)

1. Selecteer de sjabloon **[!UICONTROL Adobe Campaign Email]** en geef de nieuwsbrief een naam.

   ![[ het Schermafbeelding die het &quot;E-mail van Adobe Campaign&quot;malplaatjeselectie en het noemen gebied tonen.]](assets/aem_2.png)

1. Pas uw e-mailinhoud aan door componenten toe te voegen, zoals personalisatievelden van Adobe Campaign. [Meer informatie](https://experienceleague.adobe.com/docs/experience-manager-65/content/sites/authoring/aem-adobe-campaign/campaign.html?lang=en#editing-email-content)

1. Wanneer uw e-mail gereed is, navigeert u naar het menu **[!UICONTROL Page information]** en klikt u op **[!UICONTROL Start workflow]** .

   ![ het Schermafbeelding die het menu van de &quot;Informatie van de Pagina&quot;en de optie van het &quot;werkschema van het Begin&quot;toont.](assets/aem_3.png)

1. Selecteer in het eerste vervolgkeuzemenu **[!UICONTROL Approve Adobe Campaign]** als het workflowmodel en klik op **[!UICONTROL Start workflow]** .

1. Boven aan de pagina wordt een disclaimer weergegeven met de tekst `This page is subject to the workflow Approve for Adobe Campaign` . Klik op **[!UICONTROL Complete]** naast de disclaimer om de revisie te bevestigen en klik op **[!UICONTROL Ok]** .

   ![ Scherenshot die de ontkenning en &quot;Volledige&quot;knoop tonen.](assets/aem_4.png)

1. Klik nogmaals op **[!UICONTROL Complete]** en selecteer **[!UICONTROL Newsletter approval]** in de vervolgkeuzelijst **[!UICONTROL Next Step]** .

Uw nieuwsbrief is nu klaar en gesynchroniseerd in Adobe Campaign.

## Een Adobe Experience Manager as a Cloud Service-sjabloon importeren{#aem-templates-perso}

Zodra het malplaatje van Experience Manager in het Web van Adobe Campaign als inhoudsmalplaatje beschikbaar is, kunt u de noodzakelijke inhoud voor e-mail identificeren en opnemen, met inbegrip van verpersoonlijking.

1. Klik in het menu **[!UICONTROL Deliveries]** van Campagne Web op **[!UICONTROL Create delivery]** .

1. Selecteer de ingebouwde sjabloon **[!UICONTROL Email delivery with AEM content]** in het venster E-mailsjabloon.

   ![ Screenshot die de &quot;E-maillevering met de inhoud van AEM&quot;malplaatjeselectie toont.](assets/aem_5.png)

1. Voer een **[!UICONTROL Label]** in voor de levering en configureer aanvullende opties op basis van uw behoeften:

   * **[!UICONTROL Internal name]**: wijs een unieke id toe aan de levering.
   * **[!UICONTROL Folder]**: Sla de levering op in een specifieke map.
   * **[!UICONTROL Delivery code]**: gebruik dit veld om uw leveringen te ordenen op basis van uw eigen naamgevingsconventie.
   * **[!UICONTROL Description]**: geef een beschrijving op voor de levering.
   * **[!UICONTROL Nature]**: geef de aard van de e-mail op voor classificatiedoeleinden.

1. Definieer een **[!UICONTROL Audience]** voor uw e-mail. [Meer informatie](../email/create-email.md#define-audience)

1. Klik op **[!UICONTROL Edit content]**.

1. Klik in het menu **[!UICONTROL Edit content]** op **[!UICONTROL Select AEM content]** .

   ![ Schermafbeelding die de optie &quot;AEM-inhoud selecteren&quot; in het menu &quot;Inhoud bewerken&quot; weergeeft.](assets/aem_6.png)

1. Blader door de AEM-sjabloon en selecteer de sjabloon die u wilt importeren in Campagne Web.

   ![ Screenshot die de interface van de het malplaatjeselectie van AEM toont.](assets/aem_8.png)

1. Inhoud wordt niet automatisch gesynchroniseerd. Als er direct in Adobe Experience Manager wijzigingen in uw sjablonen worden aangebracht, selecteert u **[!UICONTROL Refresh AEM content]** om bij te werken naar de meest recente versie van uw sjabloon.

1. Als u de koppeling tussen Experience Manager en Campagne wilt verwijderen of de Experience Manager-sjabloon in de e-mailontwerper verder wilt aanpassen, klikt u op **[!UICONTROL Unlink AEM content]** .

   ![ Schermafbeelding die de optie &quot;AEM-inhoud ontkoppelen&quot; weergeeft.](assets/aem_9.png)

1. Als u persoonlijke inhoud hebt toegevoegd aan uw Experience Manager-sjabloon, klikt u op **[!UICONTROL Simulate Content]** om een voorvertoning weer te geven van de inhoud die in het bericht wordt weergegeven met testprofielen.

[Meer informatie over voorvertoningen en testprofielen](../preview-test/preview-content.md)

1. Wanneer u de voorvertoning van het bericht weergeeft, worden alle gepersonaliseerde elementen automatisch vervangen door de bijbehorende gegevens uit het geselecteerde testprofiel.

   Voeg zo nodig aanvullende testprofielen toe via de knop **[!UICONTROL Manage test profiles]** .

Je levering is nu klaar om te worden verzonden.