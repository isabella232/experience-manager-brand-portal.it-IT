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
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1124'
ht-degree: 7%

---

# Cercare le risorse in Brand Portal {#search-assets-on-brand-portal}

La funzionalità di ricerca Brand Portal consente di cercare rapidamente le risorse rilevanti utilizzando la ricerca omnisearch e la ricerca dei facet che utilizza i filtri per facilitarti di limitare ulteriormente la ricerca. Puoi anche salvare le ricerche come raccolte avanzate per il futuro.

## Cercare risorse utilizzando Omnisearch {#search-assets-using-omnisearch}

Per cercare risorse in Brand Portal:

1. Dalla barra degli strumenti, fai clic sull&#39;icona **[!UICONTROL Cerca]** oppure premi il tasto &quot;**[!UICONTROL /]**&quot; per avviare Omnisearch.

   ![](assets/omnisearchicon-1.png)

1. Nella casella di ricerca, digita una parola chiave per le risorse da cercare.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Sono necessari almeno 3 caratteri in omnisearch per visualizzare i suggerimenti di ricerca.

1. Seleziona dai suggerimenti correlati visualizzati nell’elenco a discesa per accedere rapidamente alle risorse pertinenti.

   ![](assets/assets-search-result.png)

   *Ricerca di risorse tramite omnisearch*

Per informazioni sul comportamento di ricerca con risorse con tag avanzati, consulta [comprendere i risultati e il comportamento della ricerca](https://experienceleague.adobe.com/docs/experience-manager-65/assets/using/search-assets.html).

## Ricerca tramite facet nel pannello Filtri {#search-using-facets-in-filters-panel}

I facet di ricerca nel pannello Filtri aggiungono granularità all’esperienza di ricerca e rendono efficiente la funzionalità di ricerca. I facet di ricerca utilizzano più dimensioni (predicati) che consentono di eseguire ricerche complesse. È possibile espandere facilmente il livello di dettaglio desiderato per una ricerca più mirata.

Ad esempio, se si cerca un&#39;immagine, è possibile scegliere se si desidera una bitmap o un&#39;immagine vettoriale. Puoi ridurre ulteriormente l’ambito della ricerca specificando il tipo MIME per l’immagine nel facet di ricerca Tipo file . Allo stesso modo, durante la ricerca di documenti, è possibile specificare il formato, ad esempio il formato PDF o MS Word.

![Pannello Filtri nel pannello Brand ](assets/file-type-search.png "PortalFilters in Brand Portal")

Il pannello **[!UICONTROL Filtri]** include alcuni facet standard, come- **[!UICONTROL Browser percorso]**, **[!UICONTROL Tipo file]**, **[!UICONTROL Dimensione file]**, **[!UICONTROL Stato]** e **[!UICONTROL Orientamento]**. Tuttavia, è possibile [aggiungere facet di ricerca personalizzati](../using/brand-portal-search-facets.md) o rimuovere facet di ricerca specifici dal pannello **[!UICONTROL Filtri]** aggiungendo o rimuovendo predicati nel modulo di ricerca sottostante. Vedi l&#39;elenco dei predicati di ricerca disponibili e utilizzabili su Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).[

Per applicare i filtri alla ricerca, utilizza i [facet di ricerca disponibili](../using/brand-portal-search-facets.md):

1. Fai clic sull&#39;icona di sovrapposizione e seleziona **[!UICONTROL Filtro]**.

   ![](assets/selectorrail.png)

1. Dal pannello **[!UICONTROL Filtri]** a sinistra, seleziona le opzioni appropriate per applicare i filtri pertinenti.
Ad esempio, utilizza i seguenti filtri standard:

   * **[!UICONTROL Percorso]** Browser per cercare le risorse in una directory specifica. Il percorso di ricerca predefinito del predicato Browser percorsi è `/content/dam/mac/<tenant-id>/`, che può essere configurato modificando il modulo di ricerca predefinito.
   >[!NOTE]
   >
   >Per gli utenti non amministratori, [!UICONTROL Browser percorsi] nel pannello [!UICONTROL Filtro] mostra solo la struttura del contenuto delle cartelle (e delle relative cartelle precedenti) condivise con loro.\
   >Per gli utenti amministratori, il browser Percorsi consente di passare a qualsiasi cartella in Brand Portal.

   * **[!UICONTROL Tipo di file]** per specificare il tipo (immagine, documento, multimedia, archivio) del file di risorsa che stai cercando. Inoltre, è possibile limitare l’ambito della ricerca, ad esempio, specificare il tipo MIME (Tiff, Bitmap, GIMP Images) per l’immagine o il formato (PDF o MS Word) per i documenti.
   * **[!UICONTROL File]** : consente di cercare le risorse in base alle loro dimensioni. È possibile specificare i limiti inferiori e superiori dell’intervallo di dimensioni per limitare la ricerca e specificare l’unità di misura da cercare.
   * **** Ricerca statica delle risorse in base agli stati delle risorse, ad esempio Approvazione (approvata, Modifiche richieste, Rifiutate, In sospeso) e Scadenza.
   * **[!UICONTROL Valutazione media]** per cercare le risorse in base al rating delle risorse.
   * **** Orientamento per cercare le risorse in base all’orientamento (orizzontale, verticale, quadrato) delle risorse.
   * **** Consente di cercare in stile le risorse in base allo stile (colorato e monocromatico) delle risorse.
   * **[!UICONTROL Video]** Formatico cerca le risorse video in base al loro formato (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).

   È possibile utilizzare [facet di ricerca personalizzati](../using/brand-portal-search-facets.md) nel pannello Filtri modificando il modulo di ricerca sottostante.

   * **[!UICONTROL Predicato proprietà]** se utilizzato nel modulo di ricerca, consente di cercare le risorse che corrispondono a una proprietà di metadati a cui è mappato il predicato.\
      Ad esempio, se il predicato Proprietà è mappato su [!UICONTROL `jcr:content /metadata/dc:title`], puoi cercare le risorse in base al loro titolo.\
      Il [!UICONTROL Predicato proprietà] supporta le ricerche di testo per:

      **Espressioni parziali**
Per consentire la ricerca delle risorse mediante espressioni parziali nel predicato delle proprietà, abilita la casella di controllo **[!UICONTROL Ricerca parziale]** in Modulo di ricerca.\
      Questo consente di cercare le risorse desiderate anche senza specificare le parole o espressioni precise usate nei metadati della risorsa.\
      Operazioni disponibili:
      * Specifica una parola presente nella frase cercata nel facet nel pannello Filtri . Ad esempio, se cerchi il termine **climb** (e il predicato Proprietà è mappato alla proprietà [!UICONTROL `dc:title`] ), vengono restituite tutte le risorse con la parola **climb** nella frase del titolo.
      * Specificare una parte di una parola da cercare, utilizzando il carattere jolly (*) al posto dei caratteri rimanenti.
Ad esempio, se cerchi:
         * **climb*** restituisce tutte le risorse con parole che iniziano con i caratteri &quot;climb&quot; nella frase del titolo.
         * ***** climbrestituisce tutte le risorse con parole che terminano con caratteri &quot;climb&quot; nella frase del titolo.
         * ***climb*** restituisce tutte le risorse con parole contenenti i caratteri &quot;climb&quot; nella frase del titolo.

Per consentire una ricerca senza distinzione tra maiuscole e minuscole nel predicato delle proprietà, abilita il       **Testo senza distinzione tra maiuscole e minuscolePer consentire la ricerca senza distinzione tra maiuscole e minuscole nel predicato delle proprietà, abilitare la casella di controllo**
Ignora  **** maiuscole in Modulo di ricerca. Per impostazione predefinita, la ricerca di testo nel predicato delle proprietà fa distinzione tra maiuscole e minuscole.
   >[!NOTE]
   >
   >Selezionando la casella di controllo **[!UICONTROL Ricerca parziale]**, per impostazione predefinita viene selezionato **[!UICONTROL Ignora maiuscole/minuscole]**.

   ![](assets/wildcard-prop-1.png)

   I risultati della ricerca vengono visualizzati in base ai filtri applicati, insieme al conteggio dei risultati della ricerca.

   ![](assets/omnisearch-with-filters.png)

   Risultato della ricerca di risorse con conteggio dei risultati della ricerca.

1. È possibile spostarsi facilmente su un elemento dal risultato della ricerca e tornare allo stesso risultato utilizzando il pulsante Indietro del browser senza dover ripetere la query di ricerca.

## Salva le ricerche come raccolta avanzata {#save-your-searches-as-smart-collection}

È possibile salvare le impostazioni di ricerca come raccolta avanzata per poter ripetere rapidamente la stessa ricerca senza dover ripristinare le stesse impostazioni in un secondo momento.

Per salvare le impostazioni di ricerca come raccolta avanzata:

1. Tocca o fai clic su **[!UICONTROL Salva raccolta avanzata]** e specifica un nome per la raccolta avanzata.

   Per rendere la raccolta avanzata accessibile a tutti gli utenti, seleziona **[!UICONTROL Public]**. Un messaggio conferma che la raccolta avanzata è stata creata e aggiunta all’elenco delle ricerche salvate.

   >[!NOTE]
   >
   >Agli utenti non amministratori può essere impedito di rendere pubbliche le raccolte avanzate, per evitare di avere un numero enorme di raccolte avanzate pubbliche create da utenti non amministratori su Brand Portal dell’organizzazione. Le organizzazioni possono disattivare la configurazione **[!UICONTROL Consenti creazione raccolte avanzate pubbliche]** dalle impostazioni **[!UICONTROL Generale]** disponibili nel pannello strumenti di amministrazione.

   ![](assets/save_smartcollectionui.png)

1. Per salvare la raccolta avanzata con un nome diverso e selezionare o deselezionare la casella di controllo **[!UICONTROL Public]**, fare clic su **[!UICONTROL Edit Smart Collection]**.

   ![](assets/edit_smartcollection.png)

1. Nella finestra di dialogo **[!UICONTROL Modifica raccolta avanzata]**, selezionare **[!UICONTROL Salva con nome]** e immettere un nome per la raccolta avanzata. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/saveas_smartsearch.png)
