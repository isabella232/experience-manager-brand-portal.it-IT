---
title: Origine risorsa in Brand Portal
seo-title: Origine risorsa in Brand Portal
description: Ottieni informazioni approfondite sulla funzione di determinazione origine delle risorse rilasciata nel portale dei marchi di Adobe Experience Manager Assets.
seo-description: Ottieni informazioni approfondite sulla funzione di determinazione origine delle risorse rilasciata nel portale dei marchi di Adobe Experience Manager Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
product: experience-manager
sub-product: assets
feature: brand-portal
topics: collaboration, content-velocity, sharing
doc-type: feature-video
activity: use
audience: author, marketer
version: 6.5
kt: 3838
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '457'
ht-degree: 0%

---


# Panoramica di Asset Sourcing {#overview-asset-sourcing-in-bp}

**Asset Sourcing** consente agli utenti AEM (amministratori/utenti non amministratori) di creare nuove cartelle con un’ulteriore proprietà **Asset Contribution** , in modo che la nuova cartella creata sia aperta all’invio delle risorse da parte degli utenti del Brand Portal. Questo attiva automaticamente un flusso di lavoro che crea due sottocartelle aggiuntive, denominate **SHARED** e **NEW**, all’interno della cartella **Contribution** appena creata. L’amministratore AEM definisce quindi il requisito caricando una breve descrizione dei tipi di risorse da aggiungere alla cartella dei contributi, nonché una serie di risorse di base, nella cartella **SHARED** per garantire che gli utenti BP dispongano delle informazioni di riferimento necessarie. L’amministratore può quindi concedere agli utenti attivi di Brand Portal l’accesso alla cartella dei contributi prima di pubblicare la nuova cartella **Contribution** nel Brand Portal. Dopo aver aggiunto il contenuto nella cartella **NEW** , l’utente può pubblicare nuovamente la cartella dei contributi nell’ambiente di authoring AEM. Tenete presente che potrebbero essere necessari alcuni minuti per completare l&#39;importazione e riflettere il contenuto appena pubblicato in  AEM Assets.

Inoltre, tutte le funzionalità esistenti rimangono invariate. Gli utenti di Brand Portal possono visualizzare, cercare e scaricare risorse dalla cartella dei contributi e dalle altre cartelle consentite. Inoltre, gli amministratori possono condividere ulteriormente la cartella dei contributi, modificare le proprietà e aggiungere risorse alle raccolte.

## Prerequisiti {#prerequisites}

* AEM 6.5.2 o versione successiva.
* Assicurati che l’istanza  AEM Assets sia configurata con Brand Portal. See, [Configure AEM Assets with Brand Portal](../using/configure-aem-assets-with-brand-portal.md).
* Assicurati che il tenant del Brand Portal sia configurato con un’istanza di authoring  AEM Assets.

>[!NOTE]
>
>Asset Sourcing non è supportato  AEM Assets come Cloud Service.

>[!VIDEO](https://video.tv.adobe.com/v/29365/?quality=12)

![Origine risorsa Brand Portal](assets/asset-sourcing.png)


>[!NOTE]
>
>Esiste un problema noto nella AEM 6.5.4. Gli utenti del Brand Portal non possono pubblicare le risorse della cartella dei contributi su  AEM Assets durante l’aggiornamento  console per sviluppatori di Adobi.
>
>Il problema è stato risolto nella AEM 6.5.5. È possibile aggiornare l&#39;istanza di  AEM Assets al service pack più recente AEM 6.5.5 e [aggiornare le configurazioni](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) su  Developer Console.
>
>Per la correzione immediata del AEM 6.5.4, si consiglia di [scaricare l’hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e installarlo nell’istanza di creazione.

## Consulta anche {#reference-articles}

**Per amministratori**

* [Configurare l&#39;origine delle risorse in AEM](brand-portal-configure-asset-sourcing.md)
* [Carica elenco utenti Brand Portal](brand-portal-configure-asset-sourcing.md)
* [Configurare la cartella dei contributi](brand-portal-contribution-folder.md)
* [Caricare le risorse della baseline nella cartella Contribution](brand-portal-upload-baseline-assets.md)
* [Pubblica cartella dei contributi in Brand Portal](brand-portal-publish-contribution-folder-to-brand-portal.md)

**Per utenti di Brand Portal**

* [Scaricare i requisiti delle risorse](brand-portal-download-asset-requirements.md)
* [Caricare nuove risorse nella cartella Contribution](brand-portal-upload-assets-to-contribution-folder.md)
* [Pubblica la cartella dei contributi in  AEM Assets](brand-portal-publish-contribution-folder-to-aem-assets.md)
