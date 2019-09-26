---
title: Overview of AEM Assets Brand Portal
seo-title: Panoramica di AEM Assets Brand Portal
description: AEM Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
seo-description: AEM Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: riferimento
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# Overview of AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

As a marketer, you sometimes need to collaborate with channel partners and internal business users to quickly create, manage, and deliver relevant digital content to customers. Timely delivery of relevant content across the entire customer journey is critical to driving greater demand, conversion, engagement, and customer loyalty.

Tuttavia, è una sfida sviluppare soluzioni che supportano una condivisione efficiente e sicura dei logo del marchio, delle linee guida, delle risorse delle campagne o delle riprese di prodotti approvati con team, partner e rivenditori interni estesi.

**Adobe Experience Manager (AEM) Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.** It helps improve the efficiency of asset sharing, accelerates the time-to-market for assets, and reduces the risk of non-compliance and unauthorized access.

The browser-based portal environment enables you to easily upload, browse, search, preview, and export assets in approved formats.

## User personas in Brand Portal {#Personas}

Brand Portal supports the following user roles:

* Utente ospite
* Visualizzatore
* Editor
* Administrator

The following table lists the tasks that users in these roles can perform:

|  | **Sfoglia** | **Ricerca** | **Scarica** | **Share folders** | **Condivisione di una raccolta** | **Condivisione di risorse come collegamento** | **Accesso ad Strumenti di amministrazione** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Utente ospite** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visualizzatore** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Amministratore** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

* Gli utenti ospiti possono sfogliare, accedere e cercare risorse solo nelle cartelle pubbliche e nelle raccolte.

### Guest user {#guest-user}

Ogni utente che dispone di un accesso limitato alle risorse su Brand Portal senza essere autenticato è un utente ospite. La sessione guest consente agli utenti di accedere alle cartelle e alle raccolte pubbliche. In qualità di utente ospite, potete sfogliare i dettagli delle risorse e avere una visualizzazione completa delle risorse dei membri delle cartelle pubbliche e delle raccolte. Potete cercare, scaricare e aggiungere risorse pubbliche alla raccolta [!UICONTROL Lightbox] .

Tuttavia, la sessione degli ospiti non consente di creare raccolte e ricerche salvate e di condividerle ulteriormente. Gli utenti di una sessione ospite non possono accedere alle impostazioni delle cartelle e delle raccolte e non possono condividere le risorse come collegamento. Elenco delle attività che un utente ospite può eseguire:

[Sfogliare e accedere alle risorse pubbliche](browse-assets-brand-portal.md)

[Ricerca di risorse pubbliche](brand-portal-searching.md)

[Scaricare risorse pubbliche](brand-portal-download-users.md)

[Aggiungere risorse a [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Visualizzatore {#viewer}

Un utente standard in Brand Portal è in genere un utente con il ruolo di Visualizzatore. Un utente con questo ruolo può accedere a cartelle, raccolte e risorse consentite. L’utente può anche sfogliare, visualizzare in anteprima, scaricare ed esportare risorse (rappresentazioni originali o specifiche), configurare le impostazioni dell’account e cercare risorse. Elenco delle attività che un visualizzatore può eseguire:

[Sfogliare le risorse](browse-assets-brand-portal.md)

[Ricerca di risorse](brand-portal-searching.md)

[Scaricare le risorse](brand-portal-download-users.md)

### Editor {#editor}

Un utente con il ruolo di Editor può eseguire tutte le attività che un visualizzatore può eseguire. Inoltre, in Editor è possibile visualizzare i file e le cartelle condivisi da un amministratore. L’utente con il ruolo di Editor può anche condividere contenuti (file, cartelle, raccolte) con altri utenti.

Oltre alle attività che un visualizzatore può eseguire, un editor può eseguire le seguenti attività aggiuntive:

[Condividere le cartelle](brand-portal-sharing-folders.md)

[Condivisione di una raccolta](brand-portal-share-collection.md)

[Share assets as a link](brand-portal-link-share.md)

### Administrator {#administrator}

Un amministratore include un utente contrassegnato come amministratore di sistema o amministratore di prodotti Brand Portal in [!UICONTROL Admin Console]. An administrator can add and remove system administrators and users, define presets, send email to users, and view portal usage and storage reports.

An administrator can perform all tasks that an Editor can perform the following additional tasks:

[Manage users, groups, and user roles](brand-portal-adding-users.md)

[Customize wallpaper, page headers, and emails](brand-portal-branding.md)

[Use custom search facets](brand-portal-search-facets.md)

[Uso del modulo schema metadati](brand-portal-metadata-schemas.md)

[Applicazione di predefiniti per immagini o rappresentazioni dinamiche](brand-portal-image-presets.md)

[Utilizzo dei rapporti](brand-portal-reports.md)

Oltre alle attività descritte sopra, un autore in Risorse AEM può effettuare le seguenti operazioni:

[Configurare l’integrazione di AEM Assets con Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html)

[Pubblicare le cartelle su Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Pubblicare raccolte in Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

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

1. Dalla pagina di accesso al Brand Portal, selezionate **[!UICONTROL Fate clic qui]** corrispondente a **[!UICONTROL Necessità di accesso?]**. Tuttavia, per entrare nella sessione ospite, selezionate il **[!UICONTROL Click here]** corrispondente a **[!UICONTROL Guest Access?]**.

   ![Schermata di accesso a Brand Portal](assets/bp-login-requestaccess.png)

   Viene visualizzata la pagina [!UICONTROL Richiedi accesso] .

2. Per richiedere l'accesso al Portale marchio di un'organizzazione, è necessario disporre di un [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]o [!UICONTROL Federated ID]valido.

   Nella pagina [!UICONTROL Richiedi accesso] , effettuate l’accesso con il vostro ID (scenario 1) o create un ID  Adobe (scenario 2):<br />
   ![[!UICONTROL Richiedi accesso]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. Se disponete di un [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]o [!UICONTROL Federated ID], fate clic su **[!UICONTROL Accedi]**.
Viene visualizzata la pagina [!UICONTROL Accesso] .
   2. Immetti le credenziali [!UICONTROL Adobe ID] e fai clic su **[!UICONTROL Accedi]**.<br />
   ![Adobe sign in](assets/bplogin_request_access_3.png)

   Viene nuovamente visualizzata la pagina [!UICONTROL Richiedi accesso] .<br />
   **Scenario 2**
   1. If you do not have an Adobe ID, to create one, click Get an Adobe ID from the Request Access page.
****
The Sign in page opens.
   2. Click **[!UICONTROL Get an Adobe ID]**.
The Sign up page opens.
   3. Immettete il nome e il cognome, l’ID e-mail e la password.
   4. Selezionate **[!UICONTROL Iscrizione]**.<br />
   ![](assets/bplogin_request_access_5.png)

   Viene nuovamente visualizzata la pagina [!UICONTROL Richiedi accesso] .

3. Nella pagina successiva vengono visualizzati il nome e l’ID e-mail utilizzati per richiedere l’accesso. Lasciate un commento all'amministratore e fate clic su **[!UICONTROL Invia]**.<br />

   ![](assets/bplogin-request-access.png)

## Gli amministratori di prodotto concedono l'accesso {#grant-access-to-brand-portal}

Gli amministratori di prodotti Brand Portal ricevono richieste di accesso nell’area di notifica del Portale marchio e tramite e-mail nella propria inbox.

![Accesso alla notifica richiesta](assets/bplogin_request_access_7.png)

Per concedere l’accesso, gli amministratori di prodotto devono fare clic sulla notifica pertinente nell’area di notifica del Portale marchio, quindi fare clic su **[!UICONTROL Concedi accesso]**.
In alternativa, gli amministratori di prodotto possono seguire il collegamento fornito nel messaggio e-mail di richiesta di accesso per visitare Adobe [!UICONTROL Admin Console] e aggiungere l'utente alla configurazione di prodotto pertinente.

Verrai reindirizzato alla home page di [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) . Utilizza Adobe [!UICONTROL Admin Console] per creare utenti e assegnarli ai profili di prodotto (precedentemente definiti configurazioni di prodotto), che vengono visualizzati come gruppi in Brand Portal. Per ulteriori informazioni sull’aggiunta di utenti in [!UICONTROL Admin Console], consulta [Aggiungere un utente](brand-portal-adding-users.md#add-a-user) (seguire i passaggi 4-7 della procedura per aggiungere un utente).

## Lingue Brand Portal {#brand-portal-language}

Puoi cambiare la lingua del Portale marchio dalle impostazioni [!UICONTROL di Adobe]Experience Cloud.

![Accesso alla notifica richiesta](assets/BPLang.png)

Per modificare la lingua:

1. Selezionate [!UICONTROL Utente] &gt; [!UICONTROL Modifica profilo] dal menu principale.<br />
   ![Modifica profilo](assets/EditBPProfile.png)

2. Nella pagina Impostazioni [!UICONTROL di] Experience Cloud, seleziona una lingua dal menu a discesa [!UICONTROL Lingua] .

## Notifica di manutenzione del Brand Portal {#brand-portal-maintenance-notification}

Prima che Brand Portal venga pianificato per la manutenzione, una notifica viene visualizzata come banner dopo l’accesso al Brand Portal. Una notifica di esempio:

![](assets/bp_maintenance_notification.png)

Potete ignorare questa notifica e continuare a utilizzare Brand Portal. Questa notifica viene visualizzata in ogni nuova sessione.

## Informazioni sulla versione e sul sistema {#release-and-system-information}

* [Novità](whats-new.md)
* [Note sulla versione](brand-portal-release-notes.md)
* [Formati di file supportati](brand-portal-supported-formats.md)

## Related resources {#related-resources}

* [Assistenza clienti Adobe](https://helpx.adobe.com/marketing-cloud/contact-support.html)
* [Forum su AEM](https://www.adobe.com/go/aod_forums_en)