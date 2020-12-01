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
source-wordcount: '1207'
ht-degree: 3%

---


# Supporto di video dinamici in Brand Portal {#dynamic-video-support-on-brand-portal}

Visualizzate in anteprima e riproducete i video in modo adattivo su Brand Portal con il supporto per contenuti multimediali dinamici. Scaricate inoltre le rappresentazioni dinamiche dal portale e i collegamenti condivisi.
Gli utenti di Brand Portal possono:

* Visualizzate i video in anteprima nella pagina Dettagli risorsa, Visualizzazione a schede e Condivisione collegamento.
* Riproduci codifiche video nella pagina Dettagli risorsa.
* Visualizzare le rappresentazioni dinamiche nella scheda Rappresentazioni nella pagina Dettagli risorsa.
* Scaricate codifiche video e cartelle contenenti video.

>[!NOTE]
>
>Per lavorare con i video e pubblicarli su Brand Portal, accertatevi che l’istanza di AEM Author sia configurata in modalità Dynamic Media Hybrid o Dynamic Media **[!DNL Scene 7]**.

Per visualizzare in anteprima, riprodurre e scaricare i video, Brand Portal espone agli amministratori le due configurazioni seguenti:

* [Dynamic Media Hybrid ](#configure-dm-hybrid-settings)
configurationSe l’istanza di AEM Author è in esecuzione su un supporto dinamico in modalità ibrida.
* [Dynamic  [!DNL Scene 7] ](#configure-dm-scene7-settings)
MediaconfigurationSe l&#39;istanza di AEM Author è in esecuzione in **[!DNL Scene 7]** modalità multimediale dinamica.
Imposta una di queste configurazioni in base alle configurazioni impostate nell&#39;istanza di AEM Author con cui viene replicato il tenant di Brand Portal.

>[!NOTE]
>
>I video dinamici non sono supportati sui tenant del Brand Portal configurati con AEM Author in esecuzione in modalità di esecuzione **[!UICONTROL Scene7Connect]**.

## Come vengono riprodotti i video dinamici? {#how-are-dynamic-videos-played}

![Le codifiche video vengono recuperate dal cloud](assets/VideoEncodes.png)

Se in Brand Portal sono configurate configurazioni per contenuti multimediali dinamici ([Hybrid](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)), le rappresentazioni dinamiche vengono recuperate dal server **[!DNL Scene 7]**. Le codifiche video vengono quindi visualizzate in anteprima e riprodotte senza ritardi e con distorsione della qualità.

Poiché le codifiche video non sono memorizzate nell’archivio di Brand Portal e vengono recuperate dal server **[!DNL Scene 7]**, accertati che le configurazioni per i contenuti multimediali dinamici in AEM Author Instance e Brand Portal siano le stesse.

>[!NOTE]
>
>I visualizzatori video e i predefiniti per visualizzatori non sono supportati in Brand Portal. I video vengono visualizzati in anteprima e riprodotti sui visualizzatori predefiniti in Brand Portal.

## Prerequisiti {#prerequisites}

Per lavorare con video dinamici su Brand Portal, accertatevi di:

* **Avvia AEM Author in**
modalità DM (Dynamic Media)Avvia l’istanza di AEM Author (con cui è configurato Brand Portal) su  [Dynamic Media Hybrid ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) modeor  [Dynamic  [!DNL Scene 7] Mediamode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configurare i servizi Dynamic Media Cloud su AEM**
AuthorIn base alla modalità Dynamic Media su cui è in esecuzione AEM Author, impostare uno dei  [servizi ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) Dynamic Media Cloud o  [[!DNL Scene 7] cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) service su AEM Author da  **Strumenti** |  **Cloud Services** |  **** Dynamic Media.
* **Configurare gli elementi multimediali dinamici su Brand**
PortalIn base alle configurazioni cloud Dynamic Media su AEM Author, configurare le  [impostazioni ](#configure-dm-hybrid-settings) Contenuti multimediali dinamici o  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  le impostazioni dagli strumenti amministrativi di Brand Portal.
Accertatevi che [tenant del Brand Portal separati](#separate-tenants) siano utilizzati per le istanze di AEM Author configurate con le modalità Dynamic Media Hybrid and Dynamic Media **[!UICONTROL Scene7]**, se state utilizzando funzionalità di Dynamic Media Hybrid e Dynamic Media **[!UICONTROL S7]**.
* **Pubblicare cartelle con codifiche video applicate a Brand**
PortalApplicare codifiche  [video ](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) e pubblicare la cartella contenente risorse multimediali dall’istanza di AEM Author al Portale del marchio.
* **gli IP di avanzamento in SPS se è**
abilitata l’anteprima protettaSe si utilizza un elemento multimediale dinamico **[!DNL Scene 7]** (con anteprima  [protetta ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) abilitata per una società), si consiglia all’amministratore della  **[!DNL Scene 7]** società  [ inserire nell&#39;elenco Consentiti di Inserire nell&#39;elenco Consentiti di ](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) IP di pubblico dominio per le rispettive regioni mediante l’interfaccia flash di SPS (**[!UICONTROL Scene 7]** Publishing System).
Gli IP Egress sono i seguenti:

| **Regione** | **IP Egress** |
|--- |--- |
| NA | 192,243,237,86 |
| EMEA | 185,34,189,4 |
| APAC | 63,140,44,54 |

Per elencare uno di questi IP di uscita, vedere [preparare l&#39;account per un servizio di verifica protetto](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best practice  

Per garantire che le risorse video dinamiche siano visualizzate in anteprima, riprodotte e scaricate correttamente dal Portale marchio (e dai collegamenti condivisi), seguite le seguenti procedure:

### Tenant separati per le modalità Dynamic Media Hybrid e Dynamic Media Scene 7 {#separate-tenants}

Se utilizzate sia le funzioni per contenuti multimediali dinamici **[!DNL Scene 7]** che le funzioni per file multimediali ibridi dinamici, per le istanze di AEM Author è consigliabile utilizzare locatari di Brand Portal diversi.**[!DNL Scene 7]**<br />

![Creazione e BP di una mappatura](assets/BPDynamicMedia.png)

### Stessi dettagli di configurazione per l’istanza di AEM Author e il Brand Portal

Assicurarsi che i dettagli di configurazione, come **[!UICONTROL Titolo]**, **[!UICONTROL ID registrazione]**, **[!UICONTROL URL servizio video]** (in **[!UICONTROL Elemento multimediale dinamico ibrido]**) e **[!UICONTROL Titolo]**, le credenziali (**[!UICONTROL E-mail]** e la password), a12/>Regione ]**,**[!UICONTROL  Società&#x200B;]**(in Contenuti multimediali dinamici **[!DNL Scene 7]**) sono uguali in Portale marchio e**[!UICONTROL  AEM configurazione cloud ]**.**[!UICONTROL 

###  Inserire nell&#39;elenco Consentiti gli IP delle uscite pubbliche per la modalità Dynamic Media Scene 7

Se si utilizza l’elemento multimediale dinamico **[!UICONTROL Scene7]** con [anteprima protetta abilitata](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) per distribuire risorse video al Portale marchio, **[!UICONTROL Scene7]** stabilisce un server di immagini dedicato per gli ambienti di pubblicazione per l’area di visualizzazione e le applicazioni interne. Qualsiasi richiesta a questo server controlla l’indirizzo IP di origine. Se la richiesta in entrata non si trova nell&#39;elenco approvato di indirizzi IP, viene restituita una risposta di errore.
L&#39;amministratore della **[!UICONTROL società Scene-7]** configura pertanto un elenco approvato di indirizzi IP per l&#39;ambiente **[!UICONTROL Secure Testing]** della propria azienda, tramite l&#39;interfaccia flash **[!UICONTROL SPS]** (Scene-7 Publishing System). Accertatevi che l’IP di uscita per la rispettiva area geografica (tra le seguenti) sia aggiunto a tale elenco approvato.
Per elencare uno di questi IP di uscita, vedere [preparare l&#39;account per un servizio di verifica protetto](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Gli IP di uscita sono i seguenti:

| **Regione** | **IP Egress** |
|--- |--- |
| NA | 192,243,237,86 |
| EMEA | 185,34,189,4 |
| APAC | 63,140,44,54 |

## Configurare le impostazioni per elementi multimediali dinamici (ibridi) {#configure-dm-hybrid-settings}

Se l&#39;istanza di AEM Author è in esecuzione in modalità ibrida per contenuti multimediali dinamici, utilizzate la sezione **[!UICONTROL Video]** dal pannello degli strumenti amministrativi per configurare le impostazioni del gateway per contenuti multimediali dinamici.

>[!NOTE]
>
>I [profili di codifica video](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) non vengono pubblicati nel Portale marchio, ma vengono recuperati dal server **[!UICONTROL Scene7]**. Pertanto, affinché le codifiche video vengano riprodotte correttamente in Brand Portal, accertatevi che i dettagli di configurazione siano gli stessi della [[!UICONTROL configurazione cloud Scene7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) nell&#39;istanza di AEM Author.

Per impostare configurazioni per contenuti multimediali dinamici su tenant di Brand Portal:

1. Selezionate il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore, in Brand Portal.
1. Dal pannello degli strumenti di amministrazione, selezionate la sezione **[!UICONTROL Video]**.

   ![Configurazione ibrida elementi multimediali dinamici su Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Viene visualizzata la pagina Modifica]** configurazione elemento multimediale dinamico.

   ![Dynamic Media Hybrid Configuration on Brand Portal](assets/edit-dynamic-media-config.png)

1. Specificate **[!UICONTROL ID registrazione]** e **[!UICONTROL URL servizio video]** (URL gateway DM). Assicurati che questi dettagli siano identici a quelli presenti in **[!UICONTROL Strumenti > Cloud Services]** nell&#39;istanza di AEM Author.
1. Selezionare **Save** per salvare la configurazione.

## Configurare le impostazioni Scene7 per contenuti multimediali dinamici {#configure-dm-scene7-settings}

Se l’istanza di AEM Author è in esecuzione in modalità Dynamic Media- **[!UICONTROL Scene7]**, usate la sezione **[!UICONTROL Configurazione Dynamic Media]** dal pannello degli strumenti di amministrazione per configurare le impostazioni del server **[!UICONTROL Scene7]**.

Per impostare configurazioni per contenuti multimediali dinamici **[!UICONTROL Scene7]** su tenant di Brand Portal:

1. Selezionate il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore, in Brand Portal.

2. Dal pannello degli strumenti di amministrazione, selezionate la sezione **[!UICONTROL Configurazione elemento multimediale dinamico]**.<br />
   ![DM  [!UICONTROL Scene7 ] configuration on Brand Portal](assets/DMS7-Tile.png)
   **[!UICONTROL Viene visualizzata la pagina Modifica]** configurazione elemento multimediale dinamico.<br />
   ![Configurazione di Scene7 su Brand Portal](assets/S7Config.png)

3. Fornisci:
   * **[!UICONTROL Titolo]**
   * Credenziali (**[!UICONTROL ID e-mail]** e **[!UICONTROL Password]**) per accedere al server Scene7
   * ****
Regione: accertati che questi valori siano identici a quelli dell’istanza di AEM Author.

4. Selezionare **[!UICONTROL Connetti a elemento multimediale dinamico]**.

5. Fornire il **[!UICONTROL Nome società]** e **[!UICONTROL Salvare]** la configurazione.
