---
title: Externe account beheren
description: Leer hoe u externe accounts kunt configureren
exl-id: e37d6cb0-f8fa-4f1c-9cdd-46f9666c2d18
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 1%

---

# Externe accounts beheren {#external-accounts}

>[!AVAILABILITY]
>
>* De externe rekeningen zijn momenteel beschikbaar slechts voor Stuitende berichten (POP3), het Verpletteren, en de instantie van de Uitvoering. Aanvullende accounttypen worden later toegevoegd.
>
>* Niet-ondersteunde externe accounts die zijn gemaakt in de Adobe Campaign-console zijn zichtbaar in de webgebruikersinterface, maar kunnen niet worden bewerkt of geopend.

Adobe Campaign bevat vooraf geconfigureerde externe accounts die eenvoudig kunnen worden geïntegreerd met verschillende systemen. Als u verbinding wilt maken met extra platforms of verbindingen wilt aanpassen aan uw workflow, maakt u nieuwe externe accounts met de webgebruikersinterface. Dit zorgt voor naadloze gegevensoverdracht.

## Een externe account maken {#create-ext-account}

Voer de onderstaande stappen uit om een nieuwe externe account te maken. Gedetailleerde instellingen zijn afhankelijk van het type externe account. [Meer informatie](#campaign-specific)

1. Selecteer **[!UICONTROL External accounts]** onder **[!UICONTROL Administration]** in het menu voor het linkerdeelvenster.

1. Klik op **[!UICONTROL Create external account]**.

   ![ Schermschot die de optie toont om een externe rekening in het Gebruikersinterface van het Web tot stand te brengen.](assets/external_account_create_1.png)

1. Voer uw **[!UICONTROL Label]** in en selecteer de externe account **[!UICONTROL Type]** .

   >[!NOTE]
   >
   >De montages voor campagne-specifieke types zijn gedetailleerd in [ deze sectie ](#campaign-specific).

   ![ Schermafbeelding die gebieden tonen voor het ingaan van het etiket en het selecteren van het externe accounttype.](assets/external_account_create_2.png)

1. Klik op **[!UICONTROL Create]**.

1. Wijzig in de vervolgkeuzelijst **[!UICONTROL Additional options]** het pad **[!UICONTROL Internal name]** of **[!UICONTROL Folder]** , indien nodig.

   ![ Screenshot die extra opties voor interne naam en de configuratie van de omslagweg toont.](assets/external_account_create_3.png)

1. Schakel de optie **[!UICONTROL Exported automatically in packages]** in om automatisch gegevens te exporteren die door deze externe account worden beheerd. <!--Exported where??-->

   ![ Schermafbeelding die de optie toont om automatische export in pakketten toe te laten.](assets/external_account_create_exported.png)

1. Configureer in de sectie **[!UICONTROL Details]** de toegang tot de account door referenties op te geven op basis van het gekozen externe accounttype. [Meer informatie](#bounce)

1. Klik op **[!UICONTROL Test connection]** om te controleren of de configuratie juist is.

1. Dupliceer of verwijder uw externe account vanuit het menu **[!UICONTROL More...]** .

   ![ Schermschot die het Meer menu met opties toont om de externe rekening te dupliceren of te schrappen.](assets/external_account_create_4.png)

1. Klik op **[!UICONTROL Save]** als de configuratie is voltooid.

## Campagne-specifieke externe rekeningen {#campaign-specific}

Afhankelijk van het geselecteerde externe accounttype voert u de onderstaande stappen uit om de accountinstellingen te configureren.

### Stuitberichten (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 wordt momenteel niet ondersteund.

Met de externe account Bounce mails wordt de externe POP3-account opgegeven die wordt gebruikt om verbinding te maken met de e-mailservice. Alle servers die voor POP3 toegang worden gevormd kunnen terugkeerpost ontvangen.

![ Screenshot die de de post van de Stuits (POP3) externe gebieden van de rekeningsconfiguratie toont.](assets/external_account_bounce.png)

Als u de **[!UICONTROL Bounce mails (POP3)]** externe account wilt configureren, vult u de volgende velden in:

* **[!UICONTROL Server]** - URL van de POP3-server.

* **[!UICONTROL Port]** - POP3-poortnummer (standaardpoort is 110).

* **[!UICONTROL Account]** - Naam van de gebruiker.

* **[!UICONTROL Password]** - Wachtwoord voor gebruikersaccount.

* **[!UICONTROL Encryption]** - Type gekozen codering, inclusief:
   * Standaard (POP3 als poort 110, POP3S als poort 995).
   * POP3 die overschakelt naar SSL na het verzenden van een STARTTLS.
   * POP3 niet-beveiligd (standaard poort 110).
   * POP3 beveiligd boven SSL (standaard poort 995).

* **[!UICONTROL Function]** - Selecteer **[!UICONTROL Inbound email]** om het account voor het ontvangen van inkomende e-mails te configureren of **[!UICONTROL SOAP router]** om SOAP-aanvragen af te handelen.

### Routering {#routing}

Volg onderstaande stappen om een specifieke externe account voor externe leveringen te configureren.

1. Maak een externe account. [Meer informatie](../administration/external-account.md#create-ext-account)

1. Selecteer het type **[!UICONTROL Routing]** .

   ![ Screenshot die de Verpletterende externe selectie van accounttype tonen.](assets/external-account-routing.png){zoomable="yes"}

1. Selecteer het gewenste kanaal en klik op **[!UICONTROL Create]** .

1. In de sectie voor de externe account **[!UICONTROL Details]** is **[!UICONTROL External]** standaard geselecteerd als de **[!UICONTROL Delivery mode]** .

   ![ Screenshot die de de wijzeconfiguratie van de Levering voor het Verpletteren van externe rekeningen toont.](assets/external-account-delivery-mode.png){zoomable="yes"}

   >[!NOTE]
   >
   >Momenteel is **[!UICONTROL External]** de enige beschikbare modus.

1. Als u het proces na de uitvoering van de levering wilt afhandelen, dient u dit uit te besteden aan een workflow voor nabewerking. Creeer een werkschema met een [ Externe signaal ](../workflows/activities/external-signal.md) activiteit en selecteer het van het **[!UICONTROL Post-processing]** gebied.

   ![ Schermafbeelding die de configuratie van het gebied na verwerking voor het Verpletteren van externe rekeningen toont.](assets/external-account-post-processing.png){zoomable="yes"}

1. Bewerk in het veld **[!UICONTROL Activity]** de naam van de activiteit van de nabewerkingsworkflow die in de logboeken wordt weergegeven. <!--you can edit the name of the activity that will be created if you add an external or bulk delivery to a workflow-->

### Uitvoeringsinstantie {#instance-exec}

Als u een gesegmenteerde architectuur hebt, identificeer de uitvoeringsinstanties verbonden aan de controleinstantie en vestigt verbindingen tussen hen. De transactionele berichtmalplaatjes worden opgesteld op de uitvoeringsinstantie.

![ Schermafbeelding die de van de Uitvoering instantie externe gebieden van de rekeningsconfiguratie toont.](assets/external_account_exec.png)

U configureert als volgt de externe account van **[!UICONTROL Execution instance]** :

* **[!UICONTROL URL]** - URL van de server waarop de uitvoeringsinstantie is geïnstalleerd.

* **[!UICONTROL Account]** - Naam van de rekening, die de Agent van het Centrum van het Bericht zoals bepaald in de exploitantomslag aanpast.

* **[!UICONTROL Password]** - Wachtwoord van de account zoals gedefinieerd in de operatormap.

* **[!UICONTROL Method]** - Kies tussen de webservice of FDA (Federated Data Access).

  Selecteer voor FDA uw FDA-account. Merk op dat de verbinding van de campagne aan externe systemen tot geavanceerde gebruikers en slechts beschikbaar bij de cliëntconsole wordt beperkt. [Meer informatie](https://experienceleague.adobe.com/en/docs/campaign/campaign-v8/connect/fda#_blank)

* **[!UICONTROL Create archiving workflow]** - Voor elke uitvoeringsinstantie die in het Berichtencentrum wordt geregistreerd, ongeacht of u één of meerdere instanties hebt, creeer een afzonderlijke archiveringswerkstroom voor elke externe rekening verbonden aan de uitvoeringsinstantie.