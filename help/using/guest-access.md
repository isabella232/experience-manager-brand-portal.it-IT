---
title: Accesso ospite a Brand Portal
seo-title: Accesso ospite a Brand Portal
description: Consentite agli ospiti di accedere e risparmiare l'impegno per far sì che molti utenti non debbano essere autenticati.
seo-description: Consentite agli ospiti di accedere e risparmiare l'impegno per far sì che molti utenti non debbano essere autenticati.
uuid: edb 4378 d -1710-44 a 2-97 a 6-594 d 99 f 62 fff
contentOwner: mgulati
topic-tags: introduction
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: b 9 e 9 fe 7 b -0373-42 d 1-851 b -7 c 76 b 47657 c 2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Accesso ospite a Brand Portal {#guest-access-to-brand-portal}

AEM Brand Portal consente agli ospiti di accedere al portale. Un utente ospite non necessita delle credenziali per entrare nel portale e può accedere alle risorse pubbliche (e alle raccolte) del portale. Gli utenti della sessione ospite possono aggiungere risorse alla loro lightbox (raccolta privata) e scaricare lo stesso fino alla sua sessione, ovvero 2 ore dall'inizio della sessione, a meno che l'utente ospite non decida [[! UICONTROL End Session]](#exit-guest-session).

La funzionalità di accesso degli ospiti consente alle organizzazioni di condividere [rapidamente le risorse](../using/brand-portal-sharing-folders.md#how-to-share-folders) approvate con il pubblico desiderato su larga scala, senza dover disporre di bacheci. Il Brand Portal 6.4.2 a partire è predisposto per distribuire più utenti ospiti simultanei, che è il 10% della quota utente totale per organizzazione. L'accesso degli ospiti consente di risparmiare tempo per gestire e utilizzare valutazioni su bacheca degli utenti che necessitano di funzionalità limitate su Brand Portal.\
Le organizzazioni possono abilitare (o disabilitare) l'accesso degli ospiti sull'account Brand Portal dell'organizzazione utilizzando **[!UICONTROL l'opzione Consenti accesso]** ospite dalle **[!UICONTROL impostazioni Accesso]** nel pannello Strumenti di amministrazione.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Inizia sessione ospite {#begin-guest-session}

Per entrare in Brand Portal in modo anonimo, selezionate **[!UICONTROL Clic qui]** corrispondente a **[!UICONTROL Accesso ospiti?]** nella schermata di benvenuto di Brand Portal. Gli utenti non devono cercare l'accesso e attendere che l'amministratore le autentichi per concedere l'accesso per l'utilizzo del portale marchio.

![](assets/bp-login-screen.png)

## Durata sessione ospite {#guest-session-duration}

Una sessione utente ospite rimane attiva per 2 ore. Ciò significa che lo stato della [!UICONTROL Lightbox] viene mantenuto fino a 1 ora dall'ora di inizio della sessione e, dopo 2 ore, la sessione ospite corrente viene riavviata.\
Ad esempio, un utente ospite accede a Brand Portal a 1500 ore e aggiunge le risorse a Lightbox da scaricare a 16:50 ore. Se l'utente non scarica la raccolta [!UICONTROL Lightbox] (o le relative risorse) prima di 17:00 ore, la [!UICONTROL Lightbox] diventerà vuota perché l'utente dovrà riavviare la sessione alla fine di 1 ora (1700 ore).

## Sessioni ospiti simultanei consentite {#concurrent-guest-sessions-allowed}

Il numero di sessioni ospiti simultanee è limitato al 10% della quota utente totale per organizzazione. Ciò significa che per un'organizzazione con una quota utente pari a 200, è possibile lavorare simultaneamente su 20 utenti ospiti. L'utente 21 st riceve l'accesso e può accedere come ospite solo se la sessione di uno dei 20 utenti ospiti attivi è terminata.

## Interazione dell'utente ospite con Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigazione nell'interfaccia utente ospite

Quando si immette il Brand Portal come ospite, gli utenti possono vedere tutte [le risorse e le cartelle condivise](../using/brand-portal-sharing-folders.md#sharefolders) pubblicamente o con gli utenti ospiti esclusivamente. Questa vista è solo la visualizzazione del contenuto, che visualizza le risorse in uno dei layout schede, elenco o colonne.

![](assets/disabled-folder-hierarchy1.png)

Tuttavia, gli utenti ospiti visualizzano la struttura di cartelle (a partire dalla cartella principale) e le cartelle condivise disposte all'interno delle rispettive cartelle principali all'accesso al portale brand, se gli amministratori hanno abilitato [la configurazione Abilita gerarchia](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) cartelle.

Queste cartelle principali sono cartelle virtuali e non è possibile eseguire azioni su di esse. Potete riconoscere queste cartelle virtuali con un'icona a forma di lucchetto.

Non sono disponibili attività di azione al momento del passaggio del mouse o della selezione nella [!UICONTROL vista]a schede, a differenza delle cartelle condivise. [!UICONTROL Il] pulsante Panoramica viene visualizzato quando si seleziona una cartella virtuale nella [!UICONTROL vista] a colonne e [!UICONTROL a elenco].

>[!NOTE]
>
>La miniatura predefinita delle cartelle virtuali è quella della prima cartella condivisa.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

[!UICONTROL L'opzione Impostazioni] visualizzazione consente agli utenti ospiti di regolare le dimensioni delle schede in [!UICONTROL vista a schede] o colonne da visualizzare in [!UICONTROL visualizzazione Elenco].

![](assets/nav-guest-user.png)

La [!UICONTROL struttura Contenuto] permette di spostarsi nella gerarchia delle risorse.

![](assets/guest-login-ui.png)

Brand Portal fornisce [!UICONTROL agli utenti ospiti] l'opzione Panoramica per visualizzare [!UICONTROL le Proprietà risorse] delle risorse o delle cartelle selezionate. L'opzione [!UICONTROL Panoramica] è visibile:

* Nella barra degli strumenti nella parte superiore della selezione di una risorsa o di una cartella.
* Nel menu a discesa selezionate il selettore della barra.

Selezionando l'opzione [!UICONTROL Panoramica] mentre è selezionata una risorsa o una cartella, gli utenti possono visualizzare il titolo, il percorso e l'ora della creazione delle risorse. Mentre, nella pagina dei dettagli delle risorse che seleziona [!UICONTROL Panoramica,] gli utenti possono vedere i metadati della risorsa.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL L'opzione di navigazione]** nella barra a sinistra consente di navigare dai file alle raccolte e di tornare alla sessione ospite in modo che gli utenti possano sfogliare le risorse nei file o nelle raccolte.

**[!UICONTROL L'opzione Filtro]** consente agli utenti ospiti di filtrare i file e le cartelle di risorse utilizzando i predicati di ricerca impostati dall'amministratore.

### Funzionalità degli utenti ospiti

Gli utenti ospiti possono accedere alle risorse pubbliche su Brand Portal e dispongono inoltre di alcune restrizioni come discusso ulteriormente.

Gli utenti ospiti possono:

* accedere a tutte le cartelle pubbliche e raccolte destinate a tutti gli utenti del portale brand.
* membri di Sfoglia, pagina dei dettagli e visualizzazione completa delle risorse dei membri di tutte le cartelle e raccolte pubbliche.
* cercare risorse in cartelle pubbliche e raccolte.
* aggiungere risorse alla raccolta Lightbox. Queste modifiche alla raccolta rimangono invariate durante la sessione.
* scaricare risorse direttamente o tramite la raccolta lightbox.

Gli utenti ospiti non possono:

* creare raccolte e ricerche salvate o condividerle ulteriormente.
* accesso alle impostazioni della cartella e delle raccolte.
* condividere le risorse come collegamenti.

### Scaricare le risorse nella sessione ospite

Gli utenti ospiti possono scaricare direttamente le risorse condivise o esclusivamente con gli utenti ospiti sul portale brand. Gli utenti ospiti possono anche aggiungere risorse a [!UICONTROL Lightbox] (raccolta pubblica) e scaricare la [!UICONTROL raccolta Lightbox] prima della scadenza della sessione.

Per scaricare risorse e raccolte, utilizzate l'icona di download da:

* miniature di azioni rapide, visualizzate sul passaggio del mouse sulla risorsa o sulla raccolta
* la barra degli strumenti nella parte superiore, che viene visualizzata selezionando la risorsa o la raccolta

![](assets/download-on-guest.png)

Selezionando **[!UICONTROL Abilita accelerazione download]** nella [!UICONTROL finestra di dialogo Scarica] , [potete migliorare le prestazioni di download](../using/accelerated-download.md).

## Esci dalla sessione ospite {#exit-guest-session}

Per uscire da una sessione ospite, utilizzate **[!UICONTROL Termina sessione]** dalle opzioni disponibili nell'intestazione. Tuttavia, se il browser utilizzato per la sessione ospite-è inattivo, la sessione scade automaticamente dopo due ore di inattività.

![](assets/end-guest-session.png)

## Monitoraggio delle attività degli utenti ospiti {#monitoring-guest-user-activities}

Gli amministratori possono monitorare l'interazione degli utenti ospiti con il portale brand. I report generati in Brand Portal possono fornire informazioni chiave sulle attività degli utenti ospiti. Ad esempio, **[!UICONTROL il]** rapporto Scarica può essere utilizzato per monitorare il numero di risorse scaricate dall'utente ospite. **[!UICONTROL Il rapporto Login]** utente può informare quando l'utente ospite ha eseguito l'ultimo accesso al portale e la frequenza degli accessi in una durata specificata.
