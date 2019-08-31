---
title: Amministra configurazioni tenant generali
seo-title: Amministra configurazioni tenant generali
description: Configura accelerazione download, smart smart [! UICONTROL collection] creation, public [! Creazione di raccolte UICONTROL], e consentire agli utenti admin di eliminare le risorse sui tenant.
seo-description: Configura accelerazione download, smart smart [! UICONTROL collection] creation, public [! Creazione di raccolte UICONTROL], e consentire agli utenti admin di eliminare le risorse sui tenant.
uuid: 3 c 46 cd 7 c-c 38 b -4 bc 7-b 566-93 f 977 bc 8227
contentOwner: mgulati
topic-tags: administration
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: f 4 c 237 bc-f 6 a 4-4 bc 4-af 56-3 d 9 c 3027 daf 4
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Amministra configurazioni tenant generali {#administer-general-tenant-configurations}

AEM Assets Brand Portal consente alle organizzazioni di configurare le seguenti funzionalità per tenant specifico:

* Eliminazione delle risorse per amministratori
* Creazione di raccolte pubbliche da parte di utenti non amministratori
* Creazione di raccolte smart pubblica da parte di utenti non amministratori
* Accelerazione download
* Gerarchia principale di cartelle condivise visibili agli utenti non amministratori

Queste configurazioni sono state fornite come **[!UICONTROL configurazioni Impostazioni]** generali nel pannello Strumenti di amministrazione.

![](assets/general-configs.png)

**** Configurazione per consentire agli amministratori di eliminare le risorse dal portale brand. (Il valore predefinito è abilitato)

**Configurazione B** per consentire agli utenti non amministratori di creare raccolte pubbliche. (Il valore predefinito è abilitato)

**Configurazione C** per consentire agli utenti non amministratori di creare raccolte smart pubbliche. (Il valore predefinito è abilitato)

**Configurazione D** per consentire l'accelerazione di download delle risorse scaricate dal portale e dai collegamenti condivisi. (Il valore predefinito è disattivato)

**Configurazione E** consente di visualizzare la gerarchia delle cartelle (dalla principale) di cartelle condivise agli utenti non amministratori (Editor, Visualizzatori, Utenti ospiti). (Il valore predefinito è disattivato)

## Attivare/Disattivare configurazioni Generali {#enable-disable-general-configurations}

Per attivare/disattivare ciascuna configurazione:

1. Accedete con i privilegi di amministratore.
2. Selezionate il logo AEM per accedere agli strumenti di amministrazione, dalla barra degli strumenti nella parte superiore.
3. Dal pannello Strumenti di amministrazione, selezionate **[!UICONTROL Generale]** per aprire la **[!UICONTROL pagina Impostazioni]** generali.
4. Usate il rispettivo interruttore di attivazione/disattivazione per attivare o disattivare una qualsiasi delle configurazioni Generali.
5. **[!UICONTROL Salvate le modifiche.]**
6. Disconnessione per rendere effettive le modifiche.

## Consentire agli utenti admin di eliminare le risorse da Brand Portal {#allow-admin-users-to-delete-assets-from-brand-portal}

**[!UICONTROL Consenti agli utenti di impostare]** la configurazione consente alle organizzazioni di consentire (o limitare) gli utenti con privilegi di amministratore per eliminare risorse e cartelle dal portale del brand.

## Consentire la creazione di raccolte pubbliche da parte di non amministratori {#allow-public-collections-creation-by-non-admins}

[[! La configurazione UICONTROL Consenti creazione raccolte](../using/brand-portal-share-collection.md#main-pars-text-1915052376) pubblica controlla se i non amministratori possono creare raccolte pubbliche su Brand Portal. La configurazione è attivata per impostazione predefinita. Disabilitando le organizzazioni di configurazione, potete impedire che siano presenti numerose raccolte pubbliche sul portale, in modo che lo spazio del sistema possa essere salvato.

## Consentire la creazione di raccolte smart pubbliche da parte di non amministratori {#allow-public-smart-collections-creation-by-non-admins}

[[! La configurazione di UICONTROL Consenti raccolte smart](../using/brand-portal-searching.md#main-pars-header-500620467) pubblica consente di controllare se i non amministratori possono salvare le proprie ricerche come raccolte intelligenti e renderle pubbliche per quel tenant. La configurazione è attivata per impostazione predefinita. Disabilitando le organizzazioni di configurazione, è possibile evitare di avere un numero elevato di raccolte smart pubbliche create da utenti non amministratori sul portale marchio aziendale.

## Consenti accelerazione download {#allow-download-acceleration}

[[! La configurazione dell'accelerazione UICONTROL](../using/accelerated-download.md) Consenti accelerazione consente alle organizzazioni di consentire download accelerati delle risorse dal portale brand e collegamenti condivisi, integrando con IBM Aspera Connect che è un'applicazione di installazione. L'applicazione utilizza la tecnologia proprietaria per rimuovere gli overhead TCP.

## Abilita gerarchia cartelle {#enable-folder-hierarchy}

[[! La configurazione Abilita gerarchia di UITROL](../using/brand-portal-sharing-folders.md#non-admin-user-access-to-shared-folders) consente agli amministratori di controllare il modo in cui gli utenti non amministratori (Editor, Visualizzatori e Utenti ospiti) vedono le cartelle condivise dopo l'accesso.
