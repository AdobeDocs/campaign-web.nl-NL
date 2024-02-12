---
audience: end-user
title: Afleveringsinstellingen
description: Meer informatie over de leveringsinstellingen in Campagneweb
feature: Email
exl-id: d6025dbd-0438-4fe7-abe7-0459a89e8cfa
source-git-commit: 88c6473005cfdf7a43e0d232b75db2b51dbcac40
workflow-type: tm+mt
source-wordcount: '2295'
ht-degree: 4%

---


# E-mailleveringsinstellingen {#email-del-settings}

E-mailleveringsinstellingen zijn **technische leveringsparameters** die zijn gedefinieerd in de e-mailsjabloon. Deze kunnen voor elke levering worden overbelast.

Deze instellingen zijn beschikbaar via de **Instellingen** Deze knop is beschikbaar wanneer u een leveringssjabloon voor e-mail of een leveringssjabloon voor e-mail bewerkt.

## E-mailleveringsinstellingen {#email-delivery-settings}

>[!CAUTION]
>
>Deze instellingen worden alleen ter informatie beschreven. Sommige van hen hangen van uw configuratie en toestemmingen af. Deze mogen niet in deze versie van het product worden gewijzigd.

## Typologische instellingen {#typology}

>[!CONTEXTUALHELP]
>id="acw_email_settings_typology"
>title="Typologie"
>abstract="De typologische regels staan marketers toe om bedrijfspraktijken, over alle leveringen te standaardiseren. Een typologie is een verzameling typologische regels waarmee u het verzenden van leveringen kunt beheren, filteren en prioriteren. Profielen die voldoen aan criteria binnen een typologieregel worden bij de voorbereidingsfase uitgesloten van de toedieningsdoelgroepen. De typologieën en de typologieregels worden gecreeerd in de de cliëntconsole van de Campagne."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_typology"
>title="Typologische instellingen voor de levering"
>abstract="De typologische regels staan marketers toe om bedrijfspraktijken, over alle leveringen te standaardiseren. Een typologie is een verzameling typologische regels waarmee u het verzenden van leveringen kunt beheren, filteren en prioriteren. Profielen die voldoen aan criteria binnen een typologieregel worden bij de voorbereidingsfase uitgesloten van de toedieningsdoelgroepen. De typologieën en de typologieregels worden gecreeerd in de de cliëntconsole van de Campagne."


Typologieën zijn reeksen van **typologieregels** die tijdens de voorbereidingsfase worden uitgevoerd om eenvoudig meerdere filterregels op een levering tegelijk toe te passen. Zij staan marketers toe om bedrijfspraktijken over alle leveringen te standaardiseren aangezien zij hen laten controleren, filtreren, en voorrang geven aan het verzenden van leveringen.

Wanneer het associëren van een typologie met een bericht of berichtmalplaatje, worden de typologische regels inbegrepen in de typologie uitgevoerd om de leveringsgeldigheid tijdens berichtvoorbereiding te controleren. Profielen die voldoen aan criteria binnen een typologieregel worden dan uitgesloten van het publiek dat ze levert.

De technologieën staan u toe om ervoor te zorgen uw e-mails altijd bepaalde elementen (zoals een unsubscription verbinding of een onderwerpregel) of het filtreren regels bevatten om groepen van uw voorgenomen doel (zoals abonnees, concurrenten, of niet-loyaliteitklanten) uit te sluiten.

![](assets/delivery-settings-typology.png){zoomable=&quot;yes&quot;}

>[!NOTE]
>
>De typologieën en de typologieregels worden gecreeerd in de de cliëntconsole van de Campagne. Meer informatie over drukregels en hoe u vermoeidheidsbeheer kunt configureren in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/campaign-typologies.html){target="_blank"}.

### Drukparameters {#pressure-parameters}

>[!CONTEXTUALHELP]
>id="acw_email_settings_pressure_parameters"
>title="Drukparameters voor de levering"
>abstract="Met leveringsgewichten kunt u topprioriteit-leveringen identificeren in het kader van vermoeidheidsbeheer. Berichten met het hoogste gewicht hebben prioriteit."


>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_weight"
>title="Afleveringsgewicht"
>abstract="Met leveringsgewichten kunt u topprioriteit-leveringen identificeren in het kader van drukbeheer. Berichten met het hoogste gewicht hebben prioriteit."

In deze sectie kunt u met drukparameters een **drempel** om regels voor vermoeidheidsbeheer in te stellen. Dit is het maximumaantal berichten dat gedurende een bepaalde periode naar één profiel kan worden verzonden.

Zodra deze drempelwaarde is bereikt, kunnen tot het einde van de in aanmerking genomen periode geen leveringen meer plaatsvinden. Met dit proces kunt u automatisch een profiel uitsluiten van een levering als een bericht de ingestelde drempelwaarde overschrijdt. Op deze manier voorkomt u dat een profiel te vaak wordt benaderd.

Drempelwaarden kunnen constant of variabel zijn. Dit betekent dat drempelwaarden voor een bepaalde periode kunnen variëren van het ene profiel tot het andere, of zelfs voor hetzelfde profiel.

In de **[!UICONTROL Weight type]** veld zijn drie opties beschikbaar:

* **[!UICONTROL Constant]**
* **[!UICONTROL Depends on the recipient]**
* **[!UICONTROL Defined in each rule]**

Gebruik de **[!UICONTROL Delivery weight]** veld om de leveringsprioriteit te bepalen. Elke levering heeft een gewicht dat overeenkomt met het prioriteitsniveau. Standaard is het gewicht van een levering ingesteld op 5. Aan de hand van drukregels kunt u het gewicht bepalen van de leveringen waarop ze worden toegepast. U kunt het gewicht instellen of berekenen met behulp van een formule die geschikt is voor de ontvanger. U kunt bijvoorbeeld het gewicht van een levering bepalen op basis van de belangen van de ontvanger.

Gebruik de **[!UICONTROL Delivery mode]** veld om de evaluatiemodus voor het doel te selecteren. Er zijn drie modi beschikbaar:

* **[!UICONTROL Target estimation and message personalization]**
* **[!UICONTROL Estimation and approval of the provisional target]**
* **[!UICONTROL Target evaluation]**

>[!NOTE]
>
>Het beheer van de vermoeidheid wordt gevormd in de de cliëntconsole van de Campagne. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/pressure-rules.html){target="_blank"}.

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

De **[!UICONTROL Importance of the recipient]** het veld is een formule die wordt gebruikt om te bepalen welke ontvangers worden gehouden wanneer de voorschriften inzake capaciteitstypologie worden overschreden .

>[!NOTE]
>
>De typologische regels worden gevormd in de console van de Cliënt van de Campagne. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/consistency-rules.html){target="_blank"}.

## Instellingen voor publiek {#audience}

>[!CONTEXTUALHELP]
>id="acw_email_settings_audience"
>title="Instellingen voor het publiek voor de levering"
>abstract="Selecteer een **doeltoewijzing** onder de beschikbare groepen. Doeltoewijzingen worden gedefinieerd in de Adobe Campaign v8-console. U kunt ook de uitsluitingsparameters voor de levering instellen. "

In deze sectie kunt u een **doeltoewijzing** onder de beschikbare groepen. Doeltoewijzingen worden gedefinieerd in de Adobe Campaign v8-console. De doelafbeelding is het type gegevens dat een bewerking afhandelt. Hiermee kunt u de doelgroep definiëren: ontvangers, begunstigden van contracten, exploitanten, abonnees, enz.

Meer informatie over doeltoewijzingen in [deze sectie](../audience/targeting-dimensions.md).

In de **[!UICONTROL Exclusion]** in het veld kunt u selecteren om ontvangers uit te sluiten die niet meer willen worden benaderd of die in quarantaine zijn geplaatst. [Meer informatie](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html){target="_blank"}

## Levering {#delivery}

>[!CONTEXTUALHELP]
>id="acw_email_settings_delivery"
>title="Leveringsinstellingen voor de levering"
>abstract="De parameters van de levering zijn technische montages die op uw levering van toepassing zijn. U kunt de bezorgings- en routinemodi wijzigen, e-mail-BCC activeren, verzenden met golven en ook de indeling van de verzonden e-mailberichten kiezen. Deze opties zijn beperkt tot deskundige gebruikers."

**[!UICONTROL Delivery]** parameters zijn technische instellingen die van toepassing zijn op de levering.

![](assets/delivery-settings-delivery.png){zoomable=&quot;yes&quot;}

De geïntegreerde e-mail **[!UICONTROL Routing]** de externe rekening wordt standaard verschaft. Het bevat de technische parameters waarmee de applicatie e-mailberichten kan verzenden.

U kunt de **[!UICONTROL Sending]** instellingen hieronder.

* **[!UICONTROL Delivery priority]**: Gebruik deze optie om de verzendvolgorde voor uw leveringen te wijzigen door het prioriteitsniveau in te stellen op Normaal, Hoog of Laag.

* **[!UICONTROL Message batch quantity]**: Gebruik deze optie om het aantal berichten te definiëren dat binnen hetzelfde XML-leveringspakket wordt gegroepeerd. Als de parameter op 0 wordt geplaatst, worden de berichten automatisch gegroepeerd. De pakketgrootte wordt gedefinieerd door de berekening `<delivery size>/1024`, met minimaal 8 en maximaal 256 berichten per pakket.

  >[!IMPORTANT]
  >
  >Wanneer de levering door bestaande wordt gecreeerd te dupliceren, wordt deze parameter teruggesteld.

* **[!UICONTROL Test SMTP delivery]**: Deze optie wordt gebruikt om het verzenden via SMTP te testen. De levering wordt verwerkt tot verbinding aan de server SMTP, maar wordt niet verzonden: voor elke ontvanger van de levering, verbindt de Campagne met de SMTP leverancierserver, voert SMTP RCPT aan bevel uit, en sluit de verbinding vóór het bevel SMTP DATA.

* **[!UICONTROL Email BCC]**: Deze optie wordt gebruikt om e-mailberichten op een extern systeem op te slaan via BCC door eenvoudig een BCC-e-mailadres toe te voegen aan uw berichtdoel. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/config/configuration/email-settings.html){target="_blank"}.

In de **[!UICONTROL Wave definition]** selecteert u de **[!UICONTROL Send using multiple waves]** optie om het verzonden volume geleidelijk te verhogen gebruikend golven. Zo voorkomt u dat uw berichten als spam worden gemarkeerd of dat u het aantal berichten per dag wilt beperken. Met golven kunt u leveringen in verschillende batches verdelen in plaats van tegelijkertijd grote volumes berichten te verzenden. [Meer informatie](send-using-waves.md)

U kunt ook de **[!UICONTROL Mail formats]** van de e-mailberichten die worden verzonden zoals hieronder wordt beschreven.

* **[!UICONTROL Use recipient preferences]** (standaardmodus)

  De berichtindeling wordt gedefinieerd op basis van de gegevens die zijn opgeslagen in het ontvangende profiel. Als een ontvanger berichten in een bepaalde indeling wenst te ontvangen, wordt deze indeling gebruikt. Als het veld niet is ingevuld, wordt een meerdelig alternatief bericht verzonden (zie hieronder).

* **[!UICONTROL Let recipient mail client choose the most appropriate format]**

  Het bericht bevat beide indelingen: tekst en HTML. Het formaat dat op ontvangst wordt getoond hangt van de configuratie van de de postsoftware van de ontvanger (multipart-alternatief) af.

  >[!IMPORTANT]
  >
  >Deze optie omvat beide versies van het document. Het heeft daarom invloed op de leveringstarieven, omdat de berichtgrootte groter is.

* **[!UICONTROL Send all messages in text format]**

  Het bericht wordt verzonden in tekstformaat. De indeling HTML wordt niet verzonden, maar wordt alleen voor de spiegelpagina gebruikt wanneer de ontvanger op het bericht klikt.

## Webanalyse {#web-analytics}

>[!CONTEXTUALHELP]
>id="acw_email_settings_webanalytics"
>title="Webanalytische instellingen voor levering"
>abstract="Selecteer een account voor webanalyse. Deze account is geconfigureerd in de Campagne Client Console. U kunt ook de tags definiëren die worden gedeeld met het analyseprogramma dat u gebruikt."

In deze sectie kunt u een account voor webanalyse selecteren. Dit account is geconfigureerd in de Campagne-clientconsole.

U kunt ook de tags definiëren die worden gedeeld met het analyseprogramma dat u gebruikt.

>[!NOTE]
>
>De mogelijkheden van de Analytics van het Web worden gevormd in de console van de Cliënt van de Campagne. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/connect/ac-aa.html#external-account-ac){target="_blank"}.

## Opnieuw {#retries}

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_retries"
>title="Maximum aantal pogingen"
>abstract="Als een bericht mislukt als gevolg van een tijdelijke fout, worden opnieuw pogingen uitgevoerd tot het einde van de leveringsduur."

<!--Currently not visible in UI > ??-->

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

* ****[!UICONTROL Manual]****: Aan het einde van de analysefase moet de gebruiker de levering bevestigen om te beginnen met verzenden.

* **[!UICONTROL Semi-Automatic]**: Het verzenden begint automatisch als er tijdens de analysefase geen waarschuwingsberichten worden gegenereerd.

* **[!UICONTROL Automatic]**: De verzending begint automatisch aan het einde van de analysefase, ongeacht het resultaat.

## Geldigheid {#validity}

>[!CONTEXTUALHELP]
>id="acw_email_settings_validity"
>title="Geldigheid van instellingen"
>abstract="De **Leveringsduur** in dit veld kunt u de limiet voor algemene leveringspogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, regelmatig, configureerbare herpogingen worden uitgevoerd tot de geldigheidsgrens wordt bereikt.<br>De **Geldigheidslimiet voor bronnen** wordt gebruikt voor geüploade bronnen, zoals een spiegelpagina of afbeeldingen. Wanneer de limiet is bereikt, zijn de bronnen niet meer beschikbaar."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_resources_validity"
>title="Geldigheidslimiet voor bronnen"
>abstract="De **Geldigheidslimiet voor bronnen** wordt gebruikt voor geüploade bronnen, zoals de spiegelpagina of afbeeldingen. Deze bronnen gelden voor een beperkte periode: wanneer de limiet is bereikt, zijn er geen bronnen meer beschikbaar."

>[!CONTEXTUALHELP]
>id="acw_delivery_template_settings_delivery_duration"
>title="Leveringsduur"
>abstract="De **Leveringsduur** in dit veld kunt u de limiet voor algemene leveringspogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, regelmatig, configureerbare herpogingen worden uitgevoerd tot de geldigheidsgrens wordt bereikt."

<!--
>[!CONTEXTUALHELP]
>id="acw_email_settings_resources_validity"
>title="Resources validity limit"
>abstract="The Validity limit field is used for uploaded resources, such as the mirror page or images. These resources are valid for a limited time: once the limit is reached, resources are no longer available."
-->

### Geldigheidsperiode {#validity-period}

De **[!UICONTROL Delivery duration]** in dit veld kunt u de limiet voor algemene leveringspogingen invoeren. Dit betekent dat Adobe Campaign de berichten verzendt die op de begindatum beginnen, en dan, voor berichten die een fout slechts terugkeren, regelmatig, configureerbare herpogingen worden uitgevoerd tot de geldigheidsgrens wordt bereikt.

U kunt ook datums opgeven. Selecteer **[!UICONTROL Explicitly set validity dates]**. In dit geval kunt u ook de tijd opgeven op basis van de uiterste datum voor levering en geldigheid. De huidige tijd wordt standaard gebruikt, maar u kunt deze rechtstreeks wijzigen in het invoerveld.

**[!UICONTROL Resources validity limit]** wordt gebruikt voor geüploade bronnen, voornamelijk voor de spiegelpagina en afbeeldingen. De bronnen op deze pagina zijn gedurende een beperkte tijd geldig (om schijfruimte te besparen). Na deze limiet zijn deze bronnen niet meer beschikbaar.

![](assets/delivery-settings-validity.png){zoomable=&quot;yes&quot;}

<!--Change screenshot to be consistent with prod > not sure which version is correct-->

Meer informatie over de geldigheidsperiode van de levering in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaigns/send/failures/delivery-failures.html#validity-period){target="_blank"}.

### Paginabeheer spiegelen {#mirror}

De spiegelpagina is een HTML-pagina die online toegankelijk is via een webbrowser. De inhoud is identiek aan de e-mail. Standaard wordt de spiegelpagina gegenereerd als de koppeling wordt ingevoegd in de inhoud van de e-mail.

Naast de standaardmodus zijn ook de volgende opties beschikbaar:

* **[!UICONTROL Force the generation of the mirror page]**: Gebruik deze modus om de spiegelpagina te genereren, zelfs als er geen koppeling naar de spiegelpagina is ingevoegd in de levering.
* **[!UICONTROL Do not generate the mirror page]**: Gebruik deze modus om te voorkomen dat een spiegelpagina wordt gegenereerd, zelfs als de koppeling aanwezig is in de levering.
* **[!UICONTROL Generates a mirror page accessible using only the message identifier]**: Wanneer de koppeling naar de spiegelpagina niet aanwezig is in de e-mailinhoud, gebruikt u deze optie om toegang tot de inhoud van de spiegelpagina, in het venster van het leveringslogboek, vanaf de clientconsole in te schakelen.


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

**[!UICONTROL Tracking]** parameters worden gedefinieerd in het desbetreffende gedeelte. Mogelijke opties zijn:

**[!UICONTROL Tracking validity limit]**: Gebruik deze optie als u de tijdsduur wilt wijzigen gedurende welke de tekstspatiëring op de URL&#39;s wordt geactiveerd.

**[!UICONTROL Substitution URL for expired URLs]**: Gebruik deze optie om een URL in te voeren naar een fallback-webpagina: deze wordt weergegeven zodra de tekstspatiëring is verlopen.

## Proefinstellingen {#test-setttings}

>[!CONTEXTUALHELP]
>id="acw_email_settings_testsettings"
>title="De proefdrukinstellingen voor de levering definiëren"
>abstract="Selecteer de uitsluitingsparameters en pas het label van de proefdrukken aan."

<!--Test to be replaced with Proof everywhere - currently not consistent within UI > changed to Proof to reflect UI here but not consistent in documentation either-->

U kunt de uitsluitingsparameters in deze sectie instellen. Beschikbare opties zijn:

* ****[!UICONTROL Keep doubles]**** Hiermee kunt u meerdere leveringen toestaan aan ontvangers die aan verschillende doelcriteria voldoen.

* **[!UICONTROL Keep denylisted addresses]** Hiermee kunt u profielen die niet meer het doelprofiel zijn van levering, zoals na een abonnement (opt-out), niet meer als doel instellen.

* **[!UICONTROL Keep quarantined addresses]** Hiermee kunt u profielen met een adres dat niet reageert, behouden van het doel.

U kunt ook de tabel van de proefdrukken aanpassen:

* Gebruik de **[!UICONTROL Keep the delivery code for the proof]** aan het bewijs dezelfde leveringscode te koppelen als die welke is vastgesteld voor de levering waarop het betrekking heeft.

* Standaard wordt het onderwerp van de proefdruk voorafgegaan door &#39;PROOF #&#39;, waarbij # het nummer van de proefdruk is. U kunt dit voorvoegsel wijzigen in het dialoogvenster **[!UICONTROL Label prefix]** veld.