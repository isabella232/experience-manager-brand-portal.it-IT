---
title: Asset Sourcing in Brand Portal
seo-title: Origine risorse in Brand Portal
description: Ottieni informazioni approfondite sulla funzione di determinazione origine delle risorse rilasciata in Adobe Experience Manager Assets Brand Portal.
seo-description: Ottieni informazioni approfondite sulla funzione di determinazione origine delle risorse rilasciata in Adobe Experience Manager Assets Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
sub-product: assets
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
exl-id: 2c132a7a-ed10-4856-8378-67939167ea60
source-git-commit: 88526c235a12d47f5cbb5f442683f8b0ac2f21e5
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 3%

---

# Panoramica su Asset Sourcing {#overview-asset-sourcing-in-bp}

**Asset** Source consente agli utenti AEM (amministratori/utenti non amministratori) di creare nuove cartelle con un’ulteriore proprietà  **Asset** Contribution, in modo che la nuova cartella creata sia aperta all’invio delle risorse da parte degli utenti Brand Portal. Questo attiva automaticamente un flusso di lavoro che crea due sottocartelle aggiuntive, denominate **SHARED** e **NEW**, all’interno della cartella **Contribution** appena creata. L’amministratore di AEM definisce quindi il requisito caricando una breve descrizione dei tipi di risorse da aggiungere alla cartella dei contributi, nonché un set di risorse della linea di base, nella cartella **SHARED** per garantire che gli utenti BP dispongano delle informazioni di riferimento necessarie. L’amministratore può quindi concedere agli utenti Brand Portal attivi l’accesso alla cartella dei contributi prima di pubblicare la cartella **Contribution** appena creata in Brand Portal. Al termine dell’aggiunta del contenuto nella cartella **NEW** , l’utente può pubblicare nuovamente la cartella Contributo nell’ambiente di authoring AEM. Tieni presente che potrebbero essere necessari alcuni minuti per completare l’importazione e riflettere il contenuto appena pubblicato in AEM Assets.

Inoltre, tutte le funzionalità esistenti rimangono invariate. Gli utenti di Brand Portal possono visualizzare, cercare e scaricare risorse dalla cartella dei contributi e dalle altre cartelle consentite. Inoltre, gli amministratori possono condividere ulteriormente la cartella dei contributi, modificare le proprietà e aggiungere risorse alle raccolte.

![Origine risorse Brand Portal](assets/asset-sourcing.png)

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

## Prerequisiti {#prerequisites}

* AEM Assets as a Cloud Service, AEM Assets 6.5.2 o versione successiva.
* Assicurati che la tua istanza di AEM Assets sia configurata con Brand Portal. Consulta [Configurare AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

<!--
* Ensure that your Brand Portal tenant is configured with one AEM Assets author instance.
-->

>[!NOTE]
>
>Per impostazione predefinita, la funzione Origine risorse è abilitata in AEM Assets as a Cloud Service, AEM Assets 6.5.9 e versioni successive.
>
>Le configurazioni esistenti continueranno a funzionare sulle versioni precedenti.

>[!NOTE]
>
>Esiste un problema noto in AEM Assets 6.5.4. Gli utenti Brand Portal non possono pubblicare le risorse della cartella dei contributi in AEM Assets durante l’aggiornamento ad Adobe Developer Console.
>
>Il problema è risolto in AEM 6.5.5. È possibile aggiornare l&#39;istanza AEM Assets all&#39;ultimo service pack AEM 6.5.5 e [aggiornare le configurazioni](https://docs.adobe.com/content/help/it-IT/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) in Adobe Developer Console.

<!--

>For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your author instance.
-->

<!--
## Configure Asset Sourcing {#configure-asset-sourcing}

**Asset Sourcing** is configured from within the AEM Assets author instance. The administrators can enable the Asset Sourcing feature flag configuration from the **AEM Web Console Configuration** and upload the active Brand Portal users list in **AEM Assets**.

>[!NOTE]
>
>Asset Sourcing is by default enabled on AEM Assets as a Cloud Service. The AEM administrator can directly upload the active Brand Portal users to allow them access to the Asset Sourcing feature.

>[!NOTE]
>
>Before you begin with the configuration, ensure that your AEM Assets instance is configured with Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md). 

The following video demonstrates, how to configure Asset Sourcing on your AEM Assets author instance:

>[!VIDEO](https://video.tv.adobe.com/v/29771)
-->

<!--
### Enable Asset Sourcing {#enable-asset-sourcing}

AEM administrators can enable the Asset Sourcing feature flag from within the AEM Web Console Configuration (a.k.a Configuration Manager).

>[!NOTE]
>
>This step is not applicable for AEM Assets as a Cloud Service.


**To enable Asset Sourcing:**
1. Log in to your AEM Assets author instance and open Configuration Manager. 
Default URL: http:// localhost:4502/system/console/configMgr.
1. Search using the keyword **Asset Sourcing** to locate **[!UICONTROL Asset Sourcing Feature Flag Config]**.
1. Click **[!UICONTROL Asset Sourcing Feature Flag Config]** to open the configuration window.
1. Select the **[!UICONTROL feature.flag.active.status]** check box.
1. Click **[!UICONTROL Save]**.

![](assets/enable-asset-sourcing.png)
-->


### Carica elenco utenti Brand Portal {#upload-bp-user-list}

AEM gli amministratori possono caricare il file di configurazione utente di Brand Portal (.csv) contenente l’elenco di utenti Brand Portal attivo in AEM Assets per consentire loro di accedere alla funzione Origine risorse.

Una cartella di contributo può essere condivisa solo con gli utenti Brand Portal attivi definiti nell’elenco di utenti. L’amministratore può anche aggiungere nuovi utenti nel file di configurazione e caricare l’elenco utenti modificato.

>[!NOTE]
>
>Assicurati che la tua istanza di AEM Assets sia configurata con Brand Portal. Consulta [Configurare AEM Assets con Brand Portal](../using/configure-aem-assets-with-brand-portal.md).

>[!NOTE]
>
>Il formato del file CSV è lo stesso supportato in Admin Console per l’importazione in serie da parte degli utenti. E-mail, nome e cognome sono obbligatori.

Gli amministratori possono aggiungere nuovi utenti in AEM Admin Console, consulta [Gestione utenti](brand-portal-adding-users.md) per informazioni dettagliate. Dopo aver aggiunto gli utenti in Admin Console, questi possono essere aggiunti al file di configurazione utente di Brand Portal e quindi ottenere l’autorizzazione per accedere alla cartella Contribution.

**Per caricare l’elenco degli utenti di Brand Portal:**
1. Accedi alla tua istanza AEM Assets.
1. Dal pannello **Strumenti**, passa a **[!UICONTROL Risorse]** > **[!UICONTROL Utenti Brand Portal]**.

1. Viene visualizzata la finestra dei collaboratori per il caricamento di Brand Portal.
Sfoglia dal computer locale e carica il file di configurazione **con estensione csv** contenente l&#39;elenco degli utenti Brand Portal attivi.
1. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/upload-user-list2.png)


Gli amministratori possono fornire l’accesso a utenti specifici da questo elenco di utenti durante la configurazione di una cartella di contributi. Solo gli utenti assegnati a una cartella di contributi avranno accesso alla cartella dei contributi e pubblicheranno le risorse da Brand Portal ad AEM Assets.

## Consulta anche {#reference-articles}

* [Configurare e pubblicare la cartella dei contributi in Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

* [Pubblicare la cartella dei contributi in AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
