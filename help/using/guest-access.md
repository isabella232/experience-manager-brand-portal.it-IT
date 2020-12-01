---
title: Accesso a Brand Portal come ospite
seo-title: Accesso a Brand Portal come ospite
description: Consentite l’accesso agli ospiti e salvate l’impegno a bordo di numerosi utenti che non devono essere autenticati.
seo-description: Consentite l’accesso agli ospiti e salvate l’impegno a bordo di numerosi utenti che non devono essere autenticati.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: mgulati
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
translation-type: tm+mt
source-git-commit: 1a8658a3ced4fd211a1c1606a80bb51920ca8be1
workflow-type: tm+mt
source-wordcount: '1029'
ht-degree: 1%

---


# Accesso a Brand Portal come ospite {#guest-access-to-brand-portal}

AEM Portale marchio consente agli ospiti di accedere al portale. Un utente ospite non ha bisogno di credenziali per entrare nel portale e ha accesso alle risorse pubbliche (e alle raccolte) del portale. Gli utenti della sessione ospite possono aggiungere risorse alla propria lightbox (raccolta privata) e scaricare la stessa fino alla sua durata, ossia 2 ore dall&#39;inizio della sessione, a meno che l&#39;utente ospiti non scelga di [[!UICONTROL terminare la sessione]](#exit-guest-session).

La funzionalità di accesso degli ospiti consente alle organizzazioni di [condividere rapidamente le risorse approvate](../using/brand-portal-sharing-folders.md#how-to-share-folders) con il pubblico previsto su scala senza doverle imbarcare. A partire da Brand Portal 6.4.2 è disponibile per più utenti ospiti simultanei, pari al 10% della quota totale di utenti per organizzazione. Consentendo l’accesso degli ospiti potete risparmiare tempo per gestire e inserire punteggi di utenti che devono utilizzare funzionalità limitate sul Brand Portal.\
Le organizzazioni possono abilitare (o disabilitare) l&#39;accesso degli ospiti sull&#39;account Brand Portal dell&#39;organizzazione utilizzando l&#39;opzione **[!UICONTROL Consenti accesso degli ospiti]** dalle impostazioni **[!UICONTROL Accesso]** nel pannello degli strumenti amministrativi.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Inizia sessione ospite {#begin-guest-session}

Per accedere al Portale marchio in modo anonimo, selezionare **[!UICONTROL Fare clic qui]** corrispondente a **[!UICONTROL Accesso ospiti?]** nella schermata di benvenuto di Brand Portal. Immettete il controllo di sicurezza catcha per concedere l’accesso all’utilizzo del Portale marchio.

![](assets/bp-login-screen.png)

## Durata sessione ospite {#guest-session-duration}


Una sessione utente ospite rimane attiva per 15 minuti.
Questo significa che lo stato della **[!UICONTROL Lightbox]** viene mantenuto per 15 minuti dall&#39;ora di inizio della sessione e, successivamente, lo stato Lightbox viene riavviato in modo che lo stato Lightbox venga perso.

Ad esempio, un utente ospite accede al Brand Portal a 1500 ore e aggiunge risorse a **[!UICONTROL Lightbox]** per il download alle 15:05 ore. Se l&#39;utente non scarica la raccolta **[!UICONTROL Lightbox]** (o le relative risorse) prima delle 15:15 ore (entro 15 minuti dall&#39;accesso), dovrà riavviare la sessione. La **[!UICONTROL Lightbox]** sarà vuota, il che significa che le risorse caricate non saranno più disponibili se la sessione viene persa.

## Sessioni guest simultanee consentite {#concurrent-guest-sessions-allowed}

Il numero di sessioni guest simultanee è limitato al 10% della quota utente totale per organizzazione. Ciò significa che per un&#39;organizzazione con una quota di utenti di 200, al massimo 20 utenti ospiti possono lavorare contemporaneamente. Al 21° utente viene negato l’accesso e può accedervi come ospite solo se termina la sessione di uno dei 20 utenti ospiti attivi.

## Interazione degli utenti ospiti con il portale dei marchi {#guest-user-interaction-with-brand-portal}

### Navigazione interfaccia utente per gli ospiti

Entrando nel Brand Portal come ospite, gli utenti possono vedere tutte le [risorse e cartelle condivise](../using/brand-portal-sharing-folders.md#sharefolders) pubblicamente o esclusivamente con gli utenti ospiti. Questa vista è l&#39;unica vista del contenuto, che visualizza le risorse nei layout di schede, elenchi o colonne.

![](assets/disabled-folder-hierarchy1.png)

Tuttavia, gli utenti ospiti possono vedere la struttura delle cartelle (a partire dalla cartella principale) e le cartelle condivise disposte all&#39;interno delle rispettive cartelle principali al momento dell&#39;accesso al Portale marchio, se gli amministratori hanno attivato la configurazione [Abilita gerarchia cartelle](../using/brand-portal-general-configuration.md#main-pars-header-1621071021).

Queste cartelle principali sono le cartelle virtuali e non è possibile eseguire alcuna azione su di esse. È possibile riconoscere queste cartelle virtuali con un&#39;icona a forma di lucchetto.

A differenza delle cartelle condivise, non è visibile alcuna attività di azione al passaggio del mouse o alla selezione in **[!UICONTROL vista a schede]**. **[!UICONTROL Il pulsante]** Overviewbutton viene visualizzato quando si seleziona una cartella virtuale in  **[!UICONTROL Visualizzazione]** colonne e Visualizzazione **** elenco.

>[!NOTE]
>
>La miniatura predefinita delle cartelle virtuali è la miniatura della prima cartella condivisa.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL L’]** opzione Visualizza impostazione consente agli utenti ospiti di regolare le dimensioni delle schede nelle colonne del  **[!UICONTROL visualizzatore]** a schede da visualizzare nella vista **[!UICONTROL a]** elenco.

![](assets/nav-guest-user.png)

La struttura **[!UICONTROL Contenuto]** consente di spostarsi nella gerarchia delle risorse.

![](assets/guest-login-ui.png)

Il Portale marchio offre l&#39;opzione **[!UICONTROL Panoramica]** agli utenti ospiti per visualizzare **[!UICONTROL Proprietà risorsa]** delle risorse/cartelle selezionate. L&#39;opzione **[!UICONTROL Panoramica]** è visibile:

* Nella barra degli strumenti nella parte superiore, quando si seleziona una risorsa o una cartella.
* Nell&#39;elenco a discesa quando si seleziona il selettore della barra.
Selezionando l&#39;opzione **[!UICONTROL Panoramica]** mentre è selezionata una risorsa/cartella, gli utenti possono visualizzare il titolo, il percorso e l&#39;ora della creazione della risorsa. Nella pagina dei dettagli della risorsa, invece, quando si seleziona l’opzione **[!UICONTROL Panoramica]** gli utenti possono vedere i metadati della risorsa.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)<br />

**[!UICONTROL L&#39;opzione di]** navigazione nella barra a sinistra consente di spostarsi dai file alle raccolte e di tornare alla sessione ospite in modo che gli utenti possano sfogliare le risorse nei file o nelle raccolte.

**[!UICONTROL L’opzione]** Filtro consente agli utenti ospiti di filtrare i file e le cartelle di risorse utilizzando i predicati di ricerca impostati dall’amministratore.

### Funzionalità per gli utenti ospiti

Gli utenti ospiti possono accedere alle risorse pubbliche sul Brand Portal e possono anche avere poche limitazioni, come ulteriormente discusso.

**Gli utenti ospiti possono**:

* Accedete a tutte le cartelle pubbliche e raccolte progettate per tutti gli utenti del Brand Portal.
* Sfogliate i membri, la pagina dei dettagli e visualizzate la risorsa completa dei membri di tutte le cartelle e raccolte pubbliche.
* Cercare risorse nelle cartelle pubbliche e nelle raccolte.
* Aggiungete le risorse alla raccolta lightbox. Queste modifiche alla raccolta persistono durante la sessione.
* Scaricate le risorse direttamente o attraverso la raccolta di immagini lightbox.

**Gli utenti ospiti non possono**:

* Create raccolte e ricerche salvate, o condividetele ulteriormente.
* Accedete alle impostazioni delle cartelle e delle raccolte.
* Condividi le risorse come collegamenti.

### Scaricare risorse in una sessione ospite

Gli utenti ospiti possono scaricare direttamente le risorse condivise pubblicamente o esclusivamente con gli utenti ospiti sul Brand Portal. Gli utenti ospiti possono inoltre aggiungere risorse alla raccolta **[!UICONTROL Lightbox]** (raccolta pubblica) e scaricare la raccolta **[!UICONTROL Lightbox]** prima della scadenza della sessione.

Per scaricare risorse e raccolte, utilizzate l&#39;icona di download da:

* Miniature delle azioni rapide, che vengono visualizzate quando si passa il puntatore del mouse sulla risorsa o sulla raccolta
* La barra degli strumenti nella parte superiore, che viene visualizzata quando si seleziona la risorsa o la raccolta

![](assets/download-on-guest.png)

Se si seleziona **[!UICONTROL Abilita accelerazione download]** nella finestra di dialogo [!UICONTROL Scarica], è possibile [migliorare le prestazioni di download](../using/accelerated-download.md).

## Esci dalla sessione ospite {#exit-guest-session}

Per uscire da una sessione ospite, utilizzate **[!UICONTROL Termina sessione]** dalle opzioni disponibili nell&#39;intestazione. Tuttavia, se la scheda del browser utilizzata per la sessione ospite è inattiva, la sessione scade automaticamente dopo due ore di inattività.

![](assets/end-guest-session.png)

## Monitoraggio delle attività degli utenti ospiti {#monitoring-guest-user-activities}

Gli amministratori possono monitorare l&#39;interazione degli utenti ospiti con il Brand Portal. I report generati in Brand Portal possono fornire informazioni chiave sulle attività degli utenti ospiti. Ad esempio, il rapporto **[!UICONTROL Download]** può essere utilizzato per tenere traccia del numero di risorse scaricate dall&#39;utente ospite. **[!UICONTROL Il rapporto]** Registri utente può indicare l’ultima volta che l’utente ospite ha eseguito l’accesso al portale e la frequenza degli accessi in una durata specificata.
