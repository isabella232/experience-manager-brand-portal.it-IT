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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Supporto video dinamico su Brand Portal {#dynamic-video-support-on-brand-portal}

Visualizzare in anteprima e riprodurre i video in modo adattivo [!DNL Brand Portal] con il supporto per contenuti multimediali dinamici. Scaricate anche le rappresentazioni dinamiche dal portale e dai collegamenti condivisi.
[!DNL Brand Portal] gli utenti possono:

* Visualizzare l'anteprima dei video nella pagina Dettagli risorsa, Visualizzazione a schede e condivisione di collegamenti.
* Riproducete le codifiche video nella pagina Dettagli risorsa.
* Visualizzare le rappresentazioni dinamiche nella scheda Rendering nella pagina Dettagli risorsa.
* Scaricate le codifiche video e le cartelle contenenti video.

>[!NOTE]
>
>Per lavorare con i video e pubblicarli, [!DNL Brand Portal]accertatevi che l'istanza [!DNL AEM] Autore sia impostata in modalità File multimediali dinamici o in [!DNL Scene 7] modalità File multimediali dinamici.

Per visualizzare in anteprima, riprodurre e scaricare i video, [!DNL Brand Portal] espone le due configurazioni seguenti agli amministratori:

* [Configurazione
Dynamic Media Ibrido](#configure-dm-hybrid-settings)Se [!DNL AEM] l'istanza Autore è in esecuzione sulla modalità ibrido ibrido.
* [Elemento multimediale dinamico [! Configurazione
DNL Scene 7]](#configure-dm-scene7-settings)Se l'istanza [!DNL AEM] Author è in esecuzione su un elemento multimediale[!DNL Scene 7] dinamico.
Impostate una di queste configurazioni in base alle configurazioni impostate nell'istanza [!DNL AEM] Autore con il [!DNL Brand Portal] quale tenant viene replicato.

>[!NOTE]
>
>I video dinamici non sono supportati sui [!DNL Brand Portal] tenant integrati con [!DNL AEM] l'autore in esecuzione nella [!UICONTROL modalità runmode Scene 7 Connect] .

## Come vengono riprodotti i video dinamici? {#how-are-dynamic-videos-played}

![Le codifiche video vengono recuperate dal cloud](assets/VideoEncodes.png)

Se configurazioni Dynamic Media ([Ibrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[! Configurazione di DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)[!DNL Brand Portal], le rappresentazioni dinamiche vengono recuperate dal [!DNL Scene 7] server. I codici video vengono quindi visualizzati in anteprima e riprodotti senza ritardo e distorsione nella qualità.

Poiché le codifiche video non sono memorizzate nell [!DNL Brand Portal] 'archivio e vengono recuperate dal [!DNL Scene 7] server, assicurati che le configurazioni Elemento multimediale dinamico su [!DNL AEM] Istanza autore siano [!DNL Brand Portal] uguali.

>[!NOTE]
>
>I visualizzatori video e i predefiniti per visualizzatori non sono supportati. [!DNL Brand Portal] I video vengono visualizzati in anteprima e riprodotti sui visualizzatori predefiniti in [!DNL Brand Portal].

## Prerequisiti {#prerequisites}

Per utilizzare i video dinamici su [!DNL Brand Portal], assicuratevi di:

* **Avvia[!DNL AEM]autore in modalità
DM (File multimediali dinamici)** Avvia l'istanza [!DNL AEM] Autore (con cui è integrata) [!DNL Brand Portal] In [modalità File multimediali dinamici](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) o Contenuti multimediali [dinamici [! DNL Scene 7].](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode)
* **Configura i servizi cloud Dynamic Media su[!DNL AEM]Author**
Based on the Dynamic Media Mode [!DNL AEM] Author is running, imposta i servizi cloud [Dynamic Media](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) o [[! DNL Scene 7] Servizi cloud](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) sull [!DNL AEM] 'autore da **Strumenti** | **Servizi cloud** | **Elemento multimediale dinamico**.
* **Configura Dynamic Media su Brand Portal**
in base alle configurazioni cloud di Dynamic Media in [!DNL AEM] Autore, configura [le impostazioni dei file multimediali dinamici](#configure-dm-hybrid-settings) o [[! Impostazioni DNL Scene 7](#configure-dm-scene7-settings) da [!DNL Brand Portal] strumenti amministrativi.
Verificate che [[! DNL Brand Portal] tenant](#separate-tenants) utilizzato per [!DNL AEM] le istanze Autore configurate con le modalità Dynamic Media Ibrido e Dynamic Media [!UICONTROL Scene 7] se utilizzate funzionalità di Dynamic Media Ibrido e Dynamic Media [!UICONTROL S 7].
* **Pubblicare cartelle con codifiche video applicate al portale
del marchio** Applicazione di [codifiche](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) video e Pubblicare la cartella contenente risorse multimediali avanzate da [!DNL AEM] Istanza autore a [!DNL Brand Portal].
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

Per verificare che le risorse video dinamiche vengano visualizzate in anteprima, riprodotte e scaricate da [!DNL Brand Portal] (e collegamenti condivisi), segui le seguenti pratiche:

### Tenant separato per modalità File multimediali dinamici e Scene Media Scene 7 {#separate-tenants}

Se utilizzate sia le funzioni Dynamic Media [!DNL Scene 7] che Dynamic Media Ibrido, si consiglia di utilizzare tenant diversi [!DNL Brand Portal] per [!DNL AEM] le istanze Autore configurate con [!DNL Scene 7] le modalità Dynamic Media Ibrido e Dynamic Media.
![Autore e BP una a una mappatura](assets/BPDynamicMedia.png)

### Stessi dettagli di configurazione nell'istanza AEM Author e nel portale brand

Assicurati che i dettagli di configurazione (come Titolo, ID registrazione, URL servizio video (in File multimediali diversi) e Titolo, le credenziali (E-mail e password), Regione, Società (in Contenuti multimediali [!DNL Scene 7]dinamici) siano identici in [!DNL Brand Portal] e [!DNL AEM] in configurazione cloud.

### Whitelist public egs ips for Dynamic Media Scene 7 mode

Se per distribuire le risorse video è utilizzata l'anteprima [protetta di Scene Media Scene 7](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html), [!DNL Brand Portal]Scene 7 stabilisce un server immagine dedicato per ambienti di staging o applicazioni interne. Qualsiasi richiesta a questo server controlla l'indirizzo IP di origine. Se la richiesta non proviene dall'elenco di indirizzi IP approvato, viene restituita una risposta non riuscita.
L'amministratore della società Scene -7, quindi, configura un elenco di indirizzi IP approvati per l'ambiente di verifica protetta della propria società tramite l'interfaccia utente di SPS (Scene -7 Publishing System). Accertatevi che l'IP di accesso per la rispettiva regione (da quanto segue) sia aggiunto all'elenco approvato.
Per inserire in una whitelist uno di questi IP di echi, vedete [preparare l'account per il servizio di verifica protetto](https://docs.adobe.com/content/help/en/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Gli IP di echi sono i seguenti:

| **Regione** | **IP di ammissione** |
|--- |--- |
| NA | 192.243.237.86 |
| EMEA | 185.34.189.4 |
| APAC | 63.140.44.54 |

## Configurare le impostazioni Dynamic Media (Ibrido) {#configure-dm-hybrid-settings}

Se [!DNL AEM] l'istanza Autore è in esecuzione in modalità ibrida per contenuti multimediali dinamici, utilizzate la sezione Video dal pannello Strumenti di amministrazione per configurare le impostazioni del gateway Dynamic Media.
>[!NOTE]
>
>I profili di codifica [video](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) non vengono pubblicati, [!DNL Brand Portal]bensì recuperati dal server Scene 7. Pertanto, per riprodurre correttamente le codifiche video [!DNL Brand Portal], assicuratevi che i dettagli di configurazione siano identici alla configurazione cloud [di Scene 7](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) nell'istanza [!DNL AEM] Autore.
Per configurare configurazioni Dynamic Media su [!DNL Brand Portal] tenant:

1. Selezionate il [!DNL AEM] logo per accedere agli strumenti amministrativi dalla barra degli strumenti in alto, in [!DNL Brand Portal].

2. Dal pannello Strumenti di amministrazione, selezionate la **sezione Video** .
   ![Configurazione ibrida Dynamic Media su Brand Portal](assets/DMHybrid-Video.png)
   **Si apre la pagina di configurazione** per l'elemento multimediale dinamico.
   ![Configurazione ibrida ibrida per contenuti multimediali su Brand Portal](assets/edit-dynamic-media-config.png)

3. Specificate **ID registrazione** e **URL servizio video** (URL-Gateway-Gateway). Assicurati che questi dettagli siano identici a quelli presenti in **Strumenti** &gt; **Servizi** cloud nell'istanza [!DNL AEM] Autore.

4. Selezionate **Salva** per salvare la configurazione.

## Configurare le impostazioni di Scene Media Scene 7 {#configure-dm-scene7-settings}

Se [!DNL AEM] l'istanza Autore è in esecuzione nella modalità File multimediali dinamici [!UICONTROL Scene 7] , utilizzate **la sezione Configurazione** file multimediali dinamica dal pannello Strumenti di amministrazione per configurare le [!UICONTROL impostazioni] del server Scene 7.

Per configurare configurazioni di Scene Scene Scene [!UICONTROL 7] su [!DNL Brand Portal] tenant:

1. Selezionate il [!DNL AEM] logo per accedere agli strumenti amministrativi dalla barra degli strumenti in alto, in [!DNL Brand Portal].

2. Dal pannello Strumenti di amministrazione, selezionate il riquadro **di configurazione** Elemento multimediale dinamico.
   ![Viene aperta la configurazione di Scene 7 DM nella [!DNL Brand Portal]](assets/DMS7-Tile.png)pagina Modifica configurazione file multimediale dinamica.
   ![Configurazione di Scene 7 [!DNL Brand Portal]](assets/S7Config.png)

3. Fornite:
   * Titolo
   * Credenziali (ID e-mail e password) per accedere al server Scene 7
   * Regione:
assicurati che questi valori siano identici a quelli dell'istanza [!DNL AEM] Autore.

4. Select **Connect to Dynamic Media**.

5. Fornite il nome **Società** e **salvate** la configurazione.
