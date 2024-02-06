---
audience: end-user
title: Verzenden met gebruik van golven
description: Meer informatie over de leveringsinstellingen in Campagneweb
badge: label="Beperkte beschikbaarheid"
source-git-commit: 6676aa00e3ed7ea54f1ecd9b3e87d317e5208712
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

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

Als u de lading in evenwicht wilt brengen, kunt u leveringen in verscheidene partijen verdelen. Vorm het aantal partijen en hun verhouding met betrekking tot de volledige levering, evenals het interval tussen twee golven.

>[!NOTE]
>
>U kunt alleen de grootte en de vertraging tussen twee opeenvolgende golven definiëren. De ontvankelijke selectiecriteria voor elke golf kunnen niet worden aangepast.

Volg onderstaande stappen om leveringen te verzenden met gebruik van golven.

1. Open de [leveringsinstellingen](delivery-settings.md#retries).

1. Bladeren naar de **[!UICONTROL Delivery]** sectie.

1. Selecteer de **[!UICONTROL Send using multiple waves]** -optie.

1. Om golven te vormen, kunt u of:

   * [Meerdere golven van dezelfde grootte plannen](#waves-same-size)
   * [Golven plannen volgens een kalender](#waves-calendar)

1. Bereid de levering voor en verzend deze op de gebruikelijke wijze. [Meer informatie](../msg/gs-deliveries.md)

   >[!CAUTION]
   >
   >Zorg ervoor dat de laatste golven de leveringstermijn niet overschrijden, die in het dialoogvenster **[!UICONTROL Validity]** tab. Anders kunnen sommige berichten niet worden verzonden. [Meer informatie](delivery-settings.md#validity)
   >
   >U moet ook genoeg tijd voor pogingen toestaan wanneer het vormen van de laatste golven. [Meer informatie](delivery-settings.md#retries)

1. Om uw te controleren verzendt, ga naar [leveringslogs](../monitor/delivery-logs.md).

   De leveringen die al zijn verzonden in de verwerkte golven (**[!UICONTROL Sent]** status) en de in de resterende golven te verzenden leveringen (**[!UICONTROL Pending]** status).

een specifieke regel voor typologische controle; **[!UICONTROL Wave scheduling check]**, zorgt ervoor dat de laatste golf vóór de grens van de leveringsgeldigheid wordt gepland. De typologieën van de campagne en hun regels worden gevormd in **[!UICONTROL Typology]** tabblad van de leveringsinstellingen. Meer informatie over de besturingsregels in het dialoogvenster [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html).

## Meerdere golven van dezelfde grootte plannen {#waves-same-size}

Als u deze optie selecteert, hebben alle golven de zelfde grootte (behalve laatste), en de vertraging tussen elke golf is altijd het zelfde.

![](assets/waves-same-size.png)

* Geef de grootte op voor alle golven waarin u de levering wilt splitsen. U kunt een percentage of een numerieke waarde invoeren. Alleen de laatste golf kan in grootte variëren, omdat het resterende aantal berichten moet worden opgenomen.

  Als u bijvoorbeeld **[!UICONTROL 30%]** op het overeenkomstige gebied vertegenwoordigen de eerste drie golven 30 % van alle berichten die in de levering zijn opgenomen , en de vierde 10 % .

* In de **[!UICONTROL Interval]** in, geeft u de vertraging op tussen het begin van twee opeenvolgende golven. Als u bijvoorbeeld **[!UICONTROL 2 days]** De eerste golf begint meteen, de tweede golf begint over twee dagen, de derde golf over vier dagen, enzovoort.

Één gemeenschappelijk gebruiksgeval voor het gebruiken van verscheidene golven van de zelfde grootte is met een betrokken vraagcentrum. Wanneer het leiden van een campagne van de telefoonloyaliteit, heeft uw organisatie een beperkte capaciteit om het aantal vraag te verwerken om abonnees te contacteren.

Gebruikend golven, kunt u het aantal berichten tot 20 per dag beperken, die de dagelijkse verwerkingscapaciteit van een vraagcentrum is.

Selecteer de optie **[!UICONTROL Schedule multiple waves of the same size]** -optie. Enter **[!UICONTROL 20]** als de grootte van de golven en **[!UICONTROL 1 day]** in de **[!UICONTROL Interval]** veld.

![](assets/waves-call-center.png)

## Golven plannen volgens een kalender {#waves-calendar}

Als u deze optie selecteert, moet u de begindag/tijd voor elke golf bepalen u, evenals de grootte van elke golf verzendt.

* In de **[!UICONTROL Start]** de vertraging tussen het begin van twee opeenvolgende golven opgeven.

* In de **[!UICONTROL Size]** Voer een vast getal of een percentage in.

Voeg zoveel golven toe als u nodig hebt.

In het onderstaande voorbeeld vertegenwoordigt de eerste golf 25% van het totale aantal berichten dat is opgenomen in de levering en wordt deze onmiddellijk gestart. De volgende twee golven voltooien de levering en zijn geplaatst om met intervallen van zes uur te beginnen.

![](assets/waves-calendar.png)

Eén veelgebruikte manier om meerdere golven volgens een kalender te gebruiken, is tijdens het opbladerproces.

Wanneer e-mails met een nieuw platform worden verzonden, zijn internetproviders (ISP&#39;s) verdacht van IP-adressen die niet worden herkend. Als er plotseling grote hoeveelheden e-mails worden verzonden, markeren de ISP&#39;s deze vaak als spam.

Als u wilt voorkomen dat spam wordt gemarkeerd, kunt u het verzonden volume progressief verhogen met golven. Dit zou een vlotte ontwikkeling van de startfase moeten verzekeren en u toelaten om het algemene tarief van ongeldige adressen te verminderen.

Gebruik hiervoor de opdracht **[!UICONTROL Schedule waves according to a calendar]** -optie. Stel bijvoorbeeld de eerste golf in op 10%, de tweede op 15%, de derde op 20% enzovoort.

![](assets/waves-ramp-up.png)



