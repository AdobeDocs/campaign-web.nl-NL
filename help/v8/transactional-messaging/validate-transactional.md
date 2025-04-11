---
audience: end-user
title: Transactieberichten valideren
description: Leer hoe te om een transactiebericht in het Gebruikersinterface van het Web van de Campagne te bevestigen
exl-id: 4a24792f-b9f4-4224-b3a8-75f6969b64da
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Transactieberichten valideren

Tijdens of na het maken van uw transactiemelding wilt u de inhoud mogelijk valideren met behulp van een gegevensvoorbeeld.

## Inhoud simuleren {#simulate-content}

Ga als volgt te werk om de inhoud van uw bericht te simuleren:

* Zorg ervoor dat het verpersoonlijkingspad in uw berichtinhoud overeenkomt met uw contextvoorbeeld. In het voorbeeld hieronder, om de voornaam van het testprofiel te tonen, gebruik de weg *rtEvent.ctx.basicDetails.firstName*.

  U kunt de inhoud van het bericht of de contextsteekproef wijzigen om hen te maken richten.

  ![ Schermschot die de controle van verpersoonlijkingspaden in de berichtinhoud tonen ](assets/validate-verification.png){zoomable="yes"}

* Klik op de knop **[!UICONTROL Simulate content]** om een voorvertoning van het transactiebericht weer te geven met de gegevens die in het contextvoorbeeld zijn ingevoerd.

  ![ Schermafbeelding die de Simuleren inhoudsknoop en voorproeffunctionaliteit tonen ](assets/validate-simulate.png){zoomable="yes"}

  Klik op de knop **[!UICONTROL Close]** nadat u de inhoud hebt bekeken.

* Klik op de knop **[!UICONTROL Republish]** als u wijzigingen in de inhoud hebt aangebracht.

## Bewijs verzenden

Gebruik de proefdrukfunctie om het transactiemelding te testen en te ervaren zoals het via het door u gekozen kanaal wordt verzonden, zoals e-mail, SMS of pushmelding.

In het [ venster van de simulatieinhoud ](#simulate-content), klik op de **[!UICONTROL Send proof]** knoop.

![ Schermafbeelding die de Send proefdrukknoop in het venster van de simulatieinhoud toont ](assets/transactional-proof.png){zoomable="yes"}

Voer in het nieuwe venster dat wordt weergegeven het e-mailadres of telefoonnummer in, afhankelijk van het kanaal waar u de proefdruk wilt ontvangen. Klik op de knoppen **[!UICONTROL Send proof]** en **[!UICONTROL Confirm]** nadat u het gewenste adres hebt ingevoerd. Deze actie verzendt een steekproef van uw transactiebericht, die ervoor zorgt dat alle verpersoonlijkingen, dynamische inhoud, en het formatteren correct verschijnen zoals zij voor uw eind - gebruikers.

![ Schermschot die de Send functionaliteit van de proefdruk en bevestigingsproces tonen ](assets/transactional-sendproof.png){zoomable="yes"}

Deze stap is essentieel voor het identificeren van mogelijke problemen voordat u uw transactiebericht publiceert.