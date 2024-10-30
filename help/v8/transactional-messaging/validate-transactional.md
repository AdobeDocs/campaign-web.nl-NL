---
audience: end-user
title: Transactieberichten valideren
description: Leer hoe te om een transactiebericht in het Gebruikersinterface van het Web van de Campagne te bevestigen
source-git-commit: e0d87d22d9712837f085f94f9d9ba63e96f36b36
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Transactieberichten valideren

Tijdens of na het maken van uw transactiemelding wilt u de inhoud mogelijk valideren met behulp van een gegevensvoorbeeld.

## Inhoud simuleren {#simulate-content}

Ga als volgt te werk om de inhoud van uw bericht te simuleren:

* Zorg ervoor dat het verpersoonlijkingspad in uw berichtinhoud overeenkomt met uw contextvoorbeeld. In het voorbeeld hieronder, om de voornaam van het testprofiel te tonen, gebruiken wij de weg *rtEvent.ctx.basicDetails.firstName*

  U kunt de inhoud van het bericht of het contextvoorbeeld wijzigen en deze uitlijnen.

  ![](assets/validate-verification.png){zoomable="yes"}

* Klik op de knop **[!UICONTROL Simulate content]** om een voorbeeld van uw transactiemelding weer te geven met de gegevens die u hebt ingevoerd in het contextvoorbeeld.

  ![](assets/validate-simulate.png){zoomable="yes"}

  Klik op de knop **[!UICONTROL Close]** nadat u de inhoud hebt gecontroleerd.

* Vergeet niet op de knop **[!UICONTROL Republish]** te klikken als u wijzigingen in de inhoud hebt aangebracht.

## Bewijs verzenden

Als u het transactiebericht wilt testen en ervaren zoals het via u gekozen kanaal (zoals e-mail, SMS of pushmelding) zou worden geleverd, kunt u de proefdrukfunctie gebruiken.

In het [ venster van de simulatieinhoud ](#simulate-content), klik op de **[!UICONTROL Send proof]** knoop.

![](assets/transactional-proof.png){zoomable="yes"}

Voer in het nieuwe venster dat wordt weergegeven het e-mailadres (of telefoonnummer, afhankelijk van het kanaal) in waar u de proefdruk wilt ontvangen. Wanneer u het gewenste adres hebt ingevoerd, klikt u op de knoppen **[!UICONTROL Send proof]** en **[!UICONTROL Confirm]** . Met deze actie kunt u een voorbeeld van uw transactiemelding verzenden, zodat alle personalisaties, dynamische inhoud en opmaak op de juiste wijze worden weergegeven als voor uw eindgebruikers.

![](assets/transactional-sendproof.png){zoomable="yes"}

Dit is een essentiële stap om mogelijke problemen vast te stellen voordat u uw transactiebericht publiceert.
