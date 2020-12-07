---
title: Panoramica  Portale del marchio AEM Assets
seo-title: Panoramica  Portale del marchio AEM Assets
description: ' Portale del marchio AEM Assets consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi.'
seo-description: ' Portale del marchio AEM Assets consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi.'
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
translation-type: tm+mt
source-git-commit: 7adc6b311a7f669b05dd8cc82cede62194cb8ec6
workflow-type: tm+mt
source-wordcount: '1524'
ht-degree: 9%

---


# Panoramica  Portale marchio AEM Assets {#overview-of-aem-assets-brand-portal}

In qualità di esperto di marketing, a volte devi collaborare con partner di canale e utenti aziendali interni per creare, gestire e fornire rapidamente contenuti digitali rilevanti ai clienti. La distribuzione tempestiva di contenuti rilevanti nell&#39;intero percorso del cliente è fondamentale per stimolare una maggiore domanda, conversione, coinvolgimento e fidelizzazione dei clienti.

Tuttavia, è una sfida sviluppare soluzioni che supportano una condivisione efficiente e sicura dei logo del marchio, delle linee guida, delle risorse delle campagne o delle riprese di prodotti approvati con team, partner e rivenditori interni estesi.

**Adobe Experience Manager (AEM) Assets Brand** Portal si concentra sull’esigenza dell’esperto di marketing di collaborare efficacemente con gli utenti del Brand Portal distribuiti a livello globale fornendo funzionalità di distribuzione delle risorse e contributi alle risorse.

La distribuzione delle risorse consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni attraverso dispositivi diversi. Il contributo risorse consente invece agli utenti di Brand Portal di caricare le risorse su Brand Portal e pubblicarle su  AEM Assets, senza dover accedere all’ambiente di authoring. La funzione di contributo è denominata **Risorse di origine in Brand Portal**. Inoltre, migliora l&#39;esperienza complessiva del Brand Portal nella distribuzione delle risorse e nel contributo degli utenti del Brand Portal (agenzie/team esterni), accelera il time-to-market delle risorse e riduce il rischio di non conformità e di accesso non autorizzato.
Vedere [Origine risorsa in Portale marchio](brand-portal-asset-sourcing.md).

L’ambiente portale basato su browser consente di caricare, sfogliare, cercare, visualizzare in anteprima ed esportare facilmente le risorse in formati approvati.

## Configurare AEM Assets con Brand Portal {#configure-brand-portal}

Adobe Experience Manager (AEM) Assets è configurato con Portale marchio tramite  Developer Console di Adobe, che fornisce un token IMS per l’autorizzazione del tenant del Brand Portal.

>[!NOTE]
>
>La configurazione  AEM Assets con Portale del marchio tramite  Console per sviluppatori di Adobi è supportata  AEM Assets come Cloud Service,  AEM Assets 6.3 e versioni successive.

### Prerequisiti per configurare  AEM Assets con Brand Portal {#prerequisites}

Per configurare AEM Assets con Brand Portal, è necessario quanto segue:

* Un’istanza di AEM Assets in esecuzione.
* URL del tenant di Brand Portal.
* Un utente con privilegi di amministratore di sistema nell’organizzazione IMS del tenant di Brand Portal.

Per ulteriori informazioni, vedere [configurazione  AEM Assets con Brand Poral](../using/configure-aem-assets-with-brand-portal.md).

## Personalità utente in Brand Portal {#Personas}

Brand Portal supporta i seguenti ruoli utente:

* Utente ospite
* Visualizzatore
* Editor
* Administrator

Nella tabella seguente sono elencate le attività che gli utenti di questi ruoli possono eseguire:

|  | **Sfoglia** | **Ricerca** | **Scarica** | **Condividere le cartelle** | **Condividere una raccolta** | **Condividere le risorse come collegamento** | **Accesso ad Strumenti di amministrazione** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Utente ospite** | ▲* | ▲* | ▲* | x | x | x | x |
| **Visualizzatore** | AND | AND | AND | x | x | x | x |
| **Editor** | AND | AND | AND | AND | AND | AND | x |
| **Administrator** | AND | AND | AND | AND | AND | AND | AND |

* Gli utenti ospiti possono sfogliare, accedere e cercare risorse solo nelle cartelle pubbliche e nelle raccolte.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Utente ospite {#guest-user}

Ogni utente che dispone di un accesso limitato alle risorse su Brand Portal senza essere autenticato è un utente ospite. La sessione guest consente agli utenti di accedere alle cartelle e alle raccolte pubbliche. In qualità di utente ospite, potete sfogliare i dettagli delle risorse e avere una visualizzazione completa delle risorse dei membri delle cartelle pubbliche e delle raccolte. Potete cercare, scaricare e aggiungere risorse pubbliche alla raccolta [!UICONTROL Lightbox].

Tuttavia, la sessione degli ospiti non consente di creare raccolte e ricerche salvate e di condividerle ulteriormente. Gli utenti di una sessione ospite non possono accedere alle impostazioni delle cartelle e delle raccolte e non possono condividere le risorse come collegamento. Di seguito è riportato un elenco delle attività che un utente ospite può eseguire:

[Sfogliare e accedere alle risorse pubbliche](browse-assets-brand-portal.md)

[Ricerca di risorse pubbliche](brand-portal-searching.md)

[Scaricare risorse pubbliche](brand-portal-download-assets.md)

[Aggiungere risorse a  [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

### Visualizzatore {#viewer}

Un utente standard in Brand Portal è in genere un utente con il ruolo di Visualizzatore. Un utente con questo ruolo può accedere a cartelle, raccolte e risorse consentite. L’utente può anche sfogliare, visualizzare in anteprima, scaricare ed esportare risorse (rappresentazioni originali o specifiche), configurare le impostazioni dell’account e cercare risorse. Elenco delle attività che un visualizzatore può eseguire:

[Sfogliare le risorse](browse-assets-brand-portal.md)

[Ricerca di risorse](brand-portal-searching.md)

[Scaricare le risorse](brand-portal-download-assets.md)

### Editor {#editor}

Un utente con il ruolo di Editor può eseguire tutte le attività che un visualizzatore può eseguire. Inoltre, in Editor è possibile visualizzare i file e le cartelle condivisi da un amministratore. L’utente con il ruolo di Editor può anche condividere contenuti (file, cartelle, raccolte) con altri utenti.

Oltre alle attività che un visualizzatore può eseguire, un editor può eseguire le seguenti attività aggiuntive:

[Condividere le cartelle](brand-portal-sharing-folders.md)

[Condividere una raccolta](brand-portal-share-collection.md)

[Condividere le risorse come collegamento](brand-portal-link-share.md)

### Administrator {#administrator}

Un amministratore include un utente contrassegnato come amministratore di sistema o amministratore di prodotto del Portale marchio in [!UICONTROL  Admin Console]. Un amministratore può aggiungere e rimuovere amministratori di sistema e utenti, definire predefiniti, inviare e-mail agli utenti e visualizzare rapporti sull’uso e l’archiviazione del portale.

Un amministratore può eseguire tutte le attività che un utente con privilegi di editor può eseguire le seguenti attività aggiuntive:

[Gestire utenti, gruppi e ruoli utente](brand-portal-adding-users.md)

[Personalizzare sfondi, intestazioni di pagina ed e-mail](brand-portal-branding.md)

[Utilizzare i facet di ricerca personalizzati](brand-portal-search-facets.md)

[Utilizzare il modulo schema metadati](brand-portal-metadata-schemas.md)

[Applicare predefiniti immagine o rappresentazioni dinamiche](brand-portal-image-presets.md)

[Utilizzare i rapporti](brand-portal-reports.md)

Oltre alle attività descritte sopra, un autore in  AEM Assets può eseguire le seguenti operazioni:

[Configurare AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md)

[Pubblicare cartelle su Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-folder.html)

[Pubblicare raccolte su Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-publish-collection.html)

## Alias alternativo per URL Brand Portal {#tenant-alias-for-portal-url}

A partire da Brand Portal 6.4.3, le organizzazioni possono disporre di un URL alternativo (alias) per l’URL esistente del tenant del Brand Portal. L’URL alias può essere creato con un prefisso alternativo nell’URL.\
Tenete presente che è possibile personalizzare solo il prefisso dell’URL del Portale marchio e non l’intero URL. Ad esempio, un&#39;organizzazione con un dominio esistente **[!UICONTROL geomettrix.brand-Portal.adobe.com]** può ottenere **[!UICONTROL geomettrixinc.brand-Portal.adobe.com]** creato su richiesta.

Tuttavia, l&#39;istanza di AEM Author può essere [configurata](../using/configure-aem-assets-with-brand-portal.md) solo con l&#39;URL tenant e non con l&#39;URL tenant (alternativo).

>[!NOTE]
>
>Per ottenere un alias per il nome del tenant nell&#39;URL del portale esistente, le organizzazioni devono contattare  supporto del Adobe con una nuova richiesta di creazione alias del tenant. Questa richiesta viene elaborata verificando prima se l&#39;alias è disponibile e quindi creando l&#39;alias.
>
>Per sostituire il vecchio alias o eliminarlo, è necessario seguire lo stesso processo.

## Richiesta di accesso a Brand Portal {#request-access-to-brand-portal}

Gli utenti possono richiedere l’accesso a Brand Portal dalla schermata di accesso. Queste richieste vengono inviate agli amministratori del Brand Portal, che concedono l&#39;accesso agli utenti tramite il Adobe di  [!UICONTROL  Admin Console]. Una volta concesso l’accesso, gli utenti ricevono un messaggio e-mail di notifica.

Per richiedere l’accesso, effettuate le seguenti operazioni:

1. Dalla pagina di accesso al Brand Portal, selezionate **[!UICONTROL Fate clic qui]** corrispondente a **[!UICONTROL Necessità di accesso?]**. Tuttavia, per accedere alla sessione ospite, selezionare il **[!UICONTROL Fare clic qui]** corrispondente a **[!UICONTROL Guest Access?]**.

   ![Schermata di accesso a Brand Portal](assets/bp-login-requestaccess.png)

   Viene visualizzata la pagina [!UICONTROL Richiedi accesso].

1. Per richiedere l&#39;accesso al Portale dei marchi di un&#39;organizzazione, è necessario disporre di un [!UICONTROL  Adobe ID], [!UICONTROL  Enterprise ID] o [!UICONTROL Federated ID] valido.

   Nella pagina [!UICONTROL Richiedi accesso], effettua l&#39;accesso con il tuo ID (scenario 1) o crea un [!UICONTROL  Adobe ID] (scenario 2):<br />
   ![[!UICONTROL Richiedi accesso]](assets/bplogin_request_access_2.png)

   **Scenario 1**
   1. Se si dispone di un&#39;Enterprise ID [!UICONTROL  Adobe ID],  o [!UICONTROL Federated ID], fare clic su **[!UICONTROL Accedi]**.
Viene visualizzata la pagina [!UICONTROL Accedi].
   1. Fornire le credenziali [!UICONTROL  Adobe ID] e fare clic su **[!UICONTROL Accedi]**.<br />

   ![Accesso  Adobe](assets/bplogin_request_access_3.png)

   Viene reindirizzato alla pagina [!UICONTROL Richiedi accesso].<br />
   **Scenario 2**
   1. Se non si dispone di un [!UICONTROL  Adobe ID], per crearne uno fare clic su **[!UICONTROL Ottenere un Adobe ID]** dalla pagina [!UICONTROL Richiedi accesso].
Viene visualizzata la pagina [!UICONTROL Accedi].
   1. Fare clic su **[!UICONTROL Ottieni un Adobe ID]**.
Viene visualizzata la pagina [!UICONTROL Registrati].
   1. Immettete il nome e il cognome, l’ID e-mail e la password.
   1. Selezionare **[!UICONTROL Registrati]**.<br />

   ![](assets/bplogin_request_access_5.png)

   Viene reindirizzato alla pagina [!UICONTROL Richiedi accesso].

1. Nella pagina successiva vengono visualizzati il nome e l’ID e-mail utilizzati per richiedere l’accesso. Lasciate un commento per l&#39;amministratore e fate clic su **[!UICONTROL Invia]**.<br />

   ![](assets/bplogin-request-access.png)

## Gli amministratori di prodotto concedono l&#39;accesso a {#grant-access-to-brand-portal}

Gli amministratori di prodotti Brand Portal ricevono richieste di accesso nell’area di notifica del Portale marchio e tramite e-mail nella propria inbox.

![Accesso alla notifica richiesta](assets/bplogin_request_access_7.png)

Per concedere l&#39;accesso, gli amministratori di prodotto devono fare clic sulla notifica pertinente nell&#39;area di notifica del Portale marchio, quindi fare clic su **[!UICONTROL Concedi accesso]**.
In alternativa, gli amministratori di prodotto possono seguire il collegamento fornito nel messaggio e-mail di richiesta di accesso per visitare  Adobe [!UICONTROL  Admin Console] e aggiungere l&#39;utente alla configurazione di prodotto pertinente.

Viene reindirizzato alla pagina principale [ Adobe [!UICONTROL  Admin Console]](https://adminconsole.adobe.com/enterprise/overview). Utilizzate  Adobe [!UICONTROL  Admin Console] per creare utenti e assegnarli ai profili di prodotto (precedentemente denominati configurazioni di prodotto), che vengono visualizzati come gruppi in Brand Portal. Per ulteriori informazioni sull&#39;aggiunta di utenti in [!UICONTROL  Admin Console], vedere [Aggiungi un utente](brand-portal-adding-users.md#add-a-user) (seguire i passaggi da 4 a 7 della procedura per aggiungere un utente).

## Lingue del portale del marchio {#brand-portal-language}

È possibile modificare la lingua del Portale marchio  Adobe [!UICONTROL  Impostazioni Experience Cloud].

![Accesso alla notifica richiesta](assets/BPLang.png)

Per modificare la lingua:

1. Selezionare [!UICONTROL Utente] > [!UICONTROL Modifica profilo] dal menu principale.<br />

   ![Modifica profilo](assets/EditBPProfile.png)

1. Nella pagina [!UICONTROL  Impostazioni Experience Cloud], selezionare una lingua dal menu a discesa [!UICONTROL Lingua].

## Notifica di manutenzione del Brand Portal {#brand-portal-maintenance-notification}

Prima che Brand Portal venga pianificato per la manutenzione, una notifica viene visualizzata come banner dopo l’accesso al Brand Portal. Una notifica di esempio:

![](assets/bp_maintenance_notification.png)

Potete ignorare questa notifica e continuare a utilizzare Brand Portal. Questa notifica viene visualizzata in ogni nuova sessione.

## Informazioni sulla versione e sul sistema {#release-and-system-information}

* [Novità](whats-new.md)
* [Note sulla versione](brand-portal-release-notes.md)
* [Formati di file supportati](brand-portal-supported-formats.md)

## Risorse correlate {#related-resources}

* [Assistenza clienti  Adobe](https://helpx.adobe.com/it/marketing-cloud/contact-support.html)
* [Forum su AEM](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)