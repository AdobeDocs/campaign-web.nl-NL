---
audience: end-user
title: Verbeterde e-mailontwerpervaring
description: Leer hoe u het maken van e-mail kunt stroomlijnen met herbruikbare thema's en modules, zodat uw campagnes consistent en efficiënt zijn.
badge: label="Beperkte beschikbaarheid" type="Informative"
feature: Email Design
topic: Content Management
role: User
level: Beginner, Intermediate
keywords: E-mailthema's, modules, herbruikbaarheid, consistentie van merk, e-mailontwerp, aangepaste CSS, mobiele optimalisatie
exl-id: c9e02bca-032d-4771-ad53-5bbebabc4c5d
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '1996'
ht-degree: 0%

---

# Thema&#39;s toepassen op uw e-mailinhoud {#apply-email-themes}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn2"
>title="Thema&#39;s in de e-mail-Designer (LA)"
>abstract="Pas herbruikbare themastijlen en -variabelen toe om e-mailinhoud consistent te houden met uw merk. Deze mogelijkheid is alleen beschikbaar voor een aantal organisaties (beperkte beschikbaarheid)"
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=nl-NL" text="Zie opmerkingen bij releases"

>[!CONTEXTUALHELP]
>id="acw_email_apply_theme"
>title="Een thema toepassen op uw e-mail"
>abstract="Selecteer een thema voor uw e-mail om snel een specifieke stijl toe te passen die aan uw merk en ontwerp past."

>[!AVAILABILITY]
>
>Deze mogelijkheid is in Beperkte Beschikbaarheid. Neem contact op met uw Adobe-vertegenwoordiger voor toegang.

Met thema&#39;s, hebben de niet-technische gebruikers de capaciteit om herbruikbare inhoud tot stand te brengen die een specifiek merk en een ontwerptaal door douanemateriaal bovenop de standaardmalplaatjes <!-- to achieve brand specific results--> toe te voegen past.

Deze functie stelt marketers in staat visueel aantrekkelijke, merkgebonden e-mails sneller en met minder moeite te gebruiken en biedt geavanceerde aanpassingsopties voor unieke ontwerpbehoeften.

## Afvoerkanalen en beperkingen {#themes-guardrails}

* Wanneer u een volledig nieuw e-mailbericht maakt, kunt u uw inhoud op basis van een thema maken en snel een specifieke stijl toepassen die past bij uw merk en ontwerp.

  Als u de modus Handmatig opmaken kiest, kunt u alleen thema&#39;s toepassen als u uw e-mail opnieuw instelt.

* [&#x200B; de Fragmenten &#x200B;](../content/fragments.md) zijn niet dwars-compatibel tussen de Thema&#39;s van het Gebruik en de Hand het Stileren wijzen.

   * Geachte fragmenten zijn niet beschikbaar in e-mailinhoud die zonder thema&#39;s is gemaakt.

   * Aan hefboomwerking a [&#x200B; fragment &#x200B;](../content/fragments.md) in een thema inhoud, moet dit fragment zelf tot stand gebracht hebben gebruikend thema&#39;s. [&#x200B; Leer meer &#x200B;](#leverage-themes-fragment)

   * Wanneer u een fragment in e-mailinhoud gebruikt, moet u een thema toepassen dat u voor dit fragment hebt gedefinieerd. Als u dit niet doet, kunnen er weergaveproblemen optreden, met name in Outlook 2021 en eerdere versies. [&#x200B; Leer meer &#x200B;](#leverage-themes-fragment)

* Als het gebruiken van inhoud die in HTML wordt gecreeerd, zult u op [&#x200B; verenigbaarheidswijze &#x200B;](existing-content.md) zijn en u kunt geen thema&#39;s op deze inhoud direct toepassen.

   * Om thema&#39;s toe te passen, moet u eerst de ingevoerde inhoud [&#x200B; als nieuw malplaatje &#x200B;](../content/create-email-templates.md#save-as-template) bewaren, dan dit malplaatje in een thema-compatibele inhoud omzetten. Vervolgens kunt u deze sjabloon gebruiken om uw e-mailinhoud te maken. Leer hoe te om een malplaatje om te zetten dat met handhet stileren in [&#x200B; wordt gecreeerd deze sectie &#x200B;](#theme-convertor).

   * U kunt uw geïmporteerde HTML-inhoud ook converteren. [&#x200B; Leer meer &#x200B;](existing-content.md)

  <!--To fully leverage all the capabilities of the Email Designer, including themes, you must either create a new content in Use Themes mode, or convert your imported HTML content. [Learn more](existing-content.md)-->

* Houd er rekening mee dat veel e-mailclients deze niet ondersteunen wanneer u aangepaste weblettertypen (inclusief Google-lettertypen) in uw thema&#39;s gebruikt. Definieer altijd de juiste fallback-lettertypen in uw thema om ervoor te zorgen dat deze leesbaar zijn voor alle e-mailclients.

   * Gmail en Yahoo! externe weblettertypen niet laden en worden teruggeplaatst naar systeemlettertypen, ongeacht de lettertypefamilie die in de HTML/CSS is opgegeven.
   * De enige Google-lettertypen die door Gmail worden ondersteund, zijn Roboto en Google Sans.
   * E-mailcliënten die ** steunen Webdoopvonten omvatten de Post van Apple, de Post van iOS, de Post van Android, Thunderbird, en Vooruitzichten voor macOS.

<!--If you apply a theme to a content using a [fragment](../content/fragments.md) created with Manual Styling mode, the rendering may not be optimal.-->

## Een thema maken {#create-and-edit-themes}

Volg onderstaande stappen om een thema te definiëren dat u in uw toekomstige e-mailinhoud kunt gebruiken.

1. Om begonnen te worden, creeer een nieuw [&#x200B; inhoudsmalplaatje &#x200B;](../content/create-email-templates.md).

1. Selecteer de optie **[!UICONTROL Create or edit themes]** .

   ![&#x200B; de redacteur van het malplaatje van de Inhoud die Create of geeft themaoptie uit &#x200B;](assets/theme-create.png)

1. Selecteer een Adobe-thema. In dit voorbeeld selecteert u **[!UICONTROL Default theme]** en klikt u op **[!UICONTROL Create]** .

   ![&#x200B; de plukker van het Thema met Standaard geselecteerd thema en creeer knoop &#x200B;](assets/theme-select.png)

1. U kunt ook een aangepaste sjabloon selecteren op het tabblad **[!UICONTROL My themes]** en op **[!UICONTROL Edit]** klikken om deze bij te werken.

   ![&#x200B; Mijn thema&#39;s maken een lijst van douanethema&#39;s met Edit benadrukte &#x200B;](assets/theme-edit.png)

1. Definieer op het tabblad **[!UICONTROL General settings]** het thema door het een specifieke naam te geven die aansluit bij uw merk. U kunt de standaardviewportbreedte voor uw e-mails aanpassen <!--and also export the current theme for reuse-->.

   <!--![General settings tab for theme name, viewport width, and export](assets/theme-general-settings.png)-->

1. Gebruik de rail rechts om door de verschillende lusjes te navigeren en uw ontwerpmontages bij te werken.

   ![&#x200B; Rechte spoorlijn van de redacteur van het Thema met lusjes voor kleuren, tekst, het uit elkaar plaatsen, en andere ontwerpmontages &#x200B;](assets/theme-right-pane.png)

1. Op het tabblad **[!UICONTROL Colors]** :

   * Gebruik de knop **[!UICONTROL Edit]** om een **[!UICONTROL Color palette]** met standaardkleuren voor uw merk in te stellen. Selecteer een **[!UICONTROL Preset]** om snel een kleurenschema te maken of pas elke kleur van uw thema afzonderlijk aan. U kunt ook een combinatie van beide gebruiken.

     ![&#x200B; Animatie van het uitgeven van het palet van de themakleur met vooraf instelt en douanekleuren &#x200B;](assets/theme-colors.gif)

   * Klik op **[!UICONTROL Add variant]** om meerdere kleurvarianten te maken, zoals de modus Licht en Donker, waarbij elke variant van het thema een eigen kleurenpalet en nuantiebesturingselementen heeft.

     ![&#x200B; de Varianten van de Kleur in de themaredacteur met Add variant voor extra paletten &#x200B;](assets/theme-colors-variant.png)

   * Klik voor elke variant op het pictogram **[!UICONTROL Edit]** om een afzonderlijk element te bewerken. U kunt het standaardpalet gebruiken dat u hebt gemaakt, of aangepaste kleuren.

     ![&#x200B; Animatie van het uitgeven van individuele kleuren binnen een variant van de themakleur &#x200B;](assets/theme-colors-edit-variant.gif)

1. In **[!UICONTROL Text settings]** kunt u het algemene lettertype instellen dat u voor het hele thema wilt gebruiken. Voor meer korrelige besturingselementen kunt u ook elk kop- en alineatekst bewerken om het lettertype, de grootte, de stijl enzovoort aan te passen.

   ![&#x200B; de montages van de Tekst tabel voor globale doopvont en rubriek of paragraafstijlen in een thema &#x200B;](assets/theme-text.png)

   >[!NOTE]
   >
   >Houd er bij het selecteren van aangepaste weblettertypen rekening mee dat veel e-mailclients, zoals Gmail en Yahoo! geen ondersteuning bieden voor externe weblettertypen en worden de systeemlettertypen gebruikt. Overweeg ook fallback-lettertypen op te nemen om ervoor te zorgen dat de inhoud correct wordt weergegeven voor alle e-mailclients. [&#x200B; Leer meer &#x200B;](#themes-guardrails)

1. Selecteer op het tabblad **[!UICONTROL Spacing]** een afzonderlijk element in de lijst om de ruimte tussen de verschillende componenten op de juiste wijze te bepalen.

   <!--![Spacing tab listing structure elements to adjust spacing between components](assets/theme-spacing.png)-->

1. Met de andere tabbladen aan de rechterkant kunt u elk knopelement, elke scheidingslijn, elke extra afbeeldingsopmaak en de ruimte tussen de rasterlay-outs voor dit thema afzonderlijk beheren.

   ![&#x200B; Knop die controles stileren in de het juiste spoor van de themageditor &#x200B;](assets/theme-buttons.png)

1. Klik op **[!UICONTROL Save]** om dit thema op te slaan voor toekomstig gebruik. Deze wordt nu weergegeven op het tabblad **[!UICONTROL My themes]** .

<!--A little strange upon hitting Save, because once the theme is created, you need to hit Close to go back to Design your template screen, then click Cancel if you don't want to proceed with template creation.-->

## Thema&#39;s toepassen op e-mailinhoud {#apply-themes-email}

Voer de onderstaande stappen uit om standaard- of aangepaste opmaakthema&#39;s toe te passen op een inhoudssjabloon of een e-mail.

1. In [!DNL Adobe Campaign], [&#x200B; creeer een e-maillevering &#x200B;](create-email.md) of het werk van een bestaande levering, of creeer een e-mail [&#x200B; inhoudsmalplaatje &#x200B;](../content/create-email-templates.md#create-template-from-scratch), en [&#x200B; geef de e-mailinhoud &#x200B;](get-started-email-designer.md#start-authoring) uit.

1. U kunt een van de volgende handelingen selecteren:

   * Selecteer een ingebouwde [&#x200B; e-mailmalplaatje &#x200B;](../content/use-email-templates.md) om e-mail Designer te openen. Er wordt automatisch een standaardthema toegepast dat specifiek is voor elke sjabloon.

   * Ontwerp a [&#x200B; nieuwe inhoud van kras &#x200B;](create-email-content.md) en selecteer **[!UICONTROL Use Themes]** om met een vooraf bepaald het stileren thema te beginnen.

     ![&#x200B; het beginscherm van Designer van de E-mail met de Thema&#39;s van het Gebruik en de Handmatige het Stijlen opties &#x200B;](assets/theme-from-scratch.png)

     >[!CAUTION]
     >
     >Als u de modus Handmatig opmaken kiest, kunt u alleen thema&#39;s toepassen als u het ontwerp opnieuw instelt.
     >
     >Aan hefboomwerking a [&#x200B; fragment &#x200B;](../content/fragments.md) in een thema inhoud, moet dit fragment zelf tot stand gebracht hebben gebruikend thema&#39;s. [&#x200B; Leer meer &#x200B;](#leverage-themes-fragment)

1. Klik eenmaal in de e-mail-Designer op de knop **[!UICONTROL Themes]** op de rechtertrack. Het standaardthema of het thema van de sjabloon wordt weergegeven. U kunt schakelen tussen de twee kleurvarianten voor dit thema.

   ![&#x200B; het canvas van Designer e-mail met het open paneel van Thema&#39;s die het actieve thema en de kleurenvarianten tonen &#x200B;](assets/theme-default-hero.png)

1. Klik op de pijl naast het thema dat momenteel wordt gebruikt. De lijst met beschikbare aangepaste thema&#39;s en Adobe-thema&#39;s wordt weergegeven.

   ![&#x200B; dropdown van het Thema werd uitgebreid om de thema&#39;s van Adobe en Mijn thema&#39;s te tonen &#x200B;](assets/theme-hero-change.png)

1. Klik op **[!UICONTROL My themes]** en selecteer een thema dat u hebt gemaakt.

   ![&#x200B; Mijn themalijst met een user-created thema dat in de themakiezer &#x200B;](assets/theme-select-custom.png) wordt geselecteerd

1. Klik buiten de vervolgkeuzelijst. Het nieuwe, aangepaste thema past automatisch de stijlen toe op alle e-mailcomponenten. U kunt schakelen tussen de eventuele kleurvarianten.

1. Wanneer een thema is geselecteerd in een inhoudssjabloon, kunt u op de knop **[!UICONTROL Edit theme]** klikken om het thema bij te werken. [&#x200B; Leer meer &#x200B;](#create-and-edit-themes)

   ![&#x200B; malplaatje van de Inhoud in E-mail Designer met Edit themaknoop in het paneel van Thema&#39;s &#x200B;](assets/theme-edit-in-template.png){width="40%"}

   >[!NOTE]
   >
   >Deze optie is niet beschikbaar als u thema&#39;s in e-mailinhoud gebruikt.

1. Als u een thema gebruikt met verschillende kleurvarianten, kunt u een specifieke variant kiezen voor een bepaalde structuurcomponent. Zo kunt u een kleurvariant definiëren voor de gehele inhoud en een andere variant gebruiken voor slechts één specifieke structuur.

   >[!NOTE]
   >
   >U kunt deze handeling niet uitvoeren op inhoudscomponenten.

   Hiervoor selecteert u een structuurcomponent, klikt u op **[!UICONTROL Use specific theme's variant option]** op het tabblad **[!UICONTROL Styles]** rechts en past u de gewenste variant op die structuur toe.

   ![&#x200B; Geselecteerde structuur met de variant van het thema van het Gebruik specifieke optie in het lusje van Stijlen &#x200B;](assets/theme-structure-variant.png)

   In dit voorbeeld wordt de eerste kleurvariant van het huidige thema toegepast op de hele e-mailinhoud, maar wordt de derde kleurvariant toegepast op de geselecteerde structuur. U ziet dat de achtergrondkleuren van de hoofdtekst en viewport voor die specifieke structuur afwijken van de rest van de inhoud.

U kunt op elk gewenst moment naar een ander thema gaan. De e-mailinhoud blijft ongewijzigd, maar de stijlen worden bijgewerkt met het nieuwe thema.

### Stijlen ontgrendelen {#unlocking-styles}

Wanneer een component is geselecteerd, kunt u de stijl ontgrendelen met het toegewezen pictogram op het tabblad **[!UICONTROL Styles]** .

![&#x200B; het lusje van Stijlen op een geselecteerde component die het ontgrendelingspictogram tonen &#x200B;](assets/theme-unlock-style.png){width="90%"}

Het geselecteerde thema wordt nog steeds op die component toegepast, maar u kunt de opmaakelementen ervan overschrijven. Als u thema&#39;s verandert, wordt het nieuwe thema slechts toegepast op het stileren elementen die niet met voeten werden getreden.<!--can you revert this action?-->

Bijvoorbeeld, als u een tekstcomponent ontgrendelt, kunt u <!--the font size from 11 to 14 and --> de doopvontkleur van zwart in rood veranderen:

![&#x200B; Ontgrendelde tekstcomponent met de kleur van de douanerood tekst op een witte achtergrond &#x200B;](assets/theme-unlock-style-ex-white.png){width="80%" align="center" zoomable="yes"}

Als u thema&#39;s verandert, <!--the font size is still 14 and --> is de doopvontkleur nog rood voor die component, maar de achtergrondkleur voor deze component zal met het nieuwe thema veranderen:

![&#x200B; Zelfde ontgrendelde tekst met rode kleur behouden en achtergrond bijgewerkt van een nieuw thema &#x200B;](assets/theme-unlock-style-ex-colored.png){width="80%"}

## Thema&#39;s in een fragment gebruiken {#leverage-themes-fragment}

Om een fragment in een malplaatje of een e-mail met [&#x200B; toegepaste thema&#39;s &#x200B;](#apply-themes-email) te hefboomwerking, moet dit fragment tot stand zijn gebracht zelf gebruikend thema&#39;s. Anders kunt u dit fragment niet gebruiken in de inhoud van het thema.

Voer de onderstaande stappen uit om een fragment te maken dat compatibel is met thema&#39;s.

1. Maak in [!DNL Adobe Campaign] een visueel fragment en klik op **[!UICONTROL Create]** om de inhoud van het fragment te ontwerpen. [&#x200B; leer hoe &#x200B;](../content/create-fragment.md#create-from-scratch)

1. Selecteer **[!UICONTROL Use Themes]** om te beginnen met een vooraf gedefinieerd opmaakthema.

   ![&#x200B; de beginopties van Designer van het Fragment E-mail met Geselecteerde Thema&#39;s van het Gebruik &#x200B;](assets/fragment-use-themes.png){width="100%"}

   >[!CAUTION]
   >
   >Als u de modus Handmatig opmaken kiest, kunt u alleen thema&#39;s toepassen als u het fragmentontwerp opnieuw instelt.

1. Eenmaal in de e-mail-Designer kunt u beginnen met het maken van het fragment.

1. Klik op de knop **[!UICONTROL Themes]** op de rechterrails. Het standaardthema wordt weergegeven. U kunt schakelen tussen de verschillende kleurvarianten voor dit thema.

   ![&#x200B; de inhoud van het fragment in E-mail Designer met de spoorstaaf van Thema&#39;s die het standaardthema &#x200B;](assets/fragment-default-theme.png){width="100%" align="center" zoomable="yes"} tonen

1. U kunt andere thema&#39;s selecteren om een voorvertoning van uw fragmentinhoud weer te geven. Selecteer hiertoe de pijl naast het standaardthema en klik op **[!UICONTROL Select themes]** .

   ![&#x200B; de kopbal van het Thema met pijl en Uitgezochte themacontrole voor fragmentvoorproef &#x200B;](assets/fragment-select-themes.png){width="40%"}

1. U kunt navigeren tussen de tabbladen **[!UICONTROL Adobe themes]** en **[!UICONTROL My themes]** en maximaal vijf compatibele thema&#39;s (van beide tabbladen) voor het fragment selecteren.

   ![&#x200B; Uitgezochte compatibele themadialoog met de thema&#39;s van Adobe en Mijn themalusjes &#x200B;](assets/fragment-select-compatible-themes.png){width=70%}

   >[!CAUTION]
   >
   >Wanneer het gebruiken van het fragment in een e-mailinhoud, zorg ervoor u [&#x200B; een thema &#x200B;](#apply-themes-email) toepast dat u voor dit fragment hebt bepaald. Als u dit niet doet, kunnen er weergaveproblemen optreden, met name in Outlook 2021 en eerdere versies.

1. Klik op **[!UICONTROL Close]** .

1. Selecteer nogmaals de pijl naast de **[!UICONTROL Default theme]** . U kunt nu schakelen tussen de verschillende thema&#39;s die u net hebt geselecteerd om elke stijlrendering te bekijken.

   ![&#x200B; het canvas van het Fragment met veelvoudige thema&#39;s die voor voorproef in het paneel van Thema&#39;s worden geselecteerd &#x200B;](assets/fragment-selected-themes.png){width=90%}

1. Klik nogmaals op **[!UICONTROL Select themes]** om meer thema&#39;s toe te voegen of uw selectie te wijzigen.

## Een sjabloon compatibel maken met thema&#39;s {#theme-convertor}

Met [!DNL Adobe Campaign] kunt u een sjabloon die met handmatige opmaak is gemaakt, omzetten in inhoud die compatibel is met thema&#39;s. Dit is vooral handig als u inhoudssjablonen hebt gemaakt voordat thema&#39;s werden geïntroduceerd in [!DNL Adobe Campaign] of als u externe inhoud importeert.

>[!NOTE]
>
> Slechts **e-mailmalplaatjes** kunnen worden omgezet om compatibel met thema&#39;s te zijn. Afzonderlijke e-mails kunnen niet worden geconverteerd. U moet uw inhoud eerst als een sjabloon opslaan.

1. Open een e-mail [&#x200B; inhoudsmalplaatje &#x200B;](../content/create-email-templates.md) en geef zijn inhoud uit gebruikend E-mail Designer.

1. Selecteer het pictogram **[!UICONTROL Themes]** op de rechterrails en klik op de knop **[!UICONTROL Generate theme from content]** .

   ![&#x200B; het paneel van Thema&#39;s met produceer thema van benadrukte inhoudsknoop &#x200B;](assets/generate-theme.png){width=100%}

1. Het venster **[!UICONTROL Create a theme]** wordt geopend. [!DNL Adobe Campaign] detecteert automatisch de opmaakelementen en consolideert deze in een nieuw thema.

   ![&#x200B; creeer een themadialoog die stijlen samenvatten van malplaatjeinhoud &#x200B;](assets/generate-theme-create-window.png){width=90%} worden ontdekt

1. Geef een naam op voor uw thema.

1. Breng desgewenst uw eigen aanpassingen aan, net als bij het maken van een geheel nieuw thema, zoals het toevoegen van een kleurvariant, het bewerken van lettertypen enzovoort. [&#x200B; leer hoe &#x200B;](#create-and-edit-themes)

   ![&#x200B; Gegenereerd thema in de redacteur die kleurenpalet en variantcontroles tonen &#x200B;](assets/generate-theme-colors.png){width=90%}

1. Klik op **[!UICONTROL Save]** om dit nieuwe thema op te slaan voor hergebruik. U kunt dit thema nu toepassen op inhoud, zoals elk ander thema. [&#x200B; leer hoe &#x200B;](#apply-themes-email)
