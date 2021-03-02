---
title: Note sulla versione
seo-title: Note sulla versione
description: Ottieni informazioni approfondite su funzioni, miglioramenti, problemi critici risolti e problemi noti nella versione 2021.02.0 di Adobe Experience Manager Assets Brand Portal.
seo-description: Scopri i miglioramenti, i problemi critici risolti e i problemi noti nella versione 2021.02.0 di Adobe Experience Manager Assets Brand Portal.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
translation-type: tm+mt
source-git-commit: 302bbf441453a760fe53d981a61b2eb014ebd1f0
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 6%

---


# Note sulla versione {#release-notes}

Scopri le nuove funzioni, i miglioramenti, i problemi critici risolti e i problemi noti con la versione 2021.02.0 di Adobe Experience Manager Assets Brand Portal.

## Informazioni sulla versione {#release-information}

| Prodotto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versione | 2021.02.0 |
| Data | Febbraio 2021 |

## Panoramica {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi. Consente di migliorare l’efficienza della condivisione delle risorse, di accelerare il time-to-market delle risorse e di ridurre il rischio di non conformità e di accesso non autorizzato. Brand Portal consente agli utenti di sfogliare, cercare, visualizzare in anteprima, scaricare ed esportare le risorse in formati approvati dall’azienda, in qualsiasi momento e ovunque.

## Novità di 2021.02.0 {#whats-new-in-2021.02.0}

### Nuove funzioni {#new-features}

Questa versione include le seguenti nuove funzionalità:

* La funzione Origine risorse è ora disponibile su AEM Assets as a Cloud Service. Consente agli utenti di Brand Portal di caricare le risorse nelle cartelle dei contributi consentite e pubblicare la cartella dei contributi da Brand Portal nell’istanza di AEM Assets as a Cloud Service.

* Un&#39;ulteriore impostazione **[!UICONTROL Download delle risorse]** è stata introdotta in **[!UICONTROL Impostazioni di download]**. Crea una cartella separata per ogni risorsa durante il download delle cartelle, delle raccolte o del download in blocco di risorse. Consulta [scarica impostazioni](https://docs.adobe.com/content/help/en/experience-manager-brand-portal/using/download/brand-portal-download-assets.html#configure-download).

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

* Per il download delle cartelle, viene creata una cartella separata per ogni risorsa utilizzando il collegamento di condivisione, indipendentemente dalle **[!UICONTROL impostazioni di download]**.
* Il Brand Portal **[!UICONTROL Rapporto utilizzo]** è stato modificato per riflettere solo gli utenti attivi di Brand Portal.

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemi critici risolti {#critical-issues-fixed}

Questa versione include correzioni ai seguenti problemi critici:

* Nel caso in cui vengano scaricate solo le risorse originali, la risorsa riflette la propria estensione e non si apre finché l’estensione non viene modificata manualmente in zip.
* L&#39;interfaccia utente della cartella di raccolta non risponde quando si fa clic sulla freccia di navigazione.
* **** Il pulsante di creazione è visibile in  **** Columnview anche quando le cartelle sono vuote.
* **[!UICONTROL La]** ricerca Omni non riesce con un messaggio di errore 414 (Request-URI Too Long) se il dispatcher viene bypassato durante l’accesso all’istanza di Brand Portal.
* Viene scaricata una cartella zip vuota se la risorsa contiene una virgola (`,`) nel nome del file.
* Gli utenti del visualizzatore possono aggiungere utenti alla raccolta creata.
* Si verifica un comportamento incoerente quando una risorsa (miniatura o rendering web) viene scaricata utilizzando il collegamento di condivisione.

Consulta [novità di Brand Portal 2021.02.0](whats-new.md).

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

Per verificare quali piattaforme sono certificate per l’esecuzione con questa versione di Brand Portal, consulta la colonna **Supporto per l’interfaccia touch** nella tabella della sezione **Browser supportati per l’authoring Interfaccia utente** di [Requisiti tecnici](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Collegamenti {#links}

* [Pagina del prodotto Adobe Experience Manager su adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentazione di Assets Brand Portal](https://helpx.adobe.com/it/experience-manager/brand-portal/user-guide.html)

## Accesso e supporto ai prodotti (siti con restrizioni) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se sei un cliente e hai bisogno di accedere, contatta il tuo account manager Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Accesso al prodotto](https://login.marketing.adobe.com)

* [Assistenza clienti Adobe](https://helpx.adobe.com/contact.html)
