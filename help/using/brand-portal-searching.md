---
title: Cercare risorse in Brand Portal
seo-title: Ricerca di risorse e ricerca salvata su AEM Brand Portal
description: La funzione di ricerca Brand Portal consente di cercare rapidamente risorse rilevanti utilizzando la ricerca globale e i filtri di ricerca consentono di limitare ulteriormente la ricerca. Salvate le ricerche come raccolte intelligenti per il futuro.
seo-description: La funzione di ricerca Brand Portal consente di cercare rapidamente risorse rilevanti utilizzando la ricerca globale e i filtri di ricerca consentono di limitare ulteriormente la ricerca. Salvate le ricerche come raccolte intelligenti per il futuro.
uuid: c2955198-bdc0-4853-a13a-661e6a9ec61f
contentOwner: bdhar
content-type: riferimento
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: SearchandPromote
discoiquuid: dc751cd7-f663-46d2-84c4-5bb12a4fe1ba
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# Cercare risorse in Brand Portal {#search-assets-on-brand-portal}

La funzione di ricerca Brand Portal consente di cercare rapidamente risorse rilevanti utilizzando la ricerca globale e la ricerca sfaccettata tramite filtri per limitare ulteriormente la ricerca. Potete inoltre salvare le ricerche come raccolte intelligenti per il futuro.

## Ricerca di risorse tramite Omnisearch {#search-assets-using-omnisearch}

Per cercare risorse in Brand Portal:

1. Dalla barra degli strumenti, fate clic sull’icona **[!UICONTROL Cerca]** oppure premete il tasto "**[!UICONTROL /]**" per avviare Omnisearch.

   ![](assets/omnisearchicon-1.png)

1. Nella casella di ricerca, digitate una parola chiave per le risorse da cercare.

   ![](assets/omnisearch.png)

   >[!NOTE]
   >
   >Sono necessari almeno 3 caratteri in omnisearch per visualizzare i suggerimenti di ricerca.

1. Per accedere rapidamente alle risorse pertinenti, potete scegliere tra i suggerimenti correlati visualizzati nell’elenco a discesa.

   ![](assets/assets-search-result.png)

   *Ricerca di risorse tramite omnisearch*

Per informazioni sul comportamento di ricerca con risorse con tag avanzati, consultate [Comprendere i risultati e il comportamento](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-assets.html)di ricerca.

## Ricerca mediante facet nel pannello Filtri {#search-using-facets-in-filters-panel}

I facet di ricerca nel pannello Filtri aggiungono granularità all’esperienza di ricerca e rendono efficiente la funzionalità di ricerca. I facet di ricerca utilizzano più dimensioni (predicati) che consentono di eseguire ricerche complesse. Potete facilmente approfondire fino al livello di dettaglio desiderato per una ricerca più mirata.

Ad esempio, se cercate un’immagine, potete scegliere se un elemento bitmap o un’immagine vettoriale. È possibile ridurre ulteriormente l'ambito della ricerca specificando il tipo MIME per l'immagine nel facet di ricerca Tipo file. Allo stesso modo, quando cercate documenti, potete specificare il formato, ad esempio PDF o Microsoft Word.<br />

![Filters panel in Brand Portal](assets/file-type-search.png "Filters panel in Brand Portal")

Il pannello [!UICONTROL Filtri] include alcuni facet standard, quali: browser percorso, tipo [!UICONTROL di]file, dimensioni file, [!UICONTROL stato]e orientamento. However, you can add custom search facets or remove specific search facets from the Filters panel by adding or removing predicates in the underlying Search Form. [](../using/brand-portal-search-facets.md) See the list of the available and usable search predicates on Brand Portal.[](../using/brand-portal-search-facets.md#list-of-search-predicates)

To apply filters to your search, using the available [search facets](../using/brand-portal-search-facets.md):

1. Click the overlay icon and select Filter.****

   ![](assets/selectorrail.png)

2. From the Filters panel on the left, select the appropriate options to apply the relevant filters.
****
For example, use the following standard filters:

   * **[!UICONTROL Path Browser to search assets in a specific directory.]** The default search path of the predicate for Path Browser is /content/dam/mac/&lt;tenant-id&gt;/, which can be configured by editing the default search form.****
   >[!NOTE]
   >
   >To non-admin users, [!UICONTROL Path Browser] in [!UICONTROL Filter] panel shows only the content structure of the folders (and their ancestor folders) shared with them.\
   >To admin users, Path Browser allows navigating to any folder in Brand Portal.

   * **[!UICONTROL File Type]** to specify the type (image, document, multimedia, archive) of asset file you are looking for. Further, you can narrow down the scope of your search, for example, specify the MIME type (Tiff, Bitmap, GIMP Images) for image or format (PDF or MS Word) for the documents.
   * **[!UICONTROL Dimensione]** file per cercare le risorse in base alle loro dimensioni. È possibile specificare i limiti inferiore e superiore dell'intervallo di dimensioni per limitare la ricerca e specificare l'unità di misura da cercare.
   * **[!UICONTROL Status to search for assets based on asset statuses, such as Approval (Approved, Changes Requested, Rejected, Pending) and Expiration.]**
   * **[!UICONTROL Valutazione]** media per la ricerca di risorse in base al rating delle risorse.
   * **[!UICONTROL Orientamento]** per cercare le risorse in base all’orientamento (orizzontale, verticale, quadrato) delle risorse.
   * **[!UICONTROL Stile]** per cercare risorse in base allo stile (colorato, bianco e nero) delle risorse.
   * **[!UICONTROL Video Format to search for video assets based on their format (DVI, Flash, MPEG4, MPEG, OGG Theora, QuickTime, Windows Media, WebM).]**
   È possibile utilizzare facet [di ricerca](../using/brand-portal-search-facets.md) personalizzati nel pannello Filtri modificando il modulo di ricerca sottostante.

   * **[!UICONTROL Predicato]** proprietà, se utilizzato nel modulo di ricerca, consente di cercare le risorse che corrispondono a una proprietà di metadati a cui è mappato il predicato.\
      Ad esempio, se è stato mappato su Predicato proprietà, potete cercare le risorse in base al relativo titolo. [!UICONTROL `jcr:content /metadata/dc:title`]\
      Il [!UICONTROL Predicato] proprietà supporta le ricerche di testo per:

      **Espressioni parziali**
Per consentire la ricerca delle risorse mediante espressioni parziali nel predicato delle proprietà, abilita la casella di controllo **[!UICONTROL Ricerca parziale]in Modulo di ricerca.**\
      Questo consente di cercare le risorse desiderate anche senza specificare le parole o espressioni precise usate nei metadati della risorsa.\
      È possibile:
* Specificate una parola che si verifica nella frase cercata nel facet nel pannello Filtri. For example, if you search for the term **climb** (and Property Predicate is mapped to [!UICONTROL `dc:title`] property), then all the assets with the word **climb** in their title phrase are returned.
* Specificare una parte di una parola da cercare, utilizzando il carattere jolly (*) al posto dei caratteri rimanenti.
Ad esempio, se cerchi:
      **climb*** restituisce tutte le risorse con parole che iniziano con i caratteri "climb" nella frase del titolo.
      ***climb** restituisce tutte le risorse con parole che terminano con caratteri "climb" nella frase del titolo.
      ***climb*** restituisce tutte le risorse con parole contenenti i caratteri "climb" nella frase del titolo.\
      **Testo** senza distinzione tra maiuscole e minuscole Per consentire ricerche senza distinzione tra maiuscole e minuscole nel predicato delle proprietà, abilitare la casella di controllo **[!UICONTROL Ignora maiuscole]** nel modulo di ricerca. Per impostazione predefinita, la ricerca di testo nel predicato delle proprietà fa distinzione tra maiuscole e minuscole.
   >[!NOTE]
   >
   >Selezionando la casella di controllo **[!UICONTROL Ricerca]** parziale, per impostazione predefinita viene selezionato [!UICONTROL Ignora maiuscole/minuscole] .

   ![](assets/wildcard-prop-1.png)

   I risultati della ricerca vengono visualizzati in base ai filtri applicati, insieme al conteggio dei risultati della ricerca.

   ![](assets/omnisearch-with-filters.png)

   Risultato della ricerca delle risorse con il conteggio dei risultati della ricerca

3. È possibile individuare facilmente un elemento dal risultato della ricerca e tornare allo stesso risultato utilizzando il pulsante Indietro del browser senza dover ripetere la query di ricerca.

## Salvate le ricerche come raccolta avanzata {#save-your-searches-as-smart-collection}

Potete salvare le impostazioni di ricerca come una raccolta intelligente per poter ripetere rapidamente la stessa ricerca senza dover ripristinare le stesse impostazioni in un secondo momento.

Per salvare le impostazioni di ricerca come raccolta dinamica:

1. Toccate o fate clic su **[!UICONTROL Salva raccolta]** avanzata e specificate un nome per la raccolta dinamica.

   Per rendere la raccolta intelligente accessibile a tutti gli utenti, selezionate **[!UICONTROL Pubblico]**. Un messaggio conferma che la raccolta smart è stata creata e aggiunta all'elenco delle ricerche salvate.

   >[!NOTE]
   >
   >Agli utenti non amministratori può essere impedito di rendere pubbliche le raccolte smart, per evitare che un numero enorme di raccolte pubbliche intelligenti create da utenti non amministratori nel Portale marchio dell'organizzazione. Le organizzazioni possono disattivare la configurazione **[!UICONTROL Consenti creazione]** raccolte smart pubbliche dalle impostazioni **[!UICONTROL Generali]** disponibili nel pannello degli strumenti di amministrazione.

   ![](assets/save_smartcollectionui.png)

2. Per salvare la raccolta dinamica con un nome diverso e selezionare o deselezionare la casella di controllo **[!UICONTROL Pubblica]** , fate clic su **[!UICONTROL Modifica raccolta]** avanzata.

   ![](assets/edit_smartcollection.png)

3. Nella finestra di dialogo **[!UICONTROL Modifica raccolta]** avanzata, selezionate **[!UICONTROL Salva con nome]** e immettete un nome per la raccolta dinamica. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/saveas_smartsearch.png)
