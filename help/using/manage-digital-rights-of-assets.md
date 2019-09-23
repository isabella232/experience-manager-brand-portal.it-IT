---
title: Gestione dei diritti digitali delle risorse
seo-title: Gestione dei diritti digitali delle risorse
description: Le risorse di licenza e l’impostazione della scadenza per le risorse e i collegamenti condivisi garantiscono l’utilizzo controllato di tali risorse e la loro salvaguardia.
seo-description: Le risorse di licenza e l’impostazione della scadenza per le risorse e i collegamenti condivisi garantiscono l’utilizzo controllato di tali risorse e la loro salvaguardia.
uuid: ce30e398-0109-41bf-a4d2-2fcca476f499
contentOwner: bdhar
topic-tags: download-install
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: riferimento
discoiquuid: f77003ba-31fe-4a9e-96c8-dbc4c2eba79e
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Gestione dei diritti digitali delle risorse {#manage-digital-rights-of-assets}

Garantire la distribuzione e l'utilizzo sicuri delle risorse creative e del materiale del marchio è fondamentale per proteggere il marchio. Questo può essere imposto sia all’interno dell’organizzazione che all’esterno associando una data (e un’ora) di scadenza alle risorse approvate pubblicate da AEM al Brand Portal, o concedendo in licenza queste risorse per l’uso condizionale. Inoltre, Brand Portal consente di specificare una data di scadenza per i collegamenti alle risorse condivise da Brand Portal.

Continua a leggere per scoprire in che modo le risorse sono protette su Brand Portal e comprendere le relative autorizzazioni di utilizzo.

## Scadenza risorsa {#asset-expiration}

La scadenza delle risorse è un modo efficace per controllare l’utilizzo delle risorse approvate su Brand Portal in tutta l’organizzazione. Tutte le risorse pubblicate da AEM Assets al Portale marchio possono avere una data di scadenza, che limita l’utilizzo di tali risorse a seconda dei diversi ruoli utente.

### Autorizzazioni di utilizzo relative alle risorse scadute {#usage-permissions-expired-assets}

In Brand Portal, gli amministratori possono visualizzare, scaricare e aggiungere le risorse scadute alle raccolte. mentre gli editor e i visualizzatori possono visualizzare e aggiungere solo le risorse scadute alle raccolte.

Gli amministratori possono pubblicare le risorse scadute da AEM Assets al Brand Portal. Tuttavia, le risorse scadute non possono essere condivise tramite collegamento da Brand Portal. Se selezionate una risorsa scaduta da una cartella contenente risorse scadute e non scadute, l’azione **[!UICONTROL Condividi collegamento]** non è disponibile. Tuttavia, se selezionate una cartella contenente risorse scadute e non scadute, sono disponibili le azioni [!UICONTROL Condividi] e Collegamento **** condivisione.

>[!NOTE]
>
>Una cartella può comunque essere condivisa come collegamento, anche se contiene risorse scadute. In questo caso, il collegamento non elenca le risorse scadute e vengono condivise solo le risorse non scadute.

Nella tabella seguente sono visualizzate le autorizzazioni di utilizzo delle risorse scadute:

|  | **[!UICONTROL Condivisione collegamenti]** | **[!UICONTROL Scarica]** | **[!UICONTROL Proprietà]** | **[!UICONTROL Aggiungi alla raccolta]** | **[!UICONTROL Elimina]** |
|---|---|---|---|---|---|
| **[!UICONTROL Amministratore]** | Non disponibile | Disponibile | Disponibile | Disponibile | Disponibile |
| **[!UICONTROL Editor]** | Non disponibile | Non disponibile | Disponibile | Disponibile | Non disponibile |
| **[!UICONTROL Visualizzatore]** | Non disponibile | Non disponibile | Disponibile | Disponibile | Non disponibile |
| **[!UICONTROL Utente ospite]** | Non disponibile | Non disponibile | Disponibile | Disponibile | Non disponibile |

>[!NOTE]
>
>Se Visualizzatori ed editor scaricano una cartella contenente risorse scadute e non scadute, vengono scaricate solo le risorse non scadute. Se una cartella contiene solo risorse scadute, viene scaricata una cartella vuota.

### Stato di scadenza delle risorse {#expiration-status-of-assets}

Potete visualizzare lo stato di scadenza delle risorse nella loro vista [!UICONTROL a]schede. Un flag rosso sulla scheda indica che la risorsa è scaduta.

![](assets/expired_assets_cardview.png)

>[!NOTE]
>
>Le viste Elenco e Colonna non visualizzano lo stato di scadenza delle risorse.

## Scadenza collegamento risorsa {#asset-link-expiration}

Durante la condivisione delle risorse tramite i collegamenti, gli amministratori e gli editor possono impostare una data e un'ora di scadenza utilizzando il campo **[!UICONTROL Scadenza]** della finestra di dialogo Condivisione **** collegamento. La scadenza predefinita del collegamento è di sette giorni dalla data in cui il collegamento viene condiviso.

![](assets/asset-link-sharing.png)

Garantisce che le risorse condivise come collegamenti scadano alla data e all’ora stabilite dagli amministratori e dagli editor del Brand Portal e non possono più essere visualizzate e scaricate oltre la data di scadenza. Poiché le risorse condivise tramite i collegamenti possono essere visualizzate anche da utenti esterni che non fanno parte dell’organizzazione, specificando la scadenza potete assicurarvi che le risorse approvate siano protette e non esposte a entità sconosciute oltre un determinato periodo di tempo.

Per ulteriori informazioni sulla condivisione dei collegamenti, consulta [Condivisione di risorse come collegamento](../using/brand-portal-link-share.md).

## Risorse con licenza {#licensed-assets}

Le risorse concesse in licenza sono soggette all’accettazione di un contratto di licenza prima di essere scaricate dal Brand Portal. Questo accordo per le risorse con licenza viene fornito quando scaricate direttamente la risorsa dal Portale marchio o tramite un collegamento condiviso. Sia che siano scadute o meno, le risorse protette da licenza possono essere visualizzate da tutti gli utenti. Tuttavia, il download e l’utilizzo delle risorse con licenza scadute sono limitati. Per informazioni sul comportamento delle risorse con licenza scadute e delle attività consentite in base ai ruoli utente, consultate le autorizzazioni di [utilizzo delle risorse](../using/manage-digital-rights-of-assets.md#usage-permissions-expired-assets)scadute.

Alle risorse protette da licenza è associato [un contratto di](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) licenza, che viene fatto impostando la proprietà [](https://helpx.adobe.com/experience-manager/6-5/assets/using/drm.html#DigitalRightsManagementinAssets) metadati della risorsa in AEM Assets.

Se scegli di scaricare le risorse protette da licenza, verrai reindirizzato alla pagina Gestione  copyright.

![](assets/asset-copyright-mgmt.png)

Qui è necessario selezionare la risorsa per scaricare e accettare il contratto di licenza associato. Se non accettate il contratto di licenza, il pulsante [!UICONTROL Scarica] non è attivato.

![](assets/licensed-asset-download-2.png)

Se la selezione contiene più risorse protette, selezionate una risorsa alla volta, accettate il contratto di licenza e continuate a scaricare la risorsa.

## Genera report sulle risorse scadute {#generate-report-about-expired-assets}

Gli amministratori possono generare e scaricare un rapporto in cui sono elencate tutte le risorse scadute entro un intervallo di tempo specifico. Il rapporto contiene informazioni dettagliate: come dimensione, tipo, percorso che specifica la posizione della risorsa nella gerarchia delle risorse, quando la risorsa è scaduta e quando è stata pubblicata. informazioni sulle risorse scadute. Le colonne di questo rapporto possono essere personalizzate per visualizzare più dati in base alle esigenze degli utenti.

![](assets/assets-expired.png)

Per ulteriori informazioni sulla funzione dei rapporti, consulta [Operazioni con i rapporti](../using/brand-portal-reports.md#work-with-reports).
