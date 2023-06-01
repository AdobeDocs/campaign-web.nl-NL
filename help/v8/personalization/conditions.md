---
title: Voorwaardelijke content maken
description: Leer hoe u voorwaarden definieert voor het aanpassen van uw inhoud in de gebruikersinterface van Adobe Campaign
feature: Personalization
topic: Personalization
role: Data Engineer
level: Beginner
badge: label="Alpha" type="Positief"
exl-id: b650a859-e27d-4a36-a725-a1f5bb31e014
source-git-commit: 5598a82bf745659b8c1db8cb51b1a82cfd184093
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 2%

---

# Voorwaardelijke inhoud maken{#add-conditions}

>[!CONTEXTUALHELP]
>id="acw_homepage_card3"
>title="Voorwaardelijke content maken"
>abstract="Maak voorwaardelijke inhoud om dynamische personalisatie te definiëren op basis van het profiel van de ontvanger, waarbij tekstblokken en afbeeldingen automatisch worden vervangen wanneer aan bepaalde voorwaarden wordt voldaan. Met deze functie kunt u uw campagnes op een hoger niveau brengen en uw publiek een zeer doelgerichte, persoonlijke ervaring bieden."


Voorwaardelijke inhoud is een krachtige functie waarmee u een dynamische personalisatie kunt maken op basis van het profiel van de ontvanger, waarbij tekstblokken en afbeeldingen automatisch worden vervangen wanneer aan bepaalde voorwaarden wordt voldaan. Met deze functie kunt u uw campagnes op een hoger niveau brengen en uw publiek een zeer doelgerichte, persoonlijke ervaring bieden.

Door voorwaardelijke inhoudsgebieden te vormen, kunt u geavanceerde dynamische verpersoonlijking tot stand brengen die op het profiel van de ontvanger bijvoorbeeld wordt gebaseerd. Tekstblokken, koppelingen, onderwerpregel en/of afbeeldingen worden vervangen in de inhoud van het bericht als aan een bepaalde voorwaarde is voldaan. U kunt bijvoorbeeld &#39;Mr&#39; of &#39;Mevrouw&#39; weergeven op basis van de waarde van het genderveld in de database van Adobe Campaign, of een andere link opnemen op basis van de voorkeurstaal van de ontvanger.

## Personalisatiesyntaxis{#perso-syntax}



## Werken met voorwaarden in de verpersoonlijkingseditor{#condition-perso-editor}

Een voorwaardelijke inhoud definiëren voor een levering:

1. Open een levering en bewerk de inhoud.
1. Klik op de knop **[!UICONTROL Open personalization dialog]** pictogram, bijvoorbeeld, voor SMS, op het recht van het gebied van het Bericht.

   ![](assets/open-perso-editor-sms.png)

1. Blader in de verpersoonlijkingseditor naar **[!UICONTROL Helper functions]**.
1. Klik op het pictogram ‘+’ naast het pictogram **Indien** functie. De volgende regel wordt toegevoegd aan het centrale scherm:
   `<% if (<FIELD>==<VALUE>) { %>Insert content here<% } %>`
1. Vervangen `<FIELD>` door een verpersoonlijkingsveld. Bijvoorbeeld het bedrijf van de ontvanger: `recipient.company`.
1. Vervangen `<VALUE>` met een waarde waaraan moet worden voldaan. Bijvoorbeeld, `ADOBE`.




## Voorbeeld: voorwaardelijke SMS-onderwerpregel{#condition-subject-line}

Voer de volgende stappen uit om een voorwaardelijke onderwerpregel voor een SMS-bericht te maken:

1. Open een levering en bewerk de inhoud.
1. Klik op het pictogram van het dialoogvenster Aanpassing openen rechts van de onderwerpregel.
1. Blader in de verpersoonlijkingseditor naar


```sql
<% if 
(recipient.email == 'recipient@domain.com' ) 
{ % >
<table>
    <tr>
        <td>variant A</td>
    </tr>
</table>
< % } 
else 
{ % >
<table>
    <tr>
        <td>variant B< td>
    </tr>
</table>
< % } 
%>
```
