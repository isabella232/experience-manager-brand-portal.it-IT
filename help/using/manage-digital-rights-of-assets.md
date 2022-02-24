---
title: Gestire i diritti digitali delle risorse
seo-title: Manage digital rights of assets
description: La concessione di licenze e l’impostazione della scadenza delle risorse e dei collegamenti condivisi garantiscono un utilizzo controllato di tali risorse e la loro protezione.
seo-description: Licensing assets and setting expiration for assets and shared links ensure controlled usage of these assets and safeguard them.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
role: Admin
exl-id: 86c31891-0627-41ca-b571-8dac3a074d55
source-git-commit: d1487434b10b01eaf55f34672267490fd8fd907e
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 2%

---

# Gestire i diritti digitali delle risorse {#manage-digital-rights-of-assets}

Garantire la distribuzione e l&#39;utilizzo sicuri delle risorse creative e del materiale del brand è fondamentale per proteggere il brand. Questo può essere applicato in tutta l’organizzazione e all’esterno associando una data di scadenza (e un’ora) alle risorse approvate pubblicate da AEM a Brand Portal o autorizzando tali risorse per l’uso condizionale. Inoltre, Brand Portal consente di specificare una data di scadenza per i collegamenti alle risorse condivise da Brand Portal.

Continua a leggere per sapere come sono protette le risorse su Brand Portal e per comprendere le relative autorizzazioni di utilizzo.

## Scadenza risorse {#asset-expiration}

La scadenza delle risorse è un modo efficace per controllare l’utilizzo delle risorse approvate su Brand Portal in un’organizzazione. Tutte le risorse pubblicate da AEM Assets a Brand Portal possono avere una data di scadenza, il che limita l’utilizzo di tali risorse da parte di ruoli utente diversi.

### Autorizzazioni di utilizzo relative alle risorse scadute {#usage-permissions-expired-assets}

In Brand Portal, gli amministratori possono visualizzare, scaricare e aggiungere alle raccolte le risorse scadute. Gli editor e i visualizzatori possono invece visualizzare e aggiungere alle raccolte solo le risorse scadute.

Gli amministratori possono pubblicare risorse scadute da AEM Assets in Brand Portal. Tuttavia, le risorse scadute non possono essere condivise tramite inchiostro da Brand Portal. Se selezioni una risorsa scaduta da una cartella contenente sia risorse scadute che non scadute, l’ **[!UICONTROL Condividi collegamento]** azione non disponibile. Tuttavia, se selezioni una cartella che contiene risorse scadute e non scadute, l’ [!UICONTROL Condividi] e **[!UICONTROL Condividi collegamento]** sono disponibili delle azioni.

>[!NOTE]
>
>Una cartella può ancora essere condivisa come collegamento, anche se contiene risorse scadute. In questo caso, il collegamento non elenca le risorse scadute e vengono condivise solo le risorse non scadute.

Nella tabella seguente sono visualizzate le autorizzazioni di utilizzo delle risorse scadute:

|  | **[!UICONTROL Condivisione collegamenti]** | **[!UICONTROL Scarica]** | **[!UICONTROL Proprietà]** | **[!UICONTROL Aggiungi alla raccolta]** | **[!UICONTROL Elimina]** |
|---|---|---|---|---|---|
| **[!UICONTROL Administrator]** | Non disponibile | Disponibile | Disponibile | Disponibile | Disponibile |
| **[!UICONTROL Editor]** | Non disponibile | Non disponibile | Disponibile | Disponibile | Non disponibile |
| **[!UICONTROL Visualizzatore]** | Non disponibile | Non disponibile | Disponibile | Disponibile | Non disponibile |
| **[!UICONTROL Utente ospite]** | Non disponibile | Non disponibile | Disponibile | Disponibile | Non disponibile |

>[!NOTE]
>
>Se Visualizzatori ed editor scaricano una cartella contenente risorse scadute e non scadute, vengono scaricate solo le risorse non scadute. Se una cartella contiene solo risorse scadute, viene scaricata una cartella vuota.

### Stato di scadenza delle risorse {#expiration-status-of-assets}

Puoi visualizzare lo stato di scadenza delle risorse nelle relative **[!UICONTROL Vista a schede]**. Un flag rosso sulla scheda indica che la risorsa è scaduta.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Le visualizzazioni a elenco e a colonne non mostrano lo stato di scadenza delle risorse.

## Scadenza collegamento risorsa {#asset-link-expiration}

Durante la condivisione delle risorse tramite i collegamenti, gli amministratori e gli editor possono impostare una data e un’ora di scadenza utilizzando **[!UICONTROL Scadenza]** nel campo **[!UICONTROL Condivisione collegamenti]** finestra di dialogo. La scadenza predefinita del collegamento è di sette giorni dalla data in cui il collegamento è condiviso.

![](assets/asset-link-sharing.png)

Garantisce che le risorse condivise come collegamenti scadano alla data e all’ora impostate dagli amministratori e dagli editor di Brand Portal e non possano più essere visualizzate e scaricate oltre la data di scadenza. Poiché le risorse condivise tramite i collegamenti possono essere visualizzate anche da utenti esterni che non fanno parte dell’organizzazione, specificando la scadenza puoi assicurarti che le risorse approvate siano protette e non esposte a entità sconosciute oltre un determinato periodo di tempo.

Per ulteriori informazioni sulla condivisione dei collegamenti, consulta [Condividere le risorse come collegamento](../using/brand-portal-link-share.md).

## Risorse concesse in licenza {#licensed-assets}

Le risorse concesse in licenza sono soggette all’accettazione di un contratto di licenza prima del download da Brand Portal. Questo contratto per le risorse con licenza viene stipulato quando si scarica direttamente la risorsa da Brand Portal o tramite un collegamento condiviso. Che sia scaduto o meno, le risorse protette da licenza possono essere visualizzate da tutti gli utenti. Tuttavia, il download e l’utilizzo di risorse con licenza scadute sono limitati. Per informazioni sul comportamento delle risorse con licenza scadute e delle attività consentite in base ai ruoli utente, consulta [autorizzazioni di utilizzo delle risorse scadute](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets).

Le risorse protette dalla licenza [contratto di licenza allegato](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/drm.html) a loro, che viene fatto impostando la proprietà dei metadati della risorsa in [!DNL Experience Manager Assets].

Una risorsa viene considerata protetta se contiene una delle seguenti proprietà di metadati (o entrambe):

* `xmpRights:WebStatement`: Questa proprietà si riferisce al percorso della pagina che contiene il contratto di licenza per la risorsa. `xmpRights:WebStatement` deve essere un percorso valido nel repository.
* `adobe_dam:restrictions`: Il valore di questa proprietà è un HTML non elaborato che specifica il contratto di licenza.


Se scegli di scaricare risorse protette da licenza, vieni reindirizzato al **[!UICONTROL Gestione del copyright]** a seconda delle proprietà dei metadati.

| `adobe_dam:restrictions` | `xmpRights:WebStatement` | Gestione copyright |
| --- | --- | --- |
| Sì | - | L’interfaccia viene visualizzata sia in Assets che in Brand Portal |
| - | Sì (percorso non valido) | Nessuna interfaccia |
| Sì | Sì (percorso non valido) | Nessuna interfaccia |
| Sì | Sì (percorso valido) | L’interfaccia viene visualizzata in Assets o Brand Portal </br> A seconda che il percorso sia valido per Assets o Brand Portal (o entrambi). |

![](assets/asset-copyright-mgmt.png)

Qui devi selezionare la risorsa da scaricare e accettare il contratto di licenza associato. Se non accetti il contratto di licenza, la **[!UICONTROL Scarica]** pulsante non abilitato.

![](assets/licensed-asset-download-2.png)

Se la selezione contiene più risorse protette, seleziona una risorsa alla volta, accetta il contratto di licenza e procedi con il download.

## Genera report sulle risorse scadute {#generate-report-about-expired-assets}

Gli amministratori possono generare e scaricare un elenco di tutte le risorse scadute entro un intervallo di tempo specifico. Questo rapporto include informazioni dettagliate, come dimensioni, tipo, percorso che specificano la posizione della risorsa nella gerarchia delle risorse, quando la risorsa è scaduta e quando è stata pubblicata, sulle risorse scadute. Le colonne di questo rapporto possono essere personalizzate per visualizzare più dati in base alle esigenze degli utenti.

![](assets/assets-expired.png)

Per ulteriori informazioni sulla funzione dei rapporti, consulta [Utilizzare i rapporti](../using/brand-portal-reports.md#work-with-reports).
