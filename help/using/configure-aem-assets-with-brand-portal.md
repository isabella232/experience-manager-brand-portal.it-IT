---
title: Configurare AEM Assets con Brand Portal
seo-title: Configurare AEM Assets con Brand Portal
description: Scopri come configurare AEM Assets con Brand Portal.
seo-description: Scopri come configurare AEM Assets con Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: b41f86824afd5be043c7b91035b01b71fdb69a26
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 10%

---


# Configurare AEM Assets con Brand Portal {#configure-integration}

 risorse di Adobe Experience Manager (AEM) è configurato con Brand Portal tramite Adobe Developer Console, che fornisce un token IMS per l’autorizzazione del tenant del Brand Portal. Brand Portal ora è supportato sul servizio cloud AEM Assets, AEM Assets 6.3 e versioni successive.

La configurazione dei AEM Assets potrebbe essere utile con Brand Portal consente di pubblicare e distribuire le risorse con gli utenti del Brand Portal. La configurazione del Portale del marchio su AEM 6.3 (e versioni successive) consente invece di pubblicare risorse, distribuirle risorse e apportare contributi agli utenti del Brand Portal.

>[!NOTE]
>
>***Per gli AEM Assets 6.3 e successivi***
>
>Precedentemente, Brand Portal era stato configurato nell’interfaccia classica tramite il gateway OAuth legacy, che utilizza lo scambio di token JWT per ottenere un token di accesso IMS per l’autorizzazione.
>
>La configurazione tramite OAuth legacy non è più supportata dal 6 aprile 2020 e viene modificata in configurazione tramite Adobe Developer Console.

>[!TIP]
>
>***Solo per i clienti esistenti***
>
>La configurazione del gateway OAuth legacy continuerà a funzionare per i clienti esistenti.
>
>In caso di problemi con la configurazione del gateway OAuth precedente, elimina la configurazione esistente e crea una nuova configurazione tramite Adobe Developer Console.

I passaggi per configurare i AEM Assets con Brand Portal sono diversi a seconda della versione di AEM in uso e se si sta configurando per la prima volta oppure se si stanno aggiornando le configurazioni esistenti:

| **Versione di AEM** | **Nuova configurazione** | **Configurazione aggiornamento** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Creare la configurazione](https://docs.adobe.com/content/help/en/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e versioni successive)** | [Creare la configurazione](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Aggiornamento della configurazione](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
| **AEM 6.4 (6.4.8.0 e versioni successive)** | [Creare la configurazione](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Aggiornamento della configurazione](https://docs.adobe.com/content/help/en/experience-manager-64/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-64) |
| **AEM 6.3 (6.3.3.8 e versioni successive)** | [Creare la configurazione](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html) | [Aggiornamento della configurazione](https://helpx.adobe.com/experience-manager/6-3/assets/using/brand-portal-configuring-integration.html#Upgradeconfiguration) |
| **AEM 6.2** | Contattare il supporto | Contattare il supporto |


