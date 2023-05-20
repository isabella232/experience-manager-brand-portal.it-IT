---
title: Pubblicare tag in Brand Portal
seo-title: Publish tags to Brand Portal
description: Scopri come pubblicare i tag da Experience Manager Assets a Brand Portal.
seo-description: Learn how to publish tags from Experience Manager Assets to Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
exl-id: 842656a6-1a2b-4b64-954d-1e663923a1a1
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 4%

---

# Pubblicare tag in Brand Portal {#publish-tags-to-brand-portal}

Scopri come pubblicare i tag da Experience Manager Assets a Brand Portal.

I tag sono utili per organizzare le risorse e migliorare la ricercabilità delle risorse a cui sono associati. I tag possono essere considerati come parole chiave o etichette (metadati) associate alle risorse e consentono di trovare rapidamente le risorse come risultato di una ricerca. Per informazioni su come assegnare tag alle risorse in Experience Manager Assets, consulta [utilizzare i tag per organizzare le risorse](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

I tag (associati alle risorse e alle raccolte in AEM) vengono pubblicati automaticamente in Brand Portal quando le risorse (e le raccolte) con i tag associati vengono pubblicate in Brand Portal. I tag pubblicati sono utili per consentire alle ricerche di trovare le risorse associate.

>[!NOTE]
>
>Tuttavia, si consiglia di pubblicare esclusivamente i tag in Brand Portal prima di pubblicare le risorse (e le raccolte) a cui sono associati i tag. In questo modo si garantisce una pubblicazione più rapida delle risorse (e delle raccolte) in Brand Portal.

## Gestione tag {#manage-tags}

Puoi utilizzare i tag preesistenti per allegare una risorsa o creare nuovi tag dalla console Tag AEM (**[!UICONTROL Strumenti | Assegnazione tag | Tag AEM]**). In entrambi gli scenari devi innanzitutto pubblicare i tag in Brand Portal e quindi associarli alle risorse appropriate.

Per creare tag su AEM, pubblicarli su Brand Portal e associarli alle risorse (o raccolte) appropriate, effettua le seguenti operazioni:

1. **Creare i tag**
Accedere all’istanza di AEM Author con privilegi di amministratore e **[!UICONTROL Tag AEM]** console dalla navigazione globale:

   1. Seleziona **[!UICONTROL Strumenti]**

   1. Seleziona **[!UICONTROL Generale]**

   1. Seleziona **[!UICONTROL Assegnazione tag]**

1. Seleziona **[!UICONTROL Crea]** e quindi seleziona **[!UICONTROL Crea tag]** opzione.
1. Specifica:

   * **[!UICONTROL Titolo]**

      *(obbligatorio)* Titolo da visualizzare per il tag.
   * **[!UICONTROL Nome]**
      *(obbligatorio)* Un nome per il tag. Se non viene specificato, viene creato un nome di nodo valido dal titolo. Consulta [TagID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html).
   * **Descrizione**

      *(facoltativo)* Descrizione del tag.
   * **Percorso tag**
Percorso JCR del tag.

1. Seleziona **[!UICONTROL Invia]** per creare il tag.

   Dopo aver creato un tag nell’istanza AEM, il tag sarà disponibile per essere allegato a una risorsa (utilizzando la sezione Proprietà o la sezione Gestisci tag di tale risorsa).

1. **Pubblicare il tag in Brand Portal**.

   Vai a **[!UICONTROL Tag AEM]** console ([!UICONTROL Strumenti | Assegnazione tag | Tag AEM]), seleziona il tag desiderato e pubblica su Brand Portal.

1. **Associa il tag a una risorsa (o raccolta)**.

   Seleziona una risorsa (o una raccolta) e allega il tag desiderato utilizzando la sezione Proprietà o la sezione Gestisci tag di tale risorsa. Per ulteriori informazioni su come assegnare tag alle risorse in AEM Assets, consulta [utilizzare i tag per organizzare le risorse](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

1. **Pubblicare risorse (o raccolte) in Brand Portal**.\
   Quando pubblichi una risorsa (o raccolta) in Brand Portal, il tag allegato è disponibile anche in Brand Portal.

   Per visualizzare il tag allegato alla rispettiva risorsa (o raccolta) in Brand Portal, accedi a Brand Portal e seleziona la risorsa. Nella sezione Proprietà verrà visualizzato il tag allegato.

## Promozione ricerca {#search-promote}

AEM Assets Brand Portal consente di impostare risorse specifiche come risultati principali per le ricerche basate su un tag parola chiave.

Per elevare una risorsa a livello di parola chiave di ricerca, effettua le seguenti operazioni:

1. Apri **[!UICONTROL Proprietà]** pagina di una risorsa nell’istanza di authoring AEM.
1. Vai a **[!UICONTROL Avanzate]** scheda.
1. In entrata **[!UICONTROL Promozione ricerca]** entro **[!UICONTROL Privilegi elevati per parole chiave di ricerca]** sezione, seleziona **[!UICONTROL Aggiungi]** per aggiungere parole chiave o tag di ricerca.

   ![](assets/search-promote.png)

1. Salva le modifiche.
1. Pubblica la risorsa in Brand Portal.
1. Accedi a Brand Portal. Visualizza **[!UICONTROL Avanzate]** scheda in **[!UICONTROL Proprietà]** sezione della risorsa.
Tieni presente che **[!UICONTROL Promozione ricerca]** La parola chiave è visibile anche nelle Proprietà della risorsa.
