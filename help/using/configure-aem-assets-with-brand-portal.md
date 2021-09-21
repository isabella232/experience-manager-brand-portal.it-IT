---
title: Configurare AEM Assets con Brand Portal
seo-title: Configure AEM Assets with Brand Portal
description: Scopri come configurare AEM Assets con Brand Portal.
seo-description: Get an insight into configuring AEM Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: ea3242459776037499b21b33ba40357afc8bf234
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 22%

---

# Configurare AEM Assets con Brand Portal {#configure-integration}

La configurazione di Adobe Experience Manager Assets con Brand Portal abilita la pubblicazione delle risorse, la distribuzione delle risorse e le funzioni di contributo delle risorse per gli utenti Brand Portal. Consente agli utenti di AEM Assets di pubblicare e distribuire le risorse con gli utenti di Brand Portal. Gli utenti di Brand Portal possono accedere alle risorse condivise e contribuire caricando nuove risorse nelle cartelle dei contributi delle risorse e pubblicandole nuovamente in AEM Assets.

La configurazione di AEM Assets con Brand Portal è supportata in:

* AEM Assets as a Cloud Service
* AEM Assets (on-premise e servizio gestito) 6.3 e versioni successive

AEM Assets as a Cloud Service viene configurato automaticamente con Brand Portal attivando Brand Portal da Cloud Manager. Il flusso di lavoro di attivazione crea le configurazioni richieste nel backend e attiva Brand Portal sulla stessa organizzazione IMS di AEM Assets come istanza di Cloud Service.

AEM Assets (on-premise e Managed Service) è configurato manualmente con Brand Portal tramite Adobe Developer Console, che fornisce un token Adobe Identity Management Services (IMS) per l’autorizzazione del tenant Brand Portal.

>[!NOTE]
>
>***Per AEM Assets 6.3 e versioni successive***
>
>In precedenza, Brand Portal era configurato nell’interfaccia classica tramite la versione precedente di OAuth Gateway, che utilizza lo scambio del token Web JSON (JWT) per ottenere un token IMS per l’autorizzazione.
>
>La configurazione tramite la versione precedente di OAuth non è più supportata dal 6 aprile 2020 e viene modificata in configurazione tramite Adobe Developer Console.


>[!TIP]
>
>***Solo per i clienti esistenti (on-premise e servizio gestito)***
>
>La configurazione precedente del gateway OAuth continuerà a funzionare per i clienti esistenti.
>
>In caso di problemi con la configurazione precedente di gateway OAuth, elimina la configurazione esistente e crea una nuova configurazione tramite Adobe Developer Console.

I passaggi per configurare AEM Assets con Brand Portal variano a seconda della versione AEM e se si sta configurando per la prima volta o se si stanno aggiornando le configurazioni esistenti:

| **Versione di AEM** | **Nuova configurazione** | **Configurazione dell&#39;aggiornamento** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Attiva Brand Portal](https://docs.adobe.com/content/help/it-IT/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e versioni successive)** | [Creare la configurazione](https://docs.adobe.com/content/help/it-IT/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configurazione dell&#39;aggiornamento](https://docs.adobe.com/content/help/it-IT/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e versioni successive)** | [Creare la configurazione](https://docs.adobe.com/content/help/it/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configurazione dell&#39;aggiornamento](https://docs.adobe.com/content/help/it-IT/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e versioni successive)** | [Creare la configurazione](https://helpx.adobe.com/it/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Configurazione dell&#39;aggiornamento](https://helpx.adobe.com/it/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contatta il supporto | Contatta il supporto |
