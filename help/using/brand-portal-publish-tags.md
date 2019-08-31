---
title: Pubblicare tag su Brand Portal
seo-title: Pubblicare tag su Brand Portal
description: Scopri come pubblicare tag da AEM Assets a Brand Portal.
seo-description: Scopri come pubblicare tag da AEM Assets a Brand Portal.
uuid: 4167367 e -1 af 8-476 b -97 a 5-730 c 43 bd 0816
topic-tags: pubblicazione
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: riferimento
discoiquuid: 3 c 8 e 9251-195 d -4 c 56-a 9 a 9-27 bc 8 b 2 a 82 a 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Publish tags to Brand Portal {#publish-tags-to-brand-portal}

Scopri come pubblicare tag da AEM Assets a Brand Portal.

I tag sono utili per organizzare le risorse e migliorare la ricerca delle risorse alle quali sono associate. I tag possono essere considerate come parole chiave o etichette (metadati) associati alle risorse e consentono di trovare rapidamente le risorse come risultato di una ricerca. Per sapere come assegnare tag alle risorse in Risorse AEM, consulta [Utilizzare i tag per organizzare le risorse](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

I tag (associati a risorse e raccolte in AEM) vengono pubblicati automaticamente su Brand Portal quando le risorse (e raccolte) con tag associati vengono pubblicate sul portale del marchio. I tag pubblicati sono utili per abilitare le ricerche per individuare le risorse associate.

>[!NOTE]
>
>È tuttavia consigliabile pubblicare in modo esclusivo tag su Brand Portal prima di pubblicare le risorse (e raccolte) con cui sono associati i tag. Questo garantisce una pubblicazione più veloce delle risorse (e raccolte) al portale marchio.

## Manage tags {#manage-tags}

Potete usare i tag preesistenti da allegare a una risorsa o creare nuovi tag dalla console Tag AEM (**[!UICONTROL Strumenti) | Assegnazione tag | Tag AEM]**). In entrambe le situazioni è necessario prima pubblicare i tag sul portale brand e associarli alle risorse appropriate.

Per creare tag su AEM, pubblicare i tag sul portale brand e associare i tag con risorse appropriate (o raccolte), effettuate le seguenti operazioni:

1. **Crea tag**
accedi all'istanza AEM Author con privilegi di amministratore e accedi **[!UICONTROL alla console Tag]** AEM dalla navigazione globale:

   1. Seleziona **[!UICONTROL strumenti]**

   2. Seleziona **[!UICONTROL generale]**

   3. Selezionare **[!UICONTROL i tag]**

2. Selezionate **[!UICONTROL Crea,]** quindi selezionate **[!UICONTROL Crea tag.]**
3. Specificate:

   * **[!UICONTROL Titolo]**
      *(obbligatorio)* Un titolo di visualizzazione per il tag.
   * **[!UICONTROL Nome]**
      *(obbligatorio)* Un nome per il tag. Se non viene specificato, viene creato un nome di nodo valido dal Titolo. Consultate [tagid](https://helpx.adobe.com/experience-manager/6-5/sites/developing/using/framework.html#TagID).
   * **Descrizione**
      *(Facoltativo)* Una descrizione del tag.
   * **Percorso**JCR percorso
del tag.

4. Selezionate **[!UICONTROL Invia]** per creare il tag.

   Dopo aver creato un tag nell'istanza di AEM, il tag sarà disponibile per essere allegato a una risorsa (utilizzando la sezione Proprietà o Gestisci tag della risorsa).

5. **Pubblicate il tag sul portale marchio**.

   Vai alla **[!UICONTROL console Tag]** AEM ([!UICONTROL Strumenti | Assegnazione tag | Tag AEM]), seleziona il tag desiderato e Pubblica su Brand Portal.

6. **Allegare il tag a una risorsa (o raccolta)**.

   Selezionate una risorsa (o una raccolta) e allegate il tag desiderato utilizzando la sezione Proprietà o Gestisci tag della risorsa. Per ulteriori informazioni su come assegnare tag alle risorse in Risorse AEM, consulta [Utilizzare i tag per organizzare le risorse](https://helpx.adobe.com/experience-manager/6-5/assets/using/organize-assets.html#Usetagstoorganizeassets).

7. **Pubblicare risorse (o raccolte) su Brand Portal**.\
   Quando pubblicate una risorsa (o una raccolta) sul portale marchio, il tag allegato è disponibile anche sul portale del marchio.

   Per visualizzare il tag allegato sulla rispettiva risorsa (o raccolta) in Brand Portal, effettuate l'accesso al portale brand e selezionate la risorsa, nella sezione Proprietà visualizzerete il tag allegato.

## Promozione ricerca {#search-promote}

AEM Assets Brand Portal consente di creare risorse specifiche come risultati principali per le ricerche basate su un tag parola chiave.

Per alzare una risorsa per una parola chiave di ricerca, effettuate le seguenti operazioni:

1. Aprite la **[!UICONTROL pagina Proprietà]** di una risorsa nell'istanza di creazione AEM.
2. Vai alla **[!UICONTROL scheda Avanzate]** .
3. In **[!UICONTROL Search Promote (Promuovi)]** nella sezione **[!UICONTROL Elevate for search keywords]** (Incremento delle parole chiave), selezionate **[!UICONTROL Aggiungi]** per aggiungere le parole chiave o i tag di ricerca.

   ![](assets/search-promote.png)

4. Salvate le modifiche.
5. Pubblica la risorsa in Brand Portal.
6. Accedete al portale marchio. Scheda Visualizza **[!UICONTROL avanzate]** nella **[!UICONTROL sezione Proprietà]** della risorsa.
La parola chiave **[!UICONTROL Search Promote]** è visibile anche nelle proprietà della risorsa.
