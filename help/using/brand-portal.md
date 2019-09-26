---
title: Panoramica di AEM Assets Brand Portal
seo-title: Panoramica di AEM Assets Brand Portal
description: AEM Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi.
seo-description: AEM Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: riferimento
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduzione
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: f9397850937a5adb01ec41bc3b60afa712a4ddc3

---


# Panoramica di AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

In qualità di esperto di marketing, a volte devi collaborare con partner di canale e utenti aziendali interni per creare, gestire e fornire rapidamente contenuti digitali rilevanti ai clienti. La distribuzione tempestiva di contenuti rilevanti nell'intero percorso del cliente è fondamentale per stimolare una maggiore domanda, conversione, coinvolgimento e fidelizzazione dei clienti.

Tuttavia, è una sfida sviluppare soluzioni che supportano una condivisione efficiente e sicura dei logo del marchio, delle linee guida, delle risorse delle campagne o delle riprese di prodotti approvati con team, partner e rivenditori interni estesi.

**Risorse Adobe Experience Manager (AEM) Assets Brand Portal** consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su dispositivi diversi. Consente di migliorare l'efficienza della condivisione delle risorse, di accelerare il time-to-market delle risorse e di ridurre il rischio di non conformità e di accesso non autorizzato.

L’ambiente portale basato su browser consente di caricare, sfogliare, cercare, visualizzare in anteprima ed esportare facilmente le risorse in formati approvati.

## Personalità utente in Brand Portal {#Personas}

Brand Portal supporta i seguenti ruoli utente:

* Guest user
* Visualizzatore
* Editor
* Amministratore

Nella tabella seguente sono elencate le attività che gli utenti di questi ruoli possono eseguire:

|  | **Sfoglia** | **Ricerca** | **Scarica** | **Condividere le cartelle** | **Condivisione di una raccolta** | **Condivisione di risorse come collegamento** | **Accesso ad Strumenti di amministrazione** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Guest user** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visualizzatore** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Amministratore** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Gli utenti ospiti possono sfogliare, accedere e cercare risorse solo nelle cartelle pubbliche e nelle raccolte.

### Guest user {#guest-user}

Ogni utente che dispone di un accesso limitato alle risorse su Brand Portal senza essere autenticato è un utente ospite. La sessione guest consente agli utenti di accedere alle cartelle e alle raccolte pubbliche. In qualità di utente ospite, potete sfogliare i dettagli delle risorse e avere una visualizzazione completa delle risorse dei membri delle cartelle pubbliche e delle raccolte. Potete cercare, scaricare e aggiungere risorse pubbliche alla raccolta [!UICONTROL Lightbox] .

Tuttavia, la sessione degli ospiti non consente di creare raccolte e ricerche salvate e di condividerle ulteriormente. Gli utenti di una sessione ospite non possono accedere alle impostazioni delle cartelle e delle raccolte e non possono condividere le risorse come collegamento. Here is a list of tasks that a guest user can perform:

[Sfogliare e accedere alle risorse pubbliche](browse-assets-brand-portal.md)

[Search public assets](brand-portal-searching.md)

[Download public assets](brand-portal-download-users.md)

[Add assets to [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Visualizzatore {#viewer}

A standard user in Brand Portal is typically a user with the role of Viewer. A user with this role can access permitted folders, collections, and assets. The user can also browse, preview, download, and export assets (original or specific renditions), configure account settings, and search for assets. Here is a list of tasks that a Viewer can perform:

[Browse assets](browse-assets-brand-portal.md)

[Search for assets](brand-portal-searching.md)

[Download assets](brand-portal-download-users.md)

### Editor {#editor}

A user with the role of Editor can perform all tasks that a Viewer can perform. In addition, and Editor can view the files and folders that an administrator shares. The user with the role of an Editor can also share content (files, folders, collections) with others.

Apart from the tasks that a Viewer can perform, an Editor can perform the following additional tasks:

[Condividere le cartelle](brand-portal-sharing-folders.md)

[Share a collection](brand-portal-share-collection.md)

[Condivisione di risorse come collegamento](brand-portal-link-share.md)

### Amministratore {#administrator}

Un amministratore include un utente contrassegnato come amministratore di sistema o amministratore di prodotti Brand Portal in [!UICONTROL Admin Console]. Un amministratore può aggiungere e rimuovere amministratori di sistema e utenti, definire predefiniti, inviare e-mail agli utenti e visualizzare rapporti sull’uso e l’archiviazione del portale.

Un amministratore può eseguire tutte le attività che un utente con privilegi di editor può eseguire le seguenti attività aggiuntive:

[Gestione di utenti, gruppi e ruoli utente](brand-portal-adding-users.md)

[Personalizzare sfondi, intestazioni di pagina ed e-mail](brand-portal-branding.md)

[Utilizzare facet di ricerca personalizzati](brand-portal-search-facets.md)

[Uso del modulo schema metadati](brand-portal-metadata-schemas.md)

[Applicazione di predefiniti per immagini o rappresentazioni dinamiche](brand-portal-image-presets.md)

[Utilizzo dei rapporti](brand-portal-reports.md)

Oltre alle attività descritte sopra, un autore in Risorse AEM può effettuare le seguenti operazioni:

[Configurare l’integrazione di AEM Assets con Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Publish folders to Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Publish collections to Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alias alternativo per l’URL del Brand Portal {#tenant-alias-for-portal-url}

A partire da Brand Portal 6.4.3, le organizzazioni possono disporre di un URL alternativo (alias) per l’URL esistente del tenant del Brand Portal. L’URL alias può essere creato con un prefisso alternativo nell’URL.\
Tenete presente che è possibile personalizzare solo il prefisso dell’URL del Portale marchio e non l’intero URL. Ad esempio, un’organizzazione con un dominio esistente **[!UICONTROL geomettrix.brand-Portal.adobe.com]** può creare su richiesta **[!UICONTROL geomettrixinc.brand-Portal.adobe.com]** .

Tuttavia, l'istanza di AEM Author può essere [configurata](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html) solo con l'URL dell'ID tenant e non con l'alias tenant (alternativo).

>[!NOTE]
>
>Per ottenere un alias per il nome del tenant nell'URL del portale esistente, le organizzazioni devono contattare il supporto Adobe con una nuova richiesta di creazione alias del tenant. Questa richiesta viene elaborata verificando prima se l'alias è disponibile e quindi creando l'alias.
>
>Per sostituire il vecchio alias o eliminarlo, è necessario seguire lo stesso processo.

## Richiesta di accesso a Brand Portal {#request-access-to-brand-portal}

Gli utenti possono richiedere l’accesso a Brand Portal dalla schermata di accesso. Queste richieste vengono inviate agli amministratori del Brand Portal che concedono l’accesso agli utenti tramite Adobe [!UICONTROL Admin Console]. Una volta concesso l’accesso, gli utenti ricevono un messaggio e-mail di notifica.

Per richiedere l’accesso, effettuate le seguenti operazioni:

1. Dalla pagina di accesso al Brand Portal, selezionate **[!UICONTROL Fate clic qui]** corrispondente a **[!UICONTROL Necessità di accesso?]**. However, to enter the guest session, select the Click here corresponding to Guest Access?.********

   ![Schermata di accesso a Brand Portal](assets/bp-login-requestaccess.png)

   The Request Access page opens.

2. To request access to an organization’s Brand Portal, you must have a valid Adobe ID, Enterprise ID, or Federated ID.

   In the Request Access page, sign in using your ID (scenario 1) or create an Adobe ID (scenario 2):
   ![[!UICONTROL Request access]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. If you have an Adobe ID, Enterprise ID, or Federated ID, click Sign In.
****
The Sign in page opens.
   2. Provide your Adobe ID credentials and click Sign in.****<br />
   ![Adobe sign in](assets/bplogin_request_access_3.png)

   You are redirected to the Request Access page.
   **Scenario 2**
   1. If you do not have an Adobe ID, to create one, click Get an Adobe ID from the Request Access page.
****
Viene visualizzata la pagina [!UICONTROL Accesso] .
   2. Click **[!UICONTROL Get an Adobe ID]**.
The Sign up page opens.
   3. Enter your first and last name, email ID, and password.
   4. Select Sign up.****<br />
   ![](assets/bplogin_request_access_5.png)

   Viene nuovamente visualizzata la pagina [!UICONTROL Richiedi accesso] .

3. Nella pagina successiva vengono visualizzati il nome e l’ID e-mail utilizzati per richiedere l’accesso. Lasciate un commento all'amministratore e fate clic su **[!UICONTROL Invia]**.

   ![](assets/bplogin-request-access.png)

## Gli amministratori di prodotto concedono l'accesso {#grant-access-to-brand-portal}

Gli amministratori di prodotti Brand Portal ricevono richieste di accesso nell’area di notifica del Portale marchio e tramite e-mail nella propria inbox.

![Accesso alla notifica richiesta](assets/bplogin_request_access_7.png)

Per concedere l’accesso, gli amministratori di prodotto devono fare clic sulla notifica pertinente nell’area di notifica del Portale marchio, quindi fare clic su **[!UICONTROL Concedi accesso]**.
In alternativa, gli amministratori di prodotto possono seguire il collegamento fornito nel messaggio e-mail di richiesta di accesso per visitare Adobe [!UICONTROL Admin Console] e aggiungere l'utente alla configurazione di prodotto pertinente.
![](assets/bplogin_request_access_8.png)

Verrai reindirizzato alla home page di [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) . Utilizza Adobe [!UICONTROL Admin Console] per creare utenti e assegnarli ai profili di prodotto (precedentemente definiti configurazioni di prodotto), che vengono visualizzati come gruppi in Brand Portal. Per ulteriori informazioni sull’aggiunta di utenti in [!UICONTROL Admin Console], consulta [Aggiungere un utente](brand-portal-adding-users.md#add-a-user) (seguire i passaggi 4-7 della procedura per aggiungere un utente).

## Lingue Brand Portal {#brand-portal-language}

Puoi cambiare la lingua del Portale marchio dalle impostazioni [!UICONTROL di Adobe]Experience Cloud.

![Accesso alla notifica richiesta](assets/BPLang.png)

Per modificare la lingua:

1. Selezionate [!UICONTROL Utente] &gt; [!UICONTROL Modifica profilo] dal menu principale.
   ![Modifica profilo](assets/EditBPProfile.png)

2. Nella pagina Impostazioni [!UICONTROL di] Experience Cloud, seleziona una lingua dal menu a discesa [!UICONTROL Lingua] .

## Notifica di manutenzione del Brand Portal {#brand-portal-maintenance-notification}

Prima che Brand Portal venga pianificato per la manutenzione, una notifica viene visualizzata come banner dopo l’accesso al Brand Portal. Una notifica di esempio:

![](assets/bp_maintenance_notification.png)

Potete ignorare questa notifica e continuare a utilizzare Brand Portal. Questa notifica viene visualizzata in ogni nuova sessione.

## Informazioni sulla versione e sul sistema {#release-and-system-information}

<!--* [What's new](../using/whats-new.md)-->
* [Note sulla versione](brand-portal-release-notes.md)
* [Formati di file supportati](brand-portal-supported-formats.md)

## Related resources {#related-resources}

* [Assistenza clienti Adobe](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [Forum su AEM](https://www.adobe.com/go/aod_forums_en)