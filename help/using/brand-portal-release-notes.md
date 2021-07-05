---
title: Note sulla versione
seo-title: Note sulla versione
description: Ottieni informazioni approfondite su funzioni, miglioramenti, problemi critici risolti e problemi noti nella versione Adobe Experience Manager Assets Brand Portal 2021.06.0.
seo-description: Ottieni informazioni approfondite sui miglioramenti, i problemi critici risolti e i problemi noti nella versione Adobe Experience Manager Assets Brand Portal 2021.06.0.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 54af86b96ef3c3cfe3b1c0db7772d369cac9bb71
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 11%

---

# Note sulla versione {#release-notes}

Scopri le nuove funzioni, i miglioramenti, i problemi critici risolti e i problemi noti nella versione Adobe Experience Manager Assets Brand Portal 2021.06.0.

## Informazioni sulla versione {#release-information}

| Prodotto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versione | 2021.06.0 |
| Data | Giugno 2021 |

## Panoramica {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi. Consente di migliorare l’efficienza della condivisione delle risorse, di accelerare il time-to-market delle risorse e di ridurre il rischio di non conformità e di accesso non autorizzato. Brand Portal consente agli utenti di sfogliare, cercare, visualizzare in anteprima, scaricare ed esportare le risorse in formati approvati dall’azienda, in qualsiasi momento e ovunque.

## Novità di 2021.06.0 {#whats-new-in-2021.06.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
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

<!--
### Enhancements {#enhancements}

Brand Portal 2021.06.0 is an internal release for T2E migration that introduces a new workflow to facilitate orgranization specific entitlement to the Brand Portal users. 

This release includes the following enhancements:

* For a new or migrated T2E organization, the users will have an organization specific entitlement. 


* The new users added to Admin Console will have to **Join Team** to get entitled to the T2E organization. 

* The administrators will get an additional screen to select the T2E organization while navigating from Brand Portal to Admin Console.
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.
-->


### Problemi critici risolti {#critical-issues-fixed}

Brand Portal 2021.06.0 è una versione interna che include correzioni ai seguenti problemi critici:

* Le notifiche e-mail di Asset Sourcing non vengono recapitate per alcune organizzazioni.

* I file video con estensione .mov non sono in esecuzione su Brand Portal.

* Nel menu a discesa Raccolte avanzate sono visibili solo 10 raccolte salvate.

<!--
* *_deleted tenants are listed as valid tenant which fails during the execution of TenantCustomizers/TenantUpdates where tenant id is returned as /etc/tenants/`<nodename>`.
-->

<!--
In case only the original assets are downloaded, the asset reflects its own extension and does not open until the extension is manually changed to zip. 
* The user interface of the collection folder does not respond on clicking the navigation arrow. 
* **[!UICONTROL Create]** button is visible in the **[!UICONTROL Column]** view even when the folders are empty.
* **[!UICONTROL Omni search]** fails with a 414 error message (Request-URI Too Long) if the dispatcher is bypassed while accessing the Brand Portal instance.
* An empty zip folder is downloaded if the asset contains a comma (`,`) in the file name.
* The viewer users get the option to add users to the collection they have created. 
* Inconsistent behavior is experienced when an asset (thumbnail or web rendition) is downloaded using share link.

See [what's new in Brand Portal 2021.02.0](whats-new.md).
-->

<!--
### Known Issues {#known-issues}

This release includes the following known issue:

* The users will not be able to login to Brand Portal during the migration of their existing organization to T2E. 

  However, the active users will be able to continue to work untill their current session expires or the migration is complete.   
-->

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

Per verificare quali piattaforme sono certificate per l’esecuzione con questa versione di Brand Portal, consulta la colonna **Supporto per l’interfaccia touch** nella tabella nella sezione **Browser supportati per l’interfaccia utente di authoring** di [Requisiti tecnici](https://helpx.adobe.com/experience-manager/6-4/sites/deploying/using/technical-requirements.html).

## Collegamenti {#links}

* [Pagina del prodotto Adobe Experience Manager su adobe.com](http://www.adobe.com/in/marketing-cloud/experience-manager.html)
* [Documentazione di Assets Brand Portal](https://helpx.adobe.com/it/experience-manager/brand-portal/user-guide.html)

## Accesso e supporto ai prodotti (siti con restrizioni) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se sei un cliente e hai bisogno di accedervi, contatta il tuo account manager Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

* [Accesso al prodotto](https://login.marketing.adobe.com)

* [Adobe Customer Care](https://helpx.adobe.com/contact.html)
