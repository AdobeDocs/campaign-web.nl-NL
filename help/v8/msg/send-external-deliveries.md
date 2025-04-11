---
audience: end-user
title: Aan de slag met externe leveringen
description: Meer informatie over het maken en verzenden van externe leveringen met Adobe Campaign Web
exl-id: 08fe9333-aa35-4acf-ba41-4c6895049bbc
source-git-commit: d6c6aac9d9127a770732b709873008613ae8c639
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Externe leveringen verzenden {#gs-direct-mail}

Met Adobe Campaign kunt u leveringen beheren die u buiten de campagne hebt gemaakt om via een extern systeem persoonlijke e-mails, SMS-berichten of pushberichten (iOS en Android) op grote schaal te verzenden.

<!--The supported channels are Email, Mobile (SMS), and Push (iOS and Android).-->

Bij het maken van een externe levering genereert Adobe Campaign automatisch een extractiebestand dat alle doelprofielen en geselecteerde gegevens bevat. Dit bestand wordt naar de server van uw keuze verzonden, die het verzendingsproces afhandelt.

## Een toegewezen externe account maken {#routing-external-account}

U moet een specifieke externe account configureren voor gebruik in uw externe leveringen. Het moet van het **[!UICONTROL Routing]** type zijn.

>[!NOTE]
>
>Leer hoe te om een verpletterende-type externe rekening in [ tot stand te brengen deze sectie ](../administration/external-account.md#routing).

Selecteer bijvoorbeeld het **[!UICONTROL Mobile (SMS)]** -kanaal voor de externe account. **[!UICONTROL External]** wordt standaard geselecteerd als de **[!UICONTROL Delivery mode]** .

![ Externe de wijzeconfiguratie van de rekeningslevering ](../administration/assets/external-account-delivery-mode.png){zoomable="yes"}

## De externe levering maken en verzenden {#create-external-delivery}

Zodra de specifieke externe rekening wordt gevormd, creeer de externe levering. Voer de onderstaande stappen uit.

1. Een levering maken. [ leer hoe ](create-deliveries.md)

   U hebt drie opties:

   * **in een werkschema**: Voeg een externe kanaalactiviteit (e-mail, SMS, of duw) aan uw werkschema toe. Voor gedetailleerde instructies bij het vormen van werkschema&#39;s, verwijs naar [ deze pagina ](../workflows/gs-workflow-creation.md).
   * **in een campagne**: Na het creëren van een campagne, kunt u een e-mail, SMS, of de externe levering van het drukkanaal tot stand brengen. Voor meer informatie bij vestiging uw campagne, verwijs naar [ deze pagina ](../campaigns/gs-campaigns.md).
   * **stand-alone levering**: Sluit klanten direct en onmiddellijk met een individuele externe levering aan. [ leren hoe te om een levering ](../msg/gs-deliveries.md) tot stand te brengen

1. In de levering of leveringsmalplaatje [ montages ](../advanced-settings/delivery-settings.md), selecteer de externe rekening die voor het kanaal van uw keus (in dit voorbeeld, het kanaal van SMS) wordt gecreeerd en sparen.

   ![ Externe levering die configuratie ](assets/external-delivery-routing.png){zoomable="yes"} verplettert

   >[!NOTE]
   >
   >Als u een levering creeert, zorg ervoor dat u a [ leveringsmalplaatje ](delivery-template.md) gebruikend een externe rekening van het **[!UICONTROL Routing]** type hebt geselecteerd. Anders, zult u niet de specifieke gecreeerde rekening kunnen selecteren [ hierboven ](#routing-external-account).

1. Klik in de bezorgsectie **[!UICONTROL Content]** op **[!UICONTROL Edit content]** .

   ![ geef inhoud in externe levering uit ](assets/external-delivery-edit-content.png){zoomable="yes"}

1. In tegenstelling tot een standaardlevering, ontwerpt u niet de inhoud van het bericht zelf. Definieer in plaats daarvan de eigenschappen en kolommen van het bestand dat naar het externe systeem wordt verzonden.

   ![ de eigenschappenconfiguratie van het Dossier voor externe levering ](assets/external-delivery-file-properties.png){zoomable="yes"}

   Volg de zelfde stappen zoals wanneer het ontwerpen van de inhoud van het extractiedossier door [ wordt geproduceerd direct-mailleveringen ](../direct-mail/content-direct-mail.md):

   * Definieer de eigenschappen van het extractiebestand. [Meer informatie](../direct-mail/content-direct-mail.md#properties)
   * Selecteer de kolommen met de informatie die naar het bestand moet worden geëxporteerd. [Meer informatie](../direct-mail/content-direct-mail.md#content)

1. Geef een voorvertoning van het bestand weer en verzend proefdrukken <!--not in UI right now - to check--> . [ leer hoe ](../direct-mail/send-direct-mail.md#preview-dm)

   ![ Simuleer externe levering ](assets/external-delivery-simulate.png){zoomable="yes"}

1. Verzend de levering om het extractiebestand te genereren. [ leer hoe ](../direct-mail/send-direct-mail.md#send-dm)

Zodra de levering wordt verzonden, wordt het extractiedossier automatisch geproduceerd en uitgevoerd naar de plaats die in de [ wordt gespecificeerd externe rekening ](../administration/external-account.md#create-ext-account) in de montages van het leveringsmalplaatje wordt geselecteerd.

Houd de KPI&#39;s bij vanaf de leveringspagina en de gegevens in het menu **[!UICONTROL Logs]** .