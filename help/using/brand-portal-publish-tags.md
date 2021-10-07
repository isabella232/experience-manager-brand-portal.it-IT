---
title: Pubblicare tag in Brand Portal
seo-title: Publish tags to Brand Portal
description: Scopri come pubblicare tag da Experience Manager Assets a Brand Portal.
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

Scopri come pubblicare tag da Experience Manager Assets a Brand Portal.

I tag sono utili per organizzare le risorse e migliorare la possibilità di cercare le risorse a cui sono associate. I tag possono essere paragonati a parole chiave o etichette (metadati) collegate alle risorse e consentono di trovare rapidamente le risorse in seguito a una ricerca. Per informazioni su come assegnare tag alle risorse in Experience Manager Assets, consulta [utilizzare tag per organizzare le risorse](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

I tag (associati alle risorse e alle raccolte in AEM) vengono pubblicati automaticamente in Brand Portal quando le risorse (e le raccolte) con i tag associati vengono pubblicate in Brand Portal. I tag pubblicati sono utili per consentire alle ricerche di trovare le risorse associate.

>[!NOTE]
>
>Si consiglia, tuttavia, di pubblicare esclusivamente tag in Brand Portal prima di pubblicare le risorse (e le raccolte) a cui sono associati i tag. Questo garantisce una pubblicazione più rapida delle risorse (e delle raccolte) in Brand Portal.

## Gestire i tag {#manage-tags}

Puoi utilizzare i tag preesistenti per allegarli a una risorsa o creare nuovi tag AEM console Tag (**[!UICONTROL Strumenti | Assegnazione tag | Tag AEM]**). In entrambi gli scenari, devi prima pubblicare i tag in Brand Portal e poi associarli alle risorse appropriate.

Per creare tag su AEM, pubblicare i tag su Brand Portal e associarli alle risorse appropriate (o alle raccolte), procedi come segue:

1. **Crea**
tagAccedi all’istanza di AEM Author con privilegi amministrativi e accedi a  **[!UICONTROL AEM]** Tagsconsole dalla navigazione globale:

   1. Seleziona **[!UICONTROL Strumenti]**

   1. Seleziona **[!UICONTROL Generale]**

   1. Seleziona **[!UICONTROL Tagging]**

1. Selezionare **[!UICONTROL Crea]**, quindi selezionare l&#39;opzione **[!UICONTROL Crea tag]**.
1. Specifica:

   * **[!UICONTROL Titolo]**

      *(obbligatorio)* Titolo da visualizzare per il tag.
   * **[!UICONTROL Nome]**
      *(obbligatorio)* Un nome per il tag. Se non viene specificato, dal Titolo viene creato un nome di nodo valido. Consulta [TagID](https://experienceleague.adobe.com/docs/experience-manager-65/developing/platform/tagging/framework.html).
   * **Descrizione**

      *(facoltativo)* Una descrizione del tag.
   * **Assegna tag al percorso**
JCR del tag .

1. Seleziona **[!UICONTROL Invia]** per creare il tag.

   Dopo aver creato un tag su AEM’istanza, il tag sarà disponibile per essere associato a una risorsa (tramite la sezione Proprietà o la sezione Gestione tag della risorsa).

1. **Pubblica il tag in Brand Portal**.

   Vai alla console **[!UICONTROL AEM Tag]** ([!UICONTROL Strumenti | Assegnazione tag | AEM Tag]), seleziona il tag desiderato e Pubblica in Brand Portal.

1. **Allega il tag a una risorsa (o raccolta)**.

   Seleziona una risorsa (o una raccolta) e allega il tag desiderato utilizzando la sezione Proprietà o la sezione Gestione tag della risorsa. Per ulteriori informazioni su come assegnare tag alle risorse in AEM Assets, consulta [utilizzare i tag per organizzare le risorse](https://experienceleague.adobe.com/docs/experience-manager-65/assets/managing/organize-assets.html).

1. **Pubblicare risorse (o raccolte) in Brand Portal**.\
   Quando pubblichi una risorsa (o una raccolta) in Brand Portal, il tag allegato è disponibile anche in Brand Portal.

   Per visualizzare il tag allegato sulla rispettiva risorsa (o raccolta) in Brand Portal, accedi a Brand Portal e seleziona la risorsa, nella sezione Proprietà verrà visualizzato il tag allegato.

## Promozione ricerca {#search-promote}

AEM Assets Brand Portal consente di ottenere risorse specifiche come primi risultati per le ricerche basate su un tag parola chiave.

Per elevare una risorsa per una parola chiave di ricerca, segui questi passaggi:

1. Apri la pagina **[!UICONTROL Proprietà]** di una risorsa AEM’istanza di authoring.
1. Vai alla scheda **[!UICONTROL Avanzate]** .
1. Nella sezione **[!UICONTROL Search Promote]** all&#39;interno della sezione **[!UICONTROL Elevate per parole chiave di ricerca]** , seleziona **[!UICONTROL Aggiungi]** per aggiungere parole chiave o tag di ricerca.

   ![](assets/search-promote.png)

1. Salva le modifiche.
1. Pubblica la risorsa in Brand Portal.
1. Accedi a Brand Portal. Visualizza la scheda **[!UICONTROL Avanzate]** nella sezione **[!UICONTROL Proprietà]** della risorsa.
La parola chiave **[!UICONTROL Search Promote]** è visibile anche nelle Proprietà della risorsa.
