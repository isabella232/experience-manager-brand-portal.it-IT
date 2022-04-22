---
title: Panoramica di Experience Manager Assets Brand Portal
seo-title: Overview of Experience Manager Assets Brand Portal
description: Experience Manager Assets Brand Portal consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi.
seo-description: Experience Manager Assets Brand Portal can help you easily acquire, control, and securely distribute approved creative assets to external parties and internal business users across devices.
uuid: b1e54d03-eb2e-488e-af4d-bae817dd135a
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: introduction
discoiquuid: 6aefa298-4728-4b8e-a85b-e419ee37f2f4
exl-id: 0f2c45e4-416e-451a-905b-06c5e42a9272
source-git-commit: af697978ce140a618fda59cec050dfaedb0c296b
workflow-type: tm+mt
source-wordcount: '1585'
ht-degree: 6%

---

# Panoramica di Experience Manager Assets Brand Portal {#overview-of-aem-assets-brand-portal}

In qualità di addetto al marketing, a volte è necessario collaborare con i partner di canale e gli utenti aziendali interni per creare, gestire e fornire rapidamente contenuti digitali pertinenti ai clienti. La distribuzione tempestiva di contenuti rilevanti in tutto il percorso di clienti è fondamentale per incrementare la domanda, la conversione, il coinvolgimento e la fidelizzazione dei clienti.

Tuttavia, è una sfida sviluppare soluzioni che supportino la condivisione efficiente e sicura di logo di marchio approvati, linee guida, risorse di campagne o scatti di prodotti con team interni, partner e rivenditori estesi.

**Adobe Experience Manager (AEM) Assets Brand Portal** si concentra sulla necessità per l’addetto al marketing di collaborare efficacemente con gli utenti Brand Portal distribuiti a livello globale fornendo funzionalità di distribuzione delle risorse e contributo delle risorse.

La distribuzione delle risorse consente di acquisire, controllare e distribuire in modo sicuro le risorse creative approvate a soggetti esterni e utenti aziendali interni su diversi dispositivi. Il contributo risorse consente invece agli utenti di Brand Portal di caricare le risorse in Brand Portal e pubblicarle in Experience Manager Assets, senza necessità di accedere all’ambiente di authoring. La funzione di contributo è denominata come **Origine risorse in Brand Portal**. Insieme, migliora l’esperienza complessiva di Brand Portal nella distribuzione delle risorse e il contributo degli utenti Brand Portal (agenzie/team esterni), accelera i tempi di commercializzazione delle risorse e riduce il rischio di non conformità e di accesso non autorizzato.
Vedi [Origine risorse in Brand Portal](brand-portal-asset-sourcing.md).

L’ambiente portale basato su browser consente di caricare, sfogliare, cercare, visualizzare in anteprima ed esportare facilmente le risorse nei formati approvati.

## Configurare Experience Manager Assets con Brand Portal {#configure-brand-portal}

La configurazione di Adobe Experience Manager Assets con Brand Portal abilita la pubblicazione delle risorse, la distribuzione delle risorse e le funzioni di contributo delle risorse per gli utenti Brand Portal.

>[!NOTE]
>
>La configurazione di Experience Manager Assets con Brand Portal è supportata su Experience Manager Assets as a Cloud Service, Experience Manager Assets 6.3 e versioni successive.

Experience Manager Assets as a Cloud Service viene configurato automaticamente con Brand Portal attivando Brand Portal da Cloud Manager. Il flusso di lavoro di attivazione crea le configurazioni richieste nel backend e attiva Brand Portal sulla stessa organizzazione IMS dell’istanza as a Cloud Service di Experience Manager Assets.

Experience Manager Assets (on-premise e Managed Service) è configurato manualmente con Brand Portal tramite Adobe Developer Console, che fornisce un token Adobe Identity Management Services (IMS) per l’autorizzazione del tenant Brand Portal.

Per ulteriori informazioni, consulta [configurazione di Experience Manager Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

## Utenti in Brand Portal {#Personas}

Brand Portal supporta i seguenti ruoli utente:

* Utente ospite
* Visualizzatore
* Editor
* Administrator

Nella tabella seguente sono elencate le attività che gli utenti di questi ruoli possono eseguire:

|  | **Sfogliare** | **Ricerca** | **Download** | **Condividere le cartelle** | **Condividere una raccolta** | **Condividere le risorse come collegamento** | **Accesso a Strumenti di amministrazione** |
|--- |--- |--- |--- |--- |--- |--- |--- |
| **Utente ospite** | ✓* | ✓* | ✓* | x | x | x | x |
| **Visualizzatore** | ✓ | ✓ | ✓ | x | x | x | x |
| **Editor** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | x |
| **Administrator** | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

>[!NOTE]
>
>Gli utenti ospiti possono sfogliare, accedere e cercare le risorse solo in cartelle pubbliche e raccolte.

<!--
&#42; Viewer users can access and download the public assets shared with them, and can add these assets to create their own collections.

>[!NOTE]
>
>There is a known issue that the share link for collections is currently visible to the viewer users. The viewer users does not have the privilege to add users to create a share link. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.
-->

### Utente ospite (utente leggero) {#guest-user}

Experience Manager Assets Brand Portal consente [accesso degli ospiti](#request-access-to-brand-portal) a Brand Portal. Un utente ospite non ha bisogno di credenziali per accedere al portale e ha accesso alle cartelle e alle raccolte pubbliche. In qualità di utente ospite, puoi sfogliare i dettagli delle risorse e avere una visualizzazione completa delle risorse dei membri delle cartelle pubbliche e delle raccolte. Puoi cercare, scaricare e aggiungere risorse pubbliche a [!UICONTROL Lightbox] raccolta.

Tuttavia, la sessione guest ti limita a creare raccolte e ricerche salvate e a condividerle ulteriormente. Gli utenti di una sessione guest non possono accedere alle impostazioni di cartelle e raccolte e non possono condividere le risorse come collegamento. Elenco delle attività eseguibili da un utente guest:

* [Navigare e accedere alle risorse pubbliche](browse-assets-brand-portal.md)

* [Cercare risorse pubbliche](brand-portal-searching.md)

* [Scaricare risorse pubbliche](brand-portal-download-assets.md)

* [Aggiungi risorse a [!UICONTROL Lightbox]](brand-portal-light-box.md#add-assets-to-lightbox)

Per ulteriori informazioni, consulta [accesso guest a Brand Portal](../using/guest-access.md).

### Visualizzatore (utente standard) {#viewer}

Un utente standard è un utente Brand Portal definito in [!DNL Admin Console] che ha accesso a Brand Portal con il ruolo di Visualizzatore. Un utente con questo ruolo può accedere a Brand Portal e alle cartelle, raccolte e risorse consentite. L’utente può anche sfogliare, visualizzare in anteprima, scaricare ed esportare le risorse (rappresentazioni originali o specifiche), configurare le impostazioni dell’account e cercare le risorse. Elenco delle attività eseguibili da un visualizzatore:

* [Sfogliare le risorse](browse-assets-brand-portal.md)

* [Cercare risorse](brand-portal-searching.md)

* [Scaricare le risorse](brand-portal-download-assets.md)

### Editor {#editor}

Un utente con il ruolo di Editor può eseguire tutte le attività che un Visualizzatore può eseguire. Inoltre, e Editor possono visualizzare i file e le cartelle condivisi da un amministratore. L’utente con il ruolo di Editor può anche condividere contenuti (file, cartelle, raccolte) con altri.

Oltre alle attività eseguibili da un visualizzatore, un editor può eseguire le seguenti attività aggiuntive:

* [Condividere le cartelle](brand-portal-sharing-folders.md)

* [Condividere una raccolta](brand-portal-share-collection.md)

* [Condividere le risorse come collegamento](brand-portal-link-share.md)

### Amministratore {#administrator}

Un amministratore include un utente contrassegnato come amministratore di sistema o amministratore di prodotto Brand Portal in [!UICONTROL Admin Console]. Un amministratore può aggiungere e rimuovere amministratori di sistema e utenti, definire predefiniti, inviare e-mail agli utenti e visualizzare i rapporti sull’utilizzo e l’archiviazione del portale.

>[!NOTE]
>
>In Brand Portal, un utente contrassegnato con il ruolo di amministratore del supporto in [!UICONTROL Admin Console] dispone degli stessi privilegi di un amministratore di sistema.

Un amministratore può eseguire tutte le attività che un editor può eseguire. Di seguito sono riportate le attività aggiuntive che un amministratore può eseguire:

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

## Alias alternativo per l&#39;URL di Brand Portal {#tenant-alias-for-portal-url}

A partire da Brand Portal 6.4.3, le organizzazioni possono disporre di un URL alternativo (alias) per l’URL esistente del proprio tenant Brand Portal. L’URL alias può essere creato con un prefisso alternativo nell’URL.\
Tieni presente che solo il prefisso dell’URL Brand Portal può essere personalizzato e non l’intero URL. Ad esempio, un&#39;organizzazione con un dominio esistente `geomettrix.brand-portal.adobe.com` può ottenere `geomettrixinc.brand-portal.adobe.com` creato su richiesta.

Tuttavia, l’istanza di AEM Author può essere [configurato](../using/configure-aem-assets-with-brand-portal.md) solo con l’URL dell’ID tenant e non con l’URL dell’alias del tenant (alternativo).

>[!NOTE]
>
>Per ottenere un alias per il nome del tenant nell’URL del portale esistente, le organizzazioni devono contattare il supporto clienti con una nuova richiesta di creazione di alias del tenant. Questa richiesta viene elaborata controllando prima se l&#39;alias è disponibile e quindi creando l&#39;alias.
>
>Per sostituire il vecchio alias o eliminarlo, è necessario seguire lo stesso processo.

## Richiedere l’accesso a Brand Portal {#request-access-to-brand-portal}

Gli utenti possono richiedere l’accesso a Brand Portal dalla schermata di accesso. Queste richieste vengono inviate agli amministratori di Brand Portal, che concedono l’accesso agli utenti tramite l’Adobe [!UICONTROL Admin Console]. Dopo aver concesso l’accesso, gli utenti ricevono un messaggio e-mail di notifica.

Per richiedere l&#39;accesso, procedi come segue:

1. Dalla pagina di accesso di Brand Portal, seleziona **[!UICONTROL Fai clic qui]** corrispondente a **[!UICONTROL Hai bisogno di accesso?]**. Tuttavia, per accedere alla sessione guest, seleziona la **[!UICONTROL Fai clic qui]** corrispondente a **[!UICONTROL Accesso agli ospiti?]**.

   ![Schermata di accesso di Brand Portal](assets/bp-login-requestaccess.png)

   La [!UICONTROL Richiesta di accesso] viene visualizzata la pagina .

1. Per richiedere l’accesso a Brand Portal di un’organizzazione, è necessario disporre di una [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]oppure [!UICONTROL Federated ID].

   In [!UICONTROL Richiesta di accesso] pagina, accedi con il tuo ID (scenario 1) o crea un [!UICONTROL Adobe ID] (scenario 2):

   ![[!UICONTROL Richiesta di accesso]](assets/bplogin_request_access_2.png)

   **Scenario 1**

   1. Se hai un [!UICONTROL Adobe ID], [!UICONTROL Enterprise ID]oppure [!UICONTROL Federated ID], fai clic su **[!UICONTROL Accesso]**.
La [!UICONTROL Accedere] viene visualizzata la pagina .

   1. Fornisci le [!UICONTROL Adobe ID] credenziali e fai clic su **[!UICONTROL Accedere]**.

      ![Adobe di accesso](assets/bplogin_request_access_3.png)
   Viene reindirizzato a [!UICONTROL Richiesta di accesso] pagina.

   **Scenario 2**

   1. Se non hai un [!UICONTROL Adobe ID], per crearne uno, fai clic su **[!UICONTROL Ottieni un Adobe ID]** dal [!UICONTROL Richiesta di accesso] pagina.
La [!UICONTROL Accedere] viene visualizzata la pagina .
   1. Fai clic su **[!UICONTROL Ottieni un Adobe ID]**.
La [!UICONTROL Iscriviti] viene visualizzata la pagina .
   1. Immetti nome e cognome, ID e-mail e password.
   1. Seleziona **[!UICONTROL Iscriviti]**.

      ![](assets/bplogin_request_access_5.png)
   Viene reindirizzato a [!UICONTROL Richiesta di accesso] pagina.

1. Nella pagina successiva vengono visualizzati il nome e l’ID e-mail utilizzati per richiedere l’accesso. Lascia un commento per l&#39;amministratore e fai clic su **[!UICONTROL Invia]**.

   ![](assets/bplogin-request-access.png)

## Gli amministratori di prodotto concedono l&#39;accesso {#grant-access-to-brand-portal}

Gli amministratori di prodotto Brand Portal ricevono le richieste di accesso nella propria area di notifica Brand Portal e tramite e-mail nella propria casella in entrata.

![Notifica richiesta di accesso](assets/bplogin_request_access_7.png)

Per concedere l’accesso, gli amministratori di prodotto devono fare clic sulla notifica pertinente nell’area di notifica Brand Portal, quindi fare clic su **[!UICONTROL Accesso concesso]**.
In alternativa, gli amministratori di prodotto possono seguire il collegamento fornito nell’e-mail di richiesta di accesso per visitare l’Adobe [!UICONTROL Admin Console] e aggiungi l&#39;utente alla configurazione di prodotto pertinente.

Viene reindirizzato a [Adobe [!UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) home page. Usa Adobe [!UICONTROL Admin Console] per creare utenti e assegnarli ai profili di prodotto (precedentemente noti come configurazioni di prodotto), che vengono visualizzati come gruppi in Brand Portal. Per ulteriori informazioni sull’aggiunta di utenti in [!UICONTROL Admin Console], vedi [Aggiungi un utente](brand-portal-adding-users.md#add-a-user) (segui i passaggi 4-7 della procedura per aggiungere un utente).

## Lingue Brand Portal {#brand-portal-language}

È possibile modificare la lingua di Brand Portal dall’Adobe [!UICONTROL Impostazioni Experience Cloud].

![Notifica richiesta di accesso](assets/BPLang.png)

Per modificare la lingua:

1. Seleziona [!UICONTROL Utente] > [!UICONTROL Modifica profilo] dal menu principale.

   ![Modifica profilo](assets/EditBPProfile.png)

1. On [!UICONTROL Impostazioni Experience Cloud] seleziona una lingua dalla pagina [!UICONTROL Lingua] menu a discesa.

## Notifica di manutenzione Brand Portal {#brand-portal-maintenance-notification}

Prima che Brand Portal venga pianificato per la manutenzione, una notifica viene visualizzata come banner dopo l’accesso a Brand Portal. Notifica di esempio:

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

* [Forum su AEM](https://experienceleaguecommunities.adobe.com/t5/adobe-experience-manager/ct-p/adobe-experience-manager-community)
