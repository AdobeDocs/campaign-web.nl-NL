---
title: Branding
description: Ontdek hoe u uw merk kunt configureren
audience: administration
context-tags: branding,overview;branding,main
role: Admin
level: Experienced
exl-id: 7afc802d-e90c-48c8-aa04-3ea543dfdfbc
source-git-commit: 8b93ddd9c655c9ca461f28392c70872e4005b44f
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 17%

---

# Brandmerken configureren {#branding-configure}

>[!IMPORTANT]
>
>Merken kunnen niet door eindgebruikers worden gemaakt of gewijzigd. Deze bewerkingen moeten worden uitgevoerd door de technische beheerder van Adobe Campaign. Neem voor elk verzoek contact op met de klantenservice van Adobe.

In Adobe Campaign V8 staan de merken in het menu **[!UICONTROL Administration > Platform > Branding]** .

A **[!UICONTROL Brand]** wordt bepaald door de volgende kenmerken:

* An **[!UICONTROL Identity]**, which define and personalizes your brand. Deze sectie bevat de volgende velden:

   * **[!UICONTROL Label]** zichtbaar in de interface
   * **[!UICONTROL ID]**
   * **[!UICONTROL Brand name]**
   * **[!UICONTROL Website URL]** en **[!UICONTROL Website label]** van het merk
   * **[!UICONTROL Brand logo]**

  ![](assets/branding_1.png)

* **[!UICONTROL Header parameters of sent emails]** personaliseert wat de ontvangers van uw campagnes te zien krijgen. Deze sectie bevat de volgende velden:

   * **[!UICONTROL Sender (email address)]** met het e-mailadres van het merk
   * **[!UICONTROL Sender (name)]** met de merknaam.
   * **[!UICONTROL Reply to (email address)]** met het e-mailadres waarop de klant kan antwoorden.
   * **[!UICONTROL Reply to (name)]** met de merknaam.
   * **[!UICONTROL Error (email address)]** met het e-mailadres dat moet worden gebruikt bij een fout.

  >[!IMPORTANT]
  >
  >Nadat u de koptekstparameters van de e-mails hebt bijgewerkt, controleert u de geavanceerde instellingen van de sjabloon als de naam en het e-mailadres van de afzender niet zijn gewijzigd in de e-mail die met de sjabloon is gemaakt.

  ![](assets/branding_2.png)

* **[!UICONTROL Brand configs]** definieert de servers die worden gebruikt voor tracering, ook voor het openen van pagina-toegang. Deze sectie bevat de volgende velden:

   * **[!UICONTROL Brand subdomain]** verwijst naar de specifieke subdomein-URL voor dit merk, die wordt gevraagd om te worden gedelegeerd vanuit Adobe.

  Merk op dat de configuratie voor het volgen, de spiegel, en toepassingsservers in afzonderlijke externe rekeningen verbonden aan het verpletteren wordt opgeslagen. Deze instellingen worden toegepast tijdens de provisioning en mogen niet worden gewijzigd. Als u URL&#39;s wilt weergeven, opent u het tabblad **[!UICONTROL Branding prefixes]** via uw externe account.

  ![](assets/branding_3.png)

* Met het menu **[!UICONTROL Tracking URL configs]** kunt u URL-tracering verbeteren door aanvullende parameters te definiëren voor integratie met hulpprogramma&#39;s voor webanalyse, zoals Adobe Analytics en Google Analytics.

  Gebruik het menu **[!UICONTROL Additional URL Parameters]** om extra parameters als sleutel-waardeparen samen met hun toepassingsvoorwaarden tot stand te brengen. Elke parameternaam moet uniek en niet leeg zijn en elke parameterwaarde moet niet leeg zijn. De toepassingsvoorwaarde kan leeg zijn, maar geen van deze waarden kan JST-tags bevatten.

  Deze parameters worden toegepast op bijgehouden URL&#39;s die overeenkomen met een domeinnaam die is opgegeven in de **[!UICONTROL List of Domain Names]** . Deze parameters kunnen reguliere expressies bevatten.

  **Voorbeeld:** Een bijgehouden URL als `https://www.example.com` zal `https://www.example.com/?age=21&deliveryName=DM101` worden wanneer de extra parameters `age=21` en `deliveryName=DM101` voor dat domein worden gevormd.

## Branding voor transactiemeldingen configureren {#branding-transactional-config}

>[!IMPORTANT]
>
>Deze sectie is slechts op Transactieoverseinen (het Centrum van het Bericht) van toepassing.
>
>Terwijl de transactiemogelijkheden in het Web UI van de Campagne beschikbaar zijn, moeten de hieronder stappen in de Console van de Cliënt van de Campagne v8 (controlegeval) worden uitgevoerd.

Als u het Transactionele overseinen (het Centrum van het Bericht) met branding gebruikt, wordt de extra configuratie vereist.

### Formules bijhouden voor Real-Time instanties

Wanneer branding op een Real-Time (RT) controleinstantie wordt geactiveerd, worden de specifieke het volgen opties gebruikt om het volgen formules te beheren. Deze formules worden gevormd centraal op de instantie van de Controle van RT eerder dan individueel op elke instantie van de Uitvoering van RT.

De volgende opties bepalen de volgende formules die door levering RT worden gebruikt:

* **`NmsTracking_RT_ClickFormula`**: geeft de formule aan die wordt gebruikt voor klikken op bijhouden bij RT-instanties

* **`NmsTracking_RT_OpenFormula`**: geeft de formule aan die wordt gebruikt voor open tracking bij RT-instanties

Als voor uw implementatie aangepaste volgformules voor transactieberichten zijn vereist, gebruikt u de onderstaande optie:

* **`Branding_RT_ListXtkOptions_toPublish`**: vermeld hier de XTK-optienamen voor uw aangepaste formules (gescheiden door komma&#39;s). Dit zorgt ervoor dat de levering van RT de aangepaste het volgen formules kan toepassen.