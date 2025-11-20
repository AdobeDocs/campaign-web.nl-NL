---
audience: end-user
title: Verzenden met gebruik van golven
description: Meer informatie over de leveringsinstellingen in Campagneweb
feature: Email
exl-id: d4cd5fe5-f9ac-44ac-a961-ae45131aeb3e
source-git-commit: f1911523c9076188c492da24e0cbe5c760e58a28
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# Verzenden met gebruik van golven {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Leveringen splitsen in meerdere batches"
>abstract="In plaats van tegelijkertijd hoge volumes van berichten te verzenden, bepaal golven om leveringen in verscheidene partijen te verdelen. U kunt veelvoudige golven van de zelfde grootte vormen, of een kalender voor de verschillende te verzenden golven plaatsen."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="De grootte van elke golf definiëren"
>abstract="U moet een grootte invoeren voor alle golven die u toevoegt. Voer een numerieke waarde (aantal berichten voor elke golf) of een percentage (0-100%) in."

Als u de lading in evenwicht wilt brengen, kunt u de e-mailleveringen in verscheidene partijen verdelen. Vorm het aantal partijen en hun verhouding met betrekking tot de volledige levering, evenals het interval tussen twee golven.

>[!NOTE]
>
>U kunt alleen de grootte en de vertraging tussen twee opeenvolgende golven definiëren. De ontvankelijke selectiecriteria voor elke golf kunnen niet worden aangepast.

Volg onderstaande stappen om leveringen te verzenden met gebruik van golven.

1. Open de [&#x200B; leveringsmontages &#x200B;](delivery-settings.md#retries).

1. Blader naar de sectie **[!UICONTROL Delivery]** .

1. Selecteer de optie **[!UICONTROL Send using multiple waves]** .

1. Om golven te vormen, kunt u of:

   * [Meerdere golven van dezelfde grootte plannen](#waves-same-size)
   * [Golven plannen volgens een kalender](#waves-calendar)

1. Bereid de levering voor en verzend deze op de gebruikelijke wijze. [Meer informatie](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >Zorg ervoor de laatste golven niet de leveringsdeadline overschrijden, die in het [&#x200B; lusje van de Geldigheid &#x200B;](delivery-settings.md#validity) wordt bepaald, anders zouden sommige berichten niet kunnen worden verzonden. Een specifieke typologiecontroleregel, **[!UICONTROL Wave scheduling check]** , zorgt ervoor dat de laatste golf vóór de geldigheidsgrens van de levering wordt gepland. Leer meer over controleregels in de [&#x200B; Campagne v8 (cliëntconsole) documentatie &#x200B;](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html).
   >
   >U moet ook genoeg tijd voor pogingen toestaan wanneer het vormen van de laatste golven. [Meer informatie](delivery-settings.md#retries)

1. Om uw te controleren verzendt, ga naar de [&#x200B; leveringslogboeken &#x200B;](../monitor/delivery-logs.md). U kunt de leveringen zien die reeds in de verwerkte golven (**[!UICONTROL Sent]** status) werden verzonden en de te verzenden leveringen in de resterende golven (**[!UICONTROL Pending]** status).

## Meerdere golven van dezelfde grootte plannen {#waves-same-size}

Als u deze optie selecteert, hebben alle golven de zelfde grootte (behalve laatste), en de vertraging tussen elke golf is altijd het zelfde.

![&#x200B; Voorbeeld van golven met de zelfde grootte &#x200B;](assets/waves-same-size.png){zoomable="yes"}

* Geef de grootte op voor alle golven waarin u de levering wilt splitsen. U kunt een percentage of een numerieke waarde invoeren. Alleen de laatste golf kan in grootte variëren, omdat het resterende aantal berichten moet worden opgenomen.

  Als u bijvoorbeeld **[!UICONTROL 30%]** invoert in het veld **[!UICONTROL Waves size]** , vertegenwoordigen de eerste drie golven 30% van alle berichten die in de levering zijn opgenomen en de vierde voor de resterende 10%.

* Geef in de sectie **[!UICONTROL Interval]** de vertraging op tussen het begin van twee opeenvolgende golven. Als u bijvoorbeeld **[!UICONTROL 2 days]** invoert, begint de eerste golf onmiddellijk, de tweede golf begint over twee dagen, de derde golf over vier dagen, enzovoort.

Één gemeenschappelijk gebruiksgeval voor het gebruiken van verscheidene golven van de zelfde grootte is met een betrokken vraagcentrum. Wanneer het leiden van een campagne van de telefoonloyaliteit, heeft uw organisatie een beperkte capaciteit om het aantal vraag te verwerken om abonnees te contacteren.

Gebruikend golven, kunt u het aantal berichten tot 20 per dag beperken, die de dagelijkse verwerkingscapaciteit van een vraagcentrum is.

Selecteer hiervoor de optie **[!UICONTROL Schedule multiple waves of the same size]** . Voer **[!UICONTROL 20]** in als de golfgrootte en **[!UICONTROL 1 day]** in het veld **[!UICONTROL Interval]** .

![&#x200B; Voorbeeld van golven voor vraag centreert verwerking &#x200B;](assets/waves-call-center.png){zoomable="yes"}

## Golven plannen volgens een kalender {#waves-calendar}

Als u deze optie selecteert, definieert u de begindag/tijd voor elke golf die u verzendt en de grootte van elke golf.

* Geef in de velden **[!UICONTROL Start]** de vertraging op tussen het begin van twee opeenvolgende golven.

* Voer in de kolom **[!UICONTROL Size]** een vast getal of een percentage in.

Voeg zoveel golven toe als u nodig hebt. Pas de volgorde aan uw vereisten aan.

>[!NOTE]
>
>Als u percentages gebruikt, zou het totaal voor alle golven niet 100% moeten overschrijden.

In het onderstaande voorbeeld vertegenwoordigt de eerste golf 25% van het totale aantal berichten dat is opgenomen in de levering en wordt deze onmiddellijk gestart. De volgende twee golven voltooien de levering en zijn geplaatst om met intervallen van zes uur te beginnen.

![&#x200B; Voorbeeld van golven die door kalender &#x200B;](assets/waves-calendar.png){zoomable="yes"} worden gepland

Een veelvoorkomend geval van het gebruik van meerdere golven volgens een kalender is tijdens het oplaadproces.

Wanneer e-mails met een nieuw platform worden verzonden, zijn internetproviders (ISP&#39;s) verdacht van IP-adressen die niet worden herkend. Als er plotseling grote hoeveelheden e-mails worden verzonden, markeren de ISP&#39;s deze vaak als spam.

Als u wilt voorkomen dat spam wordt gemarkeerd, verhoogt u geleidelijk het verzonden volume met behulp van golven. Dit verzekert vlotte ontwikkeling van de aanloopfase en vermindert het algemene tarief van ongeldige adressen.

Gebruik hiervoor de optie **[!UICONTROL Schedule waves according to a calendar]** . Stel bijvoorbeeld de eerste golf in op 10%, de tweede op 15%, de derde op 20% enzovoort.

![&#x200B; Voorbeeld van golven voor oprijplaat proces &#x200B;](assets/waves-ramp-up.png){zoomable="yes"}