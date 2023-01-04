---
audience: end-user
title: Geavanceerde instellingen
description: Campagne v8 Webdocumentatie
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 4fbb5e2eb0211712d17f1437986038c40ed15602
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 18%

---

# Geavanceerde instellingen {#advanced-settings}

>[!NOTE]
>
>Deze documentatie is in opbouw en wordt regelmatig bijgewerkt. De definitieve versie van deze inhoud zal in Januari 2023 klaar zijn.

Deze instellingen zijn technische leveringsparameters die in de e-mailsjabloon zijn gedefinieerd. Als u om het even welk van hen voor een specifieke levering wilt wijzigen, ga met voorzichtigheid te werk.

## E-mailleveringsinstellingen {#email-delivery-settings}

<!--
October 2022 

Note that this page is for now a placeholder to host Contextualhelp blocks

Do not delete these blocks 

Documentation on this part is targeted for december 2022
-->

Alle technische leveringsparameters van het malplaatje.
Wijzig alleen parameters, geen ontwerp hier.
Volgens toestemmingen zouden de Praktijken dit, voorzichtigheid niet moeten wijzigen. Alleen typologieregel controleren en wijzigen -> rest gedefinieerd in sjabloon

## Typologie {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="Met de typologie kunt u het verzenden van leveringen controleren, filteren en controleren."

Typologieën zijn reeksen typologieregels die tijdens de fase van de berichtanalyse worden uitgevoerd. Ze staan u toe te controleren of uw e-mails altijd bepaalde elementen (zoals een koppeling voor een uitschrijving of een onderwerpregel) of filterregels bevatten om groepen van uw beoogde doel (zoals uitgeschreven abonnees, concurrenten of niet-loyale klanten) uit te sluiten.

Wanneer u een typologie aan een bericht of berichtsjabloon koppelt, worden de typologieregels die in de typologie zijn opgenomen, uitgevoerd om de berichtgeldigheid te controleren.

### Drukparameters {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_weight"
>title="Afleveringsgewicht"
>abstract="Met leveringsgewichten kunt u topprioriteit-leveringen identificeren in het kader van drukbeheer. Berichten met het hoogste gewicht hebben prioriteit."

In deze sectie kunt u met drukparameters een drempel definiëren. Dit is het maximumaantal berichten dat over een bepaalde periode naar één profiel kan worden verzonden. Zodra deze drempelwaarde is bereikt, kunnen tot het einde van de in aanmerking genomen periode geen leveringen meer plaatsvinden. Met dit proces kunt u automatisch een profiel uitsluiten van een levering als een bericht de ingestelde drempelwaarde overschrijdt. Op deze manier voorkomt u dat een profiel te vaak wordt benaderd.

Drempelwaarden kunnen constant of variabel zijn. Dit betekent dat drempelwaarden voor een bepaalde periode kunnen variëren van het ene profiel tot het andere, of zelfs voor hetzelfde profiel.

In de **Type dikte** veld zijn drie opties beschikbaar:

De **Afleveringsgewicht** veld

De **Leveringsmodus** veld..

### Capaciteitsinstellingen {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_recipient_importance"
>title="Belang van de begunstigde"
>abstract="Het belang van de ontvanger is een formule die wordt gebruikt om te bepalen welke ontvangers worden gehouden wanneer de regels inzake capaciteitstypologie worden overschreden."

In deze sectie kunt u een capaciteitsregel selecteren die is gedefinieerd in de Adobe Campaign v8-console. Deze regel is gekoppeld aan het e-mailkanaal.

De **belang van de begunstigde** het veld is een formule die wordt gebruikt om te bepalen welke ontvangers worden gehouden wanneer de voorschriften inzake capaciteitstypologie worden overschreden .

## Doelgroep {#audience}

In deze sectie kunt u een doeltoewijzing kiezen die is gedefinieerd in de Adobe Campaign v8-console. Het maken van doeltoewijzingen is nodig als u een andere ontvangertabel gebruikt dan de tabel die door Adobe Campaign wordt geleverd.

## Levering {#delivery}

SMTP-levering testen: gebruik deze optie om het verzenden via SMTP te testen. De levering wordt verwerkt tot verbinding aan de server SMTP maar niet verzonden: voor elke ontvanger van de levering, verbindt de Campagne met de SMTP leverancierserver, voert SMTP RCPT aan bevel uit, en sluit de verbinding vóór het bevel van SMTP DATA.

BCC e-mailen: Gebruik deze optie om e-mails op te slaan op een extern systeem via BCC door eenvoudig een BCC-e-mailadres toe te voegen aan uw berichtdoel.

### Hernieuwde pogingen {#retries}

>[!CONTEXTUALHELP]
>id="acw_email_settings_retries"
>title="Maximum aantal pogingen"
>abstract="Als een bericht mislukt als gevolg van een tijdelijke fout, worden de pogingen opnieuw uitgevoerd tijdens de leveringsduur."

Voor tijdelijk niet-geleverde berichten vanwege een fout Zacht of Genegeerd wordt het automatisch opnieuw geprobeerd. Door gebrek, zijn vijf herpogingen gepland voor de eerste dag van de levering met een minimuminterval van één uur uitgespreid over de 24 uren van de dag. Elke dag opnieuw proberen wordt geprogrammeerd na dat en tot de leveringsdeadline, die in het lusje van de Geldigheid wordt bepaald.

## Goedkeuring {#approval}

**Handmatig**

**Halfautomatisch**

**Automatisch**

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Goedkeuringsmodus"
>abstract="Elke leveringsstap kan worden goedgekeurd om volledige controle en controle van de verschillende processen te waarborgen."

## Geldigheid {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery_duration"
>title="Leveringsduur"
>abstract="In het veld Leveringsduur kunt u de limiet voor algemene leveringspogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, regelmatig, configureerbare herpogingen worden uitgevoerd tot de geldigheidsgrens wordt bereikt."

>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Geldigheidslimiet voor bronnen"
>abstract="Het veld Geldigheidslimiet wordt gebruikt voor geüploade bronnen, voornamelijk voor de spiegelpagina en afbeeldingen. De bronnen op deze pagina zijn gedurende een beperkte periode geldig."


In het veld Leveringsduur kunt u de limiet voor algemene leveringspogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, regelmatig, configureerbare herpogingen worden uitgevoerd tot de geldigheidsgrens wordt bereikt.

U kunt ook datums opgeven. Selecteer hiervoor Expliciet geldigheidsdatums instellen. In dit geval kunt u ook de leverings- en geldigheidstermijn opgeven. De huidige tijd wordt standaard gebruikt, maar u kunt deze rechtstreeks wijzigen in het invoerveld.

Geldigheidslimiet van middelen: Het veld Geldigheidslimiet wordt gebruikt voor geüploade bronnen, voornamelijk voor de spiegelpagina en afbeeldingen. De bronnen op deze pagina zijn gedurende een beperkte tijd geldig (om schijfruimte te besparen).

### Paginabeheer spiegelen {#mirror}

**Paginabeheer spiegelen**

### Tracking {#tracking}

>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Geldigheidsperiode"
>abstract="Met deze optie bepaalt u de duur waarvoor de tracering wordt geactiveerd op de URL&#39;s."

**Geldigheidslimiet voor bijhouden**: Met deze optie bepaalt u de duur waarvoor de tracering wordt geactiveerd op de URL&#39;s.

**Vervangende URL voor verlopen URL&#39;s**: TBC


## Testinstellingen{#test-setttings}

**Dubbel houden**

**Op de lijst met ongewenste personen staan adressen behouden**

**Houd quarantineadressen**

**De leveringscode voor de proefdruk behouden**

**Label, voorvoegsel**