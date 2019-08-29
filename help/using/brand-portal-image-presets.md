---
title: Applicare predefiniti per immagini o rappresentazioni dinamiche
seo-title: Applicare predefiniti per immagini o rappresentazioni dinamiche
description: 'Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. I predefiniti per immagini consentono a AEM Assets Brand Portal di distribuire in modo dinamico immagini di dimensioni, formati e proprietà diverse. '
seo-description: 'Analogamente a una macro, un predefinito per immagini è una raccolta di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. I predefiniti per immagini consentono a AEM Assets Brand Portal di distribuire in modo dinamico immagini di dimensioni, formati e proprietà diverse. '
uuid: a 3 c 8705 c -5 fbd -472 c -8 b 61-f 65 b 3 e 552 c 1 b
content-type: riferimento
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: a 512 dfa 0-fef 3-4 c 3 f-a 389-a 0 a 3 a 7415 bac
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Applicare predefiniti per immagini o rappresentazioni dinamiche {#apply-image-presets-or-dynamic-renditions}

Analogamente a una macro, un predefinito per immagini è una [!UICONTROL raccolta] di comandi di ridimensionamento e formattazione predefiniti salvati con un nome. I predefiniti per immagini consentono [!DNL AEM] alle risorse [!DNL Brand Portal] di distribuire in modo dinamico immagini di dimensioni, formati e proprietà diverse.

Un predefinito per immagini viene usato per generare rappresentazioni dinamiche di immagini che possono essere visualizzate in anteprima e scaricate. Quando visualizzate l'anteprima delle immagini e le relative rappresentazioni, potete scegliere un predefinito per riformattare le immagini in base alle specifiche impostate dall'amministratore.

Per visualizzare i rendering dinamici di una risorsa in [!DNL Brand Portal], accertatevi che la rappresentazione PTIFF sia presente nell'istanza [!DNL AEM] di authoring dal punto in cui pubblicate [!DNL Brand Portal]. Quando pubblicate la risorsa, viene pubblicata anche [!DNL Brand Portal]la relativa rappresentazione PTIFF. Non è possibile generare la rappresentazione PTIFF.[!DNL Brand Portal]

>[!NOTE]
>
>Quando si scaricano le immagini e le relative rappresentazioni, non è possibile scegliere tra i predefiniti esistenti. Potete invece specificare le proprietà di un predefinito per immagini personalizzato. Per ulteriori informazioni, consultate [Applicare i predefiniti per immagini durante il download delle immagini](../using/brand-portal-image-presets.md#main-pars-text-1403412644).

Per ulteriori informazioni sui parametri richiesti durante la creazione dei predefiniti per immagini, consultate [Gestione dei predefiniti]per immagini (https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html)[!DNL AEM].

## Creare un predefinito per immagini {#create-an-image-preset}

Gli amministratori possono creare predefiniti per immagini che vengono visualizzati come rappresentazioni dinamiche nella pagina dei dettagli della risorsa. Potete creare un predefinito per immagini da zero o salvarne uno esistente con un nuovo nome. Quando create un predefinito per immagini, scegliete una dimensione per la distribuzione delle immagini e i comandi di formattazione. Quando un'immagine viene distribuita per la visualizzazione, l'aspetto viene ottimizzato in base ai comandi scelti.
È possibile notare che solo gli amministratori possono creare dei predefiniti per immagini.[!DNL Brand Portal]

È possibile notare che solo gli amministratori possono creare dei predefiniti per immagini.[!DNL Brand Portal]

>[!NOTE]
>
>Vengono create rappresentazioni dinamiche per le risorse per le quali è disponibile PTIFF. Pertanto, se per una risorsa non è stata creata la [!DNL AEM] rappresentazione TIFF piramidale e la si pubblica [!DNL Brand Portal], è possibile esportare solo le rappresentazioni di sistema, ma le rappresentazioni dinamiche vengono presentate come un'opzione.
La [!DNL AEM] modalità Ibrida Elemento multimediale dinamico deve essere attivata (autore) per creare tiff piramidali (ptiff) di una risorsa. Quando viene pubblicata una risorsa, i predefiniti [!DNL Brand Portal]per immagini vengono applicati e vengono visualizzate le rappresentazioni dinamiche.

1. Nella [!DNL AEM] barra degli strumenti in alto, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   !![](assets/[!DNL AEM]logo. png)

2. Dal pannello Strumenti di amministrazione, fate clic **su Predefiniti immagine**.

   ![](assets/admin-tools-panel-4.png)

3. Nella pagina Predefiniti immagine, fate clic su **Crea**.

   ![](assets/image_preset_homepage.png)

4. Nella pagina **Modifica predefinito** immagine, inserite i valori nelle schede **Base** e **Avanzate** , compreso un nome. Le opzioni sono delineate nelle [opzioni dei predefiniti immagine](https://docs.adobe.com/docs/en//6-0/administer/integration/dynamic-media/image-presets.html#Image%20preset%20options)[!DNL AEM]. I predefiniti vengono visualizzati nel riquadro a sinistra e possono essere utilizzati al volo con altre risorse.

   ![](assets/image_preset_create.png)

   >[!NOTE]
   >
   >Potete anche usare la pagina **Modifica predefinito** immagine per modificare le proprietà di un predefinito esistente. Per modificare un predefinito per immagini, selezionatelo dalla pagina dei predefiniti immagine e fate clic **su Modifica**.

5. Fai clic su **Salva**. Il predefinito per immagini viene creato e visualizzato nella pagina dei predefiniti per immagini.
6. Per eliminare un predefinito per immagini, selezionatelo dalla pagina dei predefiniti immagine e fate clic **su Elimina**. Nella pagina di conferma, fai clic **su Elimina** per confermare l'eliminazione. Il predefinito per immagini viene rimosso dalla pagina dei predefiniti per immagini.

## Applicare predefiniti per immagini durante l'anteprima delle immagini {#apply-image-presets-when-previewing-images}

Quando visualizzate l'anteprima delle immagini e le relative rappresentazioni, scegliete tra i predefiniti esistenti per riformattare le immagini in base alle specifiche definite dall'amministratore.

1. Nell' [!DNL Brand Portal] interfaccia, fate clic su un'immagine per aprirla.
2. Fate clic sull'icona della sovrapposizione a sinistra, quindi scegliete **Rappresentazioni**.

   ![](assets/image-preset-previewrenditions.png)

3. Nell'elenco **Rappresentazioni** , selezionate la rappresentazione dinamica appropriata, ad esempio **Miniatura**. Viene eseguito il rendering dell'immagine di anteprima in base alla vostra scelta.

   ![](assets/image-preset-previewrenditionthumbnail.png)

## Applicare i predefiniti per immagini durante il download delle immagini {#apply-image-presets-when-downloading-images}

Quando scaricate le immagini e le relative rappresentazioni, [!DNL Brand Portal]non potete scegliere tra i predefiniti per immagini esistenti. Tuttavia, potete personalizzare le proprietà dei predefiniti immagine in base alle quali desiderate riformattare le immagini.

1. Dall' [!DNL Brand Portal] interfaccia, effettuate una delle seguenti operazioni:

   * Passate il puntatore sull'immagine da scaricare. Dalle miniature delle azioni rapide disponibili, fate clic sull'icona **Scarica** .
   ![](assets/downloadsingleasset.png)

   * Selezionate l'immagine da scaricare. Dalla barra degli strumenti in alto, fate clic sull'icona **Scarica** .
   ![](assets/downloadassets.png)

2. Nella finestra **di** dialogo Scarica, selezionate le opzioni richieste a seconda se desiderate scaricare la risorsa con o senza le relative rappresentazioni.

   ![](assets/donload-assets-dialog.png)

3. Per scaricare i rendering dinamici della risorsa, selezionate l' **** opzione Rappresentazioni dinamiche.
4. Potete personalizzare le proprietà dei predefiniti immagine in base alle quali desiderate riformattare l'immagine e le relative rappresentazioni in modo dinamico durante il download. Specificate le dimensioni, il formato, lo spazio colore, la risoluzione e il modificatore immagine.

   ![](assets/dynamicrenditions.png)

5. Fate clic **su Scarica**. Le rappresentazioni dinamiche personalizzate vengono scaricate in un file ZIP insieme all'immagine e alle rappresentazioni che hai scelto di scaricare. Tuttavia, non viene creato alcun file ZIP se viene scaricata una sola risorsa, per un download rapido.
