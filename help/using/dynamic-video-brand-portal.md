---
title: Supporto di video dinamici in Brand Portal
seo-title: Dynamic video support on Brand Portal
description: Supporto di video dinamici in Brand Portal
seo-description: Dynamic video support on Brand Portal
uuid: a3502a4d-3971-4ea4-953c-44ba04446269
contentOwner: mgulati
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: download-install
discoiquuid: e18d992a-a3b5-45f2-9696-8161993213ee
exl-id: 08d6a0fb-061e-4bef-b8e2-bb8522e7482e
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '1190'
ht-degree: 2%

---

# Supporto di video dinamici in Brand Portal {#dynamic-video-support-on-brand-portal}

Anteprima e riproduzione di video in modo adattivo su Brand Portal con supporto Dynamic Media. Scarica anche le rappresentazioni dinamiche dal portale e i collegamenti condivisi.
Gli utenti Brand Portal possono:

* Visualizzare in anteprima i video nella pagina Dettagli risorsa, nella Vista a schede e nella pagina di anteprima della condivisione dei collegamenti.
* Riproduci le codifiche video nella pagina Dettagli risorsa .
* Visualizza rappresentazioni dinamiche nella scheda Rendering della pagina Dettagli risorsa.
* Scarica le codifiche video e le cartelle contenenti video.

>[!NOTE]
>
>Per lavorare con i video e pubblicarli in Brand Portal, accertati che l’istanza di authoring di Experience Manager sia configurata in modalità ibrida Dynamic Media o in modalità Dynamic Media **[!DNL Scene 7]** .

Per visualizzare in anteprima, riprodurre e scaricare i video, Brand Portal espone le due configurazioni seguenti agli amministratori:

* [Configurazione ibrida di Dynamic MediaSe l’istanza di authoring di Experience Manager è in esecuzione in modalità ibrida di contenuti multimediali dinamici. ](#configure-dm-hybrid-settings)

* [Dynamic  [!DNL Scene 7] ](#configure-dm-scene7-settings)
MediaconfigurationSe l&#39;istanza di authoring di Experience Manager è in esecuzione in **[!DNL Scene 7]** modalità Dynamic Media.
Imposta una di queste configurazioni in base alle configurazioni impostate nell’istanza di authoring di Experience Manager con cui viene replicato il tenant Brand Portal.

>[!NOTE]
>
>I video dinamici non sono supportati sui tenant Brand Portal configurati con Experience Manager Author in esecuzione in modalità runmode **[!UICONTROL Scene7Connect]**.

## Come vengono riprodotti i video dinamici? {#how-are-dynamic-videos-played}

![Le codifiche video vengono recuperate dal cloud](assets/VideoEncodes.png)

Se le configurazioni di Dynamic Media ([Configurazioni ibride](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene 7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings)) sono impostate su Brand Portal, le rappresentazioni dinamiche vengono recuperate dal server **[!DNL Scene 7]**. Le codifiche video vengono quindi visualizzate in anteprima e riprodotte senza ritardi e con distorsione nella qualità.

Poiché le codifiche video non sono memorizzate nell’archivio Brand Portal e vengono recuperate dal server **[!DNL Scene 7]** , assicurati che le configurazioni Dynamic Media nell’istanza di authoring di AEM e in Brand Portal siano le stesse.

>[!NOTE]
>
>I visualizzatori video e i predefiniti per visualizzatori non sono supportati in Brand Portal. I video vengono visualizzati in anteprima e riprodotti sui visualizzatori predefiniti in Brand Portal.

## Prerequisiti {#prerequisites}

Per lavorare con i video dinamici su Brand Portal, assicurati di:

* **Avvia AEM Author in**
modalità DM (Dynamic Media) Avvia l’istanza di authoring di AEM (con cui è configurato Brand Portal) su  [Dynamic Media Hybrid ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#EnablingDynamicMedia) modeor  [Dynamic  [!DNL Scene 7] Mediamode](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#EnablingDynamicMediainScene7mode).
* **Configura i servizi cloud Dynamic Media su AEM**
AuthorIn base alla modalità Dynamic Media su cui è in esecuzione AEM Author, imposta uno dei servizi cloud  [Dynamic Media ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dynamic.html#ConfiguringDynamicMediaCloudServices) o  [[!DNL Scene 7] Cloud ](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) Services su AEM Author da  **Strumenti**  |  **Cloud Services**  |  **Dynamic Media**.
* **Configurare Dynamic Media su Brand**
PortalIn base alle configurazioni cloud Dynamic Media su AEM Author, configurare le impostazioni  [Dynamic Media ](#configure-dm-hybrid-settings) o  [[!DNL Scene 7] ](#configure-dm-scene7-settings)  le impostazioni dagli strumenti amministrativi Brand Portal.
Assicurati che [tenant Brand Portal separati](#separate-tenants) siano utilizzati per le istanze di AEM Author configurate con le modalità Dynamic Media Hybrid e Dynamic Media **[!UICONTROL Scene7]**, se utilizzi funzionalità di Dynamic Media Hybrid e Dynamic Media **[!UICONTROL S7]**.
* **Pubblicare cartelle con codifiche video applicate a Brand**
PortalApplicare codifiche  [video ](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) e pubblicare su Brand Portal la cartella contenente risorse rich media dall’istanza di authoring di AEM.
* **Inserire nell&#39;elenco Consentiti gli IP dell&#39;evento in SPS se l&#39;anteprima sicura è**
abilitataSe utilizzi Dynamic Media-**[!DNL Scene 7]** (con anteprima  [sicura ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) abilitata per una società), si consiglia all&#39;amministratore  **[!DNL Scene 7]** della società di  [inserire nell&#39;elenco Consentiti gli ](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) IP dell&#39;uscita pubblica per le rispettive aree utilizzando l&#39;interfaccia flash SPS (**[!UICONTROL Scene 7]** Publishing System).
Gli IP Egress sono i seguenti:

| **Regione** | **IP avanzato** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63,140,44,54 |

Per inserire uno di questi IP in uscita, consulta [preparare l&#39;account per un servizio di test sicuro](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best practice  

Per garantire che le risorse video dinamiche vengano visualizzate in anteprima, riprodotte e scaricate correttamente da Brand Portal (e dai collegamenti condivisi), segui queste procedure:

### tenant separati per le modalità Dynamic Media Hybrid e Dynamic Media Scene 7 {#separate-tenants}

Se utilizzi sia le funzioni Dynamic Media **[!DNL Scene 7]** che Dynamic Media Hybrid, ti consigliamo di utilizzare tenant Brand Portal diversi per le istanze di AEM Author configurate con le modalità Dynamic Media Hybrid e Dynamic Media **[!DNL Scene 7]**.


![Autore e BP una a una mappatura](assets/BPDynamicMedia.png)

### Stessi dettagli di configurazione nell’istanza di AEM Author e in Brand Portal

Assicurati che i dettagli di configurazione, come **[!UICONTROL Titolo]**, **[!UICONTROL ID registrazione]**, **[!UICONTROL URL del servizio video]** (in **[!UICONTROL Dynamic Media Hybrid]**) e **[!UICONTROL Titolo]**, le credenziali (**[!UICONTROL E-mail]** e password), **[!UICONTROL e &lt;a 12/>Regione]**, **[!UICONTROL Società]** (in Dynamic Media **[!DNL Scene 7]**) sono uguali in Brand Portal e **[!UICONTROL AEM configurazione cloud]**.

### Inserire nell&#39;elenco Consentiti gli IP in uscita pubblici per la modalità Dynamic Media Scene 7

Se si utilizza Dynamic Media **[!UICONTROL Scene 7]** con [anteprima protetta abilitata](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) per distribuire risorse video a Brand Portal, **[!UICONTROL Scene 7]** stabilisce un server di immagini dedicato per gli ambienti di staging o le applicazioni interne. Qualsiasi richiesta a questo server controlla l&#39;indirizzo IP di origine. Se la richiesta in entrata non si trova nell’elenco di indirizzi IP approvato, viene restituita una risposta di errore.
L’ **[!UICONTROL Amministratore società Scene-7]** configura pertanto un elenco approvato di indirizzi IP per l’ambiente **[!UICONTROL Secure Testing]** della propria azienda, tramite l’interfaccia flash **[!UICONTROL SPS]** (Scene-7 Publishing System). Accertati che l’IP in uscita per la tua rispettiva area geografica (da quanto segue) sia aggiunto a tale elenco approvato.
Per inserire uno di questi IP in uscita, consulta [preparare l&#39;account per un servizio di test sicuro](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Gli IP in uscita sono i seguenti:

| **Regione** | **IP avanzato** |
|--- |--- |
| ND | 130.248.160.66, 52.151.32.108 |
| EMEA | 185.34.189.1 |
| APAC | 63,140,44,54 |

## Configurare le impostazioni Dynamic Media (ibrido) {#configure-dm-hybrid-settings}

Se l&#39;istanza di AEM Author è in esecuzione in modalità ibrida di Dynamic Media, utilizza il riquadro **[!UICONTROL Video]** dal pannello strumenti amministrativi per configurare le impostazioni del gateway Dynamic Media.

>[!NOTE]
>
>I [profili di codifica video](https://helpx.adobe.com/experience-manager/6-5/assets/using/video-profiles.html) non vengono pubblicati in Brand Portal, ma vengono recuperati dal server **[!UICONTROL Scene 7]** . Pertanto, affinché le codifiche video vengano riprodotte correttamente in Brand Portal, assicurati che i dettagli di configurazione siano gli stessi della [[!UICONTROL configurazione cloud Scene7]](https://helpx.adobe.com/experience-manager/6-5/assets/using/config-dms7.html#ConfiguringDynamicMediaCloudServices) nella tua istanza di AEM Author.

Per configurare le configurazioni Dynamic Media sui tenant Brand Portal:

1. Seleziona il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore, in Brand Portal.
1. Dal pannello degli strumenti amministrativi, seleziona il riquadro **[!UICONTROL Video]** .

   ![Configurazione ibrida Dynamic Media su Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Viene visualizzata la pagina Modifica]** configurazione Dynamic Media .

   ![Configurazione ibrida Dynamic Media su Brand Portal](assets/edit-dynamic-media-config.png)

1. Specifica **[!UICONTROL ID registrazione]** e **[!UICONTROL URL del servizio video]** (URL DM-Gateway). Assicurati che questi dettagli siano gli stessi di quelli presenti in **[!UICONTROL Strumenti > Cloud Services]** nella tua istanza di AEM Author.
1. Seleziona **Salva** per salvare la configurazione.

## Configurare le impostazioni Dynamic Media Scene7 {#configure-dm-scene7-settings}

Se l&#39;istanza di AEM Author è in esecuzione in modalità Dynamic Media- **[!UICONTROL Scene 7]**, utilizza la sezione **[!UICONTROL Configurazione Dynamic Media]** dal pannello degli strumenti amministrativi per configurare le impostazioni del server **[!UICONTROL Scene 7]**.

Per configurare le configurazioni di Dynamic Media **[!UICONTROL Scene 7]** sui tenant Brand Portal:

1. Seleziona il logo AEM per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore, in Brand Portal.

2. Dal pannello strumenti amministrativi, seleziona il riquadro **[!UICONTROL Configurazione Dynamic Media]** .

   ![Configurazione di DM  [!UICONTROL Scene 7] su Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL Viene visualizzata la pagina Modifica]** configurazione Dynamic Media .

   ![Configurazione Scene 7 su Brand Portal](assets/S7Config.png)

3. Fornire:

   * **[!UICONTROL Titolo]**
   * Credenziali (**[!UICONTROL ID e-mail]** e **[!UICONTROL Password]**) per accedere al server Scene 7
   * **[!UICONTROL Regione]**

   Assicurati che questi valori siano gli stessi della tua istanza di AEM Author.

4. Selezionare **[!UICONTROL Connetti a Dynamic Media]**.

5. Fornisci il **[!UICONTROL Nome società]** e **[!UICONTROL Salva]** la configurazione.
