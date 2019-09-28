---
title: Utilizzare facet di ricerca personalizzati
seo-title: Utilizzare facet di ricerca personalizzati
description: Gli amministratori possono aggiungere i predicati di ricerca al pannello Filtri per personalizzare la ricerca e rendere versatile la funzionalità di ricerca.
seo-description: Gli amministratori possono aggiungere i predicati di ricerca al pannello Filtri per personalizzare la ricerca e rendere versatile la funzionalità di ricerca.
uuid: 986fba5a-face5-4128-ac75-d04da5b52d45
content-type: riferimento
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Utilizzare facet di ricerca personalizzati {#use-custom-search-facets}

Gli amministratori possono aggiungere i predicati di ricerca al pannello [!UICONTROL Filtri] per personalizzare la ricerca e rendere versatile la funzionalità di ricerca.

Brand Portal supporta la ricerca [](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) sfaccettata per ricerche granulari di risorse di marchio approvate, che è possibile grazie al pannello [**** Filtri](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). I facet di ricerca sono disponibili nel pannello Filtri tramite **[!UICONTROL Modulo]** di ricerca negli strumenti di amministrazione. Un modulo di ricerca predefinito denominato Barra di ricerca Amministratore risorse esiste nella pagina Moduli di ricerca negli strumenti di amministrazione. Tuttavia, gli amministratori possono personalizzare il pannello Filtri predefinito modificando il modulo di ricerca predefinito (Barra di ricerca Amministratore risorse) aggiungendo, modificando o rimuovendo i predicati di ricerca, rendendo così versatile la funzionalità di ricerca.

Potete usare vari predicati di ricerca per personalizzare il pannello **[!UICONTROL Filtri]** . Ad esempio, aggiungete il predicato delle proprietà per cercare le risorse che corrispondono a una singola proprietà specificata in questo predicato. Aggiungete il predicato delle opzioni per cercare le risorse che corrispondono a uno o più valori specificati per una particolare proprietà. Aggiungi il predicato dell’intervallo di date per cercare le risorse create entro un intervallo di date specificato.

>[!NOTE]
>
>AEM consente alle organizzazioni di [pubblicare i moduli di ricerca personalizzati da AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) al Portale del marchio, invece di ricreare lo stesso modulo sul Portale del marchio.

## Aggiunta di un predicato di ricerca {#add-a-search-predicate}

Per aggiungere un predicato di ricerca al pannello **[!UICONTROL Filtri]** :

1. Per accedere agli strumenti amministrativi, fai clic sul logo AEM nella barra degli strumenti nella parte superiore.

   ![](assets/aemlogo.png)

1. Dal pannello degli strumenti di amministrazione, fare clic su **[!UICONTROL Cerca in moduli]**.

   ![](assets/navigation-panel-1.png)

1. Nella pagina **[!UICONTROL Moduli]** di ricerca, seleziona Barra di ricerca Amministratore **[!UICONTROL risorse]**.

   ![](assets/search-forms-page.png)

1. Sulla barra degli strumenti visualizzata nella parte superiore, fare clic su **[!UICONTROL Modifica]** per aprire il modulo di ricerca per la modifica.

   ![](assets/edit-search-form-1.png)

1. Nella pagina [!UICONTROL Modifica modulo] di ricerca, trascinate un predicato dalla scheda [!UICONTROL Seleziona predicato] al riquadro principale. Ad esempio, trascinare Predicato **[!UICONTROL proprietà]**.

   Il campo **[!UICONTROL Proprietà]** viene visualizzato nel riquadro principale e la scheda **[!UICONTROL Impostazioni]** a destra visualizza i predicati delle proprietà.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >L'etichetta dell'intestazione nella scheda **[!UICONTROL Impostazioni]** identifica il tipo di predicato selezionato.

1. Nella scheda **[!UICONTROL Impostazioni]** , inserite un'etichetta, un testo segnaposto e una descrizione per il predicato delle proprietà.

   * Selezionate Ricerca **** parziale per consentire la ricerca parziale di frasi (e di caratteri jolly) in base al valore di proprietà specificato. Per impostazione predefinita, il predicato supporta la ricerca full-text.
   * Selezionate **[!UICONTROL Ignora maiuscole/minuscole]** se desiderate che la ricerca delle risorse basata sul valore della proprietà non faccia distinzione tra maiuscole e minuscole. Per impostazione predefinita, la ricerca di valori di proprietà nel filtro di ricerca fa distinzione tra maiuscole e minuscole.
   >[!NOTE]
   >
   >Selezionando la casella di controllo **[!UICONTROL Ricerca]** parziale, per impostazione predefinita viene selezionato [!UICONTROL Ignora maiuscole/minuscole] .

1. Nel campo Nome  proprietà, aprite il selettore delle proprietà e selezionate la proprietà in base alla quale viene eseguita la ricerca. In alternativa, immettere un nome per la proprietà. Ad esempio, immettere [!UICONTROL `  jcr :content/metadata/dc:title`] o [!UICONTROL `./jcr:content/metadata/dc:title`].

   ![](assets/title-prop.png)

1. Fate clic su **[!UICONTROL Fine]** per salvare le impostazioni.
1. Dall’interfaccia utente [!UICONTROL Risorse] , fate clic sull’icona della sovrapposizione e scegliete **[!UICONTROL Filtro]** per passare al pannello **[!UICONTROL Filtri]** . Il predicato **[!UICONTROL Property]** viene aggiunto al pannello.

   ![](assets/property-filter-panel.png)

1. Immettete un titolo per la risorsa da cercare nella casella di testo **[!UICONTROL Proprietà]** . Ad esempio, "Adobe". Quando eseguite una ricerca, nei risultati della ricerca vengono visualizzate le risorse il cui titolo corrisponde a "Adobe".

## Elenco dei predicati di ricerca {#list-of-search-predicates}

Analogamente al modo in cui aggiungete un predicato **[!UICONTROL Proprietà]** , potete aggiungere i seguenti predicati al pannello **[!UICONTROL Filtri]** :

| **Nome predicato** | **Descrizione** | **Proprietà** |
|-------|-------|----------|
| [!UICONTROL Browser Percorsi] | Cercare il predicato per cercare le risorse in una determinata posizione. **** Nota: *Per un utente connesso, il browser Percorsi su Filtro mostra solo la struttura del contenuto delle cartelle (e dei relativi predecessori) condivise con l'utente.* Gli utenti <br> amministratori possono cercare le risorse in qualsiasi cartella accedendo a tale cartella utilizzando il browser Percorso. <br> Tuttavia, gli utenti non amministratori possono cercare le risorse in una cartella (accessibile a loro) spostandosi in tale cartella nel browser Percorso. | <ul><li>Etichetta campo</li><li>Percorso</li><li>Descrizione</li></ul> |
| [!UICONTROL Proprietà] | Cercare le risorse in base a una particolare proprietà di metadati. **** Nota: Se si *seleziona Ricerca parziale, per impostazione predefinita* viene selezionata l’opzione Ignora maiuscole/minuscole. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Ricerca parziale</li><li>Ignora maiuscole/minuscole</li><li> Descrizione</li></ul> |
| [!UICONTROL Multi-valore, proprietà] | Simile al predicato delle proprietà, ma consente più valori di input, separati da un delimitatore (l'impostazione predefinita è COMMA[,]), le risorse corrispondenti a qualsiasi valore di input vengono restituite nei risultati. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Supporto delimitatore</li><li>Ignora maiuscole/minuscole</li><li>Descrizione</li></ul> |
| [!UICONTROL Tag] | Cercare il predicato per cercare le risorse in base ai tag. È possibile configurare la proprietà Path per compilare vari tag nell'elenco Tag. *Nota: Gli amministratori potrebbero dover modificare il valore del percorso, ad esempio [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`], se pubblicano il modulo di ricerca da AEM, dove il percorso non include informazioni sul tenant, ad esempio [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Percorso</li><li>Descrizione</li></ul> |
| [!UICONTROL Percorso] | Cercare il predicato per cercare le risorse in una determinata posizione. | <ul><li>Etichetta campo</li><li>Percorso</li><li>Descrizione</li></ul> |  |
| [!UICONTROL Data relativa] | Consente di cercare le risorse in base alla data relativa della loro creazione. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Data relativa</li></ul> |
| [!UICONTROL Intervallo] | Consente di eseguire ricerche in predicato per cercare risorse all’interno di un intervallo specificato di valori di proprietà. Nel pannello Filtri potete specificare i valori minimi e massimi delle proprietà per l’intervallo. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Intervallo date] | Cerca predicato per cercare le risorse create entro un intervallo specificato per una proprietà data. Nel pannello Filtri, potete specificare le date di inizio e fine. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Testo intervallo (Da)</li><li>Testo intervallo (A)</li><li>Descrizione</li></ul> |
| [!UICONTROL Data] | Consente di eseguire una ricerca basata sul cursore delle risorse in base a una proprietà data. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Dimensione file] | Cercare un predicato per cercare le risorse in base alla loro dimensione. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Percorso</li><li>Descrizione</li></ul> |
| [!UICONTROL Ultima modifica risorsa] | Consente di eseguire ricerche nelle risorse in base all’ultima data di modifica. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Stato approvazione] | Cercare un predicato per cercare le risorse in base alla proprietà dei metadati di approvazione. Il nome di proprietà predefinito è **dam:status**. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Stato ritiro] | Predicato di ricerca per cercare le risorse in base allo stato di estrazione di una risorsa al momento della pubblicazione da Risorse AEM. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Ritirato da] | Cercare il predicato per cercare le risorse in base all’utente che ha estratto la risorsa. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Stato scadenza] | Cercare il predicato per cercare le risorse in base allo stato di scadenza. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Membro della raccolta] | Cercare un predicato per cercare risorse in base al fatto che una risorsa sia o meno parte di una raccolta. | Descrizione |
| [!UICONTROL Nascosto] | Questo predicato non è esplicitamente visibile agli utenti finali e viene utilizzato per eventuali vincoli nascosti generalmente per limitare il tipo di risultati della ricerca a **dam:Asset**. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |

>[!NOTE]
>
>Non utilizzate **[!UICONTROL Predicato]** opzioni, Predicato **[!UICONTROL stato]** pubblicazione e Predicato **** valutazione, in quanto questi predicati non funzionano in Brand Portal.

## Eliminare un predicato di ricerca {#delete-a-search-predicate}

Per eliminare un predicato di ricerca, effettuate le seguenti operazioni:

1. Fate clic sul logo Adobe per accedere agli strumenti amministrativi.

   ![](assets/aemlogo.png)

1. Dal pannello degli strumenti di amministrazione, fare clic su **[!UICONTROL Cerca in moduli]**.

   ![](assets/navigation-panel-2.png)

1. Nella pagina **[!UICONTROL Moduli]** di ricerca, seleziona Barra di ricerca Amministratore **[!UICONTROL risorse]**.

   ![](assets/search-forms-page.png)

1. Sulla barra degli strumenti visualizzata nella parte superiore, fare clic su **[!UICONTROL Modifica]** per aprire il modulo di ricerca per la modifica.

   ![](assets/edit-search-form-2.png)

1. Nella pagina [!UICONTROL Modifica modulo] di ricerca, selezionate il predicato da eliminare dal riquadro principale. Ad esempio, selezionare Predicato **[!UICONTROL proprietà]**.

   Nella scheda **[!UICONTROL Impostazioni]** a destra sono visualizzati i campi di predicato delle proprietà.

1. Per eliminare il predicato delle proprietà, fate clic sull'icona bin. Nella finestra di dialogo **[!UICONTROL Elimina campo]** , fare clic su **[!UICONTROL Elimina]** per confermare l’eliminazione.

   Il campo Predicato **** proprietà viene rimosso dal riquadro principale e la scheda **[!UICONTROL Impostazioni]** diventa vuota.

   ![](assets/search-form-delete-predicate.png)

1. Per salvare le modifiche, fate clic su **[!UICONTROL Fine]** nella barra degli strumenti.
1. Dall’interfaccia utente **[!UICONTROL Risorse]** , fate clic sull’icona della sovrapposizione e scegliete **[!UICONTROL Filtro]** per passare al pannello **[!UICONTROL Filtri]** . Il **[!UICONTROL predicato Proprietà]** viene rimosso dal pannello.

   ![](assets/property-predicate-removed.png)
