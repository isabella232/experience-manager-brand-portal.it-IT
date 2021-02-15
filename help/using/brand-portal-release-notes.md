---
title: Note sulla versione
seo-title: Note sulla versione
description: Ottieni informazioni approfondite su funzioni, miglioramenti, problemi critici risolti e problemi noti di Adobe Experience Manager Assets Brand Portal 2021.02.0.
seo-description: Ottenete informazioni approfondite sui miglioramenti, i problemi critici risolti e i problemi noti in Adobe Experience Manager Assets Brand Portal 2021.02.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 69cf1756a546355ed767ac13c51fb09932254dbc
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---


# Note sulla versione {#release-notes}

Scopri le nuove funzioni, i miglioramenti, i problemi critici risolti e i problemi noti di Adobe Experience Manager Assets Brand Portal 2021.02.0.

## Informazioni sulla versione {#release-information}

| Prodotto | Portale marchio Adobe Experience Manager Assets |
|---|---|
| Versione | 2021.02.0 |
| Data | Febbraio 2021 |

## Panoramica {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi. Consente di migliorare l&#39;efficienza della condivisione delle risorse, di accelerare il time-to-market delle risorse e di ridurre il rischio di non conformità e di accesso non autorizzato. Brand Portal consente agli utenti di sfogliare, cercare, visualizzare in anteprima, scaricare ed esportare risorse in formati approvati dall’azienda, in qualsiasi momento e ovunque.

## Novità in 2021.02.0 {#whats-new-in-2021.02.0}

### Nuove funzioni {#new-features}

Questa versione include le nuove funzioni seguenti:

* In **[!UICONTROL Impostazioni di download]** è stata introdotta un&#39;ulteriore impostazione **[!UICONTROL Download delle risorse]**. Crea una cartella separata per ciascuna risorsa durante il download delle cartelle, delle raccolte o del download in blocco delle risorse. Vedere [impostazioni di download](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download).

<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions. See [steps to download assets from Brand Portal](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets).
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog. See [download assets from asset details page](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#download-assets-from-asset-details-page).
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download-permissions) to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

### Miglioramenti {#enhancements}

Questa versione include i seguenti miglioramenti:

* Per il download delle cartelle, viene creata una cartella separata per ciascuna risorsa utilizzando il collegamento di condivisione, indipendentemente dalle **[!UICONTROL Impostazioni di download]**.
* Il Portale marchio **[!UICONTROL Rapporto sull&#39;utilizzo]** è stato modificato per riflettere solo gli utenti attivi del Portale marchio.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemi critici risolti {#critical-issues-fixed}

Questa versione include correzioni ai seguenti problemi critici:

* Se vengono scaricate solo le risorse originali, la risorsa riflette la sua estensione e non si apre finché l’estensione non viene modificata manualmente in zip.
* L&#39;interfaccia utente della cartella della raccolta non risponde quando si fa clic sulla freccia di navigazione.
* **[!UICONTROL Il pulsante]** Createbon è visibile nella  **** visualizzazione Colonna anche quando le cartelle sono vuote.
* **[!UICONTROL La]** ricerca Omni non riesce con un messaggio di errore 414 (URI richiesta troppo lungo) se il dispatcher viene bypassato durante l&#39;accesso all&#39;istanza del Brand Portal.
* Se la risorsa contiene una virgola (`,`) nel nome del file, viene scaricata una cartella zip vuota.
* Gli utenti del visualizzatore hanno la possibilità di aggiungere utenti alla raccolta che hanno creato.
* Si verifica un comportamento incoerente quando una risorsa (miniatura o rappresentazione Web) viene scaricata tramite il collegamento di condivisione.

Consultate [novità in Brand Portal 2021.02.0](whats-new.md).

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* Search on the **[!UICONTROL Asset Reports]** shows processing on the product interface with no search result.
* The video DM encodes are not visible to the non-admin users on the asset details page.
* The alignment of the size of individual asset renditions and total download size is distorted in the Download dialog.
-->


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

Per verificare quali piattaforme sono certificate per l&#39;esecuzione con questa versione di Brand Portal, fare riferimento alla colonna **Supporto per l&#39;interfaccia touch** nella tabella nella sezione **Browser supportati per l&#39;interfaccia utente di authoring** di [Requisiti tecnici](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Collegamenti {#links}

* [Pagina prodotto Adobe Experience Manager su adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentazione su Assets Brand Portal](https://helpx.adobe.com/it/experience-manager/brand-portal/user-guide.html)

## Accesso e supporto al prodotto (siti limitati) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se siete un cliente e richiedete l&#39;accesso, contattate il vostro responsabile commerciale  Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Accesso al prodotto](https://login.marketing.adobe.com)

* [Assistenza clienti  Adobe](https://helpx.adobe.com/contact.html)
