---
title: Utilizzare il modulo schema metadati
seo-title: Utilizzare il modulo schema metadati
description: Uno schema di metadati descrive il layout della pagina Proprietà e le proprietà dei metadati visualizzate per le risorse che utilizzano lo schema specifico. Lo schema applicato a una risorsa determina i campi di metadati visualizzati nella pagina Proprietà.
seo-description: Uno schema di metadati descrive il layout della pagina Proprietà e le proprietà dei metadati visualizzate per le risorse che utilizzano lo schema specifico. Lo schema applicato a una risorsa determina i campi di metadati visualizzati nella pagina Proprietà.
uuid: 1 a 944 a 3 b -5152-425 f-b 1 ea-bfe 3331 de 928
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
topic-tags: administration
discoiquuid: 500 b 46 da-ef 67-46 a 0-a 069-192 f 4 b 1 a 0 eca
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Utilizzare il modulo schema metadati {#use-the-metadata-schema-form}

Uno schema di metadati descrive il layout della pagina Proprietà e le proprietà dei metadati visualizzate per le risorse che utilizzano lo schema specifico. Lo schema applicato a una risorsa determina i campi di metadati visualizzati nella pagina Proprietà.

La **[!UICONTROL pagina Proprietà]** di ciascuna risorsa include proprietà di metadati predefinite a seconda del tipo MIME della risorsa. Gli amministratori possono usare l'Editor schema metadati per modificare gli schemi esistenti o aggiungere schemi di metadati personalizzati. AEM Assets Brand Portal fornisce moduli predefiniti per le risorse di vari tipi MIME. Tuttavia, è anche possibile aggiungere moduli personalizzati per tali risorse.

## Aggiungere un modulo schema metadati {#add-a-metadata-schema-form}

Per creare un nuovo modulo schema metadati, effettuate le seguenti operazioni:

1. Dalla barra degli strumenti AEM nella parte superiore, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

2. Dal pannello Strumenti di amministrazione, fate clic **[!UICONTROL su Schemi metadati]**.

   ![](assets/navigation-panel.png)

3. Nella **[!UICONTROL pagina Moduli]** schema metadati, fate clic **[!UICONTROL su Crea]**.

   ![](assets/create-metadata-schema-form.png)

4. Nella **[!UICONTROL finestra di]** dialogo Crea modulo schema, specificare il titolo del modulo Schema, quindi fare clic su **[!UICONTROL Crea]** per completare il processo di creazione del modulo.

   ![](assets/create-schema-form.png)

## Edit a metadata schema form {#edit-a-metadata-schema-form}

Potete modificare un modulo schema metadati appena aggiunto o esistente. Il modulo schema metadati contiene contenuto derivato dal relativo elemento padre, comprese schede e elementi modulo all'interno delle schede. Potete mappare o configurare questi elementi in un campo all'interno di un nodo di metadati.

Potete aggiungere nuove schede o elementi modulo al modulo schema metadati. Le schede derivate e gli elementi modulo (dall'elemento padre) sono nello stato bloccato. Non è possibile modificarle a livello di secondario.

Per modificare un modulo schema metadati, effettuate le seguenti operazioni:

1. Dalla barra degli strumenti AEM nella parte superiore, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

2. Dal pannello Strumenti di amministrazione, fate clic **[!UICONTROL su Schemi metadati]**.
3. Dalla pagina **[!UICONTROL Moduli]** schema metadati, selezionare un modulo schema per modificarne le proprietà, ad esempio **[!UICONTROL la raccolta]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >Nei modelli non modificati viene visualizzato un simbolo lucchetto. Se personalizzate uno qualsiasi dei modelli, il simbolo Blocca viene visualizzato prima che il modello scompaia.

4. Nella barra degli strumenti in alto, fate clic **[!UICONTROL su Modifica]**.

   Viene aperta **[!UICONTROL la pagina Editor]** schema metadati con la scheda **[!UICONTROL di base]** aperta a sinistra e la **[!UICONTROL scheda Crea modulo]** aperta a destra.

5. Nella **[!UICONTROL pagina Editor]** schema metadati, personalizzate la **[!UICONTROL pagina Proprietà]** della risorsa trascinando uno o più componenti da un elenco dei tipi di componente nella scheda **[!UICONTROL Crea modulo]** nella scheda **[!UICONTROL Base]** .

   ![](assets/metadata-schemaeditor-page.png)

6. Per configurare un componente, selezionatelo e modificatene le proprietà nella scheda **[!UICONTROL Impostazioni]** .

### Componenti nella scheda Crea modulo {#components-in-the-build-form-tab}

Nella **[!UICONTROL scheda Build Form (Crea modulo]** ) sono elencati gli elementi che è possibile utilizzare nel modulo schema. La **[!UICONTROL scheda Impostazioni]** fornisce gli attributi di ogni elemento selezionato nella scheda **[!UICONTROL Crea modulo]** . Nella tabella seguente sono elencati gli elementi modulo disponibili nella scheda **[!UICONTROL Build Form]** :

| Nome componente | Descrizione |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [!UICONTROL Intestazione sezione] | Aggiungete un titolo di sezione per un elenco di componenti comuni. |
| [!UICONTROL Testo su riga singola] | Aggiunge una proprietà di testo a riga singola. Viene memorizzato come stringa. |
| [!UICONTROL Multi valuetext] | Aggiunge una proprietà testo con più valori. Viene memorizzato come array di stringhe. |
| [!UICONTROL Numero] | Aggiungete un componente numerico. |
| [!UICONTROL Data] | Aggiungere un componente data. |
| [!UICONTROL A discesa] | Aggiungete un elenco a discesa. |
| [!UICONTROL Tag standard] | Aggiungi un tag. **Nota:** Gli amministratori possono dover modificare il valore del percorso, ad esempio, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`se pubblicano il modulo schema metadati da AEM, ad esempio, se il percorso non include informazioni tenant, ad esempio `/etc/tags/<custom_tag_namespace>`. |
| [!UICONTROL Tag avanzati] | I tag rilevati automaticamente se hai acquistato e configurato il componente aggiuntivo di tag smart AEM. |
| [!UICONTROL Campo nascosto] | Aggiungere un campo nascosto. Viene inviato come parametro POST quando la risorsa viene salvata. |
| [!UICONTROL Risorsa con riferimento da] | Aggiungete questo componente per visualizzare l'elenco delle risorse a cui fa riferimento la risorsa. |
| [!UICONTROL Risorsa con riferimento a] | Aggiungete un elenco di risorse che fanno riferimento alla risorsa. |
| [!UICONTROL Valutazione risorsa] | Valutazione media di una risorsa aggiunta da Risorse AEM prima della pubblicazione sul portale brand. |
| [!UICONTROL Metadati contestuali] | Aggiungete per controllare la visualizzazione di altre schede di metadati nella pagina Proprietà delle risorse. |

>[!NOTE]
>
>Non utilizzate **[!UICONTROL i Riferimenti]** prodotti, poiché non funziona.

#### Modificare il componente metadati {#edit-the-metadata-component}

Per modificare le proprietà di un componente di metadati sul modulo, fare clic sul componente e modificarne le proprietà nella scheda **[!UICONTROL Impostazioni]** .

* **[!UICONTROL Etichetta campo]**: Nome della proprietà di metadati visualizzata nella pagina Proprietà della risorsa.

* **[!UICONTROL Mappa su proprietà]**: Il valore di questa proprietà fornisce il percorso/nome relativo al nodo della risorsa in cui viene salvato nell'archivio CRX. Inizia con **"./**"perché indica che il percorso si trova sotto il nodo della risorsa.

Di seguito sono riportati i valori validi per questa proprietà:

— [!UICONTROL `./jcr:content/metadata/dc:title`]: Memorizza il valore sul nodo metadati della risorsa come proprietà [!UICONTROL `dc:title`].

— [!UICONTROL `./jcr:created`]: Visualizza la proprietà jcr sul nodo della risorsa. Se configurate queste proprietà in Proprietà visualizzazione, è consigliabile contrassegnarle come Disattiva modifica, poiché sono protette. In caso contrario, l'errore «Risorse non modificate» si verifica quando salvate le proprietà della risorsa.

* **[!UICONTROL Segnaposto]**: Utilizzate questa proprietà per fornire all'utente informazioni rilevanti sulla proprietà metadata.
* **[!UICONTROL Richiesto]**: Utilizzate questa proprietà per contrassegnare una proprietà di metadati come obbligatorio nella pagina Proprietà.
* **[!UICONTROL Disattiva modifica]**: Utilizzate questa proprietà per rendere non modificabile una proprietà di metadati nella pagina Proprietà.
* **[!UICONTROL Mostra campo vuoto in sola lettura]**: Contrassegnate questa proprietà per visualizzare una proprietà di metadati nella pagina Proprietà, anche se non ha valore. Per impostazione predefinita, quando una proprietà di metadati non ha valore, non viene elencata nella pagina Proprietà.
* **[!UICONTROL Descrizione]**: Utilizzate questa proprietà per aggiungere una breve descrizione del componente metadati.
* **[!UICONTROL Icona Elimina]**: Fare clic su questa icona per eliminare un componente dal modulo schema.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Tutti i campi di metadati sono di sola lettura nella forma di editor metadati di una risorsa. Poiché i metadati della risorsa devono essere modificati in Risorse AEM prima che una risorsa venga pubblicata sul portale del brand.

#### Aggiunta o eliminazione di una scheda nel modulo schema {#add-or-delete-a-tab-in-the-schema-form}

Il modulo schema predefinito include le schede **[!UICONTROL Base]** e **[!UICONTROL Avanzate]** . L'Editor schema consente di aggiungere o eliminare una scheda.

![](assets/add_delete_tabs_metadataschemaform.png)

* Per aggiungere una nuova scheda in un modulo schema, fare clic **[!UICONTROL su +]**. Per impostazione predefinita, la nuova scheda ha il nome «Unnamed -1». Potete modificare il nome dalla scheda **[!UICONTROL Impostazioni]** .

![](assets/add-tab-metadata-form.png)

* Per eliminare una scheda, fate clic **[!UICONTROL su x]**. Click **[!UICONTROL Save]** to save the changes.

## Applicazione di uno schema di metadati a una cartella {#apply-a-metadata-schema-to-a-folder}

Portale marchio consente di personalizzare e controllare lo schema di metadati, in modo che la [!UICONTROL pagina Proprietà] di una risorsa contenga solo le informazioni specifiche che si scelgono di rivelare. Per controllare i metadati visualizzati nella pagina [!UICONTROL Proprietà] , rimuovete i metadati richiesti dal modulo schema metadati e applicateli alla cartella specifica.

Per applicare un modulo schema metadati a una cartella, effettuate le seguenti operazioni:

1. Dalla barra degli strumenti AEM nella parte superiore, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

2. Dal pannello Strumenti di amministrazione, fate clic **[!UICONTROL su Schemi metadati]**.

3. Nella pagina **[!UICONTROL Moduli]** schema metadati, selezionate il modulo di schema che desiderate applicare a una risorsa, ad esempio [!UICONTROL i vestiti].

   ![](assets/apply-metadata-schema-form-to-folder.png)

4. Dalla barra degli strumenti in alto, fate clic **[!UICONTROL su Applica alle cartelle]**.

5. Dalla pagina **[!UICONTROL Seleziona]** cartelle, passate alla cartella in cui desiderate applicare lo **[!UICONTROL schema]** di metadati abbigliamento, ad esempio **[!UICONTROL , Guanti]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

6. Fate clic su **[!UICONTROL Applica]** per applicare il modulo schema metadati alla cartella.

   I metadati disponibili nel modulo schema metadati **[!UICONTROL abbigliamento]** vengono applicati alla **[!UICONTROL cartella Guanti]** e visibili nella pagina **[!UICONTROL Proprietà]** della cartella.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Se applicate uno schema che include schemi nidificati a una cartella contenente file video, le proprietà dei metadati dei file video potrebbero non essere renderizzate correttamente. Per assicurare il corretto rendering delle proprietà dei metadati, rimuovete gli schemi nidificati e applicate solo lo schema principale alla cartella.

## Delete a metadata schema form {#delete-a-metadata-schema-form}

Brand Portal consente di eliminare solo moduli schema personalizzati. Non consente di eliminare i moduli/modelli schema predefiniti. Tuttavia, è possibile eliminare eventuali modifiche personalizzate in questi moduli.

Per eliminare un modulo, selezionare un modulo e fare clic sull'icona **[!UICONTROL Elimina]** .

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Dopo aver eliminato le modifiche personalizzate apportate a un modulo predefinito, il **[!UICONTROL simbolo Blocca]** viene visualizzato nuovamente prima del nome del modulo nell'interfaccia Schema metadati per indicare che il modulo viene ripristinato al suo stato predefinito.

## Moduli schema per i tipi MIME {#schema-forms-for-mime-types}

### Aggiunta di nuovi moduli per tipi MIME {#adding-new-forms-for-mime-types}

Oltre ai moduli predefiniti, è possibile aggiungere moduli personalizzati per le risorse di vari tipi MIME, oppure creare un nuovo modulo con un tipo di modulo appropriato. Ad esempio, per aggiungere un nuovo modello per il **[!UICONTROL sottotipo image/png]** , creare il modulo sotto i moduli «immagine». Il titolo del modulo schema è il nome del sottotipo. In questo caso, il titolo è «png».

#### Utilizzo di un modello di schema esistente per vari tipi MIME {#using-an-existing-schema-template-for-various-mime-types}

Potete utilizzare un modello esistente per un tipo MIME diverso. Ad esempio, usate il **modulo immagine/jpeg** per le risorse del tipo MIME **image/png**.

In questo caso, crea un nuovo nodo nell [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] 'archivio CRX. Specificare un nome per il nodo e definire le proprietà seguenti:

| **Nome** | **Tipo** | **Valore** |
|---|---|---|
| exposedmimetype | Stringa | image/jpeg |
| mimetypes | Stringa[] | image/png |

* **exposedmimetype**: Nome del modulo esistente da mappare
* **mimetypes**: Elenco dei tipi MIME che utilizzano il modulo definito nell'attributo **essedmimetype**

Brand Portal mappa i seguenti tipi MIME e moduli schema:

| **Modulo schema** | **Tipi MIME** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-imageset | Multipart/Related; type=application/x-ImageSet |
| application/x-spinset | Multipart/Related; type=application/x-SpinSet |
| application/x-mixedmediaset | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg 4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

Di seguito è riportato un elenco delle proprietà di metadati predefinite:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr: content/metadata/videocodec
* jcr: content/metadata/audiocodec
* jcr: content/metadata/dc: title
* jcr: content/metadata/dc: description
* jcr: content/metadata/xmpmm: Instanceid
* jcr: content/metadata/xmpmm: Documentid
* jcr: content/metadata/dam: sha 1
* jcr: content/metadata/dam: Solutioncontext
* jcr: content/metadata/videobitrate
* jcr: content/metadata/audiobitrate
* jcr: content/usages/usedby
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr: content/ontime
* jcr: content/offtime
* jcr:content/metadata/dam:size
* jcr: content/metadata/tiff: Imagewidth
* jcr: content/metadata/tiff: Imagelength
