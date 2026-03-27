---
audience: end-user
title: De workflowactiviteit Deelnemen gebruiken
description: Leer hoe u de workflowactiviteit Deelnemen gebruikt
exl-id: 2470e5fa-5596-4441-b9b9-7e8b5d1d53aa
source-git-commit: 9b51dc84a5b6954c973e1560aad877ef770eb8f9
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Verbinden {#join}

>[!CONTEXTUALHELP]
>id="acw_homepage_welcome_rn5"
>title="Meerdere workflowvertakkingen en activiteiten samenvoegen"
>abstract="Meerdere vertakkingen worden nu ondersteund. In plaats van een vork te gebruiken, kunt u op Add tak op de toolbar klikken. De AND-join-activiteit is ook verbeterd. Het is nu een generische samenvoegactiviteit die u tussen EN en OF laat zich aansluiten opties kiezen."
>additional-url="https://experienceleague.adobe.com/docs/campaign-web/v8/release-notes/release-notes.html" text="Zie opmerkingen bij releases"

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join"
>title="AND-join-activiteit"
>abstract="De **en-sluit zich aan** activiteit staat u toe om veelvoudige uitvoeringstakken van een werkschema te synchroniseren. De regeling wordt in werking gesteld zodra alle voorgaande activiteiten zijn beëindigd. Zo weet u zeker dat bepaalde activiteiten zijn voltooid voordat u doorgaat met het uitvoeren van de workflow."

>[!CONTEXTUALHELP]
>id="acw_orchestration_join"
>title="Deelnemen aan activiteit"
>abstract="**sluit zich aan** activiteit aan laat u veelvoudige binnenkomende overgangen samenvoegen. Kies of u wilt doorgaan wanneer alle binnenkomende overgangen zijn voltooid (AND) of wanneer een binnenkomende overgang is voltooid (OR)."

**sluit zich aan** activiteit is de controle **activiteit van de a** Stroom. Meerdere uitvoeringstakken van een workflow worden gesynchroniseerd.
U kunt kiezen hoe binnenkomende overgangen worden geëvalueerd:

* **EN**: Blijft slechts nadat alle geselecteerde binnenkomende overgangen worden geactiveerd.
* **OF**: Blijft zodra één geselecteerde binnenkomende overgang wordt geactiveerd.

Wanneer **EN** wordt geselecteerd, brengt deze activiteit zijn uitgaande overgang teweeg slechts nadat alle binnenkomende overgangen worden geactiveerd. Met andere woorden, het activeert zodra alle voorgaande activiteiten zijn voltooid. Zo zorgt u ervoor dat bepaalde activiteiten zijn voltooid voordat u doorgaat met het uitvoeren van de workflow.

Wanneer **OF** wordt geselecteerd, gaat de uitvoering voort zodra één van de geselecteerde binnenkomende overgangen wordt geactiveerd. Er wordt niet op elke vertakking gewacht.

## Vorm de Join activiteit {#join-configuration}

>[!CONTEXTUALHELP]
>id="acw_orchestration_and-join_merging"
>title="Samenvoegopties"
>abstract="Selecteer de activiteiten waaraan u wilt deelnemen. In de **Primaire reeks** drop-down, kies welke binnenkomende overgangspopulatie u wilt houden."

Volg deze stappen om **te vormen verbind** activiteit:

1. Voeg meerdere activiteiten toe, zoals kanaalactiviteiten, om minstens twee verschillende uitvoeringstakken te vormen. U kunt a **Vonk** gebruiken of een afzonderlijke tak toevoegen gebruikend **vertakking** (+) toolbarknoop toevoegen. Zie [&#x200B; Orchestrate activiteiten &#x200B;](../orchestrate-activities.md#toolbar).

   ![&#x200B; Screenshot die twee takken toont.](../assets/workflow-join.png)

1. Voeg a **&#x200B;**&#x200B;activiteit aan om het even welke takken toe.

   ![&#x200B; Screenshot die de Join toegevoegde activiteit tonen.](../assets/workflow-join2.png)

1. In sluit zich aan bij opties, kies **EN** of **OF** en klik **verdergaan**.
1. In de **het samenvoegen opties** sectie, controleer alle vorige activiteiten u zich wilt aansluiten.
1. In de **Primaire reeks** drop-down, kies welke binnenkomende overgangspopulatie om te houden. De uitgaande overgang kan slechts één van de binnenkomende overgangspopulaties bevatten.

   >[!NOTE]
   >
   >Het **Primaire vastgestelde** gebied is slechts beschikbaar voor **EN** sluit zich aan bij optie.

   ![&#x200B; Scherenshot die gevormde verbindingen toont.](../assets/workflow-join3.png)

## Voorbeeld {#join-example}

In het volgende voorbeeld worden twee workflowvertakkingen getoond met een e-mail- en sms-levering. **sluit zich aan** activiteit aan, die aan **EN** wordt geplaatst, trekkers wanneer beide binnenkomende overgangen worden toegelaten. Pushmeldingen worden alleen verzonden nadat beide leveringen zijn voltooid. Als u plaatst sluit zich aan bij optie aan **OF**, worden de duwberichten verzonden zodra de eerste binnenkomende leveringsactiviteit wordt voltooid.

![&#x200B; Voorbeeld van een werkschema met twee takken, die e-mail en levering van SMS door dupberichten tonen.](../assets/workflow-join4.png){zoomable="yes"}