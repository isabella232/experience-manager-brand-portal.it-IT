---
title: Configurare l'origine delle risorse
seo-title: Configurare l'origine delle risorse
description: Scopri come configurare la funzione di determinazione origine delle risorse in Risorse AEM.
seo-description: Scopri come configurare la funzione di determinazione origine delle risorse in Risorse AEM.
uuid: null
content-type: reference
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: add4009bd99e5af8ed0c9ffea63647c166b7c75d

---


# Configurare l'origine delle risorse {#configure-asset-sourcing}

Gli amministratori di AEM possono configurare l’origine delle **risorse** dall’istanza di creazione di AEM. L’amministratore abilita la configurazione del flag della funzione Origine risorsa dalla configurazione **della console Web di** AEM e carica l’elenco degli utenti attivi del Brand Portal in **AEM Assets**.

>[!NOTE]
>
>Prima di iniziare la configurazione, accertati che l’istanza di Risorse AEM sia integrata con il Brand Portal. Consultate [Configurare l’integrazione di AEM Assets con Brand Portal](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).


Il seguente video illustra come configurare l’origine delle risorse nell’istanza di creazione di AEM:

>[!VIDEO](https://video.tv.adobe.com/v/29771?captions=ita)

## Abilita origine risorse {#enable-asset-sourcing}

Gli amministratori di AEM possono abilitare l’origine delle risorse dalla configurazione della console Web di AEM (ad esempio, una gestione della configurazione).

**Per abilitare l'origine delle risorse:**
1. Accedete all’istanza di creazione di AEM e aprite l’URL predefinito di Configuration Manager: http:// localhost:4502/system/console/configMgr
1. Effettuate una ricerca utilizzando la parola chiave **Origine** risorsa per individuare il file di configurazione del flag della funzione di origine delle **[!UICONTROL risorse]**
1. Fate clic su **[!UICONTROL Asset Sourcing Feature Flag Config]** per aprire la finestra di configurazione
1. Abilita **[!UICONTROL funzionalità casella di controllo.flag.active.status]**
1. Fai clic su **[!UICONTROL Salva]**.

![](assets/enable-asset-sourcing.png)

## Carica elenco utenti Brand Portal {#upload-bp-user-list}

Gli amministratori AEM possono caricare il file di configurazione utente (.csv) del Portale marchio contenente l’elenco di utenti attivo del Portale marchio in Risorse AEM. Una cartella di contributi può essere condivisa solo con gli utenti attivi del Brand Portal definiti nell’elenco di utenti. L’amministratore può anche aggiungere nuovi utenti nel file di configurazione e caricare l’elenco di utenti modificato.

L'amministratore può aggiungere nuovi utenti in AEM Admin Console. Per informazioni dettagliate, consultate [Gestione utenti](brand-portal-adding-users.md) . Dopo aver aggiunto gli utenti in Admin Console, questi possono essere aggiunti al file di configurazione utente del Brand Portal e quindi ottenere l’autorizzazione per accedere alla cartella dei contributi.

**Per caricare l’elenco degli utenti di Brand Portal:**
1. Accedi all’istanza di creazione AEMURL predefinito: http:// localhost:4502/aem/start.html
1. Dal pannello **Strumenti** ![](assets/tools.png) , passa a **[!UICONTROL Risorse &gt; Utenti del Brand Portal]**
   ![](assets/upload-user-list1.png)
1. Si apre la finestra Collaboratori di caricamento del portale del marchio.
Sfogliate il computer locale e caricate il file **di** configurazione (.csv) contenente l’elenco degli utenti attivi di Brand Portal.
1. Fai clic su **[!UICONTROL Salva]**.
   ![](assets/upload-user-list2.png)


Gli amministratori possono fornire l’accesso a utenti/gruppi specifici da questo elenco di utenti durante la configurazione della cartella dei contributi.

Per ulteriori informazioni, consultate [Configurare la cartella](brand-portal-contribution-folder.md)dei contributi.