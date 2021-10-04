---
title: Amministrare le configurazioni tenant generali
seo-title: Administer general tenant configurations
description: Configura l’accelerazione di download, la creazione di raccolte avanzate pubbliche, la creazione di raccolte pubbliche e abilita gli utenti amministratori a eliminare le risorse sugli tenant.
seo-description: Configure download acceleration, public smart collection creation, public collection creation, and enable admin users to delete assets on tenants.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: reference
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
role: Admin
exl-id: 5607be8e-0a7f-4692-b71b-5f66eb9ac5ee
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 3%

---

# Amministrare le configurazioni tenant generali {#administer-general-tenant-configurations}

Experience Manager Assets Brand Portal consente alle organizzazioni di configurare le seguenti funzionalità per tenant specifici:

* Eliminazione delle risorse da parte degli amministratori
* Creazione di raccolte pubbliche da parte di utenti non amministratori
* Creazione di raccolte avanzate pubbliche da parte di utenti non amministratori
* Gerarchia padre di cartelle condivise visibili agli utenti non amministratori

Queste configurazioni sono state fornite come configurazioni **[!UICONTROL Impostazioni generali]** nel pannello strumenti amministrativi.

![](assets/general-config.png)

****   Configurazione AC per consentire agli amministratori di eliminare le risorse da Brand Portal. (Il valore predefinito è abilitato)

****   Configurazione BC per consentire agli utenti non amministratori di creare raccolte pubbliche. (Il valore predefinito è abilitato)

****   Configurazione per consentire agli utenti non amministratori di creare raccolte avanzate pubbliche. (Il valore predefinito è abilitato)

****  Configurazione di DC per visualizzare la gerarchia delle cartelle (dalla radice) delle cartelle condivise agli utenti non amministratori (editor, visualizzatori, utenti ospiti). (Il valore predefinito è disabilitato)

## Attiva/disattiva le configurazioni generali {#enable-disable-general-configurations}

Per abilitare/disabilitare ciascuna di queste configurazioni:

1. Accedi con privilegi di amministratore.
1. Seleziona il logo Experience Manager per accedere agli strumenti amministrativi dalla barra degli strumenti nella parte superiore.
1. Dal pannello strumenti amministrativi, seleziona **[!UICONTROL Generale]** per aprire la pagina **[!UICONTROL Impostazioni generali]**.
1. Usare il rispettivo interruttore di attivazione/disattivazione per attivare o disattivare una qualsiasi delle configurazioni Generali.
1. **[!UICONTROL Salva le modifiche.]**
1. Esci per rendere effettive le modifiche.

## Consenti agli utenti amministratori di eliminare le risorse da Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Consenti agli utenti di]** eliminare la configurazione consente alle organizzazioni di consentire (o limitare) agli utenti con privilegi di amministratore di eliminare risorse e cartelle da Brand Portal.

## Consenti creazione raccolte pubbliche da parte di non amministratori {#allow-public-collections-creation-by-non-admins}

[[!UICONTROL Consenti ]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) creazione raccolte pubbliche controlla se i non amministratori possono creare raccolte pubbliche in Brand Portal. La configurazione è abilitata per impostazione predefinita. Disabilitando le organizzazioni di configurazione è possibile impedire l&#39;utilizzo di numerose raccolte pubbliche sul loro portale in modo da poter risparmiare spazio sul sistema.

## Consenti creazione di raccolte avanzate pubbliche da parte di utenti non amministratori {#allow-public-smart-collections-creation-by-non-admins}

[[!UICONTROL Consenti la ]](../using/brand-portal-searching.md#main-pars-header-500620467) creazione di raccolte avanzate pubbliche controlla se i non amministratori possono salvare le loro ricerche come raccolte avanzate e renderle pubbliche per quel tenant. La configurazione è abilitata per impostazione predefinita. Disabilitando le organizzazioni di configurazione puoi impedire che un numero enorme di raccolte avanzate pubbliche create da utenti non amministratori su Brand Portal dell’organizzazione.

<!-- 
## Allow download acceleration {#allow-download-acceleration}

[[!UICONTROL Allow download acceleration]](../using/accelerated-download.md) configuration lets the organizations to allow accelerated downloads of assets from Brand Portal and shared links, by integrating with IBM Aspera Connect that is an install-on-demand application. The application uses proprietary technology to remove TCP overheads.
-->

## Abilita gerarchia cartelle {#enable-folder-hierarchy}

[[!UICONTROL Abilita configurazione ]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) gerarchia cartelle consente agli amministratori di controllare come gli utenti non amministratori (editor, visualizzatori e utenti ospiti) visualizzano le cartelle condivise dopo l&#39;accesso.
