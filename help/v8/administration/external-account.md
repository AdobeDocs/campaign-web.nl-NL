---
title: Externe account beheren
description: Leer hoe u externe accounts kunt configureren
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: 8fccae9906d7a04ec1e8e10ad7be60f597a43492
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 1%

---

# Externe accounts beheren {#external-accounts}

>[!AVAILABILITY]
>
>* De externe rekeningen zijn momenteel beschikbaar slechts voor Stuitende berichten (POP3), het Verpletteren en de instantie van de Uitvoering. In de toekomst worden extra accounttypen toegevoegd.
>
>* Niet-ondersteunde externe accounts die zijn gemaakt in de Adobe Campaign-console zijn zichtbaar in de webgebruikersinterface, maar kunnen niet worden bewerkt of geopend.

Adobe Campaign wordt geleverd met een reeks vooraf geconfigureerde externe accounts voor eenvoudige integratie met verschillende systemen. Als u verbinding moet maken met extra platforms of de verbindingen moet aanpassen aan uw workflow, kunt u nu eenvoudig nieuwe externe accounts maken met de webgebruikersinterface die voldoen aan uw specifieke behoeften en zorgen voor naadloze gegevensoverdracht.

## Een externe account maken {#create-ext-account}

Voer de onderstaande stappen uit om een nieuwe externe account te maken. Gedetailleerde instellingen zijn afhankelijk van het type externe account. [Meer informatie](#campaign-specific)

1. Selecteer **[!UICONTROL External accounts]** onder **[!UICONTROL Administration]** in het menu voor het linkerdeelvenster.

1. Klik op **[!UICONTROL Create external account]**.

   ![](assets/external_account_create_1.png)

1. Voer uw **[!UICONTROL Label]** in en selecteer de externe account **[!UICONTROL Type]** .

   >[!NOTE]
   >
   >De montages voor campagne-specifieke types zijn gedetailleerd in [ deze sectie ](#campaign-specific).

   ![](assets/external_account_create_2.png)

1. Klik op **[!UICONTROL Create]**.

1. In de vervolgkeuzelijst **[!UICONTROL Additional options]** kunt u het pad **[!UICONTROL Internal name]** of **[!UICONTROL Folder]** wijzigen als dat nodig is.

   ![](assets/external_account_create_3.png)

1. Schakel de optie **[!UICONTROL Exported automatically in packages]** in als u wilt dat de gegevens die door deze externe account worden beheerd, automatisch worden geëxporteerd. <!--Exported where??-->

   ![](assets/external_account_create_exported.png)

1. In de sectie **[!UICONTROL Details]** configureert u de toegang tot de account door referenties op te geven, afhankelijk van het gekozen externe accounttype. [Meer informatie](#bounce)

1. Klik op **[!UICONTROL Test connection]** om te controleren of de configuratie correct is.

1. Vanuit het menu **[!UICONTROL More...]** kunt u uw externe account dupliceren of verwijderen.

   ![](assets/external_account_create_4.png)

1. Klik op **[!UICONTROL Save]** als de configuratie is voltooid.

## Campagne-specifieke externe rekeningen {#campaign-specific}

Afhankelijk van het geselecteerde externe accounttype voert u de onderstaande stappen uit om de accountinstellingen te configureren.

### Stuitberichten (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 wordt momenteel niet ondersteund.

Met de externe account Bounce mails wordt de externe POP3-account opgegeven die wordt gebruikt om verbinding te maken met de e-mailservice. Alle servers die voor POP3 toegang worden gevormd kunnen terugkeerpost ontvangen.

![](assets/external_account_bounce.png)

Als u de **[!UICONTROL Bounce mails (POP3)]** externe account wilt configureren, vult u de volgende velden in:

* **[!UICONTROL Server]** - URL van de POP3-server

* **[!UICONTROL Port]** - POP3-poortnummer (standaardpoort is 110)

* **[!UICONTROL Account]** - Naam van de gebruiker

* **[!UICONTROL Password]** - Wachtwoord voor gebruikersaccount

* **[!UICONTROL Encryption]** - Type gekozen codering tussen:

   * Standaard (POP3 als poort 110, POP3S als poort 995)
   * POP3 die overschakelt naar SSL na het verzenden van een STARTTLS
   * POP3 niet-beveiligd (standaard poort 110)
   * POP3 veilig boven SSL (standaard poort 995)

* **[!UICONTROL Function]** - Binnenkomende e-mail, wanneer de externe rekening wordt gevormd om inkomende e-mail, of de router van SOAP, te ontvangen om de verzoeken van SOAP te behandelen.

### Routering {#routing}

Volg onderstaande stappen om een specifieke externe account te configureren die in uw externe leveringen wordt gebruikt.

1. Maak een externe account. [Meer informatie](../administration/external-account.md#create-ext-account)

1. Selecteer het type **[!UICONTROL Routing]** .

   ![](assets/external-account-routing.png){zoomable="yes"}

1. Selecteer het gewenste kanaal en klik op **[!UICONTROL Create]** .

1. In de sectie voor de externe account **[!UICONTROL Details]** is **[!UICONTROL External]** standaard geselecteerd als de **[!UICONTROL Delivery mode]** .

   ![](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Momenteel is **[!UICONTROL External]** de enige beschikbare modus.

1. Als u het proces na de uitvoering van de levering wilt afhandelen, kunt u dit naar een workflow na de verwerking externaliseren. Om dit te doen, moet u een werkschema met een [ Externe signaal ](../workflows/activities/external-signal.md) activiteit tot stand brengen en het van het **[!UICONTROL Post-processing]** gebied selecteren.

   ![](assets/external-account-post-processing.png){zoomable="yes"}

1. In het veld **[!UICONTROL Activity]** kunt u de naam bewerken van de activiteit van de nabewerkingsworkflow die wordt weergegeven in de logboeken. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->


### Uitvoeringsinstantie {#instance-exec}

Als u een gesegmenteerde architectuur hebt, moet u de uitvoeringsinstanties identificeren verbonden aan de controleinstantie en verbindingen tussen hen vestigen. De transactionele berichtmalplaatjes worden opgesteld op de uitvoeringsinstantie.

![](assets/external_account_exec.png)

U configureert als volgt de externe account van **[!UICONTROL Execution instance]** :

* **[!UICONTROL URL]**

  URL van de server waarop de uitvoeringsinstantie is geïnstalleerd.

* **[!UICONTROL Account]**

  Naam van de rekening, moet het de Agent van het Centrum van het Bericht aanpassen zoals die in de exploitantomslag wordt bepaald.

* **[!UICONTROL Password]**

  Wachtwoord van de account zoals gedefinieerd in de map met operatoren.

* **[!UICONTROL Method]**

  Kies tussen de dienst van het Web of Federated Data Access (FDA).
Selecteer uw FDA-account in het geval van de FDA-methode. Merk op dat de verbinding van de campagne aan externe systemen tot geavanceerde gebruikers en slechts beschikbaar bij de cliëntconsole wordt beperkt. [Meer informatie](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Create archiving workflow]**

  Voor elke uitvoeringsinstantie die in het Berichtencentrum wordt geregistreerd, ongeacht of u één of meerdere instanties hebt, moet u een afzonderlijke archiveringswerkstroom voor elke externe rekening tot stand brengen verbonden aan de uitvoeringsinstantie.
