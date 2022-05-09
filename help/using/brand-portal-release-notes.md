---
title: Note sulla versione
seo-title: Release Notes
description: Ottieni informazioni approfondite su funzioni, miglioramenti, problemi critici risolti e problemi noti nella versione Adobe Experience Manager Assets Brand Portal 2022.05.0.
seo-description: Get an insight into the enhancements, critical issues fixed, and known issues in the Adobe Experience Manager Assets Brand Portal 2022.05.0 release.
uuid: 3d6ffb6f-4608-4e83-8486-5c90e06cdb43
content-type: reference
contentOwner: Anuj Kapoor
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 79ebb9fc-385c-48a8-979e-374f42517988
exl-id: e4e89080-9863-4857-8f3a-fcd516ef3271
source-git-commit: 5ca00738be59632ffcd481c2d007f869b561b9db
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 9%

---

# Note sulla versione {#release-notes}

Scopri le nuove funzioni, i miglioramenti, i problemi critici risolti e i problemi noti nella versione Adobe Experience Manager Assets Brand Portal 2022.05.0.

## Informazioni sulla versione {#release-information}

| Prodotto | Adobe Experience Manager Assets Brand Portal |
|---|---|
| Versione | 2022.05.0 |
| Data | Maggio 2022 |

## Panoramica {#overview}

Adobe Experience Manager (AEM) Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi. Consente di migliorare l’efficienza della condivisione delle risorse, di accelerare il time-to-market delle risorse e di ridurre il rischio di non conformità e di accesso non autorizzato. Brand Portal consente agli utenti di sfogliare, cercare, visualizzare in anteprima, scaricare ed esportare le risorse in formati approvati dall’azienda, in qualsiasi momento e ovunque.

## Novità nel 2022.05.0 {#whats-new-in-2022.05.0}

<!--
### New Features {#new-features}

This release includes the following new features:

* AEM Assets as a Cloud Service is now entitled to have a pre-configured Brand Portal instance. The Cloud Manager user can activate Brand Portal on the AEM Assets as a Cloud Service instance.

* Asset Sourcing feature is now available on AEM Assets as a Cloud Service. It allows the Brand Portal users to upload assets to the permitted contribution folders and publish the contribution folder from Brand Portal to AEM Assets as a Cloud Service instance. 

* An additional **[!UICONTROL Asset Download]** setting has been introduced under the **[!UICONTROL Download Settings]**. It creates a separate folder for each asset while downloading the folders, collections, or bulk download of assets. 
-->
<!-- 
* The **[!UICONTROL Download]** dialog is revamped in a list view with additional options to exclude the renditions which are not required, apply the same set of rules for similar asset types, and download the selected asset renditions.
-->

<!--
* The new **[!UICONTROL Download]** dialog now appears with all the renditions of the selected assets or folders containing assets in a list view, wherein the Brand Portal users can apply same set of renditions for similar asset types and download the selected asset renditions. 
-->

<!-- 
* Navigation to the **[!UICONTROL Files]**, **[!UICONTROL Collections]**, and **[!UICONTROL Shared Links]** is now possible from all the Brand Portal pages in one-click.  

* The **[!UICONTROL Renditions]** panel in the asset details page now allows the Brand Portal users to select the original asset and (or) specific asset renditions, and directly download them from the **[!UICONTROL Renditions]** panel without having to open the **[!UICONTROL Download]** dialog.
-->

<!--
Brand Portal users can exclude specific renditions which are not required and directly download the original asset and its renditions from the **[!UICONTROL Renditions]** panel on the asset details page. 
-->

<!-- 
* In addition to the existing **[!UICONTROL Download]** configurations, the Brand Portal administrators can also [configure permissions for different group of users]() to view and (or) download the original asset and its renditions from the asset details page. These configurations will define who can access and (or) download the asset renditions.
-->

<!--
### Enhancements {#enhancements}

Brand Portal 2021.08.0 is an internal release that introduces Business profiles for enterprise and teams customers to give organizations better control over their assets. 

This release includes the following enhancements:

* The users now have organization-specific entitlement on the new and migrated organizations. If a user is entitled to multiple organizations, the user has to select the organization at the time of login.

* The new users that are added in Admin Console must **Join Team** to get entitled to the organization. 

>[!NOTE]
>
>Business profiles are currently applicable for the new organizations that are created after August 16, 2021. 
>
>Until your organization is migrated, you can continue to use Adobe ID, Enterprise ID, or Federated ID types to access the organization.   
-->

<!-- 
* For folder download, a separate folder is created for each asset using share link irrespective of the **[!UICONTROL Download Settings]**. 
* The Brand Portal **[!UICONTROL Usage Report]** has been modified to reflect only the active Brand Portal users.
-->

<!--
* The threshold of session timeout for the guest users has been reduced from 2 hours to 15 minutes.
* The additional **[!UICONTROL View pages]** option has been removed for multi-page PDFs as the user can now view the PDF pages from the Adobe Document Cloud Viewer.

* The users are unable to search, navigate, or open folders. The user interface reflects the error message: `Failed to load data`. 
* The **[!UICONTROL Renditions]** panel does not list all the static renditions of the assets that are published to Brand Portal.
* The **[!UICONTROL Renditions]** panel lists the smart crop renditions of the asset, however, the user cannot preview or download the smart crop renditions.
* The download dialog lists the smart crop renditions of the selected asset, however, the user cannot download the smart crop renditions. 
* A non-admin user is getting only the original asset rendition when downloading an asset. The system and custom renditions are not downloaded.  
* When applying search filter to download an asset, the `Download` button is disabled in the download dialog and does not allows the user to download the asset.
* If `Smart Tags` and (or) `Color Tags` are enabled, the download dialog lists the `json` files as renditions and downloads these `json` files in the archived zip folder.
* The anonymous users are unable to download assets using a shared link because the link redirects to the Brand Portal login page. 
* The system is not reflecting the correct value for the number of active concurrent users.
-->

### Nuove funzioni {#new-features}

Brand Portal ora esegue processi automatici ogni dodici ore per eliminare tutte le risorse Brand Portal pubblicate in AEM. Di conseguenza, non è necessario eliminare manualmente le risorse nella cartella Contribution per mantenere la dimensione della cartella al di sotto del limite di soglia. Vedi [Novità di Experience Manager Assets Brand Portal](whats-new.md).


### Problemi critici risolti {#critical-issues-fixed}

Questa versione include correzioni ai seguenti problemi critici:

* Quando si scarica una cartella o una raccolta che include risorse con tag colore, viene scaricato anche un file XML.

* Quando scarichi un video che include rappresentazioni, Brand Portal crea un file .ZIP non valido.

* Quando crei predefiniti e risorse su AEM autore e li pubblichi in Brand Portal e poi selezioni rappresentazioni dinamiche durante il download delle risorse, non puoi estrarre i file scaricati. File ZIP.

* Problemi durante il download di risorse video da alcune cartelle disponibili su Brand Portal.

* Quando condividi l’URL della cartella Contribution tramite un’e-mail, i ruoli Visualizzatore ed Editor incontrano problemi durante l’accesso alla cartella principale tramite la breadcrumb.

* Il rapporto pubblicato di determinazione origine visualizza un&#39;ora di inizio del processo non corretta.


<!--
* Asset Sourcing email notifications are not delivered for some organizations. 

* Video files with extension `.mov` are not running on Brand Portal. 

* In the **[!UICONTROL Smart Collections]** dropdown list, only ten saved collections are visible. 
-->
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


### Problemi noti {#known-issues}

Questa versione include il seguente problema noto:

* Localizzazione parziale nel contenuto del report Asset sourcing .


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

Per verificare quali piattaforme sono certificate per l’esecuzione con questa versione di Brand Portal, consulta **Supporto per l’interfaccia touch** nella tabella **Browser supportati per l’interfaccia utente di authoring** sezione [Requisiti tecnici](https://experienceleague.adobe.com/docs/experience-manager-65/deploying/introduction/technical-requirements.html).

## Collegamenti {#links}

* [Pagina del prodotto Adobe Experience Manager su adobe.com](https://business.adobe.com/in/products/experience-manager/adobe-experience-manager.html)
* [Documentazione di Assets Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-brand-portal/using/home.html)

## Accesso e supporto ai prodotti (siti con restrizioni) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se sei un cliente e hai bisogno di accedervi, contatta il tuo account manager Adobe.

<!--
* [https://daycare.day.com](https://daycare.day.com) 
-->

<!--
* [Customer Support]()
-->
