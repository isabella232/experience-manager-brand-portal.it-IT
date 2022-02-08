---
title: Cercare le risorse in Brand Portal
seo-title: Asset searching and saved search on Experience Manager Assets Brand Portal
description: La funzionalità di ricerca Brand Portal consente di cercare rapidamente le risorse rilevanti utilizzando la ricerca globale e i filtri di ricerca consentono di limitare ulteriormente la ricerca. Salva le ricerche come raccolte avanzate per il futuro.
seo-description: Brand Portal search capability lets you quickly search for relevant assets using omnisearch, and search filters help you further narrow down your search. Save your searches as smart collections for future.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
exl-id: 7297bbe5-df8c-4d0b-8204-218a9fdc2292
source-git-commit: dc425522f134781b4420eb8643ee6ee65d98b6cc
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 7%

---

# Cercare le risorse in Brand Portal {#search-assets-on-brand-portal}

La funzionalità di ricerca Brand Portal consente di cercare rapidamente le risorse rilevanti utilizzando la ricerca omnisearch e la ricerca dei facet che utilizza i filtri per facilitarti di limitare ulteriormente la ricerca. Puoi cercare le risorse a livello di file o cartelle e salvare i risultati della ricerca come raccolte avanzate. Tuttavia, non è possibile cercare le risorse di una raccolta utilizzando la ricerca omnisearch o facet.

## Cercare risorse utilizzando Omnisearch {#search-assets-using-omnisearch}

Per cercare risorse in Brand Portal:

1. Dalla barra degli strumenti, fai clic sul pulsante **[!UICONTROL Ricerca]** o premere il tasto &quot;**[!UICONTROL /]**&quot; chiave per lanciare Omnisearch.

   ![](assets/omnisearchicon-1.png)

1. Nella casella di ricerca, digita una parola chiave per le risorse da cercare.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Sono necessari almeno 3 caratteri in omnisearch per visualizzare i suggerimenti di ricerca.

1. Seleziona dai suggerimenti correlati visualizzati nell’elenco a discesa per accedere rapidamente alle risorse pertinenti.

   ![](assets/assets-search-result.png)

   *Ricerca di risorse tramite omnisearch*

Per informazioni sul comportamento di ricerca con le risorse con tag avanzati, consulta [comprendere i risultati e il comportamento della ricerca](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## Ricerca tramite facet nel pannello Filtri {#search-using-facets-in-filters-panel}

I facet di ricerca nel pannello Filtri aggiungono granularità all’esperienza di ricerca e rendono efficiente la funzionalità di ricerca. I facet di ricerca utilizzano più dimensioni (predicati) che consentono di eseguire ricerche complesse. È possibile espandere facilmente il livello di dettaglio desiderato per una ricerca più mirata.

Ad esempio, se si cerca un&#39;immagine, è possibile scegliere se si desidera una bitmap o un&#39;immagine vettoriale. Puoi ridurre ulteriormente l’ambito della ricerca specificando il tipo MIME per l’immagine nel facet di ricerca Tipo file . Allo stesso modo, durante la ricerca di documenti, è possibile specificare il formato, ad esempio il formato PDF o MS Word.

![Pannello Filtri in Brand Portal](assets/file-type-search.png "Pannello Filtri in Brand Portal")

La **[!UICONTROL Filtri]** il pannello include alcuni facet standard, come **[!UICONTROL Browser Percorsi]**, **[!UICONTROL Tipo di file]**, **[!UICONTROL Dimensione file]**, **[!UICONTROL Stato]** e **[!UICONTROL Orientamento]**. Tuttavia, puoi [aggiungi facet di ricerca personalizzati](../using/brand-portal-search-facets.md) o rimuovere specifici facet di ricerca dal **[!UICONTROL Filtri]** aggiungendo o rimuovendo predicati nel modulo di ricerca sottostante. Visualizza l&#39;elenco delle opzioni disponibili e utilizzabili [predicati di ricerca in Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

Per applicare filtri alla ricerca, utilizza le opzioni disponibili [facet di ricerca](../using/brand-portal-search-facets.md):

1. Fai clic sull’icona della sovrapposizione e seleziona **[!UICONTROL Filtro]**.

   ![](assets/selectorrail.png)

1. Da **[!UICONTROL Filtri]** a sinistra, seleziona le opzioni appropriate per applicare i filtri pertinenti.
Ad esempio, utilizza i seguenti filtri standard:

   * **[!UICONTROL Browser Percorsi]** per cercare le risorse in una directory specifica. Il percorso di ricerca predefinito del predicato per il browser del percorso è `/content/dam/mac/<tenant-id>/`, che può essere configurato modificando il modulo di ricerca predefinito.
   >[!NOTE]
   >
   >Per utenti non amministratori, [!UICONTROL Browser Percorsi] in [!UICONTROL Filtro] mostra solo la struttura del contenuto delle cartelle (e delle relative cartelle precedenti) condivise con loro.\
   >Per gli utenti amministratori, il browser Percorsi consente di passare a qualsiasi cartella in Brand Portal.

   * **[!UICONTROL Tipo di file]** per specificare il tipo (immagine, documento, elementi multimediali, archivio) del file di risorse che stai cercando. Inoltre, è possibile limitare l’ambito della ricerca, ad esempio, specificare il tipo MIME (Tiff, Bitmap, GIMP Images) per l’immagine o il formato (PDF o MS Word) per i documenti.
   * **[!UICONTROL Dimensione file]** per cercare le risorse in base alle loro dimensioni. È possibile specificare i limiti inferiori e superiori dell’intervallo di dimensioni per limitare la ricerca e specificare l’unità di misura da cercare.
   * **[!UICONTROL Stato]** per cercare le risorse in base agli stati delle risorse, ad esempio Approvazione (approvata, Modifiche richieste, Rifiutate, In sospeso) e Scadenza.
   * **[!UICONTROL Valutazione media]** cercare le risorse in base al rating delle risorse.
   * **[!UICONTROL Orientamento]** per cercare le risorse in base all’orientamento (orizzontale, verticale, quadrato) delle risorse.
   * **[!UICONTROL Stile]** per cercare le risorse in base allo stile (colorato, monocromatico) delle risorse.
   * **[!UICONTROL Formato video]** per cercare risorse video in base al formato (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   È possibile utilizzare [facet di ricerca personalizzati](../using/brand-portal-search-facets.md) nel pannello Filtri modificando il modulo di ricerca sottostante.

   * **[!UICONTROL Predicato proprietà]** se utilizzato nel modulo di ricerca, consente di cercare le risorse che corrispondono a una proprietà di metadati a cui è mappato il predicato.\
      Ad esempio, se il predicato Proprietà è mappato a [!UICONTROL `jcr:content /metadata/dc:title`], puoi cercare le risorse in base al loro titolo.\
      La [!UICONTROL Predicato proprietà] supporta le ricerche di testo per:

      **Espressioni parziali**
Per consentire la ricerca delle risorse mediante espressioni parziali nel predicato delle proprietà, abilita la casella di controllo **[!UICONTROL Ricerca parziale]** in Modulo di ricerca.\
      Questo consente di cercare le risorse desiderate anche senza specificare le parole o espressioni precise usate nei metadati della risorsa.\
      Operazioni disponibili:
      * Specifica una parola presente nella frase cercata nel facet nel pannello Filtri . Ad esempio, se cerchi il termine **salire** (e il predicato Proprietà è mappato su [!UICONTROL `dc:title`] (proprietà), quindi tutte le risorse con la parola **salire** nel titolo viene restituita la frase corrispondente.
      * Specificare una parte di una parola da cercare, utilizzando il carattere jolly (*) al posto dei caratteri rimanenti.
Ad esempio, se cerchi:
         * **salita*** restituisce tutte le risorse con parole che iniziano con i caratteri &quot;climb&quot; nella frase del titolo.
         * ***salita** restituisce tutte le risorse con parole che terminano con caratteri &quot;climb&quot; nella frase del titolo.
         * ***salita*** restituisce tutte le risorse con parole contenenti i caratteri &quot;climb&quot; nella frase del titolo.

Per consentire una ricerca senza distinzione tra maiuscole e minuscole nel predicato delle proprietà, abilita il       **Testo sensibile a maiuscole e minuscole**
Per consentire una ricerca senza distinzione tra maiuscole e minuscole nel predicato delle proprietà, abilita il **[!UICONTROL Ignora maiuscole]** in Modulo di ricerca. Per impostazione predefinita, la ricerca di testo nel predicato delle proprietà fa distinzione tra maiuscole e minuscole.
   >[!NOTE]
   >
   >Al momento della selezione **[!UICONTROL Ricerca parziale]** casella di controllo, **[!UICONTROL Ignora maiuscole]** è selezionato per impostazione predefinita.

   ![](assets/wildcard-prop-1.png)

   I risultati della ricerca vengono visualizzati in base ai filtri applicati, insieme al conteggio dei risultati della ricerca.

   ![](assets/omnisearch-with-filters.png)

   Risultato della ricerca di risorse con conteggio dei risultati della ricerca.

1. È possibile spostarsi facilmente su un elemento dal risultato della ricerca e tornare allo stesso risultato utilizzando il pulsante Indietro del browser senza dover ripetere la query di ricerca.

## Salva le ricerche come raccolta avanzata {#save-your-searches-as-smart-collection}

È possibile salvare le impostazioni di ricerca come raccolta avanzata per poter ripetere rapidamente la stessa ricerca senza dover ripristinare le stesse impostazioni in un secondo momento. Tuttavia, non è possibile applicare filtri di ricerca in una raccolta.

Per salvare le impostazioni di ricerca come raccolta avanzata:

1. Tocca o fai clic su **[!UICONTROL Salvataggio di una raccolta avanzata]** e fornisci un nome per la raccolta avanzata.

   Per rendere la raccolta avanzata accessibile a tutti gli utenti, seleziona **[!UICONTROL Pubblico]**. Un messaggio conferma che la raccolta avanzata è stata creata e aggiunta all’elenco delle ricerche salvate.

   >[!NOTE]
   >
   >Agli utenti non amministratori può essere impedito di rendere pubbliche le raccolte avanzate, per evitare di avere un numero enorme di raccolte avanzate pubbliche create da utenti non amministratori su Brand Portal dell’organizzazione. Le organizzazioni possono disabilitare la **[!UICONTROL Consenti creazione raccolte avanzate pubbliche]** configurazione da **[!UICONTROL Generale]** impostazioni disponibili nel pannello strumenti di amministrazione.

   ![](assets/save_smartcollectionui.png)

1. Per salvare la raccolta avanzata con un nome diverso e selezionare o deselezionare la **[!UICONTROL Pubblico]** casella di controllo, fai clic su **[!UICONTROL Modifica raccolta avanzata]**.

   ![](assets/edit_smartcollection.png)

1. Sulla **[!UICONTROL Modifica raccolta avanzata]** finestra di dialogo, seleziona **[!UICONTROL Salva con nome]** e immetti un nome per la raccolta avanzata. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/saveas_smartsearch.png)
