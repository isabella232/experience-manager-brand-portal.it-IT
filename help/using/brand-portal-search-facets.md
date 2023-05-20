---
title: Utilizzare i facet di ricerca personalizzati
seo-title: Use custom search facets
description: Gli amministratori possono aggiungere predicati di ricerca al pannello Filtri per personalizzare la ricerca e renderla versatile.
seo-description: Administrators can add search predicates to the Filters panel to customize search and make the search functionality versatile.
uuid: 986fba5a-fac5-4128-ac75-d04da5b52d45
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 19faa028-246b-42c7-869f-97c95c7a1349
role: Admin
exl-id: c07e1268-2c83-40ba-8dcd-5dade3a10141
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1279'
ht-degree: 10%

---

# Utilizzare i facet di ricerca personalizzati {#use-custom-search-facets}

Gli amministratori possono aggiungere predicati di ricerca al [!UICONTROL Filtri] per personalizzare la ricerca e rendere versatile la funzionalità di ricerca.

Brand Portal supporta [ricerca sfaccettata](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) per ricerche granulari delle risorse del brand approvate, che è possibile grazie a [**Filtri** pannello](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). I facet di ricerca sono disponibili nel pannello Filtri tramite **[!UICONTROL Modulo di ricerca]** negli strumenti di amministrazione. Un modulo di ricerca predefinito denominato Barra di ricerca amministrazione risorse è disponibile nella pagina Cerca in Forms degli strumenti di amministrazione. Tuttavia, gli amministratori possono personalizzare il pannello Filtri predefinito modificando il modulo di ricerca predefinito (Barra di ricerca amministrazione risorse) aggiungendo, modificando o rimuovendo i predicati di ricerca, rendendo così versatile la funzionalità di ricerca.

Puoi utilizzare vari predicati di ricerca per personalizzare **[!UICONTROL Filtri]** pannello. Ad esempio, aggiungi il predicato proprietà per cercare le risorse che corrispondono a una singola proprietà specificata in questo predicato. Aggiungi il predicato options per cercare le risorse che corrispondono a uno o più valori specificati per una particolare proprietà. Aggiungi il predicato dell’intervallo di date per cercare le risorse create all’interno di un intervallo di date specificato.

>[!NOTE]
>
>Experience Manager Assets consente alle organizzazioni di [pubblicare i moduli di ricerca personalizzati da AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) in Brand Portal, invece di ricreare lo stesso modulo in Brand Portal.

## Aggiungere un predicato di ricerca {#add-a-search-predicate}

Per aggiungere un predicato di ricerca al **[!UICONTROL Filtri]** pannello:

1. Per accedere agli strumenti di amministrazione, fai clic sul logo dell’Experience Manager nella barra degli strumenti in alto.

   ![](assets/aemlogo.png)

1. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Cerca in Forms]**.

   ![](assets/navigation-panel-1.png)

1. In **[!UICONTROL Cerca in Forms]** pagina, seleziona **[!UICONTROL Barra di ricerca amministrazione risorse]**.

   ![](assets/search-forms-page.png)

1. Sulla barra degli strumenti visualizzata nella parte superiore, fai clic su **[!UICONTROL Modifica]** per aprire il modulo modifica ricerca.

   ![](assets/edit-search-form-1.png)

1. In [!UICONTROL Modifica modulo di ricerca] , trascinare un predicato dalla [!UICONTROL Seleziona predicato] al riquadro principale. Ad esempio, trascina **[!UICONTROL Predicato proprietà]**.

   Il **[!UICONTROL Proprietà]** viene visualizzato nel riquadro principale e nel **[!UICONTROL Impostazioni]** sulla destra mostra i predicati delle proprietà.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >L’etichetta dell’intestazione nel **[!UICONTROL Impostazioni]** La scheda identifica il tipo di predicato selezionato.

1. In **[!UICONTROL Impostazioni]** , immettere un&#39;etichetta, un testo segnaposto e una descrizione per il predicato proprietà.

   * Seleziona **[!UICONTROL Ricerca parziale]**, se desideri consentire la ricerca parziale per frase (e con caratteri jolly) delle risorse in base al valore della proprietà specificato. Per impostazione predefinita, il predicato supporta la ricerca full-text.
   * Seleziona **[!UICONTROL Ignora maiuscole/minuscole]**, se desideri che la ricerca delle risorse in base al valore della proprietà non faccia distinzione tra maiuscole e minuscole. Per impostazione predefinita, la ricerca dei valori delle proprietà nel filtro di ricerca fa distinzione tra maiuscole e minuscole.

   >[!NOTE]
   >
   >Alla selezione **[!UICONTROL Ricerca parziale]** casella di controllo, **[!UICONTROL Ignora maiuscole/minuscole]** è selezionato per impostazione predefinita.

1. In **[!UICONTROL Nome proprietà]** , aprire il selettore delle proprietà e selezionare la proprietà in base alla quale viene eseguita la ricerca. In alternativa, immettere un nome per la proprietà. Ad esempio, inserisci `  jcr :content/metadata/dc:title` o `./jcr:content/metadata/dc:title`.

   >[!NOTE]
   >
   >In Brand Portal, tutte le proprietà (eccetto quelle che iniziano con `xmp`) in `jcrcontent/metadata` di `dam:asset` sono indicizzati per impostazione predefinita.
   >
   >Qualsiasi proprietà indicizzata può essere utilizzata durante la creazione di un predicato di proprietà. Se è configurata una proprietà non indicizzata, la query di ricerca su una proprietà non indicizzata potrebbe non fornire alcun risultato.

   ![](assets/title-prop.png)

1. Clic **[!UICONTROL Fine]** per salvare le impostazioni.
1. Dalla sezione [!UICONTROL Risorse] interfaccia utente, fai clic sull’icona di sovrapposizione e scegli **[!UICONTROL Filtro]** per passare al **[!UICONTROL Filtri]** pannello. Il **[!UICONTROL Proprietà]** al pannello viene aggiunto il predicato.

   ![](assets/property-filter-panel.png)

1. Immetti un titolo per la risorsa da cercare nella **[!UICONTROL Proprietà]** casella di testo. Ad esempio, &quot;Adobe&quot;. Quando esegui una ricerca, nei risultati vengono visualizzate le risorse il cui titolo corrisponde a &quot;Adobe&quot;.

## Elenco dei predicati di ricerca {#list-of-search-predicates}

Simile alla modalità di aggiunta di un **[!UICONTROL Proprietà]** predicato, è possibile aggiungere i seguenti predicati al **[!UICONTROL Filtri]** pannello:

| **Nome predicato** | **Descrizione** | **Proprietà** |
|-------|-------|----------|
| **[!UICONTROL Browser Percorsi]** | Cerca predicato per cercare le risorse in una posizione particolare. **Nota:** *Per un utente connesso, il browser percorsi sul filtro mostra solo la struttura del contenuto delle cartelle (e dei relativi predecessori) condivise con l’utente.* <br> Gli utenti amministratori possono cercare le risorse in qualsiasi cartella navigando in tale cartella utilizzando il browser Percorsi. <br> Gli utenti non amministratori possono invece cercare le risorse in una cartella (a cui possono accedere) accedendo a tale cartella nel browser percorsi. | <ul><li>Etichetta campo</li><li>Percorso</li><li>Descrizione</li></ul> |
| **[!UICONTROL Proprietà]** | Cerca le risorse in base a una particolare proprietà di metadati. **Nota:** *Quando si seleziona Ricerca parziale, Ignora maiuscole/minuscole è selezionato per impostazione predefinita*. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Ricerca parziale</li><li>Ignora maiuscole/minuscole</li><li> Descrizione</li></ul> |
| **[!UICONTROL Proprietà con più valori]** | Simile al predicato proprietà ma consente più valori di input, separati da un delimitatore (il valore predefinito è VIRGOLA)[,]) le risorse che corrispondono a uno qualsiasi dei valori immessi vengono restituite nei risultati. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Supporto delimitatore</li><li>Ignora maiuscole/minuscole</li><li>Descrizione</li></ul> |
| **[!UICONTROL Tag]** | Cerca predicato per cercare le risorse in base ai tag. È possibile configurare la proprietà Path per compilare vari tag nell&#39;elenco Tag. *Nota: gli amministratori potrebbero dover modificare il valore del percorso, ad esempio [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`], se pubblicano il modulo di ricerca dall’AEM, dove il percorso non include informazioni sul tenant, ad esempio, [!UICONTROL `/etc/tags/<custom_tag_namespace>`]. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Percorso</li><li>Descrizione</li></ul> |
| **[!UICONTROL Percorso]** | Cerca predicato per cercare le risorse in una posizione particolare. | <ul><li>Etichetta campo</li><li>Percorso</li><li>Descrizione</li></ul> |  |
| **[!UICONTROL Data relativa]** | Cerca predicato per cercare le risorse in base alla data relativa di creazione. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Data relativa</li></ul> |
| **[!UICONTROL Intervallo]** | Predicato di ricerca per cercare le risorse che si trovano all’interno di un intervallo specificato di valori di proprietà. Nel pannello Filtri, potete specificare i valori minimi e massimi delle proprietà per l&#39;intervallo. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| **[!UICONTROL Intervallo date]** | Cerca predicato per cercare le risorse create all’interno di un intervallo specificato per una proprietà di data. Nel pannello Filtri puoi specificare le date di inizio e fine. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Testo intervallo (Da)</li><li>Testo intervallo (A)</li><li>Descrizione</li></ul> |
| **[!UICONTROL Data]** | Predicato di ricerca per una ricerca di risorse basata su cursore e basata su una proprietà data. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| **[!UICONTROL Dimensione file]** | Cerca predicato per cercare le risorse in base alle loro dimensioni. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Percorso</li><li>Descrizione</li></ul> |
| **[!UICONTROL Ultima modifica risorsa]** | Cerca predicato per cercare le risorse in base alla data dell’ultima modifica. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| **[!UICONTROL Stato approvazione]** | Cerca predicato per cercare le risorse in base alla proprietà dei metadati di approvazione. Il nome predefinito della proprietà è **dam:status**. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| **[!UICONTROL Stato ritiro]** | Predicato di ricerca per cercare le risorse in base allo stato di check-out di una risorsa quando è stata pubblicata da AEM Assets. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| **[!UICONTROL Ritirato da]** | Predicato di ricerca per cercare le risorse in base all’utente che ha estratto la risorsa. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| **[!UICONTROL Stato scadenza]** | Cerca predicato per cercare le risorse in base allo stato di scadenza. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| **[!UICONTROL Membro di raccolta]** | Predicato di ricerca per cercare le risorse in base al fatto che una risorsa faccia parte di una raccolta. | Descrizione |
| **[!UICONTROL Nascosto]** | Questo predicato non è visibile esplicitamente agli utenti finali e viene utilizzato per qualsiasi vincolo nascosto in genere per limitare il tipo di risultati di ricerca a **dam:Asset**. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |

>[!NOTE]
>
>Non usi **[!UICONTROL Predicato opzioni]**, **[!UICONTROL Predicato di stato pubblicazione]**, e **[!UICONTROL Predicato di valutazione]** poiché questi predicati non sono funzionali in Brand Portal.

## Eliminare un predicato di ricerca {#delete-a-search-predicate}

Per eliminare un predicato di ricerca, eseguire la procedura seguente:

1. Fai clic sul logo dell’Adobe per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

1. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Cerca in Forms]**.

   ![](assets/navigation-panel-2.png)

1. In **[!UICONTROL Cerca in Forms]** pagina, seleziona **[!UICONTROL Barra di ricerca amministrazione risorse]**.

   ![](assets/search-forms-page.png)

1. Sulla barra degli strumenti visualizzata nella parte superiore, fai clic su **[!UICONTROL Modifica]** per aprire il modulo modifica ricerca.

   ![](assets/edit-search-form-2.png)

1. In [!UICONTROL Modifica modulo di ricerca] nel riquadro principale, selezionare il predicato che si desidera eliminare. Ad esempio, seleziona **[!UICONTROL Predicato proprietà]**.

   Il **[!UICONTROL Impostazioni]** sulla destra vengono visualizzati i campi del predicato di proprietà.

1. Per eliminare il predicato della proprietà, fai clic sull’icona del raccoglitore. Il giorno **[!UICONTROL Elimina campo]** , fare clic su **[!UICONTROL Elimina]** per confermare l’azione elimina.

   Il **[!UICONTROL Predicato proprietà]** viene rimosso dal riquadro principale e il **[!UICONTROL Impostazioni]** La scheda diventa vuota.

   ![](assets/search-form-delete-predicate.png)

1. Per salvare le modifiche, fai clic su **[!UICONTROL Fine]** nella barra degli strumenti.
1. Dalla sezione **[!UICONTROL Risorse]** interfaccia utente, fai clic sull’icona di sovrapposizione e scegli **[!UICONTROL Filtro]** per passare al **[!UICONTROL Filtri]** pannello. Il **[!UICONTROL Proprietà]** il predicato viene rimosso dal pannello.

   ![](assets/property-predicate-removed.png)
