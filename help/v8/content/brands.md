---
audience: end-user
title: Merk beheren
description: Leer hoe u richtlijnen voor uw merk kunt maken en beheren
exl-id: d4d2c6bb-7fd0-49a0-9d73-356f4a24f021
source-git-commit: f238fde4a79d3303f2b5c9a2d26b11ffad8ac54e
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 1%

---

# Uw merken maken en beheren {#brands}

Merkrichtlijnen zijn een uitgebreide reeks regels en normen die de visuele en verbale identiteit van een merk definiëren. Zij dienen als referentie om te zorgen voor een consistente merkweergave op alle marketing- en communicatiekanalen.

In [!DNL Adobe Campaign Web] kunnen gebruikers handmatig merkgegevens invoeren en organiseren of documenten met brandrichtlijnen uploaden voor automatische gegevensextractie.

## Handelsmerken {#generative-access}

Als u het menu **[!UICONTROL Brands]** in [!DNL Adobe Campaign Web] wilt openen, moeten gebruikers de productprofielen **[!UICONTROL Administrator (admin)]** en **[!UICONTROL Brand kit]** krijgen toegewezen om merken te maken en te beheren. Gebruikers hebben het productprofiel [!UICONTROL AI assistant] nodig voor alleen-lezen toegang. [Meer informatie](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/admin/permissions/manage-permissions)

+++ Leer hoe u merkgerelateerde machtigingen kunt toewijzen

1. In de [ Admin Console ](https://adminconsole.adobe.com/enterprise) homepage, heb toegang tot uw product van de Campagne.

   ![ Admin Console homepage die de producttoegang van de Campagne toont ](assets/brands_admin_1.png)

1. Selecteer **[!DNL Product profile]** op basis van het niveau van toestemmingen u uw gebruiker wilt verlenen.

   ![ de profielselectie van het Product in Admin Console ](assets/brands_admin_2.png)

1. Klik op **[!DNL Add users]** om het geselecteerde productprofiel toe te wijzen.

   ![ voegt gebruikersoptie in Admin Console ](assets/brands_admin_3.png) toe

1. Typ de naam, de gebruikersgroep of het e-mailadres van de gebruiker.

1. Klik **sparen** om veranderingen toe te passen.

De rechten van gebruikers die al zijn toegewezen aan deze rol, worden automatisch bijgewerkt.

+++

## Uw merk maken {#create-brand-kit}

Volg onderstaande stappen om uw richtlijnen voor uw merk te maken en te beheren.

Gebruikers kunnen de details handmatig invoeren of een document met brandrichtlijnen uploaden om de informatie automatisch te extraheren:

1. Klik in het menu **[!UICONTROL Brands]** op **[!UICONTROL Create brand]** .

   ![ het menu van Merken met Create merkoptie ](assets/brands-1.png)

1. Voer een **[!UICONTROL Name]** in voor uw merk.

1. Sleep of selecteer het bestand om de richtlijnen van uw merk te uploaden en automatisch relevante merkgegevens te extraheren. Klik op **[!UICONTROL Create brand]**.

   Het uitpakken van informatie begint nu. Het kan enkele minuten duren voordat de bewerking is voltooid.

   ![ uploadt van het dossier voor de extractie van merkrichtlijnen ](assets/brands-2.png)

1. Uw standaarden voor het maken van inhoud en visuele weergave worden nu automatisch ingevuld. Blader door de verschillende tabbladen om de informatie naar wens aan te passen. [Meer informatie](#personalize)

1. Vanuit het geavanceerde menu van elke sectie of categorie kunt u automatisch verwijzingen toevoegen om relevante merkgegevens te extraheren.

   Gebruik de opties **[!UICONTROL Clear section]** of **[!UICONTROL Clear category]** om bestaande inhoud te verwijderen.

   ![](assets/brands-15.png)

1. Als u de configuratie hebt voltooid, klikt u op **[!UICONTROL Save]** en vervolgens op **[!UICONTROL Publish]** om uw merkenhulplijn beschikbaar te maken in AI Assistant.

1. Klik op **[!UICONTROL Edit brand]** om wijzigingen aan te brengen in uw gepubliceerde merk.

   >[!NOTE]
   >
   >Er wordt dan een tijdelijke kopie gemaakt in de bewerkingsmodus, waarbij de live versie wordt vervangen nadat deze is gepubliceerd.

   ![ geef merkoptie in het menu van Merken uit ](assets/brands-8.png)

1. Open het geavanceerde menu op het dashboard van **[!UICONTROL Brands]** door op het pictogram ![](assets/do-not-localize/Smock_More_18_N.svg) te klikken op:

   * Merk weergeven
   * Bewerken
   * Markeren als standaardmerk
   * Dupliceren
   * Publiceren
   * Publiceren ongedaan maken
   * Verwijderen

   ![ Geavanceerde menuopties in het dashboard van Banden ](assets/brands-6.png)

De richtlijnen voor uw merk zijn nu beschikbaar in het keuzemenu **[!UICONTROL Brand]** in AI Assistant. Zo kan AI Assistant inhoud en elementen genereren die zijn uitgelijnd op uw specificaties. [ Leer meer over Medewerker AI ](../content/generative-gs.md)

U kunt ook de richtlijnen van uw merk gebruiken om de kwaliteit van uw inhoud en de uitlijning van uw merk te evalueren. [ leer meer over de bevestiging van de inhoudskwaliteit ](brands-score.md#validate-quality)

![ AI hulpmenu met Merk drop-down ](assets/brands_6.png)

### Een standaardmerk instellen {#default-brand}

U kunt een standaardmerk aanwijzen dat automatisch moet worden toegepast bij het genereren van inhoud en het berekenen van uitlijningsscores tijdens het maken van de campagne.

Als u een standaardmerk wilt instellen, gaat u naar het **[!UICONTROL Brands]** -dashboard. Open het geavanceerde menu door op het pictogram ![](assets/do-not-localize/Smock_More_18_N.svg) te klikken en **[!UICONTROL Mark as default brand]** te selecteren.

![ Geavanceerde menuopties in het dashboard van Banden ](assets/brands-6.png)

