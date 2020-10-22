---
title: Note sulla versione
seo-title: Note sulla versione
description: Ottieni informazioni approfondite su funzioni, miglioramenti, problemi critici risolti e problemi noti di Adobe Experience Manager Assets Brand Portal 2020.10.0.
seo-description: Ottenete informazioni approfondite sui miglioramenti, i problemi critici risolti e i problemi noti in Adobe Experience Manager Assets Brand Portal 2020.10.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 8881e9d171c3a4e750a906caadd8aa26f6fc0674
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 7%

---


# Note sulla versione {#release-notes}

Scopri le nuove funzioni, i miglioramenti, i problemi critici risolti e i problemi noti di Adobe Experience Manager Assets Brand Portal 2020.10.0.

## Informazioni sulla versione {#release-information}

| Prodotto | Portale marchio Adobe Experience Manager Assets |
|---|---|
| Versione | 2020.10.0 |
| Data | Ottobre 2020 |

## Panoramica {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi. Consente di migliorare l&#39;efficienza della condivisione delle risorse, di accelerare il time-to-market delle risorse e di ridurre il rischio di non conformità e di accesso non autorizzato. Brand Portal consente agli utenti di sfogliare, cercare, visualizzare in anteprima, scaricare ed esportare risorse in formati approvati dall’azienda, in qualsiasi momento e ovunque.

## What&#39;s New in 2020.10.0 {#whats-new-in-2020.10.0}

### New Features {#new-features}

Questa versione include le nuove funzioni seguenti:

* La finestra di dialogo **[!UICONTROL Scarica]** è stata rinnovata in una vista a elenco con opzioni aggiuntive per escludere le rappresentazioni non richieste, applicare lo stesso set di regole per tipi di risorse simili e scaricare le rappresentazioni delle risorse selezionate.

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

* È ora possibile passare a **[!UICONTROL File]**, **[!UICONTROL Raccolte]** e Collegamenti **** condivisi da tutte le pagine Portale marchio con un solo clic.

* Il pannello **[!UICONTROL Rappresentazioni]** nella pagina dei dettagli delle risorse ora consente agli utenti del Brand Portal di selezionare la risorsa originale e (o) le rappresentazioni di risorse specifiche e di scaricarle direttamente dal pannello **[!UICONTROL Rappresentazioni]** senza dover aprire la finestra di dialogo **[!UICONTROL Scarica]** .

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

* Oltre alle configurazioni di **[!UICONTROL download]** esistenti, gli amministratori del Portale marchio possono configurare le autorizzazioni per diversi gruppi di utenti per visualizzare e (o) scaricare la risorsa originale e le relative rappresentazioni dalla pagina dei dettagli della risorsa. Queste configurazioni definiranno chi può accedere e (o) scaricare le rappresentazioni delle risorse.

### Miglioramenti {#enhancements}

Questa versione include i seguenti miglioramenti:

* La soglia di timeout sessione per gli utenti ospiti è stata ridotta da 2 ore a 15 minuti.
* L’opzione Pagine **** di visualizzazione aggiuntive è stata rimossa per i PDF con più pagine, in quanto ora l’utente può visualizzare le pagine PDF dal visualizzatore Adobe Document Cloud.


<!--
### Critical Issues Fixed {#critical-issues-fixed}

This release includes fixes to the following critical issue:

* The users are not able to view the PDF pages if the PDF contains sub assets.
-->

### Problemi noti {#known-issues}

Questa versione include il seguente problema noto:

* La ricerca nei report **[!UICONTROL delle]** risorse mostra l&#39;elaborazione nell&#39;interfaccia del prodotto senza risultati di ricerca.
* Le codifiche video DM non sono visibili agli utenti non amministratori nella pagina dei dettagli della risorsa.
* L’allineamento delle dimensioni delle rappresentazioni delle singole risorse e della dimensione totale del download è distorto nella finestra di dialogo Download.



<!--
* Download Settings configuration to configure asset download from Brand Portal. Fast download, custom renditions, and system renditions are the available configurations. 
-->

<!--
* Document Viewer has been introduced to enhance the PDF viewing experience. New options are available for viewing the PDF files in Brand Portal.

* Advances in the asset download process which improves the Brand Portal user experience while [downloading assets from Brand Portal](brand-portal-download-assets.md). Brand Portal administrators can configure **[!UICONTROL Fast Download]**, **[!UICONTROL Custom Renditions]**, and **[!UICONTROL System Renditions]** from the **[!UICONTROL Download]** settings. 

For details, see [what's new in Brand Portal 6.4.7](whats-new.md). 

### Critical Issues Fixed {#critical-issues-fixed-647}

This release includes fixes to the following critical issues:

* The viewer users are not permitted to share link for collections but the option to share is visible to them on the product interface.

* The **[!UICONTROL Download]** button on the options bar does not list all the licensed assets of the selected folder.

* The search takes longer to show the results for certain keywords.

* The **[!UICONTROL Agree]** and **[!UICONTROL Disagree]** check boxes does not appear on bulk selection of licensed and unlicensed assets during download.

* Filter-based search shows processing on the product interface with no search result. 

* The assets do not download from share link if the shared folder contains numerous and large assets.


### Known Issues {#known-issues-647}

This release includes the following known issues:

* If multiple assets are selected, license text does not appear on clicking Terms and Conditions on the license agreement page during download using share link.   

-->

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
* [Documentazione su Assets Brand Portal](https://helpx.adobe.com/it/experience-manager/brand-portal/user-guide.html)

## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se siete un cliente e richiedete l&#39;accesso, contattate il vostro responsabile commerciale  Adobe.

* [https://daycare.day.com](https://daycare.day.com)

* [Accesso al prodotto](https://login.marketing.adobe.com)

* [Assistenza clienti  Adobe](https://helpx.adobe.com/contact.html)
