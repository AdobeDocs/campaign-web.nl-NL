---
audience: end-user
title: Afleveringsinstellingen
description: Meer informatie over de leveringsinstellingen in Campagneweb
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
badge: label="Beta"
source-git-commit: d2497ad144e32f5d164d6be87ab690280c5e3dc9
workflow-type: tm+mt
source-wordcount: '2071'
ht-degree: 6%

---


# Afleveringsinstellingen {#email-del-settings}

E-mailleveringsinstellingen zijn **technische leveringsparameters** die zijn gedefinieerd in de e-mailsjabloon. Deze kunnen voor elke levering worden overbelast.

Deze instellingen zijn beschikbaar via de **Leveringsinstellingen configureren** pictogram beschikbaar bij het bewerken van een leveringssjabloon voor e-mail of een leveringssjabloon voor e-mail.


## E-mailleveringsinstellingen {#email-delivery-settings}

>[!CAUTION]
>
>Deze instellingen worden alleen ter informatie beschreven. Sommige van hen hangen van uw configuratie en toestemmingen af. Deze mogen niet in deze versie van het product worden gewijzigd.

## Typologische instellingen {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="De typologische regels staan marketers toe om bedrijfspraktijken, over alle leveringen te standaardiseren. Een typologie is een verzameling typologische regels waarmee u het verzenden van leveringen kunt beheren, filteren en prioriteren. Profielen die voldoen aan criteria binnen een typologieregel worden bij de voorbereidingsfase uitgesloten van de toedieningsdoelgroepen."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Typologische instellingen voor de levering"
>abstract="De typologische regels staan marketers toe om bedrijfspraktijken, over alle leveringen te standaardiseren. Een typologie is een verzameling typologische regels waarmee u het verzenden van leveringen kunt beheren, filteren en prioriteren. Profielen die voldoen aan criteria binnen een typologieregel worden bij de voorbereidingsfase uitgesloten van de toedieningsdoelgroepen."


Typologieën zijn reeksen van **typologieregels**, die tijdens de voorbereidingsfase worden uitgevoerd. De typologische regels staan marketers toe om bedrijfspraktijken, over alle leveringen te standaardiseren. Een typologie is een verzameling typologische regels waarmee u het verzenden van leveringen kunt beheren, filteren en prioriteren. Profielen die voldoen aan criteria binnen een typologieregel, worden uitgesloten van de toedieningsdoelgroepen tijdens de voorbereidingsfase van de levering.  Ze staan u toe te controleren of uw e-mails altijd bepaalde elementen (zoals een koppeling voor een uitschrijving of een onderwerpregel) of filterregels bevatten om groepen van uw beoogde doel (zoals uitgeschreven abonnees, concurrenten of niet-loyale klanten) uit te sluiten.

De typologische regels worden gegroepeerd binnen een typologie om gemakkelijk veelvoudige het filtreren regels op een levering in één keer toe te passen.

Wanneer het associëren van een typologie met een bericht of berichtmalplaatje, worden de typologische regels inbegrepen in de typologie uitgevoerd om de berichtgeldigheid tijdens berichtvoorbereiding te controleren.

![](assets/delivery-settings-1.png)




### Drukparameters {#pressure-parameters}


>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Drukparameters voor de levering"
>abstract="Met leveringsgewichten kunt u topprioriteit-leveringen identificeren in het kader van vermoeidheidsbeheer. Berichten met het hoogste gewicht hebben prioriteit."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Afleveringsgewicht"
>abstract="Met leveringsgewichten kunt u topprioriteit-leveringen identificeren in het kader van drukbeheer. Berichten met het hoogste gewicht hebben prioriteit."

In deze sectie kunt u met drukparameters een **drempel** het opstellen van regels voor vermoeidheidsbeheer. Dit is het maximumaantal berichten dat over een bepaalde periode naar één profiel kan worden verzonden. Zodra deze drempelwaarde is bereikt, kunnen tot het einde van de in aanmerking genomen periode geen leveringen meer plaatsvinden. Met dit proces kunt u automatisch een profiel uitsluiten van een levering als een bericht de ingestelde drempelwaarde overschrijdt. Op deze manier voorkomt u dat een profiel te vaak wordt benaderd.

Drempelwaarden kunnen constant of variabel zijn. Dit betekent dat drempelwaarden voor een bepaalde periode kunnen variëren van het ene profiel tot het andere, of zelfs voor hetzelfde profiel.

In de **Type dikte** veld zijn drie opties beschikbaar:

* **Constante**
* **Afhankelijk van de ontvanger**
* **Gedefinieerd in elke regel**

Gebruik de **Afleveringsgewicht** veld om de leveringsprioriteit te bepalen. Elke levering heeft een gewicht dat overeenkomt met het prioriteitsniveau. Standaard is het gewicht van een levering ingesteld op 5. Aan de hand van drukregels kunt u het gewicht bepalen van de leveringen waarop ze worden toegepast. U kunt het gewicht instellen of berekenen met behulp van een formule die geschikt is voor de ontvanger. U kunt bijvoorbeeld het gewicht van een levering bepalen op basis van de belangen van de ontvanger.


Gebruik de **Leveringsmodus** veld om de evaluatiemodus voor het doel te selecteren. Er zijn drie modi beschikbaar:

* **Doelschatting en berichtpersonalisatie**
* **Schatting en goedkeuring van de voorlopige doelstelling**
* **Doelevaluatie**

Moeilijkheidsbeheer wordt geleverd met **Campagne optimaliseren** invoegtoepassing. Meer informatie over drukregels en hoe u vermoeidheidsbeheer kunt configureren in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}.

### Capaciteitsinstellingen {#capacity-settings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_capacity_settings"
>title="Capaciteitsinstellingen voor de levering"
>abstract="Alvorens berichten te leveren, gebruik capaciteitsregels om ervoor te zorgen uw organisatie de levering, de binnenkomende berichten kan verwerken die de levering, en het aantal vraag kan produceren om abonnees bijvoorbeeld te contacteren. De capaciteitsregels worden gedefinieerd in de Adobe Campaign v8-console. Selecteer in dit scherm een regel die aan het e-mailkanaal is gekoppeld."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_recipient_importance"
>title="Belang van de begunstigde"
>abstract="Het belang van de ontvanger is een formule die wordt gebruikt om te bepalen welke ontvangers worden gehouden wanneer de regels inzake capaciteitstypologie worden overschreden."


In deze sectie kunt u een capaciteitsregel selecteren die is gedefinieerd in de Adobe Campaign v8-console. Deze regel is gekoppeld aan het e-mailkanaal.

De **belang van de begunstigde** het veld is een formule die wordt gebruikt om te bepalen welke ontvangers worden gehouden wanneer de voorschriften inzake capaciteitstypologie worden overschreden .

Leer meer over consistentie en capaciteitsregels en hoe te om hen te vormen in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.


## Instellingen voor publiek {#audience}


>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Instellingen voor het publiek voor de levering"
>abstract="Selecteer een **doeltoewijzing** onder de beschikbare groepen. Doeltoewijzingen worden gedefinieerd in de Adobe Campaign v8-console. U kunt ook de uitsluitingsparameters voor de levering instellen. "


In deze sectie kunt u een **doeltoewijzing** onder de beschikbare groepen. Doeltoewijzingen worden gedefinieerd in de Adobe Campaign v8-console.

Meer informatie over doeltoewijzingen in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/target-mappings.html){target="_blank"}.

## Levering {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Leveringsinstellingen voor de levering"
>abstract="De parameters van de levering zijn technische montages die op uw levering van toepassing zijn. U kunt BCC voor de levering activeren, en de levering en routinewijzen veranderen. Deze opties zijn beperkt tot deskundige gebruikers."

De parameters van de levering zijn technische montages die op uw levering van toepassing zijn.

* **Routering**: de geïntegreerde e-mail die externe rekening verplettert wordt door gebrek verstrekt. Het bevat de technische parameters waarmee de applicatie e-mailberichten kan verzenden.

* **SMTP-levering testen**: deze optie wordt gebruikt om het verzenden via SMTP te testen. De levering wordt verwerkt tot verbinding aan de server SMTP maar niet verzonden: voor elke ontvanger van de levering, verbindt de Campagne met de SMTP leverancierserver, voert SMTP RCPT aan bevel uit, en sluit de verbinding vóór het bevel SMTP DATA.

* **BCC e-mailen**: deze optie wordt gebruikt om e-mailberichten op een extern systeem op te slaan via BCC door eenvoudig een BCC-e-mailadres toe te voegen aan uw berichtdoel. Meer informatie over BCC via e-mail in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

### Web Analytics {#web-analytics}


>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Webanalytische instellingen voor levering"
>abstract="Selecteer een account voor webanalyse. Dit account is geconfigureerd in de Campagne-clientconsole. U kunt ook de tags definiëren die worden gedeeld met het analyseprogramma dat u gebruikt."

In deze sectie kunt u een account voor webanalyse selecteren. Dit account is geconfigureerd in de Campagne-clientconsole.

U kunt ook de tags definiëren die worden gedeeld met het analyseprogramma dat u gebruikt.

Meer informatie over webanalyse en campagne in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.


### Hernieuwde pogingen {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Maximum aantal pogingen"
>abstract="Als een bericht mislukt als gevolg van een tijdelijke fout, worden opnieuw pogingen uitgevoerd tot het einde van de leveringsduur."

Voor tijdelijk niet-geleverde berichten vanwege een fout Zacht of Genegeerd wordt het automatisch opnieuw geprobeerd. Door gebrek, zijn vijf herpogingen gepland voor de eerste dag van de levering met een minimuminterval van één uur uitgespreid over de 24 uren van de dag.

Meer informatie over het beheer van nieuwe pogingen vindt u in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

## Goedkeuring {#approval}

>[!CONTEXTUALHELP]
>id="acw_email_settings_approval"
>title="Goedkeuringsmodus voor levering"
>abstract="Selecteer de goedkeuringsmodus. Als de waarschuwingen tijdens de leveringsvoorbereiding worden geproduceerd, kunt u de levering vormen om te bepalen al dan niet het nog zou moeten worden uitgevoerd."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_approval"
>title="Goedkeuringsmodus voor de leveringen"
>abstract="Selecteer de goedkeuringsmodus voor leveringen op basis van deze sjabloon. Als de waarschuwingen tijdens de leveringsvoorbereiding worden geproduceerd, kunt u de levering vormen om te bepalen al dan niet het nog zou moeten worden uitgevoerd."

Als de waarschuwingen tijdens de leveringsvoorbereiding worden geproduceerd, kunt u de levering vormen om te bepalen al dan niet het nog zou moeten worden uitgevoerd. Door gebrek, moet de gebruiker het verzenden van berichten aan het eind van de analysefase bevestigen: dit is **handmatig** validatie.

U kunt een andere goedkeuringsmodus in het desbetreffende veld selecteren. Beschikbare modi zijn:

* **Handmatig**: Aan het einde van de analysefase moet de gebruiker de levering bevestigen om te beginnen met verzenden.

* **Halfautomatisch**: Het verzenden begint automatisch als er tijdens de analysefase geen waarschuwingsberichten worden gegenereerd.

* **Automatisch**: De verzending begint automatisch aan het einde van de analysefase, ongeacht het resultaat.


## Geldigheid {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Geldigheid van instellingen"
>abstract="In het veld Leveringsduur kunt u de limiet voor algemene leveringpogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, worden de regelmatige, configureerbare pogingen uitgevoerd tot de geldigheidsgrens wordt bereikt.Het gebied van de Geldigheidsgrens wordt gebruikt voor geüploade middelen, zoals de spiegelpagina of beelden. Deze bronnen gelden voor een beperkte periode: wanneer de limiet is bereikt, zijn er geen bronnen meer beschikbaar."



>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Geldigheidslimiet voor bronnen"
>abstract="Het veld Geldigheidslimiet wordt gebruikt voor geüploade bronnen, zoals de spiegelpagina of afbeeldingen. Deze bronnen gelden voor een beperkte periode: wanneer de limiet is bereikt, zijn er geen bronnen meer beschikbaar."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Leveringsduur"
>abstract="In het veld Leveringsduur kunt u de limiet voor algemene leveringpogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, regelmatig, configureerbare herpogingen worden uitgevoerd tot de geldigheidsgrens wordt bereikt."
<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

De **Leveringsduur** in dit veld kunt u de limiet voor algemene leveringspogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, regelmatig, configureerbare herpogingen worden uitgevoerd tot de geldigheidsgrens wordt bereikt.

U kunt ook datums opgeven. Selecteer **Geldigheidsdatums expliciet instellen**. In dit geval kunt u ook de tijd opgeven op basis van de uiterste datum voor levering en geldigheid. De huidige tijd wordt standaard gebruikt, maar u kunt deze rechtstreeks wijzigen in het invoerveld.

**Geldigheidslimiet voor bronnen** wordt gebruikt voor geüploade bronnen, voornamelijk voor de spiegelpagina en afbeeldingen. De bronnen op deze pagina zijn gedurende een beperkte tijd geldig (om schijfruimte te besparen). Na deze limiet zijn deze bronnen niet meer beschikbaar.

![](assets/delivery-settings-2.png)


Meer informatie over de geldigheidsperiode van de levering in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Paginabeheer spiegelen {#mirror}

De spiegelpagina is een HTML-pagina die online toegankelijk is via een webbrowser. De inhoud is identiek aan de e-mail. Standaard wordt de spiegelpagina gegenereerd als de koppeling wordt ingevoegd in de inhoud van de e-mail.

Naast de standaardmodus zijn ook de volgende opties beschikbaar:


* **[!UICONTROL Force the generation of the mirror page]**: gebruik deze modus om de spiegelpagina te genereren, zelfs als er geen koppeling naar de spiegelpagina is ingevoegd in de levering.
* **[!UICONTROL Do not generate the mirror page]**: gebruik deze modus om te voorkomen dat een spiegelpagina wordt gegenereerd, zelfs als de koppeling aanwezig is in de levering.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: wanneer de koppeling naar de spiegelpagina niet aanwezig is in de e-mailinhoud, gebruikt u deze optie om toegang tot de inhoud van de spiegelpagina, in het venster van het leveringslogboek, vanaf de clientconsole in te schakelen.


### Tracking {#tracking}

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_tracking_validity"
>title="Validity period"
>abstract="This option defines the duration for which the tracking is activated on the URLs."
-->




>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_tracking_validity"
>title="Geldigheidsperiode"
>abstract="De geldigheidsperiode bepaalt de duur waarvoor het volgen op bericht URLs wordt geactiveerd."


De volgende parameters worden bepaald in de verwante sectie. Mogelijke opties zijn:

**Geldigheidslimiet voor bijhouden**: gebruik deze optie om de duur te wijzigen waarvoor de tekstspatiëring wordt geactiveerd op de URL&#39;s.

**Vervangende URL voor verlopen URL&#39;s**: gebruik deze optie om een URL in te voeren naar een fallback-webpagina: deze wordt weergegeven zodra de tekstspatiëring is verlopen.

## Instellingen testen {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="Testinstellingen voor levering"
>abstract="Selecteer de uitsluitingsparameters en pas het label van de teste-mails aan."

U kunt de uitsluitingsparameters in deze sectie instellen. Beschikbare opties zijn:

* **Dubbel houden** Hiermee kunt u meerdere leveringen toestaan aan ontvangers die aan verschillende doelcriteria voldoen.

* **Op de lijst met ongewenste personen staan adressen behouden** Hiermee kunt u profielen die niet meer het doelprofiel zijn van levering, zoals na een abonnement (opt-out), niet meer als doel instellen.

* **Houd quarantineadressen** Hiermee kunt u profielen met een adres dat niet reageert, behouden van het doel.

U kunt ook de naam van de teste-mails aanpassen.

Gebruik de **De leveringscode voor de proefdruk behouden** om aan de teste-mail de zelfde leveringscode te associëren die voor de levering wordt bepaald waarop het betrekking heeft.

Standaard wordt het onderwerp van de teste-mail voorafgegaan door &#39;PROOF #&#39;, waarbij # het nummer van de teste-mail is. U kunt dit voorvoegsel wijzigen in het dialoogvenster **Label, voorvoegsel** veld.