---
title: Panoramica di Experience Manager Assets Brand Portal
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager Assets Brand Portal consente di acquisire, controllare e distribuire in modo semplice e sicuro le risorse creative approvate a parti esterne e utenti aziendali interni tra i dispositivi.
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: fb2ce4d39fd9e7aa69ba541bd48a6b9cddd3b4c5
workflow-type: tm+mt
source-wordcount: '1576'
ht-degree: 6%

---

# Panoramica di Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

In qualità di addetto al marketing, talvolta è necessario collaborare con partner di canale e utenti aziendali interni per creare, gestire e distribuire rapidamente contenuti digitali rilevanti ai clienti. La distribuzione tempestiva dei contenuti rilevanti all&#39;interno dell&#39;intero percorso di clienti è fondamentale per incrementare la domanda, la conversione, il coinvolgimento e la fedeltà dei clienti.

Tuttavia, è difficile sviluppare soluzioni che supportino la condivisione efficiente e sicura di loghi dei marchi approvati, linee guida, risorse per le campagne o riprese di prodotti con team interni, partner e rivenditori estesi.

**Adobe Experience Manager (AEM) Assets Brand Portal** si concentra sulla necessità dell’addetto al marketing di collaborare in modo efficace con gli utenti Brand Portal distribuiti a livello globale, fornendo funzionalità di distribuzione delle risorse e di contributo delle risorse.

La distribuzione delle risorse consente di acquisire, controllare e distribuire in modo semplice e sicuro le risorse creative approvate a parti esterne e utenti aziendali interni tra i dispositivi. Il contributo di Asset consente invece agli utenti di Brand Portal di caricare le risorse in Brand Portal e pubblicarle in Experience Manager Assets, senza dover accedere all’ambiente di authoring. La funzione di contributo viene chiamata come **Assets Sourcing in Brand Portal**. L&#39;unione di questi elementi migliora l&#39;esperienza complessiva di Brand Portal nella distribuzione delle risorse e nel contributo degli utenti Brand Portal (agenzie/team esterni), velocizza il time-to-market delle risorse e riduce il rischio di non conformità e di accesso non autorizzato.
Vedi, [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).

L’ambiente del portale basato su browser consente di caricare, sfogliare, cercare, visualizzare in anteprima ed esportare facilmente le risorse in formati approvati.

## Configurare Experience Manager Assets con Brand Portal {#configure-brand-portal}

La configurazione di Adobe Experience Manager Assets con Brand Portal consente agli utenti di Brand Portal di pubblicare risorse, distribuirle e apportare contributi.

>[!NOTE]
>
>La configurazione di Experience Manager Assets con Brand Portal è supportata in Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.3 e versioni successive.

Experience Manager Assets as a Cloud Service viene configurato automaticamente con Brand Portal attivando Brand Portal da Cloud Manager. Il flusso di lavoro di attivazione crea le configurazioni richieste nel backend e attiva Brand Portal nella stessa organizzazione IMS dell’istanza Experience Manager Assets as a Cloud Service.

Experience Manager Assets (on-premise e managed service) viene invece configurato manualmente con Brand Portal utilizzando la console Adobe Developer, che fornisce un token Adobe Identity Management Services (IMS) per l’autorizzazione del tenant Brand Portal.

Per ulteriori informazioni, consulta [configurazione di Experience Manager Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Utenti tipo in Brand Portal {#Personas}

Brand Portal supporta i seguenti ruoli utente:

* Utente ospite
* Visualizzatore
* Editor
* Amministratore

Nella tabella seguente sono elencate le attività che gli utenti di questi ruoli possono eseguire:

|  | **Sfogliare** | **Ricerca** | **Download** | **Condividere le cartelle** | **Condividere una raccolta** | **Condividere le risorse come collegamento** | **Accesso agli strumenti di amministrazione** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Utente ospite** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visualizzatore** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Amministratore** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>Gli utenti guest possono sfogliare, accedere e cercare le risorse solo nelle cartelle e raccolte pubbliche.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Utente ospite {#guest-user}

Experience Manager Assets Brand Portal consente [accesso guest](#request-access-to-brand-portal) a Brand Portal. Un utente guest non ha bisogno di credenziali per accedere al portale e ha accesso alle cartelle e alle raccolte pubbliche. In qualità di utente guest, puoi sfogliare i dettagli delle risorse e avere una visualizzazione completa delle risorse dei membri delle cartelle e raccolte pubbliche. Puoi cercare, scaricare e aggiungere risorse pubbliche in [!UICONTROL Lightbox] raccolta.

Tuttavia, la sessione ospite non consente di creare raccolte e ricerche salvate e di condividerle ulteriormente. Gli utenti di una sessione guest non possono accedere alle impostazioni di cartelle e raccolte e non possono condividere le risorse come collegamenti. Di seguito è riportato un elenco di attività che un utente guest può eseguire:

* [Sfogliare e accedere alle risorse pubbliche](browse-assets-brand-portal.md)

* [Cercare risorse pubbliche](brand-portal-searching.md)

* [Scaricare risorse pubbliche](brand-portal-download-assets.md)

* [Aggiungere risorse a [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

Per ulteriori informazioni, consulta [accesso guest a Brand Portal](../using/guest-access.md).

### Visualizzatore {#viewer}

Brand Portal definito dall&#39;utente in [!DNL Admin Console] che ha accesso a Brand Portal con il ruolo di Visualizzatore. Un utente con questo ruolo può accedere a Brand Portal e accedere a cartelle, raccolte e risorse consentite. L’utente può anche sfogliare, visualizzare in anteprima, scaricare ed esportare le risorse (rappresentazioni originali o specifiche), configurare le impostazioni dell’account e cercare le risorse. Di seguito è riportato un elenco di attività che un visualizzatore può eseguire:

* [Sfoglia risorse](browse-assets-brand-portal.md)

* [Cercare le risorse](brand-portal-searching.md)

* [Scaricare le risorse](brand-portal-download-assets.md)

### Editor {#editor}

Un utente con il ruolo di Editor può eseguire tutte le attività che un Visualizzatore può eseguire. Inoltre, e l&#39;editor può visualizzare i file e le cartelle condivisi da un amministratore. L’utente con il ruolo di editor può anche condividere contenuti (file, cartelle, raccolte) con altri utenti.

Oltre alle attività che un visualizzatore può eseguire, un editor può eseguire le seguenti attività aggiuntive:

* [Condividere le cartelle](brand-portal-sharing-folders.md)

* [Condividere una raccolta](brand-portal-share-collection.md)

* [Condividere le risorse come collegamento](brand-portal-link-share.md)

### Amministratore {#administrator}

Un amministratore include un utente contrassegnato come amministratore di sistema o amministratore di prodotto Brand Portal in [!UICONTROL Admin Console]. Un amministratore può aggiungere e rimuovere amministratori di sistema e utenti, definire predefiniti, inviare messaggi di posta elettronica agli utenti e visualizzare i report sull&#39;utilizzo del portale e sullo storage.

>[!NOTE]
>
>In Brand Portal, utente contrassegnato con il ruolo di amministratore del supporto in [!UICONTROL Admin Console] dispone degli stessi privilegi di un amministratore di sistema.

Un amministratore può eseguire tutte le attività che possono essere eseguite da un editor. Di seguito sono riportate le attività aggiuntive che un amministratore può eseguire:

* [Gestire utenti, gruppi e ruoli utente](brand-portal-adding-users.md)

* [Personalizzare sfondo, intestazioni di pagina ed e-mail](brand-portal-branding.md)

* [Utilizzare i facet di ricerca personalizzati](brand-portal-search-facets.md)

* [Utilizzare il modulo schema metadati](brand-portal-metadata-schemas.md)

* [Applicare predefiniti immagine o rappresentazioni dinamiche](brand-portal-image-presets.md)

* [Utilizzare i rapporti](brand-portal-reports.md)

Oltre alle attività di cui sopra, un autore in AEM Assets può eseguire le seguenti attività:

* [Configurare AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md)

* [Pubblicare cartelle su Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-folder.html)

* [Pubblicare raccolte su Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/brand-portal-publish-collection.html)

## Alias alternativo per URL Brand Portal {#tenant-alias-for-portal-url}

A partire da Brand Portal 6.4.3, le organizzazioni possono disporre di un URL alternativo (alias) per l’URL esistente del proprio tenant Brand Portal. L&#39;URL dell&#39;alias può essere creato inserendo un prefisso alternativo nell&#39;URL.\
Tieni presente che solo il prefisso dell’URL di Brand Portal può essere personalizzato e non l’intero URL. Ad esempio, un’organizzazione con un dominio esistente `geomettrix.brand-portal.adobe.com` può ottenere `geomettrixinc.brand-portal.adobe.com` creato su richiesta.

Tuttavia, l’istanza di AEM Author può essere [configurato](../using/configure-aem-assets-with-brand-portal.md) solo con l’URL dell’ID tenant e non con l’URL dell’alias tenant (alternativo).

>[!NOTE]
>
>Per ottenere un alias per il nome tenant nell’URL del portale esistente, le organizzazioni devono contattare l’Assistenza clienti con una nuova richiesta di creazione alias tenant. Questa richiesta viene elaborata controllando innanzitutto se l’alias è disponibile e quindi creando l’alias.
>
>Per sostituire il vecchio alias o eliminare il vecchio alias, è necessario seguire lo stesso processo.

## Richiedi accesso a Brand Portal {#request-access-to-brand-portal}

Gli utenti possono richiedere l’accesso a Brand Portal dalla schermata di accesso. Queste richieste vengono inviate agli amministratori di Brand Portal, che concedono l’accesso agli utenti tramite l’Adobe [!UICONTROL Admin Console]. Una volta concesso l’accesso, gli utenti ricevono un’e-mail di notifica.

Per richiedere l&#39;accesso, effettuare le seguenti operazioni:

1. Dalla pagina di accesso di Brand Portal, seleziona **[!UICONTROL Fai clic qui]** corrispondente a **[!UICONTROL Hai bisogno di accedere?]**. Tuttavia, per accedere alla sessione guest, selezionare **[!UICONTROL Fai clic qui]** corrispondente a **[!UICONTROL Accesso come ospite?]**.

   ![Schermata di accesso a Brand Portal](assets/bp-login-requestaccess.png)

   Il [!UICONTROL Richiedi accesso] viene visualizzata la pagina.

1. Per richiedere l’accesso al Brand Portal di un’organizzazione, devi disporre di un [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], o [!UICONTROL Federated ID].

   In [!UICONTROL Richiedi accesso] , accedere con il proprio ID (scenario 1) o creare un [!UICONTROL Adobe ID] (scenario 2)

   ![[!UICONTROL Richiedi accesso]](assets/bplogin_request_access_2.png)

   **Scenario 1**

   1. Se si dispone di [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID], o [!UICONTROL Federated ID], fai clic su **[!UICONTROL Accedi]**.
Il [!UICONTROL Accedi] viene visualizzata la pagina.

   1. Fornisci [!UICONTROL Adobe ID] e fai clic su **[!UICONTROL Accedi]**.

      ![Adobe accesso](assets/bplogin_request_access_3.png)
   Sei reindirizzato al [!UICONTROL Richiedi accesso] pagina.

   **Scenario 2**

   1. Se non si dispone di un [!UICONTROL Adobe ID], per crearne uno, fai clic su **[!UICONTROL Ottieni un Adobe ID]** dal [!UICONTROL Richiedi accesso] pagina.
Il [!UICONTROL Accedi] viene visualizzata la pagina.
   1. Clic **[!UICONTROL Ottieni un Adobe ID]**.
Il [!UICONTROL Registrati] viene visualizzata la pagina.
   1. Immetti nome e cognome, ID e-mail e password.
   1. Seleziona **[!UICONTROL Registrati]**.

      ![](assets/bplogin_request_access_5.png)
   Sei reindirizzato al [!UICONTROL Richiedi accesso] pagina.

1. Nella pagina successiva vengono visualizzati il nome e l’ID e-mail utilizzati per richiedere l’accesso. Lascia un commento per l’amministratore, quindi fai clic su **[!UICONTROL Invia]**.

   ![](assets/bplogin-request-access.png)

## Gli amministratori di prodotto concedono l’accesso {#grant-access-to-brand-portal}

Gli amministratori dei prodotti Brand Portal ricevono le richieste di accesso nella propria area di notifica Brand Portal e tramite e-mail nella propria casella in entrata.

![Notifica richiesta di accesso](assets/bplogin_request_access_7.png)

Per concedere l’accesso, gli amministratori di prodotto devono fare clic sulla notifica pertinente nell’area di notifica di Brand Portal e quindi fare clic su **[!UICONTROL Concedi l&#39;accesso]**.
In alternativa, per visitare l’Adobe, gli amministratori di prodotto possono seguire il collegamento fornito nell’e-mail di richiesta di accesso [!UICONTROL Admin Console] e aggiungi l’utente alla relativa configurazione di prodotto.

Sei reindirizzato al [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) home page. Utilizza Adobe [!UICONTROL Admin Console] per creare utenti e assegnarli a profili di prodotto (precedentemente noti come configurazioni di prodotto), che vengono visualizzati come gruppi in Brand Portal. Per ulteriori informazioni sull&#39;aggiunta di utenti in [!UICONTROL Admin Console], vedi [Aggiungi un utente](brand-portal-adding-users.md#add-a-user) (seguire i passaggi 4-7 nella procedura per aggiungere un utente).

## Lingue Brand Portal {#brand-portal-language}

È possibile cambiare la lingua di Brand Portal da Adobe [!UICONTROL Impostazioni Experience Cloud].

![Notifica richiesta di accesso](assets/BPLang.png)

Per modificare la lingua:

1. Seleziona [!UICONTROL Utente] > [!UICONTROL Modifica profilo] dal menu principale.

   ![Modifica profilo](assets/EditBPProfile.png)

1. On [!UICONTROL Impostazioni Experience Cloud] , selezionare una lingua dalla [!UICONTROL Lingua] menu a discesa.

## Notifica di manutenzione Brand Portal {#brand-portal-maintenance-notification}

Prima che Brand Portal sia pianificato per l’interruzione della manutenzione, viene visualizzata una notifica come banner dopo l’accesso a Brand Portal. Esempio di notifica:

![](assets/bp_maintenance_notification.png)

Puoi ignorare questa notifica e continuare a utilizzare Brand Portal. Questa notifica viene visualizzata in ogni nuova sessione.

## Informazioni sulla versione e sul sistema {#release-and-system-information}

* [Novità](whats-new.md)
* [Note sulla versione](brand-portal-release-notes.md)
* [Formati di file supportati](brand-portal-supported-formats.md)

## Risorse correlate {#related-resources}

<!--
* [Adobe Customer Support]()
-->

* [Forum AEM](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
