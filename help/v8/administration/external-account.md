---
title: Externe rekening
description: Leer hoe u externe accounts kunt configureren
source-git-commit: 9d022ad4ce9d001d6f5154d2778a538aae560d52
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 1%

---

# Externe accounts configureren {#external-accounts}


>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Externe accounts"
>abstract="U kunt nu verbinding maken met extra platforms of de verbindingen aanpassen aan uw workflow en eenvoudig nieuwe externe accounts maken die aan uw specifieke behoeften voldoen en zorgen voor naadloze gegevensoverdracht."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"


>[!AVAILABILITY]
>
> De externe rekeningen zijn momenteel beschikbaar slechts voor Stuitende post (POP3) en de instantie van de Uitvoering, met extra rekeningtypes die in de toekomst moeten worden toegevoegd.
> Niet-ondersteunde externe accounts die zijn gemaakt in de Adobe Campaign-console zijn zichtbaar in de webgebruikersinterface, maar kunnen niet worden bewerkt of geopend.

Adobe Campaign wordt geleverd met een reeks vooraf geconfigureerde externe accounts voor eenvoudige integratie met verschillende systemen. Als u verbinding moet maken met extra platforms of de verbindingen moet aanpassen aan uw workflow, kunt u nu eenvoudig nieuwe externe accounts maken met de webgebruikersinterface die voldoen aan uw specifieke behoeften en zorgen voor naadloze gegevensoverdracht.

## Een externe account maken {#create-ext-account}

Voer de onderstaande stappen uit om een nieuwe externe account te maken. Gedetailleerde instellingen zijn afhankelijk van het type externe account.

1. Selecteer **[!UICONTROL External accounts]** onder **[!UICONTROL Administration]** in het menu voor het linkerdeelvenster.

1. Klik op **[!UICONTROL Create external account]**.

   ![](assets/external_account_create_1.png)

1. Voer uw **[!UICONTROL Label]** in en selecteer uw externe account **[!UICONTROL Type]** .

   ![](assets/external_account_create_2.png)

1. Klik op **[!UICONTROL Create]**.

1. In de vervolgkeuzelijst **[!UICONTROL Advanced options]** kunt u het pad **[!UICONTROL Internal name]** of **[!UICONTROL Folder]** wijzigen als dat nodig is.

   ![](assets/external_account_create_3.png)

1. Schakel **[!UICONTROL Exported automatically]** in als u wilt dat de gegevens die door deze externe account worden beheerd, automatisch worden geëxporteerd.

1. Configureer de toegang tot de account door referenties op te geven, afhankelijk van het gekozen type externe account.

1. Klik op **[!UICONTROL Test the connection]** om te controleren of de configuratie correct is

1. Dupliceer of verwijder uw externe account vanuit het menu **[!UICONTROL More...]** .

   ![](assets/external_account_create_4.png)

1. Klik op **[!UICONTROL Save]** als de configuratie is voltooid.

## Campagne-specifieke externe rekeningen {#campaign-specific}

### Stuitberichten (POP3) {#bounce}

>[!AVAILABILITY]
>
> OAuth 2.0 wordt momenteel niet ondersteund.

De externe account voor Bounce Mail geeft de externe POP3-account aan die wordt gebruikt om verbinding te maken met de e-mailservice. Alle servers die voor POP3 toegang worden gevormd kunnen terugkeerpost ontvangen.

![](assets/external_account_bounce.png)

U configureert als volgt de externe account van **[!UICONTROL Bounce mails (POP3)]** :

* **[!UICONTROL Server]**

  URL van de POP3-server

* **[!UICONTROL Port]**

  POP3-poortnummer van verbinding (standaardpoort is 110)

* **[!UICONTROL Account]**

  Naam van de gebruiker

* **[!UICONTROL Password]**

  Wachtwoord gebruikersaccount

* **[!UICONTROL Encryption]**

  Type gekozen codering tussen:

   * Standaard (POP3 als poort 110, POP3S als poort 995)
   * POP3 die overschakelt naar SSL na het verzenden van een STARTTLS
   * POP3 niet-beveiligd (standaard poort 110)
   * POP3 veilig boven SSL (standaard poort 995)

* **[!UICONTROL Function]**

  Binnenkomende e-mail, wanneer de externe rekening wordt gevormd om inkomende e-mail, of SOAP router te ontvangen, om SOAP verzoeken te behandelen.

### Uitvoeringsinstantie{#instance-exec}

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
