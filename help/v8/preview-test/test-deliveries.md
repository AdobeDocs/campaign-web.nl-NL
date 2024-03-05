---
audience: end-user
title: Proefdrukken verzenden
description: Meer informatie over het definiëren en verzenden van proefdrukken
exl-id: b2677579-c95d-443d-b207-466af364c208
source-git-commit: 81fa26e44739d70218b949712a41a3d520900fa0
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Proefdrukken verzenden {#send-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_mode"
>title="Voorvertoningsmodus"
>abstract="Geef een voorvertoning van het bericht weer en test het bericht door de testpopulatie op te nemen in het hoofddoel."

Nadat de inhoud van het bericht is gedefinieerd, kunt u een voorbeeld bekijken en testen door proefdrukken naar testprofielen te verzenden. Als u gepersonaliseerde inhoud hebt ingevoegd, kunt u met behulp van testprofielgegevens controleren hoe deze inhoud in het bericht wordt weergegeven.

Om mogelijke fouten in de berichtinhoud of verpersoonlijkingsmontages te ontdekken, verzend proefdrukken naar testprofielen alvorens het naar het doelpubliek te verzenden. Telkens wanneer een wijziging wordt aangebracht, moet een bewijs worden verzonden om de meest recente inhoud te valideren. Het verzenden van proefdrukken is een belangrijke stap in het valideren van uw campagne en het identificeren van mogelijke problemen. De proefontvangers kunnen verschillende elementen controleren, zoals verbindingen, opt-out verbindingen, beelden, of spiegelpagina&#39;s, evenals om het even welke fouten in het teruggeven, inhoud, verpersoonlijkingsmontages en leveringsconfiguratie ontdekken.

## Inhoud simuleren met testontvangers {#simulate-content-test-deliveries}

>[!CONTEXTUALHELP]
>id="acw_email_preview_option_test_target"
>title="Testpopulatie"
>abstract="Selecteer een testpopulatiemodus."

Voordat u een proefdruk verzendt, moet u een doelpubliek voor de levering definiëren. [Meer informatie](../audience/add-audience.md)

Uw berichtinhoud testen:

1. Bewerk de inhoud van de levering.
1. Klik op de knop **[!UICONTROL Simulate content]**.
1. Klik op de knop **[!UICONTROL Send proof]** om proefdrukken te verzenden.

   ![](assets/simulate-test-button-email.png){zoomable=&quot;yes&quot;}

1. Selecteer de ontvangers van de proefdruk.

   Afhankelijk van het berichtkanaal, kunnen de proeven naar de volgende soorten ontvangers worden verzonden:

   * Voor SMS en e-mail kunt u [testprofielen](#test-profiles), die specifieke extra ontvangers in de database zijn. U kunt ook de opdracht [vervanging van het hoofddoel](#substitution-profiles) , die de proefdruk naar een e-mailtestadres of telefoonnummer verzendt, en verpersoonlijkingsgegevens van een bestaand profiel gebruikt. Op deze manier kunt u het bericht net zo ervaren als de ontvangers, zodat u een nauwkeurige weergave krijgt van de inhoud die het profiel zal ontvangen.

   * Voor pushberichten kunt u [abonnees](#subscribers), die fictieve abonnees zijn die aan het gegevensbestand worden toegevoegd. Ze worden gemaakt in de [!DNL Campaign] console. Meer informatie in [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/campaign-v8/audience/add-profiles/test-profiles.html){target="_blank"}

   De gedetailleerde configuratie voor elke wijze is beschikbaar hieronder.

## Testprofielen gebruiken {#test-profiles}

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_mode"
>title="Doel van het bewijs"
>abstract="U kunt een tweede bestand uploaden als &#39;doel van de proefdruk&#39; als u de levering wilt testen voordat u het hoofddoel bereikt."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_upload"
>title="Profielen uploaden"
>abstract="U kunt een tweede bestand met aanvullende profielen uploaden als u de levering wilt testen met een andere set dan de set die u voor het hoofddoel hebt gebruikt."

>[!CONTEXTUALHELP]
>id="acw_deliveries_simulate_test_sample"
>title="Sjabloonbestand"
>abstract="De opmaak van het bestand moet gelijk zijn aan die van het oorspronkelijke bestand.<br/>Ondersteunde bestandsindelingen: txt, csv. Maximale bestandsgrootte: 15 MB. Eerste regel gebruiken als kolomkop."

>[!CONTEXTUALHELP]
>id="acw_sms_preview_option_app_target"
>title="Testprofielen opnemen in het hoofdpubliek"
>abstract="Schakel deze optie in om het laatste bericht ook naar de ontvangers van de proefdrukken te verzenden."

Testprofielen zijn aanvullende ontvangers in de database. Ze worden gemaakt op basis van de **[!UICONTROL Customer management]** > **[!UICONTROL Profiles]** -menu. [Meer informatie](../audience/test-profiles.md#create-test-profiles)

De stappen voor het verzenden van proefdrukken naar testprofielen worden hieronder beschreven.

1. Klik vanaf de inhoud van de levering op de knop **[!UICONTROL Simulate content]** en de **[!UICONTROL Send proof]** knop.

1. Van de **[!UICONTROL Mode]** vervolgkeuzelijst kiest u **[!UICONTROL Test profiles]** om fictieve ontvangers aan te wijzen die het bewijs of de levering van SMS zullen ontvangen.

   ![](assets/simulate-profile-mode.png){zoomable=&quot;yes&quot;}

1. Als u al profielen hebt geselecteerd voor [voorvertoning van het bericht](preview-content.md) in het scherm van de inhoudsimulatie, worden die profielen pre-geselecteerd als proefontvangers. U kunt uw selectie wissen en/of extra ontvangers toevoegen met de opdracht **[!UICONTROL Add test profile(s)]** knop.

1. Wanneer u door het testprofiel of de profiellijsten bladert, kunt u filters gebruiken om uw zoekopdracht te verfijnen. U kunt bijvoorbeeld een regel definiëren om alle testprofielen te zoeken die **[!UICONTROL Prospect]** status. Leer hoe u regels kunt toevoegen met de opdracht [querymodel](../query/query-modeler-overview.md).

   ![](assets/simulate-test-profile-filter.png){zoomable=&quot;yes&quot;}

1. Als u het laatste bericht ook naar de ontvangers van de proefdruk wilt verzenden, selecteert u de optie **[!UICONTROL Include test population in the main target]** -optie.

   ![](assets/simulate-include-test.png){zoomable=&quot;yes&quot;}

1. Nadat de testprofielen zijn geselecteerd, kunt u [het bewijs verzenden](#send-test).

## Vervangende profielgegevens {#substitution-profiles}

Gebruik profielvervanging om proefdrukken naar een specifiek e-mailadres of telefoonnummer te verzenden, terwijl de gegevens van een bestaand profiel van het [!DNL Adobe Campaign] database. Deze modus kan alleen worden geselecteerd als het publiek van de levering is gedefinieerd.

Voer de volgende stappen uit om profielgegevens van het hoofddoel te vervangen:

1. Klik vanaf de inhoud van de levering op de knop **[!UICONTROL Simulate content]** en de **[!UICONTROL Send proof]** knop.

1. Van de **[!UICONTROL Mode]** vervolgkeuzelijst kiest u **[!UICONTROL Substitute from main target]** om een bewijs naar een specifiek e-mailadres of telefoonnummer te verzenden terwijl het tonen van gegevens van een bestaand profiel.

   >[!CAUTION]
   >
   >Als u geen [publiek](../audience/about-recipients.md) voor uw levering, **[!UICONTROL Substitute from main target]** Deze optie wordt grijs weergegeven en u kunt geen vervangingsprofielen selecteren.

1. Klik op de knop **[!UICONTROL Add address]** en geeft u het e-mailadres of telefoonnummer op dat de proefdruk ontvangt.

   ![](assets/simulate-add-substitution-address.png){zoomable=&quot;yes&quot;}

   >[!NOTE]
   >
   >U kunt elk e-mailadres of telefoonnummer invoeren. Op deze manier kunt u proefdrukken naar alle ontvangers verzenden, zelfs als deze geen gebruikers van [!DNL Adobe Campaign].

1. Selecteer het profiel in het doel dat u voor de levering hebt gedefinieerd om als vervangend profiel te gebruiken. U kunt ook [!DNL Adobe Campaign] Selecteer een willekeurig profiel in het doel. De profielgegevens van het geselecteerde profiel worden weergegeven in de proefdruk.

1. Bevestig de ontvanger en herhaal de bewerking om zoveel e-mailadressen of telefoonnummers toe te voegen als nodig is.

   ![](assets/simulate-profile-substitute.png){zoomable=&quot;yes&quot;}

1. Als u het laatste bericht ook naar de ontvangers van de proefdruk wilt verzenden, selecteert u de optie **[!UICONTROL Include test population in the main target]** -optie.

1. Als de vervangende profielen zijn geselecteerd, kunt u [het bewijs verzenden](#send-test).

## Proefdrukken verzenden naar app-abonnees {#subscribers}

Bij het ontwerpen met pushberichten kunnen proefdrukken alleen naar uw app-abonnees worden verzonden. Volg onderstaande stappen om deze te selecteren.

1. Klik op de knop **[!UICONTROL Simulate content]** en de **[!UICONTROL Send proof]** knop.

   ![](assets/simulate-test-button-push.png){zoomable=&quot;yes&quot;}

1. Als u al abonnees hebt geselecteerd op [voorvertoning van de levering](preview-content.md) in het scherm van de inhoudsimulatie, worden die profielen pre-geselecteerd als testabonnees.

   U kunt uw selectie wissen en/of extra abonnees toevoegen met behulp van de toegewezen knop.

   ![](assets/simulate-test-subscribers.png){zoomable=&quot;yes&quot;}

1. Als u het laatste pushbericht ook naar de testabonnees wilt verzenden, selecteert u de optie **[!UICONTROL Include test population in the main target]** -optie.

1. Als de abonnees zijn geselecteerd, kunt u [het bewijs verzenden](#send-test).

## De proefdruk verzenden {#send-test}

Volg onderstaande stappen om de proefdruk naar de geselecteerde ontvangers te verzenden.

1. Klik op de knop **[!UICONTROL Send proof]**.

1. Bevestig de verzendende.

   ![](assets/simulate-send-test.png){zoomable=&quot;yes&quot;}

1. Verzend zoveel proefdrukken als nodig zijn tot u de inhoud van uw levering hebt voltooid.

Als u klaar bent, kunt u de levering voorbereiden en naar het hoofddoel verzenden. Leer hoe in de speciale secties hieronder:

* [Uw e-mail verzenden](../monitor/prepare-send.md)
* [Uw pushmelding verzenden](../push/send-push.md#send-push)
* [Verstuur je SMS-verzending](../sms/send-sms.md#send-sms)

## Toegang verzonden proefdrukken {#access-test-deliveries}

Zodra de proefdrukken zijn verzonden, kunt u hun logboeken openen van **[!UICONTROL Simulate content]** scherm.

Deze logboeken staan u toe om tot alle proeven toegang te hebben die voor de geselecteerde levering worden verzonden, en om specifieke statistieken met betrekking tot hun het verzenden te visualiseren. [Leer hoe u leveringslogboeken kunt controleren](../monitor/delivery-logs.md)

![](assets/simulate-test-log.png){zoomable=&quot;yes&quot;}

U kunt verzonden proefdrukken ook openen vanuit de [leveringslijst](../msg/gs-messages.md), zoals elke levering.

![](assets/simulate-deliveries-list.png){zoomable=&quot;yes&quot;}
