---
audience: end-user
title: Aan de slag met aangepaste externe kanalen
description: Meer informatie over het maken en verzenden van aangepaste externe kanalen met Adobe Campaign Web
source-git-commit: 7438ce1805cde00cf5b76f05d72bd19d2ef2343a
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# Aan de slag met aangepaste externe kanalen {#gs-custom-channel}

U kunt, direct van het Web UI van Adobe Campaign, levering ordenen en uitvoeren die op de douanekranalen wordt gebaseerd die met derden worden geïntegreerd. Het maken van het aangepaste externe kanaal wordt uitgevoerd in de clientconsole.

U kunt externe leveringen van aangepaste kanalen configureren in workflows of als zelfstandige leveringen, uw publiek definiëren en aanpasbare exportbestanden genereren met alle benodigde contact- en personalisatiegegevens.

>[!NOTE]
>
>De rapportering is niet beschikbaar in UI van het Web voor de externe leveringen van het douanekanaal. U moet naar de clientconsole bladeren om rapporten te openen.

In de onderstaande stappen wordt de procedure voor een zelfstandige (one-shot) levering in detail beschreven. De meeste stappen zijn gelijkaardig om centrumleveringen te roepen. Voor meer details, verwijs naar deze [ pagina ](../call-center/create-call-center.md).

Ga als volgt te werk om een nieuwe, zelfstandige, externe levering te maken en te verzenden:

1. Creeer het douane externe kanaal, [ lees meer ](#create-channel)
1. Creeer de levering, [ lees meer ](#create-delivery)
1. Bepaal het publiek, [ lees meer ](#select-audience)
1. Bewerk de inhoud, [ lees meer ](#edit-content)
1. De voorproef en verzendt de levering, [ lees meer ](#preview-send)

## Het aangepaste externe kanaal maken{#create-channel}

Eerst, moet u het douane externe kanaal vormen. Hier volgen de belangrijkste stappen die moeten worden uitgevoerd in de clientconsole:

1. Vorm het schema om het nieuwe kanaal aan de lijst van beschikbare kanalen toe te voegen.
1. Creeer een nieuwe verpletterende externe rekening.
1. Creeer een nieuw leveringsmalplaatje verbonden aan het nieuwe kanaal.

Voor meer details, verwijs naar de [ documentatie van de Console van de Cliënt ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/custom-channel.html)

## De levering maken{#create-delivery}

Voer de volgende stappen uit om de levering te maken en de eigenschappen ervan te configureren:

1. Selecteer het menu **[!UICONTROL Deliveries]** en klik op de knop **[!UICONTROL Create delivery]** .

1. Kies het gewenste externe kanaal, selecteer de bijbehorende sjabloon en klik op **[!UICONTROL Create delivery]** om te bevestigen.

   ![ Schermafbeelding die de verwezenlijking van een douanelevering tonen ](assets/cus-create.png){zoomable="yes"}


1. Voer onder **[!UICONTROL Properties]** een **[!UICONTROL Label]** in voor de levering.

   ![ Screenshot die de eigenschappen configuratie voor een douanelevering tonen ](assets/cus-properties.png){zoomable="yes"}

Voor meer details bij leveringsverwezenlijking, verwijs naar het vraagcentrum [ documentatie ](../call-center/create-call-center.md#create-delivery).

## De doelgroep definiëren{#select-audience}

Nu moet u het publiek definiëren dat voor het extractiebestand wordt gebruikt.

1. Klik in de sectie **[!UICONTROL Audience]** van de leveringspagina op **[!UICONTROL Select audience]** .

1. Kies een bestaand publiek of maak een eigen publiek.

   ![ Schermschot die publieksselectie voor een douanelevering tonen ](assets/cc-audience2.png){zoomable="yes"}

Voor meer details op publieksdefinitie, verwijs naar het vraagcentrum [ documentatie ](../call-center/create-call-center.md#select-audience).

## De inhoud bewerken{#edit-content}

Nu, geven wij de inhoud van het extractiedossier uit dat door de levering van het douanekanaal zal worden geproduceerd.

1. Klik op de knop **[!UICONTROL Edit content]** vanaf de leveringspagina.

1. Geef een **[!UICONTROL File name]** op, selecteer een **[!UICONTROL File format]** en voeg zoveel kolommen toe als nodig zijn voor het extractiebestand.

   ![ Screenshot die de opties van de attributenconfiguratie voor het extractiedossier toont.](assets/cc-content-attributes.png)

Voor meer details op inhoudsuitgave, verwijs naar het callcenter [ documentatie ](../call-center/create-call-center.md#edit-content).

## De levering voorvertonen en verzenden{#preview-send}

Als de inhoud klaar is voor levering, kunt u een voorvertoning weergeven met testprofielen en proefdrukken verzenden. Vervolgens kunt u de levering verzenden om het extractiebestand te genereren.

1. Klik op de pagina met inhoud voor levering op de knop **[!UICONTROL Simulate content]** en selecteer testprofielen.

   ![ Schermafbeelding die de simulatie inhoudsoptie in de pagina van de leveringsinhoud tonen ](assets/cus-simulate.png){zoomable="yes"}

1. Klik op de leveringspagina op **[!UICONTROL Review & send]** en klik op **[!UICONTROL Prepare]** . Dan, bevestig.

   ![ Schermafbeelding die de voor- optie en logboekenmenu toont ](assets/cus-prepare.png){zoomable="yes"}

1. Klik op **[!UICONTROL Send]** om door te gaan met het uiteindelijke verzendproces en bevestig het vervolgens.

Voor meer details op voorproef en verzend, verwijs naar het vraagcentrum [ documentatie ](../call-center/create-call-center.md#preview-send).
