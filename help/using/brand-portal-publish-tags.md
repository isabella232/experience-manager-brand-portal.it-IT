---
title: Pubblicare tag in Brand Portal
seo-title: Pubblicare tag in Brand Portal
description: Scoprite come pubblicare i tag da  AEM Assets a Brand Portal.
seo-description: Scoprite come pubblicare i tag da  AEM Assets a Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 4%

---


# Pubblicare tag in Brand Portal {#publish-tags-to-brand-portal}

Scoprite come pubblicare i tag da  AEM Assets a Brand Portal.

I tag sono utili per organizzare le risorse e migliorarne la ricercabilità. I tag possono essere considerati come parole chiave o etichette (metadati) associate alle risorse e consentono di trovare rapidamente le risorse come risultato di una ricerca. Per informazioni su come assegnare tag alle risorse in  AEM Assets, consultate [usare i tag per organizzare le risorse](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

I tag (associati alle risorse e alle raccolte in AEM) vengono pubblicati automaticamente in Brand Portal quando le risorse (e le raccolte) con i tag associati vengono pubblicate in Brand Portal. I tag pubblicati sono utili per consentire alle ricerche di trovare le risorse associate.

>[!NOTE]
>
>È tuttavia consigliabile pubblicare esclusivamente i tag in Brand Portal prima di pubblicare le risorse (e le raccolte) a cui sono associati i tag. Questo consente di pubblicare più rapidamente le risorse (e le raccolte) in Brand Portal.

## Gestire i tag {#manage-tags}

Potete usare i tag preesistenti per allegarli a una risorsa o creare nuovi tag dalla console Tag AEM (**[!UICONTROL Strumenti | Assegnazione tag | Tag AEM]**). In entrambi gli scenari è prima necessario pubblicare i tag in Brand Portal e quindi associarli alle risorse appropriate.

Per creare tag su AEM, pubblicate i tag su Brand Portal e associate i tag alle risorse appropriate (o raccolte), effettuate le seguenti operazioni:

1. **Crea**
tagAccedi all’istanza di AEM Author con privilegi amministrativi e accedi a  **[!UICONTROL AEM console]** Tag dalla navigazione globale:

   1. Selezionare **[!UICONTROL Strumenti]**

   1. Selezionare **[!UICONTROL Generale]**

   1. Selezionare **[!UICONTROL Tagging]**

1. Selezionare **[!UICONTROL Crea]**, quindi selezionare l&#39;opzione **[!UICONTROL Crea tag]**.
1. Specifica:

   * **[!UICONTROL Titolo]**

      *(obbligatorio)* Titolo visualizzato per il tag .
   * **[!UICONTROL Nome]**
      *(obbligatorio)* Un nome per il tag . Se non viene specificato, dal Titolo viene creato un nome di nodo valido. Vedere [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descrizione**

      *(facoltativo)* Una descrizione del tag .
   * **Assegna tag al percorso**
PathJCR del tag .

1. Selezionare **[!UICONTROL Invia]** per creare il tag.

   Dopo aver creato un tag sull’istanza AEM, il tag sarà disponibile per essere allegato a una risorsa (tramite la sezione Proprietà o la sezione Gestione tag della risorsa).

1. **Pubblicate il tag su Brand Portal**.

   Vai alla console **[!UICONTROL AEM Tag]** ([!UICONTROL Strumenti | Assegnazione tag | AEM Tag]), selezionate il tag desiderato e Pubblica sul portale dei marchi.

1. **Associate il tag a una risorsa (o raccolta)**.

   Selezionate una risorsa (o una raccolta) e allegate il tag desiderato tramite la sezione Proprietà o la sezione Gestione tag della risorsa. Per ulteriori informazioni su come assegnare i tag alle risorse in  AEM Assets, consultate [usare i tag per organizzare le risorse](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

1. **Pubblicate risorse (o raccolte) in Brand Portal**.\
   Quando pubblicate una risorsa (o una raccolta) in Brand Portal, il tag allegato è disponibile anche in Brand Portal.

   Per visualizzare il tag allegato sulla rispettiva risorsa (o raccolta) nel Portale marchio, accedete a Brand Portal e selezionate la risorsa, nella sezione Proprietà verrà visualizzato il tag allegato.

## Promozione ricerca {#search-promote}

 Portale del marchio AEM Assets consente di ottenere risorse specifiche come primi risultati per ricerche basate su un tag parola chiave.

Per elevare una risorsa per una parola chiave di ricerca, effettuate le seguenti operazioni:

1. Aprite la pagina **[!UICONTROL Properties]** di una risorsa nell’istanza AEM’autore.
1. Vai alla scheda **[!UICONTROL Avanzate]**.
1. In **[!UICONTROL Search Promote]** nella sezione **[!UICONTROL Elevate for search keywords]**, selezionare **[!UICONTROL Add]** per aggiungere le parole chiave o i tag di ricerca.

   ![](assets/search-promote.png)

1. Salva le modifiche.
1. Pubblica la risorsa in Brand Portal.
1. Effettuate l&#39;accesso al Brand Portal. Visualizzare la scheda **[!UICONTROL Avanzate]** nella sezione **[!UICONTROL Proprietà]** della risorsa.
La parola chiave **[!UICONTROL Search Promote]** è visibile anche nelle proprietà della risorsa.
