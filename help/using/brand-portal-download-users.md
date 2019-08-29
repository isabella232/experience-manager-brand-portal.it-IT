---
title: Scaricare le risorse
seo-title: Scaricare le risorse
description: Tutti gli utenti possono scaricare contemporaneamente più risorse e cartelle. In questo modo, le risorse del marchio approvate possono essere distribuite in modo sicuro per l'utilizzo offline.
seo-description: Tutti gli utenti possono scaricare contemporaneamente più risorse e cartelle. In questo modo, le risorse del marchio approvate possono essere distribuite in modo sicuro per l'utilizzo offline.
uuid: 4 b 57118 e-a 76 e -4 d 8 a -992 a-cb 3 c 3097 bc 03
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: download-install
discoiquuid: f 90 c 2214-beea -4695-9102-8 b 952 bc 9 fd 17
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Scaricare le risorse {#download-assets}

Tutti gli utenti possono scaricare contemporaneamente più risorse e [!DNL Brand Portal]cartelle. In questo modo, le risorse del marchio approvate possono essere distribuite in modo sicuro per l'utilizzo offline. Continuate a leggere per scoprire come scaricare le risorse approvate [!DNL Brand Portal]e cosa attendersi dalle prestazioni [di download](../using/brand-portal-download-users.md#main-pars-header).

>[!NOTE]
>
>Solo gli amministratori possono scaricare le risorse scadute. Per ulteriori informazioni sulle risorse scadute, consulta [Gestione dei diritti digitali delle risorse](../using/manage-digital-rights-of-assets.md).

## Passaggi per scaricare le risorse {#steps-to-download-assets}

Per scaricare risorse o cartelle contenenti risorse, [!DNL Brand Portal]effettuate le seguenti operazioni:

1. Dall' [!DNL Brand Portal] interfaccia, effettuate una delle seguenti operazioni:

   * Selezionate le cartelle o le risorse da scaricare. Dalla barra degli strumenti in alto, fate clic sull'icona **Scarica** .
   ![](assets/downloadassets-1.png)

   * Per scaricare una singola cartella o una singola risorsa, passate il mouse sulla cartella o sulla risorsa. Dalle miniature delle azioni rapide disponibili, fate clic sull'icona **Scarica** .
   ![](assets/downloadsingleasset-1.png)

   >[!NOTE]
   >
   >Se le risorse che state scaricando includono anche risorse con licenza, verrete reindirizzati alla **pagina Gestione** copyright. In questa pagina, selezionate le risorse, fate clic **su Accetto**, quindi su **Scarica**. Se scegli di non d'accordo, le risorse con licenza non vengono scaricate.\
   >Alle risorse protette da licenza è [associato](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) un contratto di licenza, che viene eseguito impostando la proprietà [dei metadati della risorsa](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) in [!DNL AEM] Assets.

   ![](assets/licensed-asset-download-1.png)

   La **finestra di** dialogo Scarica viene visualizzata con l'opzione **delle risorse** selezionata per impostazione predefinita.

   ![](assets/donload-assets-dialog-1.png)

   >[!NOTE]
   >
   >Se le risorse che state scaricando sono file di immagini e selezionate solo l'opzione **Risorse** nella finestra di dialogo Scarica, ma non [sono autorizzate dall'amministratore ad avere accesso ai rendering originali dei file](../using/brand-portal-adding-users.md#main-pars-procedure-202029708) immagine, non vengono scaricati né scaricati i file immagine, indicando che l'amministratore è stato limitato dall'amministratore per accedere alle rappresentazioni originali.

   ![](assets/restrictaccess-note.png)

2. Per scaricare i rendering delle risorse oltre alle risorse, selezionate **Rappresentazioni**. Tuttavia, per consentire il download di rappresentazioni generate automaticamente insieme a rappresentazioni personalizzate, deselezionate **Escludi rappresentazioni** generazione automatica, che per impostazione predefinita è selezionata.

   ![](assets/exclude-auto-renditions.png)

   Per scaricare solo le rappresentazioni, deselezionate **Risorse**.

   >[!NOTE]
   >
   >Per impostazione predefinita, vengono scaricate solo le risorse. Tuttavia, i rendering originali dei file immagine non vengono scaricati se l'amministratore non [dispone dell'autorizzazione per accedere ai rendering originali dei file immagine](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   * Per accelerare il download dei file di risorse, [!DNL Brand Portal]selezionate **Abilita l'opzione di accelerazione** download e [seguite la procedura guidata](../using/accelerated-download.md#main-pars-header-405749062). Per saperne di più sul download rapido delle risorse, consulta [Guida per accelerare i download da [! DNL Brand Portal]](../using/accelerated-download.md).

   * Per applicare un predefinito per immagini [personalizzato alla risorsa e alle relative rappresentazioni](../using/brand-portal-image-presets.md#applyimagepresetswhendownloadingimages), selezionate **Rappresentazioni dinamiche**. Per applicare il predefinito per immagini personalizzato durante il download della risorsa e le relative rappresentazioni, specificate le proprietà personalizzate del predefinito per immagini (dimensione, formato, spazio colore, risoluzione e modificatore immagine). Per scaricare solo le rappresentazioni dinamiche, eliminate **le risorse**.
   ![](assets/dynamic-renditions.png)

   >[!NOTE]
   >
   >Per visualizzare in anteprima (o scaricare) rappresentazioni dinamiche di qualsiasi risorsa, verificate che il file multimediale dinamico sia attivato e [!UICONTROL che sia presente la] rappresentazione tiff piramidale della risorsa nell'istanza [!DNL AEM] di creazione, da dove le risorse sono state pubblicate. Quando una risorsa viene pubblicata, [!DNL Brand Portal]viene pubblicata anche la rappresentazione [!UICONTROL tiff] piramidale. Non è possibile generare [!UICONTROL la rappresentazione tiff] piramidale.[!DNL Brand Portal]

   * Per mantenere la [!DNL Brand Portal] gerarchia delle cartelle durante il download delle risorse, selezionate **Crea cartella separata per ciascuna risorsa**. Per impostazione predefinita, [!DNL Brand Portal] la gerarchia delle cartelle viene ignorata e tutte le risorse vengono scaricate in una cartella del sistema locale.

   * Per inviare una notifica e-mail agli utenti con un collegamento per il download delle risorse, selezionate **Invia per e-mail**.
   ![](assets/download-link.png)

   >[!NOTE]
   >
   >Il collegamento di download sulla notifica e-mail scade dopo 45 giorni.
   >
   >Gli amministratori possono personalizzare i messaggi e-mail, ossia logo, descrizione e piè di pagina, utilizzando la [funzione Branding](../using/brand-portal-branding.md) .

3. Fate clic **su Scarica**.

   Le risorse (e le rappresentazioni se selezionate) vengono scaricate come file ZIP nella cartella locale. Tuttavia, non viene creato alcun file ZIP se una singola risorsa viene scaricata senza rendering, garantendo così un download rapido.

   I rendering originali delle risorse selezionate non vengono scaricati se l'amministratore non [è autorizzato ad accedere alle rappresentazioni originali](../using/brand-portal-adding-users.md#main-pars-procedure-202029708).

   >[!NOTE]
   >
   >Le risorse selezionate singolarmente e scaricate sono visibili nel rapporto scaricato delle risorse. Tuttavia, se una cartella contenente risorse viene scaricata, non viene visualizzata né la cartella né le risorse nel rapporto scaricato delle risorse.

   Per scoprire come scaricare le risorse dai collegamenti condivisi, consulta [Scaricare le risorse dai collegamenti condivisi](../using/brand-portal-link-share.md#main-pars-header-1703469193).

## Prestazioni di download attese {#expected-download-performance}

L'esperienza di download dei file può variare per gli utenti in posizioni client diverse, a seconda di fattori quali la connessione Internet locale e la latenza server. Le prestazioni di download previste per il file 2 GB osservato in posizioni client diverse sono riportate di seguito, con [!DNL Brand Portal] server in Oregon negli Stati Uniti:

| Percorso cliente | Latenza tra client e server | Velocità di download prevista | Tempo impiegato per scaricare un file da 2 GB |
|-------------------------|-----------------------------------|-------------------------|------------------------------------|
| USA occidentale (N. California) | 18 millisecondi | 7.68 MB/s | 4 minuti |
| USA occidentale (Oregon) | 42 millisecondi | 3.84 MB/s | 9 minuti |
| USA orientale (N. Virginia) | 85 millisecondi | 1.61 MB/s | 21 minuti |
| APAC (Tokyo) | 124 millisecondi | 1.13 MB/s | 30 minuti |
| Noida | 275 millisecondi | 0.5 MB/s | 68 minuti |
| Sydney | 175 millisecondi | 0.49 MB/s | 69 minuti |
| Londra | 179 millisecondi | 0.32 MB/s | 106 minuti |
| Singapore | 196 millisecondi | 0.5 MB/s | 68 minuti |

**Nota**: I dati citati vengono osservati in condizioni di test, che possono variare per gli utenti che si trovano in posizioni diverse in presenza di latenza e larghezza di banda diverse.
