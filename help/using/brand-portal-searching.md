---
title: Cercare risorse su Brand Portal
seo-title: Ricerca delle risorse e ricerca salvata su AEM Brand Portal
description: La funzionalità di ricerca Brand Portal consente di cercare rapidamente risorse pertinenti tramite Omnisearch e i filtri di ricerca consentono di ridurre ulteriormente la ricerca. Salvate le ricerche come raccolte intelligenti per future.
seo-description: La funzionalità di ricerca Brand Portal consente di cercare rapidamente risorse pertinenti tramite Omnisearch e i filtri di ricerca consentono di ridurre ulteriormente la ricerca. Salvate le ricerche come raccolte intelligenti per future.
uuid: c 2955198-bdc 0-4853-a 13 a -661 e 6 a 9 ec 61 f
contentOwner: bdhar
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: Searchandpromote
discoiquuid: dc 751 cd 7-f 663-46 d 2-84 c 4-5 bb 12 a 4 fe 1 ba
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Cercare risorse su Brand Portal {#search-assets-on-brand-portal}

[!DNL Brand Portal] La funzionalità di ricerca consente di cercare rapidamente risorse pertinenti tramite omniricerca e la ricerca con facet che utilizza filtri per ridurre ulteriormente la ricerca. Potete inoltre salvare le ricerche come [!UICONTROL raccolte intelligenti] per il futuro.

## Cercare risorse tramite Omnisearch {#search-assets-using-omnisearch}

Per cercare le risorse in [!DNL Brand Portal]:

1. Dalla barra degli strumenti, fate clic sull'icona **di ricerca** o premete il tasto «**/**» per avviare Omnisearch.

   ![](assets/omnisearchicon-1.png)

2. Nella casella di ricerca, digitate una parola chiave per le risorse da cercare.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Per visualizzare i suggerimenti di ricerca sono necessari almeno 3 caratteri.

3. Scegli tra i suggerimenti correlati visualizzati nell'elenco a discesa per accedere rapidamente alle risorse pertinenti.

   ![](assets/assets-search-result.png)

   Ricerca risorse tramite omnisearch

## Ricerca utilizzando i facet nel pannello Filtri {#search-using-facets-in-filters-panel}

I facet di ricerca nel pannello Filtri aggiungono granularità all'esperienza di ricerca e rendono le funzionalità di ricerca efficienti. I facet di ricerca utilizzano più dimensioni (predicati) che consentono di eseguire ricerche complesse. Puoi trovare facilmente il livello di dettaglio per una ricerca più mirata.

Ad esempio, se state cercando un'immagine, potete scegliere se visualizzare un'immagine bitmap o vettoriale. Potete ridurre ulteriormente l'ambito della ricerca specificando il tipo MIME per l'immagine nel facet di ricerca Tipo file. Allo stesso modo, quando si ricercano documenti, è possibile specificare il formato, ad esempio PDF o Word Word.

![Pannello Filtri nel [!DNL Brand Portal]](assets/file-type-search.png "pannello Filtri in [! DNL Brand Portal]")

Il pannello Filtri include alcuni facet standard, come Browser percorsi, Tipo file, Dimensione file, Stato e Orientamento. Tuttavia, [potete aggiungere facet di ricerca personalizzati](../using/brand-portal-search-facets.md) o rimuovere facet di ricerca specifici dal pannello **Filtri** aggiungendo o rimuovendo i predefiniti nel modulo di ricerca sottostante. Consultate l'elenco dei predicati [di ricerca disponibili e utilizzabili sul portale brand](../using/brand-portal-search-facets.md#list-of-search-predicates).

Per applicare filtri alla ricerca utilizzando i facet [di ricerca disponibili](../using/brand-portal-search-facets.md):

1. Fate clic sull'icona della sovrapposizione e selezionate **Filtro**.

   ![](assets/selectorrail.png)

2. Dal pannello **Filtri** a sinistra, selezionate le opzioni appropriate per applicare i filtri pertinenti.
Ad esempio, utilizzate i seguenti filtri standard:

   * **Browser Percorsi** per cercare le risorse in una directory specifica. Il percorso di ricerca predefinito per il browser percorso è */content/dam/mac/ &lt; tenant-id &gt;/*, che può essere configurato modificando il modulo di ricerca predefinito.
   >[!NOTE]
   >
   >Per gli utenti non amministratori, nel pannello dei percorsi nel pannello Filtro viene visualizzata solo la struttura del contenuto delle cartelle (e delle relative cartelle antenate) condivise con loro.\
   >Per gli utenti admin, il browser Percorsi consente di passare a qualsiasi cartella.[!DNL Brand Portal]

   * **Tipo di file** per specificare il tipo (immagine, documento, multimedia, archivio) del file di risorse ricercato. Inoltre, potete limitare l'ambito della ricerca, ad esempio, specificando il tipo MIME (Tiff, Bitmap, Immagini GIMP) per l'immagine o il formato (PDF o MS Word) per i documenti.
   * **Dimensione** file per cercare le risorse in base alle loro dimensioni. Potete specificare i limiti inferiore e superiore per l'intervallo di dimensioni per limitare la ricerca e specificare l'unità di misura da cercare.
   * **Stato** per cercare risorse in base agli stati delle risorse, ad esempio Approvazione (Approvato, Modifiche richieste, Rifiutato, In sospeso) e Scadenza.
   * **Valutazione media** per cercare risorse in base alla valutazione delle risorse.
   * **Orientamento** per cercare le risorse in base all'orientamento (orizzontale, verticale, quadrato) delle risorse.
   * **Consente** di cercare le risorse in base allo stile (colorato, monocromatico) delle risorse.
   * **Formato video** per la ricerca di risorse video in base al formato (DVI, Flash, MPEG 4, MPEG, OGG Theora, quicktime, Windows Media, webm).
   Potete usare [i facet di ricerca personalizzati](../using/brand-portal-search-facets.md) nel pannello Filtri modificando il modulo di ricerca sottostante.

   * **Predicato proprietà** Se utilizzata nel modulo di ricerca, consente di cercare risorse che corrispondono a una proprietà di metadati alla quale il predicato viene mappato.\
      Ad esempio, se la funzione Predicato proprietà è mappata `jcr:content /metadata/dc:title`, puoi cercare le risorse in base al titolo.\
      Predicato proprietà supporta le ricerche di testo:

      **Espressioni parziali**
Per consentire la ricerca delle risorse mediante espressioni parziali nel predicato delle proprietà, abilita la casella di controllo **Ricerca parziale** in Modulo di ricerca.\
      Questo consente di cercare le risorse desiderate anche senza specificare le parole o espressioni precise usate nei metadati della risorsa.\
      Potete:
* Specificate una parola che si verifichi nella frase di ricerca nel facet nel pannello Filtri. For example, if you search for the term **climb** (and Property Predicate is mapped to `dc:title` property), then all the assets with the word **climb** in their title phrase are returned.
* Specificare una parte di una parola da cercare, utilizzando il carattere jolly (*) al posto dei caratteri rimanenti.
Ad esempio, se cerchi:
      **scale *** restituisce tutte le risorse contenenti parole che iniziano con i caratteri «rimbalzi» nella frase title.
      *** rimbalzare** tutte le risorse contenenti parole che terminano con caratteri «rimbalzati» nella frase titolo.
      *** height *** restituisce tutte le risorse contenenti parole contenenti i caratteri "jump" nella propria frase title.\
      **Testo
senza distinzione tra maiuscole e minuscole** Per consentire la ricerca di proprietà senza distinzione tra maiuscole e minuscole, abilitare la **casella di** controllo Ignora caso in Modulo di ricerca. Per impostazione predefinita, la ricerca di testo sul predicato delle proprietà fa distinzione tra maiuscole e minuscole.
   >[!NOTE]
   >
   >Selezionando la **casella di** controllo Ricerca parziale, **Ignora caso** è selezionato per impostazione predefinita.

   ![](assets/wildcard-prop-1.png)

   I risultati della ricerca vengono visualizzati in base ai filtri applicati, insieme al conteggio dei risultati della ricerca.

   ![](assets/omnisearch-with-filters.png)

   Risultato della ricerca delle risorse con conteggio dei risultati della ricerca

3. Potete facilmente passare a un elemento dal risultato di ricerca e tornare allo stesso risultato di ricerca utilizzando il pulsante Indietro nel browser senza dover ripetere la query di ricerca.

## Salvare le ricerche come raccolta intelligente {#save-your-searches-as-smart-collection}

Potete salvare le impostazioni di ricerca come una raccolta avanzata per poter ripetere rapidamente la stessa ricerca senza dover ripetere le stesse impostazioni in un secondo momento.

Per salvare le impostazioni di ricerca come una raccolta dinamica:

1. Toccate/fate clic **su Salva raccolta** avanzata e fornite un nome per la raccolta dinamica.

   Per rendere la raccolta dinamica accessibile a tutti gli utenti, selezionate **Pubblica.** Un messaggio conferma che la raccolta avanzata è stata creata e aggiunta all'elenco delle ricerche salvate.

   >[!NOTE]
   >
   >Gli utenti non amministratori possono impedire che [!UICONTROL le raccolte intelligenti] vengano rese pubbliche, per evitare di avere un numero elevato di raccolte smart [!UICONTROL pubbliche] create da utenti non amministratori nell'organizzazione [!DNL Brand Portal]. Le organizzazioni possono disattivare la **configurazione di creazione[!UICONTROL delle raccolte]smart** pubblica da Impostazioni **generali** disponibili nel pannello Strumenti di amministrazione.

   ![](assets/save_smartcollectionui.png)

1. Per salvare la raccolta avanzata con un nome diverso, e selezionate o deselezionate la casella **di** controllo Pubblica, fate clic su **Modifica raccolta dinamica**.

   ![](assets/edit_smartcollection.png)

1. Nella finestra **di dialogo Modifica raccolta** dinamica, selezionate **Salva con nome** e immettete un nome per la raccolta dinamica. Fai clic su **Salva**.

   ![](assets/saveas_smartsearch.png)
