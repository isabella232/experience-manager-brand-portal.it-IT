---
title: Applicazione di predefiniti per immagini o rappresentazioni dinamiche
seo-title: Applicazione di predefiniti per immagini o rappresentazioni dinamiche
description: 'Analogamente a una macro, un predefinito per immagini è una raccolta predefinita di comandi di ridimensionamento e formattazione salvati con un nome. I predefiniti per immagini consentono a AEM Assets Brand Portal di distribuire dinamicamente immagini di dimensioni, formati e proprietà diverse. '
seo-description: 'Analogamente a una macro, un predefinito per immagini è una raccolta predefinita di comandi di ridimensionamento e formattazione salvati con un nome. I predefiniti per immagini consentono a AEM Assets Brand Portal di distribuire dinamicamente immagini di dimensioni, formati e proprietà diverse. '
uuid: a3c8705c-5fbd-472c-8b61-f65b3e552c1b
content-type: riferimento
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: a512dfa0-fef3-4c3f-a389-a0a3a7415back
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Applicazione di predefiniti per immagini o rappresentazioni dinamiche {#apply-image-presets-or-dynamic-renditions}

Analogamente a una macro, un predefinito per immagini è una raccolta predefinita di comandi di ridimensionamento e formattazione salvati con un nome. I predefiniti per immagini consentono a AEM Assets Brand Portal di distribuire dinamicamente immagini di dimensioni, formati e proprietà diverse.

Per generare rappresentazioni dinamiche delle immagini da visualizzare in anteprima e scaricare, viene utilizzato un predefinito per immagini. Quando visualizzate l’anteprima delle immagini e delle relative rappresentazioni, potete scegliere un predefinito per riformattare le immagini in base alle specifiche impostate dall’amministratore.

Per visualizzare le rappresentazioni dinamiche di una risorsa in Brand Portal, accertatevi che la relativa rappresentazione in forma piramidale esista nell’istanza di creazione AEM da cui pubblicate nel Brand Portal. Quando pubblicate la risorsa, la relativa rappresentazione PTIFF viene pubblicata anche sul Brand Portal. Non è possibile generare la rappresentazione PTIFF dal Portale marchio.

>[!NOTE]
>
>Quando si scaricano le immagini e le relative rappresentazioni, non è possibile scegliere tra i predefiniti esistenti. Potete invece specificare le proprietà di un predefinito per immagini personalizzato. Per ulteriori informazioni, consultate [Applicare i predefiniti per immagini durante il download delle immagini](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

Per ulteriori informazioni sui parametri richiesti per la creazione dei predefiniti per immagini, consultate [Gestione dei predefiniti](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html)per immagini.

## Creare un predefinito per immagini {#create-an-image-preset}

Gli amministratori possono creare dei predefiniti per immagini da visualizzare come rappresentazioni dinamiche nella pagina dei dettagli della risorsa. Potete creare un predefinito per immagini da zero o salvarne uno esistente con un nuovo nome. Quando create un predefinito per immagini, scegliete una dimensione per la distribuzione delle immagini e i comandi di formattazione. Quando un’immagine viene trasmessa per la visualizzazione, il suo aspetto viene ottimizzato in base ai comandi scelti.
Solo gli amministratori possono creare predefiniti per immagini in Brand Portal.

Solo gli amministratori possono creare predefiniti per immagini in Brand Portal.

>[!NOTE]
>
>Le rappresentazioni dinamiche di un’immagine vengono create utilizzando il TIFF piramidale. Se il TIFF piramidale non è disponibile per alcuna risorsa, le rappresentazioni dinamiche per tale risorsa non possono essere recuperate nel portale marchio.
Se l’istanza di AEM (Author) è in esecuzione in modalità **ibrida** Dynamic Media, le rappresentazioni TIFF piramidali delle risorse immagine vengono create e salvate nell’archivio AEM. Se invece l’istanza di AEM (Author) è in esecuzione in modalità ****Dynamic Media Scene7, sul server Scene 7 sono presenti rappresentazioni TIFF piramidali delle risorse immagine.
Quando tali risorse vengono pubblicate sul portale del marchio, vengono applicati i predefiniti per immagini e vengono visualizzate le rappresentazioni dinamiche.

1. Dalla barra degli strumenti di AEM nella parte superiore, fate clic sul logo Adobe per accedere agli strumenti amministrativi.

1. Dal pannello degli strumenti di amministrazione, fate clic su Predefiniti **** immagine.

   ![](assets/admin-tools-panel-4.png)

1. Nella pagina dei predefiniti per immagini, fate clic su **[!UICONTROL Crea]**.

   ![](assets/image_preset_homepage.png)

1. Nella pagina **[!UICONTROL Modifica predefinito]** immagine, inserite i valori nelle schede **[!UICONTROL Base]** e **[!UICONTROL Avanzate]** , a seconda dei casi, compreso un nome. Le opzioni sono descritte nelle opzioni [Predefinito](https://docs.adobe.com/docs/en/AEM/6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)immagine. I predefiniti vengono visualizzati nel riquadro a sinistra e possono essere usati al volo con altre risorse.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >Potete anche usare la pagina **[!UICONTROL Modifica predefinito]** immagine per modificare le proprietà di un predefinito esistente. Per modificare un predefinito per immagini, selezionatelo dalla pagina dei predefiniti per immagini e fate clic su **[!UICONTROL Modifica]**.

1. Fai clic su **[!UICONTROL Salva]**. Il predefinito per immagini viene creato e visualizzato nella pagina dei predefiniti per immagini.
1. Per eliminare un predefinito per immagini, selezionatelo dalla pagina dei predefiniti per immagini e fate clic su **[!UICONTROL Elimina]**. Nella pagina di conferma, fate clic su **[!UICONTROL Elimina]** per confermare l’eliminazione. Il predefinito per immagini viene rimosso dalla pagina dei predefiniti per immagini.

## Applicazione di predefiniti per immagini durante l’anteprima delle immagini {#apply-image-presets-when-previewing-images}

Quando visualizzate l’anteprima delle immagini e delle relative rappresentazioni, scegliete uno dei predefiniti esistenti per riformattare le immagini in base alle specifiche impostate dall’amministratore.

1. Dall’interfaccia Brand Portal, fate clic su un’immagine per aprirla.
1. Fate clic sull'icona della sovrapposizione a sinistra, quindi scegliete **[!UICONTROL Rappresentazioni]**.

   ![](assets/image-preset-previewrenditions.png)

1. Dall'elenco **[!UICONTROL Rappresentazioni]** , selezionare la rappresentazione dinamica appropriata, ad esempio **[!UICONTROL Miniatura]**. Il rendering dell'immagine di anteprima è basato sulla scelta della rappresentazione.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Applicare i predefiniti per immagini durante il download delle immagini {#apply-image-presets-when-downloading-images}

Quando scaricate immagini e relative rappresentazioni da Brand Portal, non potete scegliere tra i predefiniti per immagini esistenti. Tuttavia, potete personalizzare le proprietà dei predefiniti per immagini in base ai quali desiderate riformattare le immagini.

1. Dall’interfaccia Brand Portal, effettuate una delle seguenti operazioni:

   * Passate il puntatore sull’immagine da scaricare. Dalle miniature delle azioni rapide disponibili, fai clic sull’icona **[!UICONTROL Scarica]** .
   ![](assets/downloadsingleasset.png)

   * Selezionate l’immagine da scaricare. Dalla barra degli strumenti nella parte superiore, fate clic sull'icona **[!UICONTROL Scarica]** .
   ![](assets/downloadassets.png)

1. Nella finestra di dialogo **[!UICONTROL Scarica]** , selezionate le opzioni desiderate a seconda che la risorsa venga scaricata con o senza le relative rappresentazioni.

   ![](assets/donload-assets-dialog.png)

1. Per scaricare le rappresentazioni dinamiche della risorsa, seleziona l’opzione rappresentazioni **[!UICONTROL dinamiche]** .
1. Potete personalizzare le proprietà dei predefiniti per immagini in base alle quali desiderate riformattare dinamicamente l’immagine e le relative rappresentazioni durante il download. Specificate le dimensioni, il formato, lo spazio colore, la risoluzione e il modificatore di immagine.

   ![](assets/dynamicrenditions.png)

1. Fate clic su **[!UICONTROL Scarica]**. Le rappresentazioni dinamiche personalizzate vengono scaricate in un file ZIP insieme all'immagine e alle rappresentazioni che avete scelto di scaricare. Tuttavia, se viene scaricata una singola risorsa, non viene creato alcun file ZIP che ne garantisca la rapidità di download.
