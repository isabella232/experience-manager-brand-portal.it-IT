---
title: Supporto di video dinamici in Brand Portal
seo-title: Supporto di video dinamici in Brand Portal
description: Supporto di video dinamici in Brand Portal
seo-description: Supporto di video dinamici in Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 3%

---


# Supporto di video dinamici in Brand Portal {#dynamic-video-support-on-brand-portal}

Visualizzate in anteprima e riproducete i video in modo adattivo su Brand Portal con il supporto di Dynamic Media. Scaricate inoltre le rappresentazioni dinamiche dal portale e i collegamenti condivisi.
Gli utenti di Brand Portal possono:

* Visualizzate i video in anteprima nella pagina Dettagli risorsa, Visualizzazione a schede e Condivisione collegamento.
* Riproduci codifiche video nella pagina Dettagli risorsa.
* Visualizzare le rappresentazioni dinamiche nella scheda Rappresentazioni nella pagina Dettagli risorsa.
* Scaricate codifiche video e cartelle contenenti video.

>[!NOTE]
>
>Per lavorare con i video e pubblicarli su Brand Portal, accertatevi che l’istanza AEM Author sia configurata in modalità Dynamic Media Hybrid o in **[!DNL Scene 7]** modalità Dynamic Media.

Per visualizzare in anteprima, riprodurre e scaricare i video, Brand Portal espone agli amministratori le due configurazioni seguenti:

* [Configurazione](#configure-dm-hybrid-settings)ibrida Dynamic Media Se l&#39;istanza AEM Author è in esecuzione in modalità ibrida multimediale dinamica.
* [Dynamic [!DNL Scene 7] Mediaconfiguration](#configure-dm-scene7-settings)Se l&#39;istanza AEM Author è in esecuzione in modalità Dynamic Media **[!DNL Scene 7]** .
Impostate una di queste configurazioni in base alle configurazioni impostate nell&#39;istanza AEM Author con cui viene replicato il tenant di Brand Portal.

>[!NOTE]
>
>I video dinamici non sono supportati negli tenant del Brand Portal configurati con AEM Author in esecuzione in modalità di esecuzione di **[!UICONTROL Scene7 Connect]** .

## Come vengono riprodotti i video dinamici? {#how-are-dynamic-videos-played}

![Le codifiche video vengono recuperate dal cloud](assets/VideoEncodes.png)

Se le configurazioni Dynamic Media (configurazioni[ibride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) ) sono configurate sul Portale marchio, le rappresentazioni dinamiche vengono recuperate dal **[!DNL Scene 7]** server. Le codifiche video vengono quindi visualizzate in anteprima e riprodotte senza ritardi e con distorsione della qualità.

Poiché le codifiche video non sono memorizzate nell’archivio di Brand Portal e vengono recuperate dal **[!DNL Scene 7]** server, accertatevi che le configurazioni Dynamic Media in Istanza AEM Author e Portale marchio siano le stesse.

>[!NOTE]
>
>I visualizzatori video e i predefiniti per visualizzatori non sono supportati in Brand Portal. I video vengono visualizzati in anteprima e riprodotti sui visualizzatori predefiniti in Brand Portal.

## Prerequisiti {#prerequisites}

Per lavorare con video dinamici su Brand Portal, accertatevi di:

* **Avvia AEM Author in modalità** DM (Dynamic Media) Avvia l’istanza di AEM Author (con cui è configurato Brand Portal) in modalità [ibrida](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) Dynamic Media o in modalità [ [!DNL Scene 7] Dynamic](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)Mediamode.
* **Configurare i servizi cloud Dynamic Media su AEM Author** In base al AEM Author di modalità Dynamic Media è in esecuzione, impostare i servizi [cloud](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Dynamic Media o i servizi [[!DNL Scene 7] ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) cloud su AEM Author da **Strumenti** | Servizi **cloud** | **Dynamic Media**.
* **Configurare Dynamic Media su Brand Portal** In base alle configurazioni cloud Dynamic Media su AEM Author, configurare le impostazioni [](#configure-dm-hybrid-settings) Dynamic Media o [[!DNL Scene 7] le impostazioni](#configure-dm-scene7-settings) dagli strumenti amministrativi di Brand Portal.
Accertatevi che per le istanze AEM Author configurate con le modalità Dynamic Media Hybrid e Dynamic Media [Scene7](#separate-tenants) vengano utilizzati tenant **** separati di Brand Portal, se utilizzate le funzionalità di Dynamic Media Hybrid e Dynamic Media **[!UICONTROL S7]**.
* **Pubblicate cartelle con codifiche video applicate a Brand Portal** Applicate codifiche [video](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) e pubblicate la cartella contenente risorse multimediali dall’istanza AEM Author al Portale marchio.
* **gli IP di avanzamento in SPS se l’anteprima protetta è abilitata** Se utilizzate Dynamic Media-**[!DNL Scene 7]** (con l’anteprima [protetta abilitata](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) per una società), si consiglia all’amministratore della **[!DNL Scene 7]** società [inserire nell&#39;elenco Consentiti gli IP](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) di uscita pubblici per le rispettive regioni mediante l’interfaccia flash di SPS (**[!UICONTROL Scene 7]** Publishing System).
Gli IP Egress sono i seguenti:

| **Regione** | **IP Egress** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Per elencare uno di questi IP di uscita, vedete [preparare l&#39;account per un servizio](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)di verifica protetto.

## Best practice 

Per garantire che le risorse video dinamiche siano visualizzate in anteprima, riprodotte e scaricate correttamente dal Portale marchio (e dai collegamenti condivisi), seguite le seguenti procedure:

### Tenant separati per le modalità Dynamic Media Hybrid e Dynamic Media Scene 7 {#separate-tenants}

Se utilizzate sia le funzioni Dynamic Media **[!DNL Scene 7]** che le funzioni Dynamic Media Hybrid, si consiglia di utilizzare tenant Brand Portal diversi per le istanze AEM Author configurate con le modalità Dynamic Media Hybrid e Dynamic Media **[!DNL Scene 7]** .<br />

![Creazione e BP di una mappatura](assets/BPDynamicMedia.png)

### Stessi dettagli di configurazione per l’istanza AEM Author e il Brand Portal

Accertatevi che i dettagli di configurazione, quali **[!UICONTROL Titolo]**, ID **** registrazione, URL **[!UICONTROL servizio]** video (in **[!UICONTROL Dynamic Media Hybrid]**) e **[!UICONTROL Titolo]****** ******** **[!DNL Scene 7]******, credenziali (Email e Password), IDRegione, Societàvideo (in Dynamic Media) siano identici in Brand Portal e ad AEMcloud configurationPAPA.

###  Inserire nell&#39;elenco Consentiti gli IP delle uscite pubbliche per la modalità Dynamic Media Scene7

Se Dynamic Media **[!UICONTROL Scene 7]** dispone di un’anteprima [protetta abilitata](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)per distribuire risorse video al Portale del marchio, **[!UICONTROL Scene 7]** stabilisce un server di immagini dedicato per gli ambienti di pubblicazione per pre-produzione o le applicazioni interne. Qualsiasi richiesta a questo server controlla l’indirizzo IP di origine. Se la richiesta in entrata non si trova nell&#39;elenco approvato di indirizzi IP, viene restituita una risposta di errore.
L’amministratore della società **[!UICONTROL Scene-7]** configura quindi un elenco approvato di indirizzi IP per l’ambiente di verifica **** protetta della propria azienda, tramite **[!UICONTROL SPS]** (Scene-7 Publishing System) e l’interfaccia utente Flash. Accertatevi che l’IP di uscita per la rispettiva area geografica (tra le seguenti) sia aggiunto a tale elenco approvato.
Per elencare uno di questi IP di uscita, vedete [preparare l&#39;account per un servizio](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service)di verifica protetto.
Gli IP di uscita sono i seguenti:

| **Regione** | **IP Egress** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configurare le impostazioni Dynamic Media (ibrido) {#configure-dm-hybrid-settings}

Se l’istanza AEM Author è in esecuzione in modalità ibrida per contenuti multimediali dinamici, usate la sezione **[!UICONTROL Video]** dal pannello degli strumenti amministrativi per configurare le impostazioni del gateway Dynamic Media.

>[!NOTE]
>
>I profili [di codifica](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) video non vengono pubblicati sul Portale marchio, ma vengono recuperati dal server **[!UICONTROL Scene7]** . Per riprodurre correttamente le codifiche video in Brand Portal, accertatevi pertanto che i dettagli di configurazione siano identici a quelli della configurazione [[!UICONTROL cloud]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Scene7 nell’istanza AEM Author.

Per configurare le configurazioni Dynamic Media sui tenant di Brand Portal:

1. Selezionate il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore del Portale marchio.
1. Dal pannello degli strumenti di amministrazione, selezionate la sezione **[!UICONTROL Video]** .

   ![Configurazione ibrida Dynamic Media sul portale del marchio](assets/DMHybrid-Video.png)

   **[!UICONTROL Viene visualizzata la pagina Modifica configurazione]** Dynamic Media.

   ![Configurazione ibrida Dynamic Media su Brand Portal](assets/edit-dynamic-media-config.png)

1. Specificate l&#39;ID **** registrazione e l&#39;URL **[!UICONTROL del servizio]** video (URL gateway DM). Accertati che questi dettagli siano identici a quelli disponibili in **[!UICONTROL Strumenti > Servizi]** cloud nell’istanza AEM Author.
1. Selezionate **Salva** per salvare la configurazione.

## Configurare le impostazioni di Dynamic Media Scene7 {#configure-dm-scene7-settings}

Se l’istanza AEM Author è in esecuzione in modalità Dynamic Media- **[!UICONTROL Scene 7]** , usate la sezione Configurazione **** Dynamic Media dal pannello degli strumenti di amministrazione per configurare le impostazioni del server di **[!UICONTROL Scene 7]** .

Per configurare le configurazioni di Dynamic Media **[!UICONTROL Scene 7]** per gli tenant di Brand Portal:

1. Selezionate il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore del Portale marchio.

2. Dal pannello degli strumenti di amministrazione, selezionate la sezione Configurazione **** Dynamic Media.<br />
   ![Configurazione DM [!UICONTROL Scene 7] su Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Viene visualizzata la pagina Modifica configurazione]** Dynamic Media.<br />
   ![Configurazione di Scene7 su Brand Portal](assets/S7Config.png)

3. Fornisci:
   * **[!UICONTROL Titolo]**
   * Credenziali (ID **[!UICONTROL e-]** mail e **[!UICONTROL password]**) per accedere al server Scene7
   * **[!UICONTROL Regione]** Assicurarsi che questi valori siano identici a quelli dell&#39;istanza AEM Author.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. Immettete il nome **[!UICONTROL della]** società e **[!UICONTROL salvate]** la configurazione.
