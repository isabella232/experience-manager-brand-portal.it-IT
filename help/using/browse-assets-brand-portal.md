---
title: Sfogliare le risorse su Brand Portal
seo-title: Sfogliare le risorse su Brand Portal
description: Sfogliate le risorse, incrociate le gerarchie di risorse ed effettuate ricerche nelle risorse, utilizzando diverse opzioni di visualizzazione ed elementi dell'interfaccia utente nel Brand Portal.
seo-description: Sfogliate le risorse, incrociate le gerarchie di risorse ed effettuate ricerche nelle risorse, utilizzando diverse opzioni di visualizzazione ed elementi dell'interfaccia utente nel Brand Portal.
uuid: 178ce217-0050-4922-a204-f4539d46f539
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: introduction
discoiquuid: a70ce694-81d1-4829-9e61-b6412e013e5c
translation-type: tm+mt
source-git-commit: ca60fe1b76c6e99d835457627fcc4bf402b6bd87
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 4%

---


# Sfogliare le risorse sul Portale marchio {#browsing-assets-on-brand-portal}

 AEM Assets Brand Portal offre diverse funzionalità ed elementi dell’interfaccia utente che semplificano la navigazione tra le risorse, l’attraversamento delle gerarchie di risorse e la ricerca delle risorse utilizzando diverse opzioni di visualizzazione.

AEM logo nella barra degli strumenti AEM nella parte superiore facilita l’accesso degli utenti amministratori al pannello degli strumenti amministrativi.

![](assets/aemlogo.png)

![](assets/admin-tools-panel-2.png)

![](assets/bp_subheader.png)<br />

Il selettore della barra in alto a sinistra nel Portale marchio viene visualizzato a discesa per mostrare le opzioni che consentono di navigare nelle gerarchie delle risorse, semplificare la ricerca e visualizzare le risorse.

![](assets/siderail-1.png)

Potete visualizzare, navigare e selezionare le risorse utilizzando una delle viste disponibili (Scheda, Colonna ed Elenco) nel selettore di visualizzazione in alto a destra in Brand Portal.

![](assets/viewselector.png)

## Visualizzazione e selezione delle risorse {#viewing-and-selecting-resources}

In tutte le viste la visualizzazione, la navigazione e la selezione funzionano allo stesso modo, ma con lievi variazioni a seconda della vista in uso.

Puoi visualizzare, navigare e selezionare (per ulteriori azioni) le risorse con una delle viste disponibili:

* Vista a colonne
* Vista a schede
* Vista a elenco 

### Vista a schede

![](assets/card-view.png)

La vista a schede mostra schede informative per ogni elemento al livello corrente, Queste schede forniscono i seguenti dettagli:

* Una rappresentazione visiva della risorsa o della cartella.
* Tipo
* Titolo
* Nome
* Data e ora in cui la risorsa è stata pubblicata su Brand Portal da AEM
* Dimensione
* Dimensioni

Per navigare verso il basso nella gerarchia, toccate o fate clic sulle schede (facendo attenzione a evitare le azioni rapide) oppure risalite utilizzando le [breadcrumb nell&#39;intestazione](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

![](assets/cardquickactions.png)

#### Vista a schede per utenti non amministratori

Schede di cartelle, nella vista a schede, visualizzate le informazioni sulla gerarchia delle cartelle per utenti non amministratori (Editor, Visualizzatore e Utente ospite). Questa funzionalità consente agli utenti di conoscere la posizione delle cartelle a cui accedono, rispetto alla gerarchia padre.
Le informazioni sulla gerarchia delle cartelle sono particolarmente utili per distinguere le cartelle con nomi simili ad altre cartelle condivise da una gerarchia di cartelle diversa. Se gli utenti non amministratori non sono a conoscenza della struttura di cartelle delle risorse condivise con loro, le risorse e le cartelle con nomi simili potrebbero confondersi.

* I percorsi visualizzati sulle rispettive schede vengono troncati per adattarsi alle dimensioni delle schede. Tuttavia, gli utenti possono vedere il percorso completo come una descrizione al passaggio del mouse sul percorso troncato.

![](assets/folder-hierarchy1.png)

**Opzione Panoramica per visualizzare le proprietà della risorsa**

L’opzione Panoramica è disponibile per gli utenti non amministratori (editor, visualizzatori, utenti ospiti) per visualizzare le proprietà delle risorse o delle cartelle selezionate. L&#39;opzione Panoramica è visibile:

* nella barra degli strumenti in alto, quando si seleziona una risorsa o una cartella.
* nell’elenco a discesa quando si seleziona il selettore della barra.

Selezionando l&#39;opzione **[!UICONTROL Panoramica]** mentre è selezionata una risorsa/cartella, gli utenti possono visualizzare il titolo, il percorso e l&#39;ora della creazione della risorsa. Nella pagina dei dettagli della risorsa, invece, l’opzione Panoramica permette agli utenti di visualizzare i metadati della risorsa.

![](assets/overview-option.png)

![](assets/overview-rail-selector.png)

#### Visualizzare le impostazioni nella vista a schede

**[!UICONTROL Visualizza]** impostazioni si apre una finestra di dialogo quando si seleziona  **[!UICONTROL Visualizza]** impostazioni dal selettore della vista. Consente di ridimensionare le miniature delle risorse nella vista a schede. In questo modo, potete personalizzare la visualizzazione e controllare il numero di miniature visualizzate.

![](assets/cardviewsettings.png)

### Vista a elenco 

![](assets/list-view.png)

Nella vista a elenco sono visualizzate le informazioni relative a ciascuna risorsa al livello corrente. La vista Elenco fornisce i seguenti dettagli:

* Miniatura delle risorse
* Nome
* Titolo
* Paese
* Tipo
* Dimension
* Dimensione
* Valutazione
* Percorso cartella che mostra la gerarchia delle risorse<sup>*</sup>
* Data di pubblicazione della risorsa su Brand Portal

La colonna Percorso consente di identificare facilmente la posizione della risorsa nella gerarchia delle cartelle. Per spostarti verso il basso nella gerarchia, tocca o fai clic sul nome della risorsa, quindi fai di nuovo clic sulle breadcrumb [nell&#39;intestazione](https://helpx.adobe.com/experience-manager/6-5/sites/authoring/using/basic-handling.html#TheHeader).

<!--
Comment Type: draft lastmodifiedby="mgulati" lastmodifieddate="2018-08-17T03:12:05.096-0400" type="annotation">Removed:- "Selecting assets in list view To select all items in the list, use the checkbox at the upper left of the list. When all items in the list are selected, this check box appears checked. To deselect all, click or tap the checkbox. When only some items are selected, it appears with a minus sign. To select all, click or tap the checkbox. To deselect all, click or tap the checkbox again. You can change the order of items using the dotted vertical bar at the far right of each item in the list. Tap/click the vertical selection bar and drag the item to a new position in the list."
 -->

### Visualizzare le impostazioni nella vista a elenco

La vista Elenco mostra la risorsa **[!UICONTROL Name]** come prima colonna per impostazione predefinita. Vengono inoltre visualizzate informazioni aggiuntive, ad esempio risorse **[!UICONTROL Titolo]**, **[!UICONTROL Impostazioni internazionali]**, **[!UICONTROL Tipo]**, **[!UICONTROL Dimension]**, **[!UICONTROL Dimensioni]**, **[!UICONTROL Valutazione]**, stato di pubblicazione. Tuttavia, è possibile selezionare le colonne da visualizzare utilizzando **[!UICONTROL Visualizza impostazioni]**.

![](assets/list-view-setting.png)

### Vista a colonne

![](assets/column-view.png)

Utilizzate la vista a colonne per navigare in una struttura di contenuto attraverso una serie di colonne a cascata. Questa visualizzazione consente di visualizzare e scorrere la gerarchia delle risorse.

Quando si seleziona una risorsa nella prima colonna (all’estrema sinistra), vengono visualizzate le risorse secondarie nella seconda colonna a destra. Quando si seleziona una risorsa nella seconda colonna, vengono visualizzate le risorse secondarie nella terza colonna a destra e così via.

Per spostarvi in alto e in basso nella struttura ad albero, toccate o fate clic sul nome della risorsa o sulla freccia a destra del nome della risorsa.

* Il nome della risorsa e la freccia vengono evidenziati quando si tocca o si fa clic su di essi.
* Toccando o facendo clic sulla miniatura, la risorsa viene selezionata.
* Quando è selezionata questa opzione, sulla miniatura viene sovrapposto un segno di spunta e il nome della risorsa viene evidenziato.
* I dettagli della risorsa selezionata sono visualizzati nella colonna finale.

Quando una risorsa è selezionata nella vista a colonne, la rappresentazione visiva della risorsa viene visualizzata nella colonna finale con i seguenti dettagli:

* Titolo
* Nome
* Dimensioni
* Data e ora in cui la risorsa è stata pubblicata su Brand Portal da AEM
* Dimensione
* Tipo
* Ulteriori dettagli, per passare alla pagina dei dettagli della risorsa

<!--
Comment Type: draft

<h3>Selecting Resources</h3>
-->

<!--
Comment Type: draft

<p>Selecting a specific resource depends on a combination of the view and the device:</p>
-->

<!--
Comment Type: draft

<table border="1" cellpadding="1" cellspacing="0" width="100%">
<tbody>
<tr>
<td> </td>
<td>Select</td>
<td>Deselect</td>
</tr>
<tr>
<td>Column View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
<tr>
<td>Card View<br /> </td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap-and-hold the card</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the card</li>
<li>Mobile device:<br /> Tap the card</li>
</ul> </td>
</tr>
<tr>
<td>List View</td>
<td>
<ul>
<li>Desktop:<br /> Mouseover, then use the check mark quick action</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
<td>
<ul>
<li>Desktop:<br /> Click the thumbnail</li>
<li>Mobile device:<br /> Tap the thumbnail</li>
</ul> </td>
</tr>
</tbody>
</table>
-->

<!--
Comment Type: draft

Deselecting All
-->

<!--
Comment Type: draft

<p>In all cases, as you select items the count of the items selected is displayed at the upper right of the toolbar.</p>
<p>You can deselect all items and exit selection mode by clicking or tapping the X next to the count.</p>
-->

<!--
Comment Type: draft

<p>In all views, all items can be deselected by tapping escape on the keyboard if you are using a desktop device.</p>
-->

## Struttura contenuto {#content-tree}

Oltre a queste viste, utilizzate la vista ad albero per espandere la gerarchia delle risorse mentre visualizzate e selezionate le risorse o le cartelle desiderate.

Per aprire la vista ad albero, toccate/fate clic sul selettore della barra in alto a sinistra e selezionate la struttura ad albero **[!UICONTROL Contenuto]** dal menu.

![](assets/contenttree.png)

Dalla gerarchia dei contenuti, individuate la risorsa desiderata.

![](assets/content-tree.png)

## Dettagli risorsa {#asset-details}

La pagina dei dettagli della risorsa consente di visualizzare una risorsa, scaricarla, condividere il collegamento della risorsa, spostarla in una raccolta o visualizzare la pagina delle relative proprietà. Consente inoltre di passare alla pagina dei dettagli di altre risorse della stessa cartella in successione.

![](assets/asset-detail.png)

Per visualizzare i metadati della risorsa o le relative diverse rappresentazioni, usate il selettore della barra laterale nella pagina dei dettagli della risorsa.

![](assets/asset-overview.png)

Potete visualizzare tutte le rappresentazioni disponibili della risorsa nella pagina dei dettagli della risorsa e selezionare una rappresentazione per visualizzarla in anteprima.

![](assets/renditions.png)

Per aprire la pagina delle proprietà della risorsa, utilizzate l&#39;opzione **[!UICONTROL Proprietà (p)]** presente nella barra superiore.

![](assets/asset-properties.png)

Potete anche visualizzare un elenco di tutte le relative risorse correlate (risorse di origine o derivate in AEM) nella pagina delle proprietà di una risorsa, poiché anche la relazione tra risorse viene pubblicata da AEM al Portale marchio.
