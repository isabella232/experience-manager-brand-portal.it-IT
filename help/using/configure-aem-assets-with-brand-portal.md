---
title: Configurare Experience Manager Assets con Brand Portal
seo-title: Configure Experience Manager Assets with Brand Portal
description: Scopri come configurare Experience Manager Assets con Brand Portal.
seo-description: Get an insight into configuring Experience Manager Assets with Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
role: Admin
exl-id: 261c0e84-6b3d-459c-b6b9-a9af106d6943
source-git-commit: 454b05c05359a2068cc29124f826d5bd25a1bad1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 6%

---

# Configurare Experience Manager Assets con Brand Portal {#configure-integration}

La configurazione di Adobe Experience Manager Assets con Brand Portal abilita la pubblicazione delle risorse, la distribuzione delle risorse e le funzioni di contributo delle risorse per gli utenti Brand Portal. Consente agli utenti di Experience Manager Assets di pubblicare e distribuire le risorse con gli utenti di Brand Portal. Gli utenti di Brand Portal possono accedere alle risorse condivise e contribuire caricando nuove risorse nelle cartelle dei contributi delle risorse e pubblicandole nuovamente in Experience Manager Assets.

La configurazione di Experience Manager Assets con Brand Portal è supportata in:

* Experience Manager Assets as a Cloud Service
* Experience Manager Assets (on-premise e Managed Service) 6.5 e versioni successive

Experience Manager Assets as a Cloud Service viene configurato automaticamente con Brand Portal attivando Brand Portal da Cloud Manager. Il flusso di lavoro di attivazione crea le configurazioni richieste nel backend e attiva Brand Portal sulla stessa organizzazione IMS dell’istanza as a Cloud Service di Experience Manager Assets.

Al contrario, Experience Manager Assets (on-premise e servizio gestito) viene configurato manualmente con Brand Portal tramite la console Adobe Developer, che fornisce un token Adobe Identity Management Services (IMS) per l’autorizzazione del tenant Brand Portal.

>[!NOTE]
>
>***Per Experience Manager Assets 6.5 e versioni successive***
>
>In precedenza, Brand Portal era configurato nell’interfaccia classica tramite la versione precedente di OAuth Gateway, che utilizza lo scambio del token Web JSON (JWT) per ottenere un token IMS per l’autorizzazione.
>
>La configurazione tramite la versione precedente di OAuth non è più supportata dal 6 aprile 2020 e viene modificata in configurazione tramite la console Adobe Developer.


>[!TIP]
>
>***Solo per i clienti esistenti (on-premise e servizio gestito)***
>
>La configurazione precedente del gateway OAuth continuerà a funzionare per i clienti esistenti.
>
>In caso di problemi con la configurazione del gateway OAuth legacy, elimina la configurazione esistente e crea una nuova configurazione tramite la console Adobe Developer.

I passaggi per configurare AEM Assets con Brand Portal variano a seconda della versione AEM e se si sta configurando per la prima volta o se si stanno aggiornando le configurazioni esistenti:

| **Versione di AEM** | **Nuova configurazione** | **Configurazione dell&#39;aggiornamento** |
|---|---|---|
| **AEM Assets as a Cloud Service** | [Attiva Brand Portal](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/assets/brand-portal/configure-aem-assets-with-brand-portal.html) | - |
| **AEM 6.5 (6.5.4.0 e versioni successive)** | [Creare la configurazione](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html) | [Configurazione dell&#39;aggiornamento](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) |
