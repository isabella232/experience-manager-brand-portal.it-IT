---
title: Note sulla versione
seo-title: Note sulla versione
description: Ottenete informazioni approfondite su funzioni, miglioramenti, problemi critici risolti e problemi noti nella release di Adobe Experience Manager Assets Brand Portal 6.4.6.
seo-description: Ottenete informazioni approfondite sui miglioramenti, i problemi critici risolti e i problemi noti nella release di Adobe Experience Manager Assets Brand Portal 6.4.6.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: e0aeb9a69c81add2d87463fc87d6d08ae57722b9

---


# Note sulla versione {#release-notes}

Ottenete informazioni approfondite sulle nuove funzioni, i miglioramenti, i problemi critici risolti e i problemi noti in Adobe Experience Manager Assets Brand Portal 6.4.6.

## Informazioni sulla versione {#release-information}

| Prodotto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versione | 6.4.6 |
| Data | Marzo 2020 |

## Panoramica {#overview}

Il Portale delle risorse di Adobe Experience Manager (AEM) Assets Brand consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su dispositivi diversi. Consente di migliorare l&#39;efficienza della condivisione delle risorse, di accelerare il time-to-market delle risorse e di ridurre il rischio di non conformità e di accesso non autorizzato. Brand Portal consente agli utenti di sfogliare, cercare, visualizzare in anteprima, scaricare ed esportare risorse in formati approvati dall’azienda, in qualsiasi momento e ovunque.

## What&#39;s New in 6.4.6 {#what-s-new-in-646}

### Nuove funzioni {#new-feature}

Questa versione include le nuove funzioni seguenti:

* Captcha per l’accesso degli ospiti al Brand Portal. Per ulteriori informazioni, consultate Accesso [ospiti al Brand Portal](../using/guest-access.md) .

### Miglioramenti {#enhancements-646}

Questa versione di Brand Portal include i seguenti miglioramenti:

* AEM Assets è ora configurato con Brand Portal tramite Adobe I/O, che fornisce un token IMS per l&#39;autorizzazione del tenant del Brand Portal.

   >[!NOTE]
   >
   >La configurazione tramite OAuth legacy non è più supportata dal 6 aprile 2020 e viene modificata in configurazione tramite I/O Adobe.


>[!TIP]
>
>***Solo per i clienti esistenti***
>
>Si consiglia di continuare a utilizzare la configurazione gateway OAuth esistente. In caso di problemi con la configurazione del gateway OAuth precedente, elimina la configurazione esistente e crea una nuova configurazione tramite Adobe I/O.


Per ulteriori informazioni, consulta [Configurare AEM Assets con il portale dei marchi](configure-aem-assets-with-brand-portal.md)

### Problemi critici risolti {#critical-issues-fixed}

Questa versione include correzioni ai seguenti problemi critici:

* I valori a discesa dello schema di metadati non sono visibili nelle proprietà della risorsa.

* Il sottoschema metadati non visualizza le schede in base al tipo di mimetismo nelle proprietà della risorsa.

* Lo schema di metadati Annulla pubblicazione compila un messaggio di errore anche se lo schema viene rimosso nel backend.

* L&#39;immagine di anteprima non viene visualizzata per una risorsa pubblicata.

* L’utente non può pubblicare o annullare la pubblicazione delle risorse contenenti virgolette singole nel nome.

* I termini e le condizioni non vengono visualizzati durante il download di più risorse.

* Sono state risolte vulnerabilità di sicurezza minori.

### Problemi noti {#known-issues}

Questa versione include i seguenti problemi noti:

* Gli utenti di Brand Portal non sono in grado di pubblicare le risorse delle cartelle dei contributi in Risorse AEM al momento dell’aggiornamento ad Adobe I/O su AEM 6.5.4.

   Questo problema verrà risolto nel service pack successivo 6.5.5.

   Per una correzione immediata su AEM 6.5.4, si consiglia di [scaricare l’hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e installarlo nell’istanza di creazione.

* L&#39;opzione Exclude System Renditions (Escludi rappresentazioni di sistema) non funziona correttamente durante il download di una risorsa.


## Lingue {#languages}

L’interfaccia utente di Brand Portal è disponibile nelle seguenti lingue:

* Inglese
* Tedesco
* Francese
* Spagnolo
* Italiano
* Portoghese brasiliano
* Giapponese
* Cinese semplificato
* Coreano

## Piattaforme certificate {#certified-platforms}

Per verificare quali piattaforme sono certificate per l’esecuzione con questa versione di Brand Portal, fate riferimento alla colonna **Supporto per l’interfaccia** touch nella tabella nella sezione Browser **supportati per l’authoring dell’interfaccia** utente dei requisiti [](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html)tecnici.

## Collegamenti {#links}

* [Pagina prodotto Adobe Experience Manager su adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentazione su Assets Brand Portal](https://helpx.adobe.com/experience-manager/brand-portal/user-guide.html)

## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se siete un cliente e richiedete l&#39;accesso, contattate il vostro account manager Adobe.

* [](https://daycare.day.com) Accesso [al prodotto](https://login.marketing.adobe.com)

* [Assistenza clienti Adobe](https://helpx.adobe.com/contact.html)
