---
title: Opsommingen beheren
description: Leer hoe u met opsommingen werkt
exl-id: d2a30fef-2cc4-49af-9f5d-d42c6396a8ab
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Opsommingen beheren {#enumerations}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn4"
>title="Opsommingen maken"
>abstract="U kunt opsommingen nu rechtstreeks maken via de Adobe Campaign Web User Interface. Een opsomming is een lijst met waarden die door het systeem worden voorgesteld om velden te vullen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html?lang=nl-NL" text="Zie opmerkingen bij releases"

>[!CONTEXTUALHELP]
>id="acw_enumerations_list"
>title="Opsommingen"
>abstract="Een opsomming is een lijst met waarden die door het systeem worden voorgesteld om velden te vullen. Gebruik opsommingen om de waarden van deze velden te standaardiseren, hulp bij gegevensinvoer of gebruik binnen query&#39;s."

>[!CONTEXTUALHELP]
>id="acw_enumerations_properties"
>title="Properties"
>abstract="Definieer de eigenschappen van de opsomming, zoals de naam, de interne naam en het type. **[!UICONTROL Closed]** opsommingen hebben een vaste lijst met waarden die alleen via het menu **[!UICONTROL Enumerations]** kunnen worden gewijzigd. Met **[!UICONTROL Open]** -opsommingen kunnen gebruikers rechtstreeks nieuwe waarden toevoegen in de velden die op deze opsomming zijn gebaseerd. **[!UICONTROL System]** opsommingen zijn gekoppeld aan systeemvelden. **[!UICONTROL Emoticon]** opsommingen worden gebruikt om de emoticonlijst bij te werken."

>[!CONTEXTUALHELP]
>id="acw_enumerations_values"
>title="Lijst met opsommingswaarden"
>abstract="Als u een waarde aan de opsomming wilt toevoegen, klikt u op de knop **[!UICONTROL Add value]** en configureert u deze zo nodig."

## Wat zijn opsommingen? {#about}

Een opsomming is een lijst met waarden die door het systeem worden voorgesteld om velden te vullen. Gebruik opsommingen om de waarden van deze velden te standaardiseren, hulp bij gegevensinvoer of gebruik binnen query&#39;s. De lijst met waarden wordt weergegeven als een vervolgkeuzelijst waaruit u de waarde kunt selecteren die in het veld moet worden ingevoerd. In de vervolgkeuzelijst is ook voorspelbare invoer mogelijk: voer de eerste letters in en de toepassing vult de rest in.

De waarden voor dit type veld worden gedefinieerd via het menu **[!UICONTROL Administration]** / **[!UICONTROL Enumerations]** in het linkernavigatievenster.

![ Lijst van de Opsomming die in het menu van het Beleid ](assets/enumeration-list.png) wordt getoond

## Een opsomming maken {#create}

Ga als volgt te werk om een opsomming te maken:

1. Navigeer naar het menu **[!UICONTROL Enumerations]** en klik op de knop **[!UICONTROL Create enumeration]** .

1. Voer een **[!UICONTROL Label]** en een **[!UICONTROL Internal name]** in voor de opsomming.

   ![ creeer opsommingsscherm dat etiket en interne naamgebieden toont ](assets/enumeration-create.png)

1. Selecteer de opsomming **[!UICONTROL Type]** :

   * **[!UICONTROL Closed]** opsommingen hebben een vaste lijst met waarden die alleen via het menu **[!UICONTROL Enumerations]** kunnen worden gewijzigd.
   * Met **[!UICONTROL Open]** -opsommingen kunnen gebruikers rechtstreeks nieuwe waarden toevoegen in de velden die op deze opsomming zijn gebaseerd.
   * **[!UICONTROL System]** opsommingen zijn gekoppeld aan systeemvelden.
   * **[!UICONTROL Emoticon]** opsommingen worden gebruikt om de emoticonlijst bij te werken.

1. Klik op **[!UICONTROL Create]**. De weergave van de opsommingsdetails, waarmee u waarden aan de lijst kunt toevoegen.

   ![ het scherm van de detail van de Opsomming die opties tonen om waarden toe te voegen ](assets/enumeration-details.png)

1. Als u een waarde wilt toevoegen, klikt u op de knop **[!UICONTROL Add value]** en configureert u deze vervolgens naar wens:

   * **[!UICONTROL Label]**: Het label dat in de opsomming moet worden weergegeven.
   * **[!UICONTROL Internal name]**: de interne naam van de waarde (voor systeemopsommingen).
   * **[!UICONTROL U+ (internal name)]** (emoticon opsommingen): De unicode-code voor het emoticon (voor emoticon opsommingen).

   ![ voeg waardescherm toe die gebieden voor etiket, interne naam, en unicode code tonen ](assets/enumeration-emoticon.png)

1. Sla uw wijzigingen op. De opsomming wordt bijgewerkt in de schermen waar deze wordt gebruikt.

## Hoofdlettergebruik: vooraf gedefinieerde waarden toevoegen aan een opsomming {#uc}

Standaard kunnen gebruikers met het veld Oorsprong in het scherm met profieldetails elke waarde vrij invoeren.

![ de detailsscherm die van het Profiel het gebied van de Oorsprong tonen ](assets/enumeration-uc-profile.png)

Elke keer dat een gebruiker een waarde voor het veld invoert, wordt de waarde automatisch toegevoegd aan de opsomming &#39;Oorsprong&#39;. Dit kan in de loop der tijd leiden tot overbodige, inconsistente of onjuiste waarden in de lijst met waarden.

![ opsomming van de Oorsprong die inconsistente user-entered waarden ](assets/enumeration-uc-choice.png) tonen

Definieer een set vooraf gedefinieerde waarden om de consistentie van de gegevens te garanderen en gebruikers te helpen bij het invullen van het veld. Voer de volgende stappen uit:

1. Ga naar het menu **[!UICONTROL Enumerations]** en open de opsomming &quot;Oorsprong&quot;.

2. Controleer de lijst met door de gebruiker ingevoerde waarden en pas deze op. Klik op de knop met de ellips naast een waarde om deze te verwijderen. Als de lijst te veel inconsistenties bevat, verwijdert u de volledige opsomming en maakt u deze helemaal opnieuw.

   ![ het Scherm die opties tonen om user-Enter waarden ](assets/enumeration-uc-clean.png) op te schonen

3. Voeg vooraf gedefinieerde waarden toe. Klik hiertoe op de knop **[!UICONTROL Add value]** en voer de vooraf gedefinieerde waarden in die gebruikers moeten selecteren.

   ![ het Scherm die vooraf bepaalde waarden tonen die aan de opsomming worden toegevoegd ](assets/enumeration-uc-create.png)

4. Als u consistentie wilt afdwingen, schakelt u het opsommingstype over op **[!UICONTROL Closed]** . Hiermee beperkt u gebruikers tot vooraf gedefinieerde waarden. Als flexibiliteit nodig is, houdt u deze **[!UICONTROL Open]** aan om invoer van nieuwe gebruikers toe te staan.

5. Ga terug naar het scherm met profieldetails. In het veld Oorsprong worden nu de vooraf gedefinieerde waarden voor de selectie weergegeven.

   ![ de detailsscherm die van het Profiel vooraf bepaalde waarden op het gebied van de Oorsprong tonen ](assets/enumeration-uc-populated.png)