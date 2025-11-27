---
title: Branding
description: Ontdek hoe u uw merk kunt toewijzen
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 8f6a5255-0245-497b-880f-d91ea82ee19e
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 14%

---

# Uw merk toewijzen {#branding-assign}

## Een merk koppelen aan een sjabloon {#linking-a-brand-to-a-template}

Om de parameters te gebruiken die voor een merk worden bepaald, moet het met een leveringsmalplaatje worden verbonden. Hiervoor moet u een sjabloon maken of bewerken.

Je template wordt gekoppeld aan het merk. In de e-maileditor maken de elementen zoals **Email address of default sender**, **Default sender name** of **Logo** gebruik van de geconfigureerde merkdata.

>[!BEGINTABS]

>[!TAB  het Web van Adobe Campaign ]

Om een leveringsmalplaatje tot stand te brengen, kunt u een ingebouwde malplaatje dupliceren, een bestaande levering in een malplaatje omzetten of een leveringsmalplaatje van kras tot stand brengen. [Meer informatie](../../msg/delivery-template.md)

Nadat u de sjabloon hebt gemaakt, kunt u deze koppelen aan een merk. Dit doet u als volgt:

1. Blader naar het tabblad **[!UICONTROL Templates]** in het linkermenu van **[!UICONTROL Deliveries]** en selecteer een leveringssjabloon.

   ![](assets/branding_assign_web_1.png)

1. Klik op **[!UICONTROL Settings]**.

   ![](assets/branding_assign_web_2.png)

1. Open op het tabblad **[!UICONTROL Delivery]** het veld **[!UICONTROL Branding]** en selecteer het merk dat u aan de sjabloon wilt koppelen.

   ![](assets/branding_assign_web_3.png)

1. Bevestig uw selectie en sla uw sjabloon op.

U kunt deze sjabloon nu gebruiken om uw leveringen te verzenden.

>[!TAB  Adobe Campaign V8 ]

Om een leveringsmalplaatje tot stand te brengen, kunt u een ingebouwde malplaatje dupliceren, een bestaande levering in een malplaatje omzetten of een leveringsmalplaatje van kras tot stand brengen. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/create-templates.html?lang=nl-NL)

Nadat u de sjabloon hebt gemaakt, kunt u deze koppelen aan een merk. Dit doet u als volgt:

1. Blader naar **[!UICONTROL Resources]** `>` **[!UICONTROL Templates]** `>` **[!UICONTROL Delivery templates]** in Adobe Campaign Explorer.

1. Selecteer een leveringssjabloon of dupliceer een bestaande sjabloon.

   ![](assets/branding_assign_V8_1.png)

1. Open **[!UICONTROL Properties]** van de geselecteerde leveringssjabloon.

   ![](assets/branding_assign_V8_2.png)

1. Selecteer op het tabblad **[!UICONTROL General]** uw merk in de vervolgkeuzelijst **[!UICONTROL Branding]** .

   ![](assets/branding_assign_V8_3.png)

1. Zodra gevormd, uitgezochte **O.K.**.

U kunt deze sjabloon nu gebruiken om uw leveringen te verzenden.

>[!ENDTABS]

## Een merk toewijzen aan uw levering {#assigning-a-brand-to-an-email}

>[!BEGINTABS]

>[!TAB  het Web van Adobe Campaign ]

Volg de onderstaande stappen om een nieuwe, zelfstandige levering te maken.

1. Blader naar het menu **[!UICONTROL Deliveries]** op de linkertrack en klik op de knop **[!UICONTROL Create delivery]** .

   ![](assets/branding_assign_web_4.png)

1. Selecteer E-mail of Duw bericht als kanaal en kies een leveringsmalplaatje van de lijst.

1. Klik op de knop **[!UICONTROL Create delivery]** ter bevestiging.

1. Klik op **[!UICONTROL Properties]** op de pagina **[!UICONTROL Settings]** .

   ![](assets/branding_assign_web_5.png)

1. Open het veld **[!UICONTROL Delivery]** via het tabblad **[!UICONTROL Branding]** .

   ![](assets/branding_assign_web_6.png)

1. Selecteer het merk dat u aan het malplaatje wilt verbinden.

   ![](assets/branding_assign_web_7.png)

1. Pas uw leveringen verder aan. Voor meer informatie over het creëren van een e-mail verwijs naar [&#x200B; creeer uw eerste e-mail &#x200B;](../../email/create-email.md) sectie.

>[!TAB  Adobe Campaign V8 ]

Volg de onderstaande stappen om een nieuwe, zelfstandige levering te maken.

1. Blader naar het tabblad **[!UICONTROL Campaigns]** om een nieuwe levering te maken.

1. Klik op **[!UICONTROL Deliveries]** en klik op de knop **[!UICONTROL Create]** boven de lijst met bestaande leveringen.

   ![](assets/branding_assign_V8_4.png)

1. Selecteer een leveringssjabloon.

1. Open **[!UICONTROL Properties]** van de geselecteerde leveringssjabloon.

   ![](assets/branding_assign_V8_5.png)

1. Selecteer op het tabblad **[!UICONTROL General]** uw merk in de vervolgkeuzelijst **[!UICONTROL Branding]** .

   ![](assets/branding_assign_V8_6.png)

1. Zodra gevormd, uitgezochte **O.K.**.

1. Pas uw leveringen verder aan. Voor meer informatie over het creëren van een e-mail verwijs naar het [&#x200B; Ontwerp en verzend e-mails &#x200B;](../../email/create-email.md) sectie.

1. U kunt ook merkgegevens toevoegen met de aanpassingsvelden. Navigeer naar **[!UICONTROL Branding]** en selecteer de merkgerelateerde aanpassingsblokken die u wilt invoegen (zoals de merknaam, de URL van het logo, de URL van de website, informatie over de afzender, enz.).

>[!ENDTABS]


## Branding controleren die is gekoppeld aan transactieberichten {#check-branding-transactional}

>[!IMPORTANT]
>
>Deze sectie is slechts op Transactieoverseinen (het Centrum van het Bericht) van toepassing.
>
>Terwijl de transactiemogelijkheden in het Web UI van de Campagne beschikbaar zijn, moeten de controlestappen hieronder in de Console van de Cliënt van de Campagne v8 (controlegeval) worden uitgevoerd.

Transactionele leveringen die van uitvoerinstanties in real time (RT) aan de controleinstantie worden gesynchroniseerd repliceren geen eigenschappen zoals het verpletteren of het brandmerken. Deze gesynchroniseerde leveringen worden geproduceerd wekelijks van het zelfde malplaatje om leveringsindicatoren in de controleinstantie terug te brengen.

Wegens dit, toont de controleinstantie het standaardmerk. Het daadwerkelijke merk en het verpletteren van montages die tijdens berichtuitvoering worden gebruikt worden bepaald in het transactionele berichtmalplaatje op de controleinstantie.

Om te verifiëren welk merk voor een transactiemelding werd gebruikt:

1. Identificeer de interne naam van het transactiesjabloon dat naar Real-Time is gepubliceerd (bijvoorbeeld `TransactionalMessaging4768`).

   ![](assets/branding-transactional.png)

1. In de controleinstantie, onderzoek naar deze interne naam onder **Transactionele berichtmalplaatjes**.

   ![](assets/branding-transactional2.png)

1. Open de sjabloon om het merk en andere verwante eigenschappen weer te geven.
