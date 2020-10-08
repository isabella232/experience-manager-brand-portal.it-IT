---
title: Configurare AEM Assets con Brand Portal
seo-title: Configurare AEM Assets con Brand Portal
description: Scopri come configurare  AEM Assets con Brand Portal.
seo-description: Scopri come configurare  AEM Assets con Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ecd53a7d92dd020e6a3527793ff11efadcb531ee
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 10%

---


# Configurare AEM Assets con Brand Portal {#configure-integration}

La configurazione di Adobe Experience Manager Assets come Cloud Service con Adobe Experience Manager Assets Brand Portal consente di pubblicare e distribuire risorse con gli utenti del Brand Portal. La configurazione di AEM 6.3 (e versioni successive) con Brand Portal consente invece agli utenti del Brand Portal di pubblicare risorse, distribuirle e fornire contributi alle risorse.

Adobe Experience Manager Assets è configurato con Brand Portal tramite  Adobe Developer Console, che fornisce un token  Adobe Identity Management Services (IMS) per l’autorizzazione del tenant del Brand Portal.

>[!NOTE]
>
>***Per  AEM Assets 6.3 e versioni successive***
>
>In precedenza, Brand Portal era stato configurato nell’interfaccia classica tramite Legacy OAuth Gateway, che utilizza lo scambio JSON Web Token (JWT) per ottenere un token IMS per l’autorizzazione.
>
>La configurazione tramite OAuth legacy non è più supportata dal 6 aprile 2020 e viene modificata in configurazione tramite  console per sviluppatori di Adobe.

>[!TIP]
>
>***Solo per i clienti esistenti***
>
>La configurazione del gateway OAuth legacy continuerà a funzionare per i clienti esistenti.
>
>In caso di problemi con la configurazione del gateway OAuth precedente, elimina la configurazione esistente e crea una nuova configurazione tramite  console Sviluppatore di Adobe.

I passaggi per configurare  AEM Assets con Brand Portal sono diversi a seconda della versione AEM e se si sta configurando per la prima volta o si stanno aggiornando le configurazioni esistenti:

| **Versione di AEM** | **Nuova configurazione** | **Configurazione aggiornamento** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Creare la configurazione](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e versioni successive)** | [Creare la configurazione](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Aggiornamento della configurazione](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e versioni successive)** | [Creare la configurazione](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Aggiornamento della configurazione](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e versioni successive)** | [Creare la configurazione](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Aggiornamento della configurazione](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contattare il supporto | Contattare il supporto |
