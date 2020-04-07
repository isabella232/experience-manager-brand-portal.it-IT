---
title: Configurare AEM Assets con Brand Portal
seo-title: Configurare AEM Assets con Brand Portal
description: Ottieni informazioni approfondite sulla configurazione di Risorse AEM con Brand Portal.
seo-description: Ottieni informazioni approfondite sulla configurazione di Risorse AEM con Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: 75d69f85a4178b78eba15a13f865a602e73d3a88

---


# Configurare AEM Assets con Brand Portal {#configure-integration}

Risorse Adobe Experience Manager (AEM) è configurato con Brand Portal tramite Adobe I/O, che fornisce un token IMS per l’autorizzazione del tenant del Brand Portal. Brand Portal ora è supportato dal servizio cloud AEM Assets 6.3 e versioni successive.

La configurazione di Risorse AEM potrebbe essere utile con il Brand Portal e consente di pubblicare e distribuire le risorse con gli utenti del Brand Portal. La configurazione del Portale del marchio su AEM 6.3 (e versioni successive) consente invece di pubblicare risorse, distribuirle risorse e apportare contributi agli utenti del Brand Portal.

>[!NOTE]
>
>***Per AEM Assets 6.3 e versioni successive***
>
>Precedentemente, Brand Portal era stato configurato nell’interfaccia classica tramite il gateway OAuth legacy, che utilizza lo scambio di token JWT per ottenere un token di accesso IMS per l’autorizzazione.
>
>La configurazione tramite OAuth legacy non è più supportata dal 6 aprile 2020 e viene modificata in configurazione tramite I/O Adobe.


>[!TIP]
>
>***Solo per i clienti esistenti***
>
>Si consiglia di continuare a utilizzare la configurazione gateway OAuth esistente. Se si verificano problemi con la configurazione del gateway OAuth precedente, eliminate la configurazione esistente e create una nuova configurazione tramite Adobe I/O.


I passaggi per configurare Risorse AEM con Portale marchio variano a seconda della versione di AEM in uso e se si sta configurando per la prima volta o si stanno aggiornando le configurazioni esistenti:

| **Versione di AEM** | **Nuova configurazione** | **Configurazione aggiornamento** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Crea configurazione](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brandportal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e versioni successive)** | [Crea configurazione](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Aggiornamento della configurazione](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e versioni successive)** | [Crea configurazione](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Aggiornamento della configurazione](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e versioni successive)** | [Crea configurazione](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Aggiornamento della configurazione](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contattare il supporto | Contattare il supporto |


<!--
   Comment Type: draft

   <li> </li>
   -->

<!--
   Comment Type: draft

   <li>Step text</li>
   -->
