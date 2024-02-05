---
audience: end-user
title: Verzenden met gebruik van golven
description: Meer informatie over de leveringsinstellingen in Campagneweb
badge: label="Beperkte beschikbaarheid"
source-git-commit: 3bfcf3c5a5e054995993d38a073733fef8ea4be9
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 1%

---


# Verzenden met gebruik van golven {#send-using-waves}

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_definition"
>title="Waves-definitie"
>abstract="Definieer golven om leveringen in verschillende batches te splitsen in plaats van tegelijkertijd hoge volumes berichten te verzenden."

>[!CONTEXTUALHELP]
>id="acw_deliveries_waves_size"
>title="Grootte van de golf"
>abstract="De grootte van de golf wordt vereist. Voer een numerieke waarde (aantal berichten) of een percentage (0-100%) in het veld Grootte in."

Als u de lading in evenwicht wilt brengen, kunt u leveringen in verscheidene partijen verdelen. Configureer het aantal partijen en hun verhouding ten opzichte van de volledige levering.

>[!NOTE]
>
>U kunt alleen de grootte en de vertraging tussen twee opeenvolgende golven definiëren. De ontvankelijke selectiecriteria voor elke golf kunnen niet worden gevormd.

1. Open de [leveringsinstellingen](delivery-settings.md#retries) en ga naar de **[!UICONTROL Delivery]** tab.
1. Selecteer de **[!UICONTROL Send using multiple waves]** en klik op de knop **[!UICONTROL Define waves...]** koppeling.

1. Om golven te vormen, kunt u of:

   * **[!UICONTROL Schedule multiple waves of the same size]**.

     Als u bijvoorbeeld **[!UICONTROL 30%]** op het overeenkomstige gebied, zal elke golf 30% van de berichten vertegenwoordigen inbegrepen in de levering, behalve laatste, die 10% van de berichten zal vertegenwoordigen.

     ![](assets/waves-same-size.png)

     In de **[!UICONTROL Interval]** in, geeft u de vertraging op tussen het begin van twee opeenvolgende golven. Als u bijvoorbeeld **[!UICONTROL 2d]** De eerste golf begint onmiddellijk, de tweede golf begint over twee dagen, de derde golf over vier dagen, enzovoort.

   * **[!UICONTROL Schedule waves according to a calendar]**.

     In de **[!UICONTROL Start]** de vertraging tussen het begin van twee opeenvolgende golven opgeven. In de **[!UICONTROL Size]** Voer een vast getal of een percentage in.

     In het volgende voorbeeld vertegenwoordigt de eerste golf 25% van het totale aantal berichten inbegrepen in de levering en zal onmiddellijk beginnen. De volgende twee golven voltooien de levering en zijn geplaatst om met intervallen van zes uur te beginnen.

     ![](assets/waves-calendar.png)

     een specifieke regel voor typologische controle; **[!UICONTROL Wave scheduling check]**, zorgt ervoor dat de laatste golf vóór de grens van de leveringsgeldigheid wordt gepland. De typologieën van de campagne en hun regels worden gevormd in **[!UICONTROL Typology]** tabblad van de leveringsinstellingen. Meer informatie over de besturingsregels in het dialoogvenster [Campagne v8-documentatie (clientconsole)](https://experienceleague.adobe.com/docs/campaign/automation/campaign-optimization/control-rules.html).

     >[!IMPORTANT]
     >
     >Zorg ervoor dat de laatste golven de leveringstermijn niet overschrijden, die in het dialoogvenster **[!UICONTROL Validity]** tab. Anders kunnen sommige berichten niet worden verzonden. [Meer informatie](delivery-settings.md#validity)
     >
     >U moet ook genoeg tijd voor pogingen toestaan wanneer het vormen van de laatste golven. [Meer informatie](delivery-settings.md#retries)

1. Om uw te controleren verzendt, ga naar [leveringslogs](../monitor/delivery-logs.md).

De leveringen die al zijn verzonden in de verwerkte golven (**[!UICONTROL Sent]** status) en de in de resterende golven te verzenden leveringen (**[!UICONTROL Pending]** status).

De twee onderstaande voorbeelden zijn de meest gebruikte voorbeelden voor het gebruik van meerdere golven.

* **Tijdens het opvoerproces**

  Wanneer e-mails met een nieuw platform worden verzonden, zijn internetproviders (ISP&#39;s) verdacht van IP-adressen die niet worden herkend. Als er plotseling grote hoeveelheden e-mails worden verzonden, markeren de ISP&#39;s deze vaak als spam.

  Als u wilt voorkomen dat spam wordt gemarkeerd, kunt u het verzonden volume progressief verhogen met golven. Dit zou een vlotte ontwikkeling van de startfase moeten verzekeren en u toelaten om het algemene tarief van ongeldige adressen te verminderen.

  Gebruik hiervoor de opdracht **[!UICONTROL Schedule waves according to a calendar]** -optie. Stel bijvoorbeeld de eerste golf in op 10%, de tweede op 15% enzovoort.

  ![](assets/waves-ramp-up.png)

* **Campagnes die een callcenter impliceren**

  Wanneer het leiden van een campagne van de telefoonloyaliteit, heeft uw organisatie een beperkte capaciteit om het aantal vraag te verwerken om abonnees te contacteren.

  Gebruikend golven, kunt u het aantal berichten tot 20 per dag beperken, die de dagelijkse verwerkingscapaciteit van een vraagcentrum is.

  Selecteer de optie **[!UICONTROL Schedule multiple waves of the same size]** -optie. Enter **[!UICONTROL 20]** als de grootte van de golf en **[!UICONTROL 1d]** in de **[!UICONTROL Period]** veld.

  ![](assets/waves-call-center.png)