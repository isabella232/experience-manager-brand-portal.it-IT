---
title: Utilizzare il modulo schema metadati
seo-title: Use the metadata schema form
description: Uno schema di metadati descrive il layout della pagina Proprietà e le proprietà dei metadati visualizzate per le risorse che utilizzano lo schema specifico. Lo schema applicato a una risorsa determina i campi di metadati che vengono visualizzati nella relativa pagina Proprietà.
seo-description: A metadata schema describes the layout of the Properties page and the metadata properties displayed for assets that use the particular schema. The schema that you apply to an asset determines the metadata fields that appear on its Properties page.
uuid: 1a944a3b-5152-425f-b1ea-bfe3331de928
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
topic-tags: administration
discoiquuid: 500b46da-ef67-46a0-a069-192f4b1a0eca
role: Admin
exl-id: fbedff90-a6cb-4175-8308-817cc9f5b450
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1718'
ht-degree: 11%

---

# Utilizzare il modulo schema metadati {#use-the-metadata-schema-form}

Uno schema di metadati descrive il layout della pagina Proprietà e le proprietà dei metadati visualizzate per le risorse che utilizzano lo schema specifico. Lo schema applicato a una risorsa determina i campi di metadati che vengono visualizzati nella relativa pagina Proprietà.

Il **[!UICONTROL Proprietà]** La pagina di ciascuna risorsa include proprietà di metadati predefinite che dipendono dal tipo MIME della risorsa. Gli amministratori possono utilizzare l’Editor schema metadati per modificare schemi esistenti o aggiungere schemi di metadati personalizzati. Experience Manager Assets Brand Portal fornisce moduli predefiniti per risorse di vari tipi MIME. Tuttavia, puoi anche aggiungere moduli personalizzati per tali risorse.

## Aggiungere un modulo schema metadati {#add-a-metadata-schema-form}

Per creare un nuovo modulo schema metadati, effettuare le seguenti operazioni:

1. Dalla barra degli strumenti nella parte superiore, fai clic sul logo dell’Experience Manager per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

1. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Schemi metadati]**.

   ![](assets/navigation-panel.png)

1. Il giorno **[!UICONTROL Forms schema metadati]** pagina, fai clic su **[!UICONTROL Crea]**.

   ![](assets/create-metadata-schema-form.png)

1. In **[!UICONTROL Crea modulo schema]** , specificare il titolo del modulo Schema e quindi fare clic su **[!UICONTROL Crea]** per completare il processo di creazione del modulo.

   ![](assets/create-schema-form.png)

## Modificare un modulo schema metadati {#edit-a-metadata-schema-form}

Puoi modificare un modulo schema metadati appena aggiunto o esistente. Il modulo schema metadati contiene contenuto derivato dal relativo elemento padre, incluse schede ed elementi modulo all’interno di schede. Puoi mappare o configurare questi elementi modulo su un campo all’interno di un nodo di metadati.

È possibile aggiungere nuove schede o elementi del modulo al modulo schema metadati. Le schede e gli elementi modulo derivati (dall&#39;elemento padre) sono nello stato bloccato. Non è possibile modificarli a livello di elemento secondario.

Per modificare un modulo schema metadati, effettuare le seguenti operazioni:

1. Dalla barra degli strumenti nella parte superiore, fai clic sul logo dell’Experience Manager per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

1. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Schemi metadati]**.
1. Dalla sezione **[!UICONTROL Forms schema metadati]** , selezionare un modulo schema per modificarne le proprietà, ad esempio **[!UICONTROL raccolta]**.

   ![](assets/metadata-schema-forms.png)

   >[!NOTE]
   >
   >I modelli non modificati presentano prima un simbolo di blocco. Se personalizzi uno dei modelli, il simbolo Blocca prima del modello scompare.

1. Dalla barra degli strumenti nella parte superiore, fai clic su **[!UICONTROL Modifica]**.

   Il **[!UICONTROL Editor schema metadati]** viene aperta la pagina con **[!UICONTROL Base]** scheda aperta a sinistra e **[!UICONTROL Genera modulo]** sulla destra.

1. In **[!UICONTROL Editor schema metadati]** , personalizzare la pagina **[!UICONTROL Proprietà]** della risorsa trascinando uno o più componenti da un elenco di tipi di componenti in **[!UICONTROL Genera modulo]** scheda a **[!UICONTROL Base]** scheda.

   ![](assets/metadata-schemaeditor-page.png)

1. Per configurare un componente, selezionalo e modificane le proprietà in **[!UICONTROL Impostazioni]** scheda.

### Componenti nella scheda Genera modulo {#components-in-the-build-form-tab}

Il **[!UICONTROL Genera modulo]** La scheda elenca gli elementi che è possibile utilizzare nel modulo schema. Il **[!UICONTROL Impostazioni]** fornisce gli attributi di ogni elemento selezionato nella scheda **[!UICONTROL Genera modulo]** scheda. Nella tabella seguente sono elencati gli elementi modulo disponibili in **[!UICONTROL Genera modulo]** scheda:

| Nome componente | Descrizione |
|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[!UICONTROL Intestazione sezione]** | Aggiungi un’intestazione di sezione per un elenco di componenti comuni. |
| **[!UICONTROL Testo su riga singola]** | Aggiungi una proprietà di testo a riga singola. Viene memorizzato come stringa. |
| **[!UICONTROL Testo con più valori]** | Aggiungi una proprietà di testo con più valori. Viene memorizzato come array di stringhe. |
| **[!UICONTROL Numero]** | Aggiungi un componente numero. |
| **[!UICONTROL Data]** | Aggiungi un componente data. |
| **[!UICONTROL A discesa]** | Aggiungi un elenco a discesa. |
| **[!UICONTROL Tag standard]** | Aggiungi un tag. **Nota:** Gli amministratori potrebbero dover modificare il valore del percorso, ad esempio, `/etc/tags/mac/<tenant_id>/<custom_tag_namespace>`, se pubblicano il modulo schema metadati da Experience Manager Assets, dove il percorso non include informazioni sul tenant, ad esempio, `/etc/tags/<custom_tag_namespace>`. |
| **[!UICONTROL Tag avanzati]** | Se hai acquistato e configurato il componente aggiuntivo smart tag di Experience Manager Assets, vengono rilevati automaticamente i tag. |
| **[!UICONTROL Campo nascosto]** | Aggiungi un campo nascosto. Viene inviato come parametro POST al salvataggio della risorsa. |
| **[!UICONTROL Risorsa con riferimento da]** | Aggiungi questo componente per visualizzare l’elenco delle risorse a cui fa riferimento la risorsa. |
| **[!UICONTROL Risorsa con riferimento a]** | Aggiungi per visualizzare un elenco di risorse che fanno riferimento alla risorsa. |
| **[!UICONTROL Valutazione risorsa]** | Valutazione media di una risorsa aggiunta da Experience Manager Assets prima che venga pubblicata in Brand Portal. |
| **[!UICONTROL Metadati contestuali]** | Aggiungi per controllare la visualizzazione di altre schede di metadati nella pagina Proprietà delle risorse. |

>[!NOTE]
>
>Non usi **[!UICONTROL Riferimenti prodotto]**, in quanto non è funzionale.

#### Modificare il componente metadati {#edit-the-metadata-component}

Per modificare le proprietà di un componente metadati nel modulo, fai clic sul componente e modificane le proprietà nel **[!UICONTROL Impostazioni]** scheda.

* **[!UICONTROL Etichetta campo]**: nome della proprietà dei metadati visualizzata nella pagina Proprietà della risorsa.

* **[!UICONTROL Mappa su proprietà]**: il valore di questa proprietà fornisce il percorso/nome relativo del nodo della risorsa in cui viene salvato nell’archivio CRX. Inizia con &quot;**./**&quot; perché indica che il percorso si trova sotto il nodo della risorsa.

Di seguito sono riportati i valori validi per questa proprietà:

-- `./jcr:content/metadata/dc:title`: memorizza il valore come proprietà nel nodo di metadati della risorsa [!UICONTROL `dc:title`].

-- `./jcr:created`: visualizza la proprietà jcr sul nodo della risorsa. Se configuri queste proprietà come View Properties (Visualizza proprietà), è consigliabile contrassegnarle con l’opzione Disattiva modifica, in quanto sono protette. In caso contrario, al momento di salvare le proprietà della risorsa si verifica l’errore “Impossibile modificare le risorse”.

* **[!UICONTROL Segnaposto]**: utilizza questa proprietà per fornire all’utente tutte le informazioni pertinenti relative alla proprietà dei metadati.
* **[!UICONTROL Obbligatorio]**: utilizza questa proprietà per contrassegnare una proprietà di metadati come obbligatoria nella pagina Proprietà.
* **[!UICONTROL Disattiva modifica]**: utilizza questa proprietà per impedire la modifica di una proprietà di metadati nella pagina Proprietà.
* **[!UICONTROL Mostra campo vuoto in sola lettura]**: contrassegna questa proprietà per visualizzare una proprietà di metadati nella pagina Proprietà anche se non ha un valore. Per impostazione predefinita, quando una proprietà di metadati non ha un valore, non viene elencata nella pagina Proprietà.
* **[!UICONTROL Descrizione]**: utilizza questa proprietà per aggiungere una breve descrizione del componente metadati.
* **[!UICONTROL Icona Elimina]**: fai clic su questa icona per eliminare un componente dal modulo schema.

![](assets/delete_icon_editmetadataschemaform.png)

>[!NOTE]
>
>Tutti i campi di metadati sono di sola lettura nel modulo dell’editor di metadati di una risorsa. Poiché i metadati della risorsa devono essere modificati in Experience Manager Assets prima che una risorsa venga pubblicata in Brand Portal.

#### Aggiungere o eliminare una scheda nel modulo schema {#add-or-delete-a-tab-in-the-schema-form}

Il modulo schema predefinito include **[!UICONTROL Base]** e **[!UICONTROL Avanzate]** schede. L’editor dello schema consente di aggiungere o eliminare una scheda.

![](assets/add_delete_tabs_metadataschemaform.png)

* Per aggiungere una nuova scheda a un modulo schema, fai clic su **[!UICONTROL +]**. Per impostazione predefinita, la nuova scheda è denominata &quot;Unnamed-1&quot;. Puoi modificare il nome dalla sezione **[!UICONTROL Impostazioni]** scheda.

![](assets/add-tab-metadata-form.png)

* Per eliminare una scheda, fare clic su **[!UICONTROL x]**. Clic **[!UICONTROL Salva]** per salvare le modifiche.

## Applicare uno schema di metadati a una cartella {#apply-a-metadata-schema-to-a-folder}

Brand Portal consente di personalizzare e controllare lo schema metadati in modo che **[!UICONTROL Proprietà]** pagina di una risorsa mostra solo le informazioni specifiche che scegli di visualizzare. Per controllare i metadati visualizzati in **[!UICONTROL Proprietà]** , rimuovi i metadati richiesti dal modulo schema metadati e applicali alla cartella specifica.

Per applicare un modulo schema metadati a una cartella, effettua le seguenti operazioni:

1. Dalla barra degli strumenti nella parte superiore, fai clic sul logo dell’Experience Manager per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

1. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Schemi metadati]**.

1. Dalla sezione **[!UICONTROL Forms schema metadati]** , seleziona il modulo schema da applicare a una risorsa, ad esempio, **[!UICONTROL abbigliamento]**.

   ![](assets/apply-metadata-schema-form-to-folder.png)

1. Dalla barra degli strumenti nella parte superiore, fai clic su **[!UICONTROL Applica a cartelle]**.

1. Dalla sezione **[!UICONTROL Seleziona cartelle]** , passare alla cartella alla quale si desidera applicare la **[!UICONTROL abbigliamento]** schema metadati, ad esempio, **[!UICONTROL Guanti]**.

   ![](assets/apply_metadata_schemaformtofoldergloves.png)

1. Clic **[!UICONTROL Applica]** per applicare il modulo schema metadati alla cartella.

   I metadati disponibili nella sezione **[!UICONTROL abbigliamento]** il modulo schema metadati viene applicato al **[!UICONTROL Guanti]** e visibile nella **[!UICONTROL Proprietà]** della cartella.

   ![](assets/folder_metadata_properties.png)

>[!NOTE]
>
>Se applichi uno schema che include schemi nidificati a una cartella contenente file video, le proprietà dei metadati per i file video potrebbero non essere riprodotte correttamente. Per garantire il corretto rendering delle proprietà dei metadati, rimuovi gli schemi nidificati e applica alla cartella solo lo schema principale.

## Eliminare un modulo schema metadati {#delete-a-metadata-schema-form}

Brand Portal consente di eliminare solo i moduli schema personalizzati. Non consente di eliminare i moduli/modelli di schema predefiniti. Tuttavia, è possibile eliminare qualsiasi modifica personalizzata in questi moduli.

Per eliminare un modulo, selezionarlo e fare clic su **[!UICONTROL Elimina]** icona.

![](assets/delete_icon_metadataschemaeditorform.png)

>[!NOTE]
>
>Dopo aver eliminato le modifiche personalizzate apportate a un modulo predefinito, **[!UICONTROL Blocca]** Il simbolo viene nuovamente visualizzato prima del nome del modulo nell&#39;interfaccia Schema metadati per indicare che il modulo è tornato allo stato predefinito.

## Moduli schema per TIPI MIME {#schema-forms-for-mime-types}

### Aggiunta di nuovi moduli per tipi MIME {#adding-new-forms-for-mime-types}

Oltre ai moduli predefiniti, puoi aggiungere moduli personalizzati per risorse di vari tipi MIME o creare un nuovo modulo in un tipo di modulo appropriato. Ad esempio, per aggiungere un nuovo modello per il sottotipo **[!UICONTROL image/png]**, crea il modulo sotto i moduli “image”. Il titolo del modulo schema è il nome del sottotipo. In questo caso, il titolo è &quot;png&quot;.

#### Utilizzo di un modello di schema esistente per vari tipi MIME {#using-an-existing-schema-template-for-various-mime-types}

Puoi utilizzare un modello esistente per un tipo MIME diverso. Ad esempio, utilizza **image/jpeg** modulo per risorse di tipo MIME **image/png**.

In questo caso, crea un nuovo nodo in corrispondenza di [!UICONTROL `/etc/dam/metadataeditor/mimetypemappings`] nell’archivio CRX. Specifica un nome per il nodo e definisci le seguenti proprietà:

| **Nome** | **Tipo** | **Valore** |
|---|---|---|
| exposedmimetype | Stringa | image/jpeg |
| mimetipi | Stringa[] | image/png |

* **exposedmimetype**: nome del modulo esistente da mappare
* **mimetipi**: elenco di tipi MIME che utilizzano il modulo definito in **exposedmimetype** attributo

Brand Portal mappa i seguenti tipi MIME e moduli schema:

| **Modulo schema** | **Tipi MIME** |
|---|---|
| image/jpeg | image/pjpeg |
| image/tiff | image/x-tiff |
| application/pdf | application/postscript |
| application/x-ImageSet | Multipart/Related; type=application/x-ImageSet |
| application/x-SpinSet | Multipart/Related; type=application/x-SpinSet |
| application/x-MixedMediaSet | Multipart/Related; type=application/x-MixedMediaSet |
| video/quicktime | video/x-quicktime |
| video/mpeg4 | video/mp4 |
| video/avi | video/avi, video/msvideo, video/x-msvideo |
| video/wmv | video/x-ms-wmv |
| video/flv | video/x-flv |

Di seguito è riportato un elenco delle proprietà dei metadati predefinite:

* jcr:content/metadata/cq:tags
* jcr:content/metadata/dc:format
* jcr:content/metadata/dam:status
* jcr:content/metadata/videoCodec
* jcr:content/metadata/audioCodec
* jcr:content/metadata/dc:title
* jcr:content/metadata/dc:description
* jcr:content/metadata/xmpMM:InstanceID
* jcr:content/metadata/xmpMM:DocumentID
* jcr:content/metadata/dam:sha1
* jcr:content/metadata/dam:solutionContext
* jcr:content/metadata/videoBitrate
* jcr:content/metadata/audioBitrate
* jcr:content/usages/usedBy
* jcr:content/jcr:lastModified
* jcr:content/metadata/prism:expirationDate
* jcr:content/onTime
* jcr:content/offTime
* jcr:content/metadata/dam:size
* jcr:content/metadata/tiff:LarghezzaImmagine
* jcr:content/metadata/tiff:LunghezzaImmagine
