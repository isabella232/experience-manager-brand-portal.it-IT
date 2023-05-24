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
source-git-commit: f56918ea8eb14ba04b7e141f4f1cae318e532512
workflow-type: tm+mt
source-wordcount: '1250'
ht-degree: 4%

---

# Supporto di video dinamici in Brand Portal {#dynamic-video-support-on-brand-portal}

Anteprima e riproduzione di video in modo adattivo su Brand Portal con supporto Dynamic Media. Scarica anche le rappresentazioni dinamiche dal portale e dai collegamenti condivisi.
Gli utenti di Brand Portal possono:

* Visualizza l’anteprima dei video nelle pagine Dettagli risorsa, Scheda e Condivisione collegamenti.
* Riproduci le codifiche video nella pagina Dettagli risorsa.
* Visualizza le rappresentazioni dinamiche nella scheda Rappresentazioni della pagina Dettagli risorsa.
* Scarica le codifiche video e le cartelle contenenti i video.

>[!NOTE]
>
>Per lavorare con i video e pubblicarli in Brand Portal, assicurati che l’istanza Autore dell’Experience Manager sia impostata sulla modalità ibrida di Dynamic Media o su Dynamic Media **[!DNL Scene7]** modalità.

Per visualizzare in anteprima, riprodurre e scaricare i video, Brand Portal espone agli amministratori le due configurazioni seguenti:

* [Configurazione ibrida Dynamic Media](#configure-dm-hybrid-settings)
Se l’istanza Autore Experience Manager è in esecuzione in modalità ibrida per elementi multimediali dinamici.
* [Dynamic Media [!DNL Scene7] configurazione](#configure-dm-scene7-settings)
Se l’istanza Autore Experience Manager è in esecuzione su Dynamic Media:**[!DNL Scene7]** modalità.
Imposta una di queste configurazioni in base alle configurazioni impostate nell’istanza Autore Experience Manager con cui viene replicato il tenant Brand Portal.

>[!NOTE]
>
>I video dinamici non sono supportati nei tenant Brand Portal configurati con Experience Manager Author in esecuzione su **[!UICONTROL Scene7Connect]** modalità di esecuzione.

## Come vengono riprodotti i video dinamici? {#how-are-dynamic-videos-played}

![Le codifiche video vengono recuperate dal cloud](assets/VideoEncodes.png)

Se configurazioni Dynamic Media ([Ibrido](../using/dynamic-video-brand-portal.md#configure-dm-hybrid-settings) o [[!DNL Scene7]](../using/dynamic-video-brand-portal.md#configure-dm-scene7-settings) configurazioni) sono impostate su Brand Portal, le rappresentazioni dinamiche vengono recuperate da **[!DNL Scene7]** server. Le codifiche video vengono quindi visualizzate in anteprima e riprodotte senza ritardi e con una distorsione della qualità.

Poiché le codifiche video non vengono memorizzate nell’archivio Brand Portal e vengono recuperate da **[!DNL Scene7]** server, assicurati che le configurazioni di Dynamic Media nell’istanza di authoring di Adobe Experience Manager e in Brand Portal siano le stesse.

>[!NOTE]
>
>I visualizzatori video e i predefiniti visualizzatore non sono supportati in Brand Portal. I video vengono visualizzati in anteprima e riprodotti sui visualizzatori predefiniti in Brand Portal.

## Prerequisiti {#prerequisites}

Per lavorare con i video dinamici su Brand Portal, assicurati di:

* **Avvia Experience Manager Author in modalità Dynamic Media**
Avvia l’istanza Autore Experience Manager (con cui è configurato Brand Portal) in [DYNAMIC MEDIA - [!DNL Scene7] modalità](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=en#enabling-dynamic-media-in-scene-mode) o in [Dynamic Media - Modalità ibrida](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html) o
* **Configurare i Cloud Services Dynamic Media in Experience Manager Author**
In base alla modalità Dynamic Media (modalità Scene7 o modalità ibrida) in cui è in esecuzione l’Experience Manager Author, imposta [CLOUD SERVICES DYNAMIC MEDIA ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=it#configuring-dynamic-media-cloud-services) o [Cloud Services Dynamic Media (modalità ibrida)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dynamic.html?lang=en#configuring-dynamic-media-cloud-services) su Autore Experience Manager da **Strumenti** | **Cloud Services** | **Dynamic Media**.
* **Configurare Dynamic Media su Brand Portal**
In base alle configurazioni cloud di Dynamic Media in Experience Manager Author, configura [Impostazioni Dynamic Media](#configure-dm-hybrid-settings) o [[!DNL Scene7] impostazioni](#configure-dm-scene7-settings) da strumenti di amministrazione di Brand Portal.
Assicurati che [tenant Brand Portal separati](#separate-tenants) sono utilizzati per Experience Manager le istanze di authoring configurate in Dynamic Media - **[!UICONTROL Scene7]** e Dynamic Media - modalità ibrida. Soprattutto se utilizzi funzionalità di Dynamic Media **[!UICONTROL S7]** e Dynamic Media Hybrid.
* **Pubblicare cartelle con codifiche video applicate a Brand Portal**
Applica [codifiche video](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) e pubblica la cartella contenente le risorse rich media dall’istanza Experience Manager Author a Brand Portal.
* **Inserisce nell&#39;elenco Consentiti IP in uscita in SPS se l&#39;anteprima protetta è abilitata**
Se si utilizza Dynamic Media-**[!DNL Scene7]** (con [anteprima protetta abilitata](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html) per un’azienda), si consiglia quindi di: **[!DNL Scene7]** amministratore società [inserire nell&#39;elenco Consentiti gli IP in uscita pubblici](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service) per le rispettive regioni che utilizzano SPS (**[!UICONTROL Scene7]** Publishing System) Flash UI.
Gli IP in uscita sono i seguenti:

| **Regione** | **IP in uscita** |
|--- |--- |
| ND | 130.248.160.68,  20.94.203.130 |
| EMEA | 185.34.189.3,  51.132.146.75 |
| APAC | 63.140.44.54 |

Per inserire nell’elenco Consentiti uno di questi IP in uscita, consulta [preparare l’account per il servizio di test protetto](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).

## Best practice

Per garantire che le risorse video dinamiche vengano visualizzate correttamente in anteprima, riprodotte e scaricate da Brand Portal (e dai collegamenti condivisi), procedi come segue:

### Tenant separati per le modalità Dynamic Media - Scene7 e Dynamic Media - Ibrido {#separate-tenants}

Se si utilizzano entrambi i tipi di Dynamic Media - **[!DNL Scene7]** modalità e Dynamic Media - Funzioni in modalità ibrida, utilizza tenant Brand Portal diversi, ad Experience Manager istanze Author configurate con Dynamic Media - **[!DNL Scene7]** e Dynamic Media - modalità ibrida.


![Mappatura uno a uno tra Author e BP](assets/BPDynamicMedia.png)

### Stessi dettagli di configurazione nell’istanza Experience Manager Author e in Brand Portal

Assicurati che i dettagli di configurazione siano gli stessi in Brand Portal e **[!UICONTROL Configurazione cloud Experience Manager]**. Gli stessi dettagli di configurazione includono:

* **[!UICONTROL Titolo]**
* **[!UICONTROL ID registrazione]**
* **[!UICONTROL URL servizio video]** in **[!UICONTROL Dynamic Media - Modalità ibrida]**
* **[!UICONTROL Titolo]**
* Credenziali (**[!UICONTROL E-mail]** e password)
* **[!UICONTROL Regione]**
* **[!UICONTROL Azienda]** in Dynamic Media - **[!DNL Scene7]** modalità

### Inserire nell&#39;elenco Consentiti IP pubblici in uscita per la modalità Dynamic Media Scene7

Se Dynamic Media **[!UICONTROL Scene7]**-avere [anteprima protetta abilitata](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html)-viene utilizzato per distribuire risorse video a Brand Portal, quindi **[!UICONTROL Scene7]** stabilisce un server immagini dedicato per gli ambienti di staging o le applicazioni interne. Qualsiasi richiesta inviata a questo server controlla l’indirizzo IP di origine. Se la richiesta in ingresso non si trova nell’elenco approvato di indirizzi IP, viene restituita una risposta di errore.
Il **[!UICONTROL Scene7]** L’Amministratore dell’azienda configura quindi un elenco approvato di indirizzi IP per l’indirizzo dell’azienda **[!UICONTROL Test protetto]** ambiente, tramite **[!UICONTROL SPS]** (Scene7 Publishing System) Interfaccia utente flash. Accertati che l’IP in uscita per la tua rispettiva regione (dal seguente) sia aggiunto all’elenco approvato.
Per inserire nell’elenco Consentiti uno di questi IP in uscita, consulta [preparare l’account per il servizio di test protetto](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/upload-publish/testing-assets-making-them-public.html#testing-the-secure-testing-service).
Gli IP in uscita sono i seguenti:

| **Regione** | **IP in uscita** |
|--- |--- |
| ND | 130.248.160.66, 20.94.203.130 |
| EMEA | 51.132.146.75, 130.248.244.202, 130.248.244.203, 130.248.244.204, 130.248.244.210, 130.248.244.211, 130.248.244.212 |
| APAC | 63.140.44.54 |

## Configurare le impostazioni di Dynamic Media (ibrido) {#configure-dm-hybrid-settings}

Se l’istanza Autore Experience Manager è in esecuzione in modalità ibrida per elementi multimediali dinamici, utilizza **[!UICONTROL Video]** affiancare dal pannello strumenti di amministrazione per configurare le impostazioni del gateway di Dynamic Media.

>[!NOTE]
>
>Il [profili di codifica video](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/video-profiles.html) non sono pubblicati in Brand Portal, ma vengono recuperati dal file **[!UICONTROL Scene7]** server. Pertanto, affinché le codifiche video possano essere riprodotte correttamente in Brand Portal, assicurati che i dettagli di configurazione siano gli stessi della [CLOUD SERVICES DYNAMIC MEDIA ([!DNL Scene7] mode)](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/config-dms7.html?lang=it#configuring-dynamic-media-cloud-services) nell’istanza Autore dell’Experience Manager.

Per impostare le configurazioni di Dynamic Media sui tenant Brand Portal:

1. Seleziona il logo di Experience Manager in modo da poter accedere agli strumenti di amministrazione dalla barra degli strumenti nella parte superiore, in Brand Portal.
1. Dal pannello Strumenti di amministrazione, selezionare **[!UICONTROL Video]** affiancare.

   ![Configurazione ibrida Dynamic Media su Brand Portal](assets/DMHybrid-Video.png)

   **[!UICONTROL Modifica configurazione Dynamic Media]** viene visualizzata la pagina.

   ![Configurazione ibrida di Dynamic Media su Brand Portal](assets/edit-dynamic-media-config.png)

1. Specifica **[!UICONTROL ID registrazione]** e **[!UICONTROL URL servizio video]** (URL di DM-Gateway). Assicurati che questi dettagli siano identici a quelli riportati in **[!UICONTROL Strumenti > Cloud Services]** nell’istanza Autore dell’Experience Manager.
1. Seleziona **Salva** per salvare la configurazione.

## Configurare le impostazioni di Dynamic Media Scene7 {#configure-dm-scene7-settings}

Se l’istanza Autore Experience Manager è in esecuzione su Dynamic Media- **[!UICONTROL Scene7]** , quindi utilizza **[!UICONTROL Configurazione Dynamic Media]** riquadro dal pannello strumenti di amministrazione per configurare **[!UICONTROL Scene7]** impostazioni del server.

Per configurare Dynamic Media **[!UICONTROL Scene7]** configurazioni sui tenant Brand Portal:

1. Seleziona il logo di Experience Manager in modo da poter accedere agli strumenti di amministrazione dalla barra degli strumenti nella parte superiore, in Brand Portal.

2. Dal pannello Strumenti di amministrazione, selezionare **[!UICONTROL Configurazione Dynamic Media]** affiancare.

   ![DM [!UICONTROL Scena 7] configurazione in Brand Portal](assets/DMS7-Tile.png)

   **[!UICONTROL Modifica configurazione Dynamic Media]** viene visualizzata la pagina.

   ![Configurazione Scene7 su Brand Portal](assets/S7Config.png)

3. Fornisci:

   * **[!UICONTROL Titolo]**
   * Credenziali (**[!UICONTROL ID e-mail]** e **[!UICONTROL Password]**) per accedere al server Scene7
   * **[!UICONTROL Regione]**

   Assicurati che questi valori siano identici a quelli presenti nell’istanza Autore dell’Experience Manager.

4. Seleziona **[!UICONTROL Connetti a Dynamic Media]**.

5. Fornisci **[!UICONTROL Nome dell’azienda]**, e **[!UICONTROL Salva]** la configurazione.
