---
title: Supporto video dinamico su Brand Portal
seo-title: Supporto video dinamico su Brand Portal
description: Supporto video dinamico su Brand Portal
seo-description: Supporto video dinamico su Brand Portal
uuid: a 3502 a 4 d -3971-4 ea 4-953 c -44 ba 04446269
contentOwner: mgulati
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: riferimento
topic-tags: download-install
discoiquuid: e 18 d 992 a-a 3 b 5-45 f 2-9696-8161993213 ee
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Supporto video dinamico su Brand Portal {#dynamic-video-support-on-brand-portal}

Visualizzare in anteprima e riprodurre i video in modo adattivo su Brand Portal con supporto per contenuti multimediali dinamici. Scaricate anche le rappresentazioni dinamiche dal portale e dai collegamenti condivisi.
Gli utenti del Portale brand possono:

* Visualizzare l'anteprima dei video nella pagina Dettagli risorsa, Visualizzazione a schede e condivisione di collegamenti.
* Riproducete le codifiche video nella pagina Dettagli risorsa.
* Visualizzare le rappresentazioni dinamiche nella scheda Rendering nella pagina Dettagli risorsa.
* Scaricate le codifiche video e le cartelle contenenti video.

>[!NOTE]
>
>Per lavorare con i video e per pubblicarli sul portale marchio, accertatevi che l'istanza AEM Author sia impostata su Modalità Media ibrida o su File multimediali [!DNL Scene 7] dinamici.

Per visualizzare in anteprima, riprodurre e scaricare i video, il portale marchio espone le due configurazioni seguenti agli amministratori:

* [Configurazione elemento multimediale dinamico Se](#configure-dm-hybrid-settings)
l'istanza AEM Author è in esecuzione sulla modalità ibrida di elementi multimediali dinamici.
* [Elemento multimediale dinamico [! Configurazione
DNL Scene 7]](#configure-dm-scene7-settings)Se l'istanza AEM Author è in esecuzione su elementi multimediali[!DNL Scene 7] dinamici.
Impostate una di queste configurazioni in base alle configurazioni impostate nell'istanza AEM Author con il tenant di Brand Portal.

>[!NOTE]
>
>I video dinamici non sono supportati sui tenant di Brand Portal integrati con AEM Author in esecuzione in [!UICONTROL Scene 7 Connect] .

## Come vengono riprodotti i video dinamici? {#how-are-dynamic-videos-played}

![Le codifiche video vengono recuperate dal cloud](assets/VideoEncodes.png)

Se configurazioni Dynamic Media ([Ibrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[! Le](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurazioni DNL Scene 7] sono configurate sul portale brand, le rappresentazioni dinamiche vengono recuperate dal [!DNL Scene 7] server. I codici video vengono quindi visualizzati in anteprima e riprodotti senza ritardo e distorsione nella qualità.

Poiché le codifiche video non sono memorizzate nell'archivio di Brand Portal e vengono recuperate dal [!DNL Scene 7] server, assicurati che le configurazioni Contenuti multimediali dinamici in AEM Author Instance e Brand Portal siano uguali.

>[!NOTE]
>
>I visualizzatori video e i predefiniti per visualizzatori non sono supportati nel portale del marchio. I video vengono visualizzati in anteprima e riprodotti sui visualizzatori predefiniti in Brand Portal.

## Prerequisiti {#prerequisites}

Per lavorare con i video dinamici sul portale marchio, assicuratevi di:

* **Avviate AEM Author in modalità
DM (Elementi multimediali dinamici)** Avvia l'istanza AEM Author (con il quale il portale del brand è integrato) in [modalità File multimediali dinamici](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) o Contenuti multimediali [dinamici [! DNL Scene 7].](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)
* **Configura i servizi cloud di Dynamic Media su AEM Author**
Based in the Dynamic Media mode is running on, set either of [Dynamic Media cloud services](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) or [[! Servizi](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) cloud DNL Scene 7] su AEM Author da **Strumenti** | **Servizi cloud** | **Elemento multimediale dinamico**.
* **Configura Dynamic Media su Brand Portal**
in base alle configurazioni cloud di Media Media in AEM Author, configura [le impostazioni dei file multimediali dinamici](#configure-dm-hybrid-settings) o [[! Impostazioni DNL Scene 7]](#configure-dm-scene7-settings) dagli strumenti di amministrazione di Brand Portal.
Accertatevi che i tenant [separati del Portale brand](#separate-tenants) vengano utilizzati per le istanze AEM Author configurate con le modalità File multimediali dinamici e Scene Media [!UICONTROL Scene 7] se utilizzate funzionalità di Dynamic Media Ibrido e Dynamic Media [!UICONTROL S 7].
* **Pubblicare cartelle con codifiche video applicate al Portale
del brand** Applicano [codifiche video](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) e pubblicare la cartella contenente risorse multimediali avanzate dall'istanza AEM Author al portale del brand.
* **Whitelist Egress IP in SPS se l'anteprima protetta è abilitata**
se l'utilizzo di Contenuti multimediali dinamici[!DNL Scene 7] (con [anteprima protetta attivata](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) per una società), si consiglia all'amministratore [!DNL Scene 7] della società [di inserire gli IP di echi pubblici](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) per le rispettive aree utilizzando l'interfaccia utente SPS ([!UICONTROL Scene 7] Publishing System).
Gli IP di Egress sono i seguenti:

| **Regione** | **IP di ammissione** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

Per inserire in una whitelist uno di questi IP di echi, vedete [preparare l'account per il servizio di verifica protetto](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best practice

Per verificare che le risorse video dinamiche vengano visualizzate in anteprima, riprodotte e scaricate da Portal (e collegamenti condivisi), seguite le seguenti pratiche:

### Tenant separato per modalità File multimediali dinamici e Scene Media Scene 7 {#separate-tenants}

Se utilizzate sia le funzioni Dynamic Media [!DNL Scene 7] che Dynamic Media Ibrido, si consiglia di utilizzare i diversi tenant Brand Portal per le istanze AEM Author configurate con [!DNL Scene 7] le modalità Dynamic Media Ibrido e Dynamic Media.
![Autore e BP una a una mappatura](assets/BPDynamicMedia.png)

### Stessi dettagli di configurazione nell'istanza AEM Author e nel portale brand

Assicurati che i dettagli di configurazione ( [!UICONTROL come Titolo], [!UICONTROL ID registrazione], [!UICONTROL URL servizio video] (in [!UICONTROL Elemento multimediale dinamico)]e [!UICONTROL Titolo], le credenziali ([!UICONTROL E-mail] e password), [!UICONTROL Regione], [!UICONTROL Società] (in Contenuti multimediali [!DNL Scene 7]dinamici) siano identici in Portale marchio e [!UICONTROL configurazione cloud AEM].

### Whitelist public egs ips for Dynamic Media Scene 7 mode

Se per distribuire le risorse video al portale del brand viene utilizzata l'anteprima protetta di Scene Media [!UICONTROL Scene 7][](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html), [!UICONTROL Scene 7] stabilisce un server di immagini dedicato per ambienti di staging o applicazioni interne. Qualsiasi richiesta a questo server controlla l'indirizzo IP di origine. Se la richiesta non proviene dall'elenco di indirizzi IP approvato, viene restituita una risposta non riuscita.
L'amministratore della società [!UICONTROL Scene -7] , quindi, configura un elenco di indirizzi IP approvati per l'ambiente di verifica [!UICONTROL protetta della propria] società tramite [!UICONTROL l'interfaccia utente di SPS] (Scene -7 Publishing System). Accertatevi che l'IP di accesso per la rispettiva regione (da quanto segue) sia aggiunto all'elenco approvato.
Per inserire in una whitelist uno di questi IP di echi, vedete [preparare l'account per il servizio di verifica protetto](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Gli IP di echi sono i seguenti:

| **Regione** | **IP di ammissione** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configurare le impostazioni Dynamic Media (Ibrido) {#configure-dm-hybrid-settings}

Se l'istanza AEM Author è in esecuzione in modalità ibrida per contenuti multimediali dinamici, utilizzate [!UICONTROL la sezione Video] dal pannello Strumenti di amministrazione per configurare le impostazioni del gateway Dynamic Media.
>[!NOTE]
>
>I profili di codifica [video non](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) vengono pubblicati sul portale di brand, bensì vengono estratti dal server [!UICONTROL Scene 7] . Pertanto, per riprodurre correttamente le codifiche video nel portale brand, assicuratevi che i dettagli di configurazione siano identici a quelli di [[! Configurazione cloud UICONTROL Scene 7](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) nell'istanza AEM Author.
Per configurare configurazioni Dynamic Media sui tenant di Brand Portal:

1. Selezionate il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore del portale marchio.

2. Dal pannello Strumenti di amministrazione, selezionate la **[!UICONTROL sezione Video]** .

![Configurazione ibrida Dynamic Media su Brand Portal](assets/DMHybrid-Video.png)

**[!UICONTROL Si apre la pagina di configurazione]** per l'elemento multimediale dinamico.

![Configurazione ibrida ibrida per contenuti multimediali su Brand Portal](assets/edit-dynamic-media-config.png)

3. Specificate **[!UICONTROL ID registrazione]** e **[!UICONTROL URL servizio video]** (URL-Gateway-Gateway). Assicurati che questi dettagli siano identici a quelli presenti in **[!UICONTROL Strumenti &gt; Servizi]** cloud nell'istanza AEM Author.

4. Selezionate **Salva** per salvare la configurazione.

## Configurare le impostazioni di Scene Media Scene 7 {#configure-dm-scene7-settings}

Se l'istanza AEM Author è in esecuzione nella modalità File multimediali dinamici [!UICONTROL di Scene 7] , utilizzate **[!UICONTROL la sezione Configurazione]** file multimediali dinamica dal pannello Strumenti di amministrazione per configurare le [!UICONTROL impostazioni] del server Scene 7.

Per configurare configurazioni di Scene [!UICONTROL 7] Dynamic Media su Brand Portal:

1. Selezionate il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore del portale marchio.

2. Dal pannello Strumenti di amministrazione, selezionate il riquadro **[!UICONTROL di configurazione]** Elemento multimediale dinamico.
   ![Configurazione di DM [!UICONTROL Scene 7] su Brand Portal](assets/DMS7-Tile.png)

[!UICONTROL Si apre la pagina di configurazione] per l'elemento multimediale dinamico.

![Configurazione di Scene 7 su Brand Portal](assets/S7Config.png)

3. Fornite:
   * [!UICONTROL Titolo]
   * Credenziali ([!UICONTROL ID e-mail] e [!UICONTROL password]) per accedere al server Scene 7
   * [!UICONTROL Regione]:
assicurati che questi valori siano identici a quelli dell'istanza AEM Author.

4. Select **[!UICONTROL Connect to Dynamic Media]**.

5. Fornite il nome **[!UICONTROL Società]** e **[!UICONTROL salvate]** la configurazione.
