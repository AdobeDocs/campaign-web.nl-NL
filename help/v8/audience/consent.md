---
audience: end-user
title: Toestemming
description: Meer informatie over toestemming op Adobe Campaign Web
badge: label="Beperkte beschikbaarheid"
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 6%

---

# Toestemming beheren {#manage-consent}

## Algemene aanbevelingen {#general-recommendations}

Met Adobe Campaign kunt u gegevens verzamelen, waaronder persoonlijke en gevoelige informatie. Het is van essentieel belang dat de ontvangers hun toestemming verkrijgen en controleren in overeenstemming met gegevensbeschermingsvoorschriften zoals de GDPR (General Data Protection Regulation) en andere toepasselijke privacywetten.

* U moet zich eerst onthouden van het verzenden van ongewenste e-mail, pushberichten en SMS-berichten (&quot;spam&quot;). Adobe steunt sterk de principes van toestemmings marketing om de waarde en de loyaliteit van het klantenleven te bevorderen. Adobe verbiedt het gebruik van Adobe Campaign voor het verzenden van ongevraagde berichten. [Meer informatie](#denylisted-profiles)

* Zorg altijd ontvangers akkoord gaan om mededelingen te ontvangen door hen de capaciteit te verstrekken om van uw leveringen <!-- and keep honoring opt-out requests as quickly as possible--> te weigeren. [Meer informatie](#opt-out)

* Gebruik het abonnementbeheerproces om de voorkeuren van ontvangers te beheren en te volgen welke ontvangers hebben gekozen voor specifieke typen abonnementen. [Meer informatie](../../delivery/using/about-services-and-subscriptions.md)

## Weigeren beheren {#opt-out}

Het is een wettelijke vereiste om ontvangers de mogelijkheid te bieden zich af te melden voor het ontvangen van communicatie van een merk. Deze keuze moet ook worden nagekomen. <!--Learn more about the applicable legislation in the [Adobe Campaign Classic v7 documentation](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/privacy/privacy-and-recommendations.html#privacy-regulations){target="_blank"}.-->

**waarom is het belangrijk?**

* Als u deze voorschriften niet naleeft, brengt u juridische risico&#39;s met zich mee voor uw merk.
* Het helpt vermijden verzendend ongevraagde mededelingen naar ontvangers, die hen kunnen leiden om uw berichten als spam te merken en uw reputatie te schaden.

Wanneer het verzenden van leveringen gebruikend het Web van Adobe Campaign, zorg ervoor klanten van toekomstige mededelingen kunnen afmelden. Als het abonnement is opgezegd, worden profielen automatisch verwijderd uit het publiek van toekomstige marketingberichten.

### E-mailopt-out {#email-opt-out}

Om ontvangers toe te staan om van het ontvangen van e-mailmededelingen af te melden, omvat een **unsubscribe verbinding** in elk e-mailbericht dat naar ontvangers wordt verzonden.

Voer de volgende stappen uit:

1. Maak een externe bestemmingspagina en host deze op het externe systeem van uw keuze.

1. Maak een e-maillevering. [ leer hoe ](../email/create-email.md)

1. Voeg een koppeling in uw e-mailinhoud in. [ leer hoe ](../email/message-tracking.md#insert-links)

   ![ verbinding van het Tussenvoegsel in e-mailinhoud ](../email/assets/message-tracking-insert-link.png)

1. Plak in het veld **[!UICONTROL Url]** de koppeling naar de landingspagina van derden.

1. Klik op het pictogram **[!UICONTROL Links]** in het linkerdeelvenster om de lijst weer te geven met alle URL&#39;s in de inhoud die u wilt bijhouden.

1. Klik op het potloodpictogram naast de nieuwe koppeling om deze te bewerken.

1. Wijzig **[!UICONTROL Tracking Type]** en plaats het aan **[!UICONTROL Opt out]**.

   ![ geef het volgen type voor opt-out ](../email/assets/message-tracking-edit-a-link.png) uit

1. Klik op **[!UICONTROL Save]** en verzend het bericht. [Meer informatie](../monitor/prepare-send.md)

1. Zodra het bericht wordt ontvangen, als de ontvanger de unsubscribe verbinding klikt, wordt uw landende pagina getoond.

1. Wanneer de ontvanger het formulier voor de landingspagina verzendt, worden de profielgegevens bijgewerkt. [Meer informatie](#denylisted-profiles)

<!--Any other option available such as one-click opt-out link or List-Unsubscribe (to include an unsubscribe link in the email header) to enable opt-out in a delivery?-->

## Gevoegde op lijst van gewenste personen profielen {#denylisted-profiles}

Na een unsubscription (opt-out), worden de profielen toegevoegd aan de **lijst van gewezen personen** voor een bepaald kanaal. Dit betekent dat zij niet langer het doelwit zijn van leveringen.

>[!NOTE]
>
>Als een profiel op de lijst van gewezen personen voor het e-mailkanaal twee e-mailadressen heeft, worden beide adressen van levering uitgesloten.

In de sectie **[!UICONTROL No longer contact]** van het tabblad **[!UICONTROL Details]** van het profiel kunt u controleren of er zich op de lijst van gewezen personen een of meer kanalen bevinden in de sectie  van het profiel. [Meer informatie](../audience/about-recipients.md#access)

![ de status van de lijst van gewezen personen van de controle in profieldetails ](assets/profile-no-longer-contact.png)

<!--Denylisted status on quarantine list

Additionally, when recipients report your message as spam, or reply to an SMS message with a keyword such as "STOP", their address or phone number is quarantined with the **[!UICONTROL Denylisted]** status. Their profile is updated accordingly.

QUESTION: When a user marks an email as spam, is the profile's No longer contact section also updated? Apparently no (not the same = quarantine vs denylist)

>[!NOTE]
>
>The **[!UICONTROL Denylisted]** status refers to the address only, the profile is not on the denylist, so that the user continues receiving SMS messages and push notifications.

Learn more about Feedback loops in the [Delivery Best Practices Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/transition-process/infrastructure.html#feedback-loops){target="_blank"}.

Learn more on quarantine in the [Campaign v8 (client console) documentation](https://experienceleague.adobe.com/docs/campaign/campaign-v8/send/failures/quarantines.html#non-deliverable-bounces){target="_blank"}.-->