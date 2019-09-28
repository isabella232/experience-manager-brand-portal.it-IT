---
title: Pubblicare i tag su Brand Portal
seo-title: Pubblicare i tag su Brand Portal
description: Scopri come pubblicare i tag da AEM Assets al Brand Portal.
seo-description: Scopri come pubblicare i tag da AEM Assets al Brand Portal.
uuid: 4167367e-1af8-476b-97a5-730c43bd0816
topic-tags: pubblicazione
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: riferimento
discoiquuid: 3c8e9251-195d-4c56-a9a9-27bc8b2a82a4
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

Scopri come pubblicare i tag da AEM Assets al Brand Portal.

I tag sono utili per organizzare le risorse e migliorarne la ricercabilità. I tag possono essere considerati parole chiave o etichette (metadati) associate alle risorse e consentire di trovare rapidamente le risorse come risultato di una ricerca. Per informazioni su come assegnare tag a risorse in Risorse AEM, consultate [Utilizzo di tag per organizzare le risorse](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

I tag (associati alle risorse e alle raccolte in AEM) vengono pubblicati automaticamente in Brand Portal quando le risorse (e le raccolte) con i tag associati vengono pubblicate in Brand Portal. I tag pubblicati sono utili per consentire alle ricerche di trovare le risorse associate.

>[!NOTE]
>
>È tuttavia consigliabile pubblicare esclusivamente i tag in Brand Portal prima di pubblicare le risorse (e le raccolte) a cui sono associati i tag. Questo consente di pubblicare più rapidamente le risorse (e le raccolte) in Brand Portal.

## Manage tags {#manage-tags}

Puoi usare i tag preesistenti per allegarli a una risorsa o creare nuovi tag dalla console Tag AEM (**[!UICONTROL Strumenti)| Assegnazione tag| Tag]** AEM). In entrambi gli scenari è prima necessario pubblicare i tag in Brand Portal e quindi associarli alle risorse appropriate.

Per creare tag su AEM, pubblicare i tag su Brand Portal e associare i tag alle risorse appropriate (o alle raccolte), effettuate le seguenti operazioni:

1. **Crea tag** Accedi all’istanza di AEM Author con privilegi amministrativi e accedi alla console Tag **** AEM dalla navigazione globale:

   1. Seleziona **[!UICONTROL strumenti]**

   1. Seleziona **[!UICONTROL generale]**

   1. Seleziona **[!UICONTROL tag]**

1. Selezionate **[!UICONTROL Crea]** , quindi selezionate l’opzione **[!UICONTROL Crea tag]** .
1. Specificate:

   * **[!UICONTROL Titolo]**
      *(obbligatorio)* Titolo visualizzato per il tag .
   * **[!UICONTROL Nome]**
      *(obbligatorio)* Un nome per il tag . Se non viene specificato, dal Titolo viene creato un nome di nodo valido. Consulta [TagID](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descrizione**
      *(facoltativo)* Una descrizione del tag.
   * **Percorso** JCR del tag.

1. Selezionate **[!UICONTROL Invia]** per creare il tag.

   Dopo aver creato un tag sull’istanza di AEM, il tag sarà disponibile per essere allegato a una risorsa (tramite la sezione Proprietà o la sezione Gestione tag della risorsa).

1. **Pubblicate il tag su Brand Portal**.

   Vai alla console Tag **** AEM ([!UICONTROL Strumenti)| Assegnazione tag| Tag]AEM), selezionate il tag desiderato e Pubblica sul portale dei marchi.

1. **Associate il tag a una risorsa (o raccolta)**.

   Selezionate una risorsa (o una raccolta) e allegate il tag desiderato utilizzando la sezione Proprietà o la sezione Gestione tag della risorsa. Per ulteriori informazioni su come assegnare i tag alle risorse in Risorse AEM, consultate [Utilizzo dei tag per organizzare le risorse](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

1. **Pubblicate risorse (o raccolte) in Brand Portal**.\
   Quando pubblicate una risorsa (o una raccolta) in Brand Portal, il tag allegato è disponibile anche in Brand Portal.

   Per visualizzare il tag allegato sulla rispettiva risorsa (o raccolta) nel Portale marchio, accedete a Brand Portal e selezionate la risorsa, nella sezione Proprietà verrà visualizzato il tag allegato.

## Promozione ricerca {#search-promote}

AEM Assets Brand Portal consente di ottenere risorse specifiche come primi risultati per ricerche basate su un tag parola chiave.

Per elevare una risorsa per una parola chiave di ricerca, effettuate le seguenti operazioni:

1. Aprite la pagina **[!UICONTROL Proprietà]** di una risorsa nell’istanza di creazione di AEM.
1. Vai alla scheda **[!UICONTROL Avanzate]** .
1. Nella sezione **[!UICONTROL Search Promote]** in **[!UICONTROL Elevate for search keywords]** , selezionare **[!UICONTROL Aggiungi]** per aggiungere le parole chiave o i tag di ricerca.

   ![](assets/search-promote.png)

1. Salvate le modifiche.
1. Pubblica la risorsa in Brand Portal.
1. Effettuate l'accesso al Brand Portal. Visualizzare la scheda **[!UICONTROL Avanzate]** nella sezione **[!UICONTROL Proprietà]** della risorsa.
La parola chiave **[!UICONTROL Search Promote]** è visibile anche nelle proprietà della risorsa.
