---
title: Accesso a Brand Portal come ospite
seo-title: Guest Access to Brand Portal
description: Consentire l'accesso degli utenti ospiti e risparmiare il lavoro per l'onboarding di numerosi utenti senza autenticazione.
seo-description: Allow guest access and save the effort to onboard numerous users without authentication.
uuid: edb4378d-1710-44a2-97a6-594d99f62fff
contentOwner: VG
topic-tags: introduction
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: b9e9fe7b-0373-42d1-851b-7c76b47657c2
exl-id: ecce0a45-abae-41c4-9ea7-5dfdcf19e5ea
source-git-commit: 51dc6f9c3b3a59751d7910513279e52906d97b88
workflow-type: tm+mt
source-wordcount: '1026'
ht-degree: 0%

---

# Accesso a Brand Portal come ospite {#guest-access-to-brand-portal}

Experience Manager Assets Brand Portal consente l’accesso guest al portale. Un utente ospite non ha bisogno di credenziali per accedere al portale e ha accesso alle risorse pubbliche (e alle raccolte) del portale. Gli utenti della sessione guest possono aggiungere risorse a lightbox (raccolta privata) e scaricare lo stesso finché la sessione non dura, ovvero 2 ore dall&#39;inizio della sessione, a meno che l&#39;utente ospite non scelga di [[!UICONTROL terminare sessione]](#exit-guest-session).

La funzionalità di accesso degli ospiti consente alle organizzazioni di [condividere rapidamente le risorse approvate](../using/brand-portal-sharing-folders.md#how-to-share-folders) con il pubblico previsto su larga scala senza doverle caricare. Brand Portal 6.4.2 e versioni successive è attrezzata per servire più utenti guest simultanei, che rappresenta il 10% della quota utente totale per organizzazione. Consentendo agli utenti ospiti l’accesso si risparmia tempo nella gestione e nella gestione di punteggi di utenti con funzionalità limitate su Brand Portal.\
Le organizzazioni possono abilitare (o disabilitare) l&#39;accesso guest sull&#39;account Brand Portal dell&#39;organizzazione utilizzando l&#39;opzione **[!UICONTROL Consenti accesso guest]** dalle impostazioni **[!UICONTROL Accesso]** nel pannello strumenti amministrativi.

<!--
Comment Type: annotation
Last Modified By: mgulati
Last Modified Date: 2018-08-17T10:42:59.879-0400
Removed the first para: "AEM Assets Brand Portal allows public users to enter the portal anonymously and have restricted access to the allowed public resources as guests. Organization users with guest role need not seek access and authentication from administrators."
-->

![](assets/enable-guest-access.png)

## Inizia sessione ospite {#begin-guest-session}

Per accedere in modo anonimo a Brand Portal, selezionare **[!UICONTROL Fare clic qui]** corrispondente a **[!UICONTROL Accesso guest?]** nella schermata di benvenuto di Brand Portal. Inserisci il controllo di sicurezza captcha per concedere l’accesso all’utilizzo di Brand Portal.

![](assets/bp-login-screen.png)

## Durata sessione ospite {#guest-session-duration}


Una sessione utente guest rimane attiva per 15 minuti.
Questo significa che lo stato della **[!UICONTROL Lightbox]** viene mantenuto per 15 minuti dall&#39;ora di inizio della sessione e dopo di che la sessione guest corrente si riavvia in modo che lo stato Lightbox venga perso.

Ad esempio, un utente guest accede a Brand Portal a 1500 ore e aggiunge risorse a **[!UICONTROL Lightbox]** per il download alle 15:05 ore. Se l&#39;utente non scarica la raccolta **[!UICONTROL Lightbox]** (o le relative risorse) prima delle 15:15 ore (entro 15 minuti dall&#39;accesso), deve riavviare la sessione. La **[!UICONTROL Lightbox]** è vuota e le risorse caricate non sono più disponibili se la sessione è stata persa.

## Sessioni ospiti simultanee consentite {#concurrent-guest-sessions-allowed}

Il numero di sessioni guest simultanee è limitato al 10% della quota utente totale per organizzazione. Significa che per un&#39;organizzazione con una quota di utenti di 200, un massimo di 20 utenti ospiti può lavorare contemporaneamente. Al 21° utente viene negato l’accesso e può accedervi come ospite solo se termina la sessione di uno dei 20 utenti attivi.

>[!NOTE]
>
>Brand Portal non invia notifiche se il numero di utenti con licenza supera il valore contrattuale (quota). Inoltre, non limita alcuna attività degli utenti con licenza.

## Interazione con gli utenti ospiti con Brand Portal {#guest-user-interaction-with-brand-portal}

### Navigazione nell’interfaccia utente degli ospiti

All&#39;ingresso in Brand Portal come ospite, gli utenti possono vedere pubblicamente tutte le [risorse e cartelle condivise](../using/brand-portal-sharing-folders.md#sharefolders) o esclusivamente con gli utenti ospiti. Questa visualizzazione è l’unica visualizzazione contenuto, che visualizza le risorse nei layout di schede, elenchi o colonne.

![](assets/disabled-folder-hierarchy1.png)

Tuttavia, se gli amministratori hanno abilitato la configurazione [Abilita gerarchia cartelle](../using/brand-portal-general-configuration.md#main-pars-header-1621071021), gli utenti guest visualizzano la struttura delle cartelle (a partire dalla cartella principale) e le cartelle condivise organizzate all’interno delle rispettive cartelle principali al momento dell’accesso a Brand Portal.

Queste cartelle principali sono le cartelle virtuali e non è possibile eseguire azioni su di esse. È possibile riconoscere queste cartelle virtuali con un&#39;icona di blocco.

A differenza delle cartelle condivise, non sono visibili attività di azione al passaggio del mouse o alla selezione in **[!UICONTROL Vista a schede]**. **** Il pulsante Panoramica viene visualizzato quando si seleziona una cartella virtuale in Vista a  **[!UICONTROL colonne]** e Vista a  **[!UICONTROL elenco]**.

>[!NOTE]
>
>La miniatura predefinita delle cartelle virtuali è l&#39;immagine in miniatura della prima cartella condivisa.

![](assets/enabled-hierarchy1.png) ![](assets/hierarchy1-nonadmin.png) ![](assets/hierarchy-nonadmin.png) ![](assets/hierarchy2-nonadmin.png)

**[!UICONTROL L’opzione Visualizza]** impostazione consente agli utenti ospiti di regolare le dimensioni delle schede nelle colonne  **[!UICONTROL Vista]** a schede da visualizzare nella Vista a  **[!UICONTROL elenco]**.

![](assets/nav-guest-user.png)

La **[!UICONTROL Struttura contenuto]** consente di spostarsi nella gerarchia delle risorse.

![](assets/guest-login-ui.png)

Brand Portal fornisce l’opzione **[!UICONTROL Panoramica]** agli utenti ospiti per visualizzare **[!UICONTROL Proprietà risorsa]** delle risorse/cartelle selezionate. L&#39;opzione **[!UICONTROL Panoramica]** è visibile:

* Nella barra degli strumenti in alto, seleziona una risorsa o una cartella.
* Nell’elenco a discesa selezionando il selettore della barra.

Selezionando l’opzione **[!UICONTROL Panoramica]** mentre è selezionata una risorsa/cartella, gli utenti possono vedere il titolo, il percorso e l’ora della creazione della risorsa. Nella pagina dei dettagli della risorsa, invece, l’opzione **[!UICONTROL Panoramica]** consente agli utenti di visualizzare i metadati della risorsa.

![](assets/overview-option-1.png)

![](assets/overview-rail-selector-1.png)

**** L’opzione Navigazione nella barra a sinistra consente di spostarsi dai file alle raccolte e di tornare alla sessione guest in modo che gli utenti possano sfogliare le risorse in file o raccolte.

**** L’opzione Filtro consente agli utenti ospiti di filtrare file e cartelle di risorse utilizzando i predicati di ricerca impostati dall’amministratore.

### Funzionalità degli utenti ospiti

Gli utenti ospiti possono accedere alle risorse pubbliche su Brand Portal e possono inoltre discutere ulteriormente di alcune restrizioni.

**Gli utenti ospiti possono**:

* Accedi a tutte le cartelle pubbliche e le raccolte destinate a tutti gli utenti Brand Portal.
* Sfoglia i membri, la pagina dei dettagli e visualizza tutte le risorse dei membri di tutte le cartelle e raccolte pubbliche.
* Cercare risorse in cartelle e raccolte pubbliche.
* Aggiungi le risorse alla raccolta Lightbox. Queste modifiche alla raccolta persistono durante la sessione.
* Scarica le risorse direttamente o tramite la raccolta Lightbox.

**Gli utenti ospiti non possono**:

* Crea raccolte e ricerche salvate o condividile ulteriormente.
* Accedi alle impostazioni della cartella e delle raccolte.
* Condividi le risorse come collegamenti.

### Scaricare risorse in una sessione guest

Gli utenti ospiti possono scaricare direttamente le risorse condivise pubblicamente o esclusivamente con gli utenti ospiti su Brand Portal. Gli utenti ospiti possono anche aggiungere risorse alla raccolta **[!UICONTROL Lightbox]** (raccolta pubblica) e scaricare la raccolta **[!UICONTROL Lightbox]** prima della scadenza della sessione.

Per scaricare risorse e raccolte, utilizza l’icona di download da:

* Miniature delle azioni rapide, visualizzate al passaggio del mouse sulla risorsa o sulla raccolta
* Barra degli strumenti nella parte superiore, visualizzata selezionando la risorsa o la raccolta

![](assets/download-on-guest.png)

Selezionando **[!UICONTROL Abilita accelerazione download]** nella finestra di dialogo [!UICONTROL Scarica] puoi [migliorare le prestazioni di download](../using/accelerated-download.md).

## Esci dalla sessione guest {#exit-guest-session}

Per uscire da una sessione guest, utilizza **[!UICONTROL End Session]** dalle opzioni disponibili nell&#39;intestazione. Tuttavia, se la scheda del browser utilizzata per la sessione guest è inattiva, la sessione scade automaticamente dopo due ore di inattività.

![](assets/end-guest-session.png)

## Monitoraggio delle attività degli utenti guest {#monitoring-guest-user-activities}

Gli amministratori possono monitorare l’interazione degli utenti ospiti con Brand Portal. I rapporti generati in Brand Portal possono fornire informazioni chiave sulle attività degli utenti ospiti. Ad esempio, il rapporto **[!UICONTROL Download]** può essere utilizzato per tenere traccia del conteggio delle risorse scaricate dall’utente ospite. **[!UICONTROL Il rapporto]** Registri utente può indicare quando l’utente ospite ha effettuato l’ultimo accesso al portale e la frequenza degli accessi in una determinata durata.
