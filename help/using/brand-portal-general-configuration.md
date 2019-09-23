---
title: Amministra configurazioni tenant generali
seo-title: Amministra configurazioni tenant generali
description: Configurate l'accelerazione del download, la creazione pubblica dello smart [!UICONTROL collection], la creazione pubblica [!UICONTROL collection] e abilitate gli utenti admin a eliminare le risorse sui tenant.
seo-description: Configurate l'accelerazione del download, la creazione pubblica dello smart [!UICONTROL collection], la creazione pubblica [!UICONTROL collection] e abilitate gli utenti admin a eliminare le risorse sui tenant.
uuid: 3c46cd7c-c38b-4bc7-b566-93f977bc8227
contentOwner: mgulati
topic-tags: administration
content-type: riferimento
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f4c237bc-f6a4-4bc4-af56-3d9c3027daf4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Amministra configurazioni tenant generali {#administer-general-tenant-configurations}

AEM Assets Brand Portal consente alle organizzazioni di configurare le seguenti funzionalità per tenant specifici:

* Eliminazione delle risorse da parte degli amministratori
* Creazione di raccolte pubbliche da parte di utenti non amministratori
* Creazione di raccolte smart pubbliche da parte di utenti non amministratori
* Accelerazione del download
* Gerarchia principale delle cartelle condivise visibile agli utenti non amministratori

Queste configurazioni sono state fornite come configurazioni **[!UICONTROL Impostazioni]** generali nel pannello degli strumenti amministrativi.

![](assets/general-configs.png)

**Configurazione per** consentire agli amministratori di eliminare le risorse dal Brand Portal. (Il valore predefinito è attivato)

**B** Configurazione per consentire agli utenti non amministratori di creare raccolte pubbliche. (Il valore predefinito è attivato)

**C** Configurazione per consentire agli utenti non amministratori di creare raccolte smart pubbliche. (Il valore predefinito è attivato)

**D** Configurazione per consentire l'accelerazione del download delle risorse scaricate dal portale e dai collegamenti condivisi. (Il valore predefinito è disabilitato)

**E** Configuration per visualizzare la gerarchia delle cartelle (dalla radice) delle cartelle condivise a utenti non amministratori (editor, visualizzatori, utenti ospiti). (Il valore predefinito è disabilitato)

## Attiva/Disattiva configurazioni generali {#enable-disable-general-configurations}

Per attivare/disattivare ciascuna delle seguenti configurazioni:

1. Effettuate l'accesso con i privilegi di amministratore.
2. Selezionate il logo AEM per accedere agli strumenti amministrativi, dalla barra degli strumenti nella parte superiore.
3. Dal pannello degli strumenti di amministrazione, selezionate **[!UICONTROL Generale]** per aprire la pagina Impostazioni **** generali.
4. Utilizzate il rispettivo interruttore di attivazione/disattivazione per attivare o disattivare una qualsiasi delle configurazioni Generali.
5. **[!UICONTROL Salvate le modifiche.]**
6. Disconnessione per rendere attive le modifiche.

## Consentire agli utenti amministratori di eliminare le risorse dal Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Consentire agli utenti di eliminare]** la configurazione consente alle organizzazioni di consentire (o limitare) agli utenti con privilegi di amministratore di eliminare risorse e cartelle dal Brand Portal.

## Consenti creazione raccolte pubbliche da parte di utenti non amministratori {#allow-public-collections-creation-by-non-admins}

[La configurazione [!UICONTROL Consenti creazione raccolte pubbliche]](../using/brand-portal-share-collection.md#main-pars-text-1915052376) controlla se i non amministratori possono creare raccolte pubbliche sul Portale marchio. La configurazione è abilitata per impostazione predefinita. Disattivando le organizzazioni di configurazione è possibile impedire l'utilizzo di numerose raccolte pubbliche sul proprio portale per consentire il salvataggio dello spazio del sistema.

## Consenti creazione di raccolte smart pubbliche da parte di utenti non amministratori {#allow-public-smart-collections-creation-by-non-admins}

[La configurazione [!UICONTROL Consenti creazione di raccolte avanzate pubbliche]](../using/brand-portal-searching.md#main-pars-header-500620467) controlla se i non amministratori possono salvare le ricerche come raccolte intelligenti e renderle pubbliche per quel tenant. La configurazione è abilitata per impostazione predefinita. Disattivando le organizzazioni di configurazione è possibile impedire che un numero enorme di raccolte pubbliche intelligenti create da utenti non amministratori nel Brand Portal dell'organizzazione.

## Consenti accelerazione download {#allow-download-acceleration}

[La configurazione [!UICONTROL Consenti accelerazione download]](../using/accelerated-download.md) consente alle organizzazioni di consentire il download accelerato di risorse dal Portale marchio e collegamenti condivisi, integrando con IBM Aspera Connect un'applicazione install-on-demand. L'applicazione utilizza una tecnologia proprietaria per rimuovere le spese generali TCP.

## Abilita gerarchia cartelle {#enable-folder-hierarchy}

[La configurazione [!UICONTROL Abilita gerarchia cartelle]](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) consente agli amministratori di controllare il modo in cui gli utenti non amministratori (editor, visualizzatori e utenti ospiti) vedono le cartelle condivise dopo l'accesso.
