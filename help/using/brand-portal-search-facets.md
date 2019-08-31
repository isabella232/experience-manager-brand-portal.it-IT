---
title: Utilizzare facet di ricerca personalizzati
seo-title: Utilizzare facet di ricerca personalizzati
description: Gli amministratori possono aggiungere predicati di ricerca al pannello Filtri per personalizzare la ricerca e rendere la funzionalità di ricerca versatile.
seo-description: Gli amministratori possono aggiungere predicati di ricerca al pannello Filtri per personalizzare la ricerca e rendere la funzionalità di ricerca versatile.
uuid: 986 fba 5 a-fac 5-4128-ac 75-d 04 da 5 b 52 d 45
content-type: riferimento
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 19 faa 028-246 b -42 c 7-869 f -97 c 95 c 7 a 1349
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Utilizzare facet di ricerca personalizzati {#use-custom-search-facets}

Gli amministratori possono aggiungere predicati di ricerca al [!UICONTROL pannello Filtri] per personalizzare la ricerca e rendere la funzionalità di ricerca versatile.

Brand Portal supporta [ricerche granulari](../using/brand-portal-searching.md#search-using-facets-in-filters-panel) per le risorse di marchio approvate, che è possibile a causa del pannello [**Filtri**](../using/brand-portal-searching.md#search-using-facets-in-filters-panel). I facet di ricerca sono disponibili nel pannello Filtri tramite **[!UICONTROL il modulo Ricerca]** negli strumenti di amministrazione. Nella pagina Moduli di ricerca in Strumenti di amministrazione è presente un modulo di ricerca denominato Asset Admin Search Rail. Tuttavia, gli amministratori possono personalizzare il pannello Filtri predefiniti modificando il modulo di ricerca predefinito (Barra di ricerca Risorse amministratore) aggiungendo, modificando o rimuovendo predicati di ricerca, rendendo la funzionalità di ricerca versatile.

Potete usare vari predicati di ricerca per personalizzare il **[!UICONTROL pannello Filtri]** . Ad esempio, aggiungere la predicato di proprietà per cercare risorse che corrispondono a una singola proprietà specificata in questa predicato. Aggiungete la predicato delle opzioni per cercare le risorse che corrispondono a uno o più valori specificati per una particolare proprietà. Aggiungi l'predicato di date per cercare le risorse create in un intervallo date specificato.

>[!NOTE]
>
>AEM consente alle organizzazioni [di pubblicare moduli di ricerca personalizzati da AEM Author](../using/publish-schema-search-facets-presets.md#publish-search-facets-to-brand-portal) a Brand Portal, anziché ricreare lo stesso modulo su Brand Portal.

## Aggiungere un predicato di ricerca {#add-a-search-predicate}

Per aggiungere un predicato di ricerca al **[!UICONTROL pannello Filtri]** :

1. Per accedere agli strumenti di amministrazione, fai clic sul logo AEM dalla barra degli strumenti nella parte superiore.

   ![](assets/aemlogo.png)

2. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Cerca moduli]**.

   ![](assets/navigation-panel-1.png)

3. Nella pagina **[!UICONTROL Moduli]** di ricerca, seleziona **[!UICONTROL Barra di ricerca Amministrazione risorse]**.

   ![](assets/search-forms-page.png)

4. Nella barra degli strumenti visualizzata in alto, fate clic **[!UICONTROL su Modifica]** per aprire il modulo di ricerca di modifica.

   ![](assets/edit-search-form-1.png)

5. Nella pagina [!UICONTROL Modifica modulo] di ricerca, trascinare un predicato dalla scheda [!UICONTROL Seleziona predicato] nel riquadro principale. Ad esempio, trascinare **[!UICONTROL Predicato proprietà]**.

   Il **[!UICONTROL campo Proprietà]** viene visualizzato nel riquadro principale e nella **[!UICONTROL scheda Impostazioni]** a destra sono visualizzati i predicati delle proprietà.

   ![](assets/partial-prop-predicate.png)

   >[!NOTE]
   >
   >L'etichetta dell'intestazione nella scheda **[!UICONTROL Impostazioni]** identifica il tipo di predicato selezionato.

6. Nella scheda **[!UICONTROL Impostazioni]** , immettete un'etichetta, un testo segnaposto e una descrizione per il predicato della proprietà.

   * Selezionate **[!UICONTROL Ricerca]** parziale, se desiderate consentire la ricerca parziale delle frasi (ricerca con caratteri jolly) in base al valore della proprietà specificata. Per impostazione predefinita, il predicato supporta la ricerca full-text.
   * Selezionate **[!UICONTROL Ignora caso]**, se desiderate che la ricerca delle risorse in base al valore della proprietà sia senza distinzione tra maiuscole e minuscole. Per impostazione predefinita, la ricerca di valori delle proprietà nel filtro di ricerca fa distinzione tra maiuscole e minuscole.
   >[!NOTE]
   >
   >Selezionando la **[!UICONTROL casella di]** controllo Ricerca parziale, [!UICONTROL Ignora caso] è selezionato per impostazione predefinita.

7. Nel campo [!UICONTROL Nome] proprietà, aprire il selettore proprietà e selezionare la proprietà in base alla quale viene eseguita la ricerca. In alternativa, immettete un nome per la proprietà. Ad esempio, immettete [!UICONTROL `  jcr :content/metadata/dc:title`] o [!UICONTROL `./jcr:content/metadata/dc:title`].

   ![](assets/title-prop.png)

8. Fate clic su **[!UICONTROL Fine]** per salvare le impostazioni.
9. Nell' [!UICONTROL interfaccia] utente di Risorse, fai clic sull'icona della sovrapposizione e scegli **[!UICONTROL Filtro]** per passare al **[!UICONTROL pannello Filtri]** . Il predicato **[!UICONTROL Proprietà]** viene aggiunto al pannello.

   ![](assets/property-filter-panel.png)

10. Inserite un titolo per la risorsa da cercare nella casella **[!UICONTROL di]** testo Proprietà. Ad esempio, "Adobe". Quando eseguite una ricerca, nei risultati della ricerca vengono visualizzate le risorse con il titolo corrispondente ad «Adobe».

## Elenco dei predicati di ricerca {#list-of-search-predicates}

Simile al modo in cui aggiungete un **[!UICONTROL predicato Proprietà]** , potete aggiungere i seguenti predefiniti al pannello **[!UICONTROL Filtri]** :

| **Predicato nome** | **Descrizione** | **Proprietà** |
|-------|-------|----------|
| [!UICONTROL Browser Percorsi] | Cerca di cercare le risorse in una determinata posizione. **Nota:***Per un utente connesso, il browser Percorsi sul filtro mostra solo la struttura del contenuto delle cartelle (e dei relativi predecessori) condivise con l'utente.*<br> Gli utenti Admin possono cercare le risorse in qualsiasi cartella accedendo alla cartella utilizzando Browser Percorsi. <br> Tuttavia, gli utenti non amministratori possono cercare le risorse in una cartella (ad accesso facilitato) accedendo a quella cartella nel browser Percorsi. | <ul><li>Etichetta campo</li><li>Percorso</li><li>Descrizione</li></ul> |
| [!UICONTROL Proprietà] | Cercare le risorse in base a una particolare proprietà di metadati. **Nota:***Selezionando Cerca parziale, Ignora caso è selezionato per impostazione predefinita*. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Ricerca parziale</li><li>Ignora maiuscole/minuscole</li><li> Descrizione</li></ul> |
| [!UICONTROL Proprietà con più valori] | Analogamente alla predicato della proprietà, ma consente più valori di input, separati da un carattere di delimitazione (il valore predefinito è COMMA[,]) le risorse che corrispondono a qualsiasi valore immesso vengono restituite nei risultati. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Supporto delimitatore</li><li>Ignora maiuscole/minuscole</li><li>Descrizione</li></ul> |
| [!UICONTROL Tag] | Cerca di cercare le risorse in base ai tag. È possibile configurare la proprietà Percorso per compilare vari tag nell'elenco Tag. * Nota: Gli amministratori potrebbero dover modificare il valore del percorso, ad esempio, [!UICONTROL `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`]se pubblicano il modulo di ricerca da AEM, ad esempio, se il percorso non include informazioni tenant [!UICONTROL `/etc/tags/<custom_tag_namespace>`], ad esempio. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Percorso</li><li>Descrizione</li></ul> |
| [!UICONTROL Percorso] | Cerca di cercare le risorse in una determinata posizione. | <ul><li>Etichetta campo</li><li>Percorso</li><li>Descrizione</li></ul> |  |
| [!UICONTROL Data relativa] | Cerca di cercare le risorse in base alla data relativa della creazione. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Data relativa</li></ul> |
| [!UICONTROL Intervallo] | Cerca di cercare le risorse che si trovano entro una gamma specificata di valori delle proprietà. Nel pannello Filtri, potete specificare valori minimi e massimi delle proprietà per l'intervallo. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Intervallo date] | Cerca di cercare le risorse create entro un intervallo specificato per una proprietà data. Nel pannello Filtri, potete specificare le date di inizio e fine. | <ul><li>Etichetta campo</li><li>Segnaposto</li><li>Nome proprietà</li><li>Testo intervallo (Da)</li><li>Testo intervallo (A)</li><li>Descrizione</li></ul> |
| [!UICONTROL Data] | Predicato di ricerca per una ricerca basata su cursori basata su una proprietà data. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Dimensione file] | Cerca di cercare le risorse in base alle loro dimensioni. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Percorso</li><li>Descrizione</li></ul> |
| [!UICONTROL Ultima modifica risorsa] | Cerca di cercare le risorse in base alla data dell'ultima modifica. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Stato approvazione] | Cerca di cercare le risorse in base alla proprietà di metadati di approvazione. Il nome della proprietà predefinita è **dam: status**. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Stato ritiro] | Cerca di cercare le risorse in base allo stato di ritiro di una risorsa pubblicata da Risorse AEM. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Ritirato da] | Cerca di cercare le risorse in base all'utente che ha ritirato la risorsa. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Stato scadenza] | Cerca di cercare le risorse in base allo stato di scadenza. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |
| [!UICONTROL Membro della raccolta] | Cerca di cercare le risorse in base al fatto che una risorsa sia parte di una raccolta. | Descrizione |
| [!UICONTROL Nascosto] | Questo predicato non è esplicitamente visibile agli utenti finali e viene utilizzato per eventuali vincoli nascosti in genere per limitare i risultati di ricerca a **DAM: Risorsa**. | <ul><li>Etichetta campo</li><li>Nome proprietà</li><li>Descrizione</li></ul> |

>[!NOTE]
>
>Non utilizzate **[!UICONTROL Predicato opzioni]**, **[!UICONTROL Predicato stato pubblicazione]** e Predicato **[!UICONTROL valutazione]** , poiché questi predicati non funzioneranno in Brand Portal.

## Eliminare un predicato di ricerca {#delete-a-search-predicate}

Per eliminare una predicato di ricerca, effettuate le seguenti operazioni:

1. Fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

2. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Cerca moduli]**.

   ![](assets/navigation-panel-2.png)

3. Nella pagina **[!UICONTROL Moduli]** di ricerca, seleziona **[!UICONTROL Barra di ricerca Amministrazione risorse]**.

   ![](assets/search-forms-page.png)

4. Nella barra degli strumenti visualizzata in alto, fate clic **[!UICONTROL su Modifica]** per aprire il modulo di ricerca di modifica.

   ![](assets/edit-search-form-2.png)

5. Nella pagina [!UICONTROL Modifica modulo] di ricerca, selezionare la predicato da eliminare dal riquadro principale. Ad esempio, selezionare **[!UICONTROL Predicato proprietà]**.

   Nella **[!UICONTROL scheda Settings]** (Impostazioni) a destra sono visualizzati i campi predicato delle proprietà.

6. Per eliminare il predicato della proprietà, fate clic sull'icona del raccoglitore. Nella finestra **[!UICONTROL di]** dialogo Elimina campo, fare clic su **[!UICONTROL Elimina]** per confermare l'azione di eliminazione.

   Il campo **[!UICONTROL Predicato]** proprietà viene rimosso dal riquadro principale e la scheda **[!UICONTROL Impostazioni]** viene lasciata vuota.

   ![](assets/search-form-delete-predicate.png)

7. Per salvare le modifiche, fate clic su **[!UICONTROL Fine]** nella barra degli strumenti.
8. Nell' **[!UICONTROL interfaccia]** utente di Risorse, fai clic sull'icona della sovrapposizione e scegli **[!UICONTROL Filtro]** per passare al **[!UICONTROL pannello Filtri]** . Il predicato **[!UICONTROL Proprietà]** viene rimosso dal pannello.

   ![](assets/property-predicate-removed.png)
