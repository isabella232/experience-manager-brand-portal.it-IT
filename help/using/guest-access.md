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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Accesso ospite a Brand Portal {#guest-access-to-brand-portal}

[!DNL AEM Brand portal] consente agli ospiti di accedere al portale. Un utente ospite non necessita delle credenziali per entrare nel portale e può accedere alle risorse pubbliche (e alle raccolte) del portale. Gli utenti della sessione ospite possono aggiungere risorse alla loro lightbox (raccolta privata) e scaricare lo stesso fino alla sua sessione, ovvero 2 ore dall'inizio della sessione, a meno che l'utente ospite non decida di [terminare la sessione.](#exit-guest-session)

La funzionalità di accesso degli ospiti consente alle organizzazioni di condividere [rapidamente le risorse](../using/brand-portal-sharing-folders.md#how-to-share-folders) approvate con il pubblico desiderato su larga scala, senza dover disporre di bacheci. [!DNL Brand Portal] La versione 6.4.2 è fornita per distribuire più utenti ospiti simultanei, che è il 10% della quota utente totale per organizzazione. L'accesso agli ospiti consente di risparmiare tempo per gestire e gestire i punteggi degli utenti che necessitano di utilizzare funzionalità limitate.[!DNL Brand Portal]\
Le organizzazioni possono abilitare (o disabilitare) l'accesso degli ospiti all [!DNL Brand Portal] 'account dell'organizzazione utilizzando **l'opzione Consenti accesso** ospite dalle **impostazioni Accesso** nel pannello Strumenti di amministrazione.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Inizia sessione ospite {#begin-guest-session}

Per entrare in Brand Portal in modo anonimo, selezionate **[!UICONTROL Clic qui]** corrispondente a **[!UICONTROL Accesso ospiti?]** nella [!DNL Brand Portal] schermata di benvenuto. Gli utenti non devono cercare l'accesso e attendere che l'amministratore le autentichi per concedere [!DNL Brand Portal]l'accesso.

![](assets/bp-login-screen.png)

## Durata sessione ospite {#guest-session-duration}

Una sessione utente ospite rimane attiva per 2 ore. Ciò significa che lo stato della [!UICONTROL scatola luminosa] viene mantenuto fino a 1 ora dall'ora di inizio della sessione e dopo 2 ore la sessione ospite corrente viene riavviata.\
Ad esempio, un utente ospite accede a [!DNL Brand Portal] 1500 ore e aggiunge le risorse a Lightbox da scaricare a 16:50 ore. Se l'utente non scarica la raccolta [!UICONTROL Lightbox] (o le relative risorse) prima di 17:00 ore, la [!UICONTROL lightbox] diventerà vuota perché l'utente dovrà riavviare la sessione alla fine di 1 ora (1700 ore).

## Sessioni ospiti simultanei consentite {#concurrent-guest-sessions-allowed}

Il numero di sessioni ospiti simultanee è limitato al 10% della quota utente totale per organizzazione. Ciò significa che per un'organizzazione con una quota utente pari a 200, è possibile lavorare simultaneamente su 20 utenti ospiti. Al 21 ° utente viene negato l'accesso e sarà possibile accedere come ospite solo al termine della sessione di uno dei 20 utenti ospiti attivi.

## Interazione dell'utente ospite con Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigazione nell'interfaccia utente ospite

Quando si immette l' [!DNL Brand Portal] ospite, gli utenti sono in grado di vedere tutte [le risorse e le cartelle condivise](../using/brand-portal-sharing-folders.md#sharefolders) pubblicamente o con gli utenti ospiti esclusivamente. Questa vista è solo la visualizzazione del contenuto, che visualizza le risorse in uno dei layout schede, elenco o colonne.

![](assets/disabled-folder-hierarchy1.png)

Tuttavia, gli utenti ospiti visualizzano la struttura di cartelle (a partire dalla cartella principale) e le cartelle condivise disposte all'interno delle rispettive cartelle principali all'accesso, [!DNL Brand Portal]se gli amministratori hanno abilitato [la configurazione Abilita gerarchia](../using/brand-portal-general-configuration.md#main-pars-header-1621071021) cartelle.

Queste cartelle principali sono cartelle virtuali e non è possibile eseguire azioni su di esse. Potete riconoscere queste cartelle virtuali con un'icona a forma di lucchetto.

Non sono disponibili attività di azione al momento del passaggio del mouse o della selezione nella vista a schede, a differenza delle cartelle condivise. Il pulsante Panoramica viene visualizzato quando si seleziona una cartella virtuale nella vista a colonne e a elenco.

>[!NOTE]
>
>La miniatura predefinita delle cartelle virtuali è quella della prima cartella condivisa.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

L'opzione Impostazioni visualizzazione consente agli utenti ospiti di regolare le dimensioni delle schede in vista a schede o colonne da visualizzare in visualizzazione Elenco.

![](assets/nav-guest-user.png)

La struttura Contenuto permette di spostarsi nella gerarchia delle risorse.

![](assets/guest-login-ui.png)

[!DNL Brand Portal] fornisce **l'opzione Panoramica** agli utenti ospiti per visualizzare le Proprietà risorse delle risorse o delle cartelle selezionate. L'opzione Panoramica è visibile:

1. Nella barra degli strumenti nella parte superiore della selezione di una risorsa o di una cartella.
2. Nel menu a discesa selezionate il selettore della barra.

Selezionando l'opzione Panoramica mentre è selezionata una risorsa o una cartella, gli utenti possono visualizzare il titolo, il percorso e l'ora della creazione delle risorse. Mentre, nella pagina dei dettagli delle risorse che seleziona Panoramica, gli utenti possono vedere i metadati della risorsa.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**[!UICONTROL L'opzione di navigazione]** nella barra a sinistra consente di navigare dai file alle [!UICONTROL raccolte] e di tornare alla sessione ospite in modo che gli utenti possano sfogliare le risorse nei file o nelle [!UICONTROL raccolte].

**L'opzione Filtro** consente agli utenti ospiti di filtrare i file e le cartelle di risorse utilizzando i predicati di ricerca impostati dall'amministratore.

### Funzionalità degli utenti ospiti

Gli utenti ospiti possono accedere alle risorse pubbliche e [!DNL Brand Portal]dispongono inoltre di alcune restrizioni come discusso ulteriormente.

Gli utenti ospiti possono:

* accedere a tutte le cartelle pubbliche e [!UICONTROL raccolte] destinate a tutti [!DNL Brand Portal] gli utenti.
* membri di Sfoglia, pagina dei dettagli e visualizzazione completa delle risorse dei membri di tutte le cartelle e [!UICONTROL raccolte pubbliche].
* cercare risorse in cartelle pubbliche e [!UICONTROL raccolte].
* aggiungere risorse alla [!UICONTROL raccolta Lightbox]. Queste modifiche alla [!UICONTROL raccolta] rimangono invariate durante la sessione.
* scaricare risorse direttamente o tramite [!UICONTROL la raccolta lightbox].

Gli utenti ospiti non possono:

* creare [!UICONTROL raccolte] e ricerche salvate o condividerle ulteriormente.
* accesso alle impostazioni della cartella e [!UICONTROL delle raccolte] .
* condividere le risorse come collegamenti.

### Scaricare le risorse nella sessione ospite

Gli utenti ospiti possono scaricare direttamente le risorse condivise o esclusivamente con gli utenti ospiti. [!DNL Brand Portal] Gli utenti ospiti possono anche aggiungere risorse a [!UICONTROL Lightbox] ( [!UICONTROL raccolta pubblica]) e scaricare la [!UICONTROL raccolta lightbox] prima della scadenza della sessione.

Per scaricare risorse e [!UICONTROL raccolte], utilizzate l'icona di download da:

* miniature di azioni rapide, visualizzate sul passaggio del mouse sulla risorsa o [!UICONTROL sulla raccolta]
* la barra degli strumenti nella parte superiore, che viene visualizzata selezionando la risorsa o [!UICONTROL la raccolta]

![](assets/download-on-guest.png)

Selezionando **Abilita accelerazione download** nella finestra di dialogo Scarica, [potete migliorare le prestazioni di download](../using/accelerated-download.md).

## Esci dalla sessione ospite {#exit-guest-session}

Per uscire da una sessione ospite, utilizzate **Termina sessione** dalle opzioni disponibili nell'intestazione. Tuttavia, se il browser utilizzato per la sessione ospite-è inattivo, la sessione scade automaticamente dopo due ore di inattività.

![](assets/end-guest-session.png)

## Monitoraggio delle attività degli utenti ospiti {#monitoring-guest-user-activities}

Gli amministratori possono monitorare l'interazione degli utenti ospiti con l ' [!DNL Brand Portal]. I report generati possono [!DNL Brand Portal] fornire informazioni chiave sulle attività degli utenti ospiti. Ad esempio, **il** rapporto Scarica può essere utilizzato per monitorare il numero di risorse scaricate dall'utente ospite. **Il rapporto Login** utente può informare quando l'utente ospite ha eseguito l'ultimo accesso al portale e la frequenza degli accessi in una durata specificata.
