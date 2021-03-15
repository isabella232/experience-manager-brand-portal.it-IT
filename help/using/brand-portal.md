---
title: Panoramica di AEM Assets Brand Portal
seo-title: Panoramica di AEM Assets Brand Portal
description: AEM Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi.
seo-description: AEM Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: 59eeaedd7f66a0a5affa53f82f3ebbb2bcea535d
workflow-type: tm+mt
source-wordcount: '1554'
ht-degree: 7%

---


# Panoramica di AEM Assets Brand Portal {#overview-of-aem-assets-brand-portal}

In qualità di addetto al marketing, a volte è necessario collaborare con i partner di canale e gli utenti aziendali interni per creare, gestire e fornire rapidamente contenuti digitali pertinenti ai clienti. La distribuzione tempestiva di contenuti rilevanti in tutto il percorso di clienti è fondamentale per incrementare la domanda, la conversione, il coinvolgimento e la fidelizzazione dei clienti.

Tuttavia, è una sfida sviluppare soluzioni che supportino la condivisione efficiente e sicura di logo di marchio approvati, linee guida, risorse di campagne o scatti di prodotti con team interni, partner e rivenditori estesi.

**Adobe Experience Manager (AEM) Assets Brand** Portal si concentra sulla necessità dell’addetto al marketing di collaborare in modo efficace con gli utenti di Brand Portal distribuiti a livello globale, fornendo funzionalità di distribuzione delle risorse e contributi alle risorse.

La distribuzione delle risorse consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi. Il contributo risorse consente invece agli utenti di Brand Portal di caricare le risorse su Brand Portal e pubblicarle in AEM Assets, senza necessità di accedere all’ambiente di authoring. La funzione di contributo è denominata **Origine risorse in Brand Portal**. Insieme, migliora l’esperienza complessiva di Brand Portal nella distribuzione delle risorse e nel contributo degli utenti di Brand Portal (agenzie/team esterni), accelera il time-to-market delle risorse e riduce il rischio di non conformità e di accesso non autorizzato.
Consulta [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).

L’ambiente portale basato su browser consente di caricare, sfogliare, cercare, visualizzare in anteprima ed esportare facilmente le risorse nei formati approvati.

## Configurare AEM Assets con Brand Portal {#configure-brand-portal}

La configurazione di Adobe Experience Manager Assets con Brand Portal consente agli utenti di Brand Portal di pubblicare risorse, distribuirle risorse e apportare risorse.

>[!NOTE]
>
>La configurazione di AEM Assets con Brand Portal è supportata in AEM Assets as a Cloud Service, AEM Assets 6.3 e versioni successive.

AEM Assets as a Cloud Service viene configurato automaticamente con Brand Portal attivando Brand Portal da Cloud Manager. Il flusso di lavoro di attivazione crea le configurazioni richieste nel backend e attiva Brand Portal nella stessa organizzazione IMS di AEM Assets come istanza di Cloud Service.

Al contrario, AEM Assets (on-premise e Managed Service) viene configurato manualmente con Brand Portal utilizzando Adobe Developer Console, che fornisce un token Adobe Identity Management Services (IMS) per l’autorizzazione del tenant di Brand Portal.

Per ulteriori informazioni, consulta [configurazione di AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Utenti e utenti in Brand Portal {#Personas}

Brand Portal supporta i seguenti ruoli utente:

* Utente ospite
* Visualizzatore
* Editor
* Administrator

Nella tabella seguente sono elencate le attività che gli utenti di questi ruoli possono eseguire:

|  | **Sfoglia** | **Ricerca** | **Scarica** | **Condividere le cartelle** | **Condividere una raccolta** | **Condividere le risorse come collegamento** | **Accesso a Strumenti di amministrazione** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Utente ospite** | Sì* | Sì* | Sì* | x | x | x | x |
| **Visualizzatore** | . | . | . | x | x | x | x |
| **Editor** | . | . | . | . | . | . | x |
| **Administrator** | . | . | . | . | . | . | . |

* Gli utenti ospiti possono sfogliare, accedere e cercare le risorse solo in cartelle pubbliche e raccolte.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Utente ospite {#guest-user}

Qualsiasi utente con accesso limitato alle risorse su Brand Portal senza autenticazione è un utente ospite. La sessione guest consente agli utenti di accedere a cartelle e raccolte pubbliche. In qualità di utente ospite, puoi sfogliare i dettagli delle risorse e avere una visualizzazione completa delle risorse dei membri delle cartelle pubbliche e delle raccolte. Puoi cercare, scaricare e aggiungere risorse pubbliche alla raccolta [!UICONTROL Lightbox].

Tuttavia, la sessione guest ti limita a creare raccolte e ricerche salvate e a condividerle ulteriormente. Gli utenti di una sessione guest non possono accedere alle impostazioni di cartelle e raccolte e non possono condividere le risorse come collegamento. Elenco delle attività eseguibili da un utente guest:

[Navigare e accedere alle risorse pubbliche](browse-assets-brand-portal.md)

[Cercare risorse pubbliche](brand-portal-searching.md)

[Scaricare risorse pubbliche](brand-portal-download-assets.md)

[Aggiungere risorse a  [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Visualizzatore {#viewer}

Un utente standard in Brand Portal è in genere un utente con il ruolo di Visualizzatore. Un utente con questo ruolo può accedere a cartelle, raccolte e risorse consentite. L’utente può anche sfogliare, visualizzare in anteprima, scaricare ed esportare le risorse (rappresentazioni originali o specifiche), configurare le impostazioni dell’account e cercare le risorse. Elenco delle attività eseguibili da un visualizzatore:

[Sfogliare le risorse](browse-assets-brand-portal.md)

[Cercare risorse](brand-portal-searching.md)

[Scaricare le risorse](brand-portal-download-assets.md)

### Editor {#editor}

Un utente con il ruolo di Editor può eseguire tutte le attività che un Visualizzatore può eseguire. Inoltre, e Editor può visualizzare i file e le cartelle condivisi da un amministratore. L’utente con il ruolo di Editor può anche condividere contenuti (file, cartelle, raccolte) con altri.

Oltre alle attività eseguibili da un visualizzatore, un editor può eseguire le seguenti attività aggiuntive:

[Condividere le cartelle](brand-portal-sharing-folders.md)

[Condividere una raccolta](brand-portal-share-collection.md)

[Condividere le risorse come collegamento](brand-portal-link-share.md)

### Administrator {#administrator}

Un amministratore include un utente contrassegnato come amministratore di sistema o amministratore di prodotto di Brand Portal in [!UICONTROL Admin Console]. Un amministratore può aggiungere e rimuovere amministratori di sistema e utenti, definire predefiniti, inviare e-mail agli utenti e visualizzare i rapporti sull’utilizzo e l’archiviazione del portale.

Un amministratore può eseguire tutte le attività che un editor può eseguire:

[Gestire utenti, gruppi e ruoli utente](brand-portal-adding-users.md)

[Personalizzare sfondo, intestazioni di pagina ed e-mail](brand-portal-branding.md)

[Utilizzare i facet di ricerca personalizzati](brand-portal-search-facets.md)

[Utilizzare il modulo schema metadati](brand-portal-metadata-schemas.md)

[Applicare predefiniti immagine o rappresentazioni dinamiche](brand-portal-image-presets.md)

[Utilizzare i rapporti](brand-portal-reports.md)

Oltre alle attività di cui sopra, un autore in AEM Assets può eseguire le seguenti attività:

[Configurare AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md)

[Pubblicare cartelle su Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Pubblicare raccolte su Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alias alternativo per l’url di Brand Portal {#tenant-alias-for-portal-url}

A partire da Brand Portal 6.4.3, le organizzazioni possono disporre di un URL alternativo (alias) per l’URL esistente del tenant di Brand Portal. L’URL alias può essere creato con un prefisso alternativo nell’URL.\
Tieni presente che solo il prefisso dell’URL di Brand Portal può essere personalizzato e non l’intero URL. Ad esempio, un&#39;organizzazione con un dominio esistente **[!UICONTROL geomettrix.brand-portal.adobe.com]** può ottenere **[!UICONTROL geomettrixinc.brand-portal.adobe.com]** creato su richiesta.

Tuttavia, l’istanza di authoring AEM può essere [configurata](../using/configure-aem-assets-with-brand-portal.md) solo con l’URL dell’ID tenant e non con l’URL dell’alias del tenant (alternativo).

>[!NOTE]
>
>Per ottenere un alias per il nome del tenant nell’URL del portale esistente, le organizzazioni devono contattare il supporto Adobe con una nuova richiesta di creazione dell’alias del tenant. Questa richiesta viene elaborata controllando prima se l&#39;alias è disponibile e quindi creando l&#39;alias.
>
>Per sostituire il vecchio alias o eliminarlo, è necessario seguire lo stesso processo.

## Richiedere l’accesso a Brand Portal {#request-access-to-brand-portal}

Gli utenti possono richiedere l’accesso a Brand Portal dalla schermata di accesso. Queste richieste vengono inviate agli amministratori di Brand Portal che concedono l’accesso agli utenti tramite l’Adobe [!UICONTROL Admin Console]. Dopo aver concesso l’accesso, gli utenti ricevono un messaggio e-mail di notifica.

Per richiedere l&#39;accesso, procedi come segue:

1. Dalla pagina di accesso di Brand Portal, seleziona **[!UICONTROL Fai clic qui]** corrispondente a **[!UICONTROL Hai accesso?]**. Tuttavia, per accedere alla sessione guest, selezionare il **[!UICONTROL Fare clic qui]** corrispondente a **[!UICONTROL Guest Access?]**.

   ![Schermata di accesso di Brand Portal](assets/bp-login-requestaccess.png)

   Viene visualizzata la pagina [!UICONTROL Richiedi accesso] .

1. Per richiedere l’accesso a Brand Portal di un’organizzazione, è necessario disporre di un [!UICONTROL Federated ID], [!UICONTROL Enterprise ID] o [!UICONTROL Adobe ID] valido.

   Nella pagina [!UICONTROL Richiedi accesso], accedi utilizzando il tuo ID (scenario 1) o crea un [!UICONTROL Adobe ID] (scenario 2):<br />
   ![[!UICONTROL Richiesta di accesso]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. Se disponi di un&#39;Enterprise ID [!UICONTROL Adobe ID],  o [!UICONTROL Federated ID], fai clic su **[!UICONTROL Accedi]**.
Viene visualizzata la pagina [!UICONTROL Accedi] .
   1. Fornisci le tue credenziali [!UICONTROL Adobe ID] e fai clic su **[!UICONTROL Accedi]**.<br />

   ![Adobe di accesso](assets/bplogin_request_access_3.png)

   Verrai reindirizzato alla pagina [!UICONTROL Richiedi accesso].<br />
   **Scenario 2**
   1. Se non disponi di un [!UICONTROL Adobe ID], per crearne uno fai clic su **[!UICONTROL Ottieni un Adobe ID]** dalla pagina [!UICONTROL Richiedi accesso].
Viene visualizzata la pagina [!UICONTROL Accedi] .
   1. Fai clic su **[!UICONTROL Ottieni un Adobe ID]**.
Viene visualizzata la pagina [!UICONTROL Iscriviti] .
   1. Immetti nome e cognome, ID e-mail e password.
   1. Seleziona **[!UICONTROL Iscriviti]**.<br />

   ![](assets/bplogin_request_access_5.png)

   Verrai reindirizzato alla pagina [!UICONTROL Richiedi accesso] .

1. Nella pagina successiva vengono visualizzati il nome e l’ID e-mail utilizzati per richiedere l’accesso. Lascia un commento per l&#39;amministratore e fai clic su **[!UICONTROL Invia]**.<br />

   ![](assets/bplogin-request-access.png)

## Gli amministratori di prodotto concedono l&#39;accesso a {#grant-access-to-brand-portal}

Gli amministratori di prodotto di Brand Portal ricevono le richieste di accesso nell’area di notifica di Brand Portal e tramite e-mail nella casella in entrata.

![Notifica richiesta di accesso](assets/bplogin_request_access_7.png)

Per concedere l’accesso, gli amministratori di prodotto devono fare clic sulla notifica pertinente nell’area di notifica di Brand Portal, quindi fare clic su **[!UICONTROL Concedi accesso]**.
In alternativa, gli amministratori di prodotto possono seguire il collegamento fornito nell’e-mail di richiesta di accesso per visitare l’Adobe [!UICONTROL Admin Console] e aggiungere l’utente alla configurazione di prodotto pertinente.

Viene eseguito il reindirizzamento alla pagina principale [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview). Utilizza l’Adobe [!UICONTROL Admin Console] per creare utenti e assegnarli ai profili di prodotto (precedentemente noti come configurazioni di prodotto), che vengono visualizzati come gruppi in Brand Portal. Per ulteriori informazioni sull&#39;aggiunta di utenti in [!UICONTROL Admin Console], vedere [Aggiungere un utente](brand-portal-adding-users.md#add-a-user) (seguire i passaggi 4-7 della procedura per aggiungere un utente).

## Lingue di Brand Portal {#brand-portal-language}

Puoi modificare la lingua di Brand Portal dall’Adobe [!UICONTROL Impostazioni Experience Cloud].

![Notifica richiesta di accesso](assets/BPLang.png)

Per modificare la lingua:

1. Seleziona [!UICONTROL Utente] > [!UICONTROL Modifica profilo] dal menu principale.<br />

   ![Modifica profilo](assets/EditBPProfile.png)

1. Nella pagina [!UICONTROL Impostazioni Experience Cloud], seleziona una lingua dal menu a discesa [!UICONTROL Lingua].

## Notifica di manutenzione di Brand Portal {#brand-portal-maintenance-notification}

Prima che Brand Portal venga programmato per la manutenzione, una notifica viene visualizzata come banner dopo l’accesso a Brand Portal. Notifica di esempio:

![](assets/bp_maintenance_notification.png)

Puoi ignorare questa notifica e continuare a utilizzare Brand Portal. Questa notifica viene visualizzata in ogni nuova sessione.

## Informazioni sulla versione e sul sistema {#release-and-system-information}

* [Novità](whats-new.md)
* [Note sulla versione](brand-portal-release-notes.md)
* [Formati di file supportati](brand-portal-supported-formats.md)

## Risorse correlate {#related-resources}

* [Adobe Customer Care](https://helpx.adobe.com/it/marketing-cloud/contact-support.html)
* [Forum su AEM](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)