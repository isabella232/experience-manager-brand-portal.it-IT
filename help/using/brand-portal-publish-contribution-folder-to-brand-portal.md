---
title: 'Configurare e pubblicare la cartella dei contributi da Experience Manager Assets a Brand Portal '
seo-title: Configure and publish contribution folder from Experience Manager Assets to Brand Portal
description: Scopri come configurare e pubblicare una cartella di contributi da Experience Manager Assets a Brand Portal.
seo-description: Get an insight into configuring and publishing a contribution folder from Experience Manager Assets to Brand Portal.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 9acad588-977a-45de-b544-f2cc8874ba12
source-git-commit: 3845d9fa17e75d59493383303ca0978349ca0401
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# Configurare la cartella dei contributi in Experience Manager Assets {#configure-contribution-folder}

Per l’origine collaborativa delle risorse, gli utenti Experience Manager Assets (amministratori e utenti non amministratori che dispongono dell’autorizzazione) possono creare nuove cartelle di tipo **Contributo risorsa**, verifica che la nuova cartella creata sia aperta all’invio delle risorse da parte degli utenti Brand Portal.  Questo attiva automaticamente un flusso di lavoro che crea altre due sottocartelle, denominate **CONDIVISO** e **NUOVO** all&#39;interno della **Contributo** cartella.

L’utente di Experience Manager Assets definisce quindi i requisiti delle risorse caricando una breve descrizione dei tipi di risorse da aggiungere alla cartella dei contributi, nonché un set di risorse della linea di base, nel **CONDIVISO** per garantire agli utenti di Brand Portal le informazioni necessarie. L’amministratore può quindi concedere agli utenti Brand Portal attivi l’accesso alla cartella dei contributi prima di pubblicare la nuova cartella Contribution in Brand Portal.

Il video seguente illustra come configurare una cartella Contribution in Experience Manager Assets:

>[!VIDEO](https://video.tv.adobe.com/v/30547)

L’utente Experience Manager Assets esegue le seguenti attività durante la configurazione di una cartella di contributi:

* [Crea cartella contributi](#create-contribution-folder)
* [Caricare i requisiti delle risorse e assegnare i collaboratori](#configure-contribution-folder-properties)
* [Caricare le risorse della linea di base](#uplad-new-assets-to-contribution-folder)
* [Pubblicare la cartella dei contributi da Experience Manager Assets a Brand Portal](#publish-contribution-folder-to-brand-portal)

## Crea cartella contributi {#create-contribution-folder}


Gli amministratori di Experience Manager Assets e gli utenti non amministratori che dispongono dell’autorizzazione per creare una nuova cartella possono creare una cartella di contributo in Experience Manager Assets.
Per creare una cartella dei contributi, crea una nuova cartella di tipo Contributo risorse, in modo che la nuova cartella creata sia aperta all’invio delle risorse da parte degli utenti Brand Portal.  Questo attiva automaticamente un flusso di lavoro che crea due sottocartelle aggiuntive, denominate SHARED e NEW, all’interno della cartella dei contributi.


>[!NOTE]
>
>Gli amministratori possono creare più cartelle di contributi delle risorse all’interno di una cartella.
>
>Una cartella contributo risorse contiene cartelle NUOVE e CONDIVISE per la distribuzione e il contributo delle risorse. Non creare una risorsa, una cartella o una cartella di contributo all’interno di una cartella di contributo.


È possibile configurare le proprietà della cartella dei contributi separatamente e durante la creazione della cartella dei contributi. In questo esempio, configuriamo le proprietà separatamente.

**Per creare una cartella di contributo:**

1. Accedi alla tua istanza Experience Manager Assets.

1. Passa a **[!UICONTROL Risorse]** > **[!UICONTROL File]**. Elenca tutte le cartelle esistenti nell&#39;archivio Experience Manager Assets.

1. Fai clic su **[!UICONTROL Crea]** per creare una nuova cartella. **[!UICONTROL Crea cartella]** viene visualizzata la finestra di dialogo .

1. Invio **[!UICONTROL Titolo]** e **[!UICONTROL Nome]** della cartella e seleziona la **[!UICONTROL Contributo risorsa]** casella di controllo.
Si consiglia di utilizzare lettere minuscole senza spazio per denominare la cartella.

1. Fai clic su **[!UICONTROL Crea]**. Puoi visualizzare la cartella dei contributi elencata nell’archivio di Experience Manager Assets.

   >[!NOTE]
   >
   >Un utente non amministratore può creare e condividere una cartella di contributo delle risorse ma non può modificarla o eliminarla.


   ![](assets/create-contribution-folder.png)

1. Fai clic per aprire la cartella dei contributi. Sono disponibili due sottocartelle:**[!UICONTROL CONDIVISO]** e **[!UICONTROL NUOVO]** vengono create automaticamente all’interno della cartella dei contributi.

   ![](assets/contribution-folder.png)


## Configurare le proprietà della cartella dei contributi {#configure-contribution-folder-properties}

L’amministratore di Experience Manager Assets esegue le attività seguenti durante la configurazione delle proprietà di una cartella di contributi.

* **Aggiungi descrizione**: Fornisci una descrizione di alto livello della cartella dei contributi.
* **Carica breve**: Carica il documento Requisito risorse contenente informazioni relative alle risorse.
* **Aggiungi collaboratori**: Aggiungi gli utenti Brand Portal per concedere loro l’accesso alla cartella dei contributi.

Per requisito risorsa si intendono i dettagli forniti dagli amministratori per aiutare i collaboratori (utenti Brand Portal) a comprendere la necessità e i requisiti della cartella dei contributi. L’amministratore carica un documento relativo ai requisiti delle risorse che contiene una breve descrizione del tipo di risorse da aggiungere alla cartella Contributo e alle informazioni relative alle risorse, ad esempio scopo, tipo di immagini, dimensione massima, ecc.

**Per configurare le proprietà della cartella dei contributi:**

1. Accedi alla tua istanza Experience Manager Assets.

1. Passa a **[!UICONTROL Risorse > File]** e individua la cartella contribuzione.
1. Seleziona la cartella dei contributi e fai clic su **[!UICONTROL Proprietà]** per aprire la finestra delle proprietà della cartella.

   ![](assets/properties.png)

   ![](assets/contribution-folder-property1.png)

1. Passa a **[!UICONTROL Contributo risorsa]** scheda .
1. Inserisci di alto livello **[!UICONTROL Descrizione]** della cartella Contribution.
1. Fai clic su **[!UICONTROL Carica breve]** per sfogliare dal computer locale e caricare un **Documento sui requisiti delle risorse**.

   ![](assets/upload.png)

1. In **[!UICONTROL Aggiungi utente]** aggiungi gli utenti Brand Portal con i quali desideri condividere la cartella dei contributi. Questi utenti possono accedere e caricare il contenuto nella cartella dei contributi utilizzando l’interfaccia di Brand Portal.
1. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/contribution-folder-property3.png)

>[!NOTE]
>
>I risultati della ricerca si basano sull’elenco di utenti Brand Portal configurato in Experience Manager Assets. Verifica di disporre dell’elenco utenti Brand Portal aggiornato.

Gli amministratori possono scaricare `user.csv` file da [!DNL Admin Console] e utilizzarlo come modello di base per l’aggiunta di utenti Brand Portal. Vai a [!UICONTROL Utenti] e fai clic su [!UICONTROL Esportare l’elenco degli utenti in formato CSV] per scaricare `users.csv` file. Nell’elenco degli utenti di esempio riportato di seguito sono descritti gli attributi necessari per aggiungere gli utenti. L’unico attributo obbligatorio per una voce utente è il `Email` e tutti gli altri attributi sono facoltativi.

[Ottieni file](assets/users.csv)

## Caricare risorse nella cartella Contribution {#uplad-new-assets-to-contribution-folder}

L’utente di Experience Manager Assets carica un set di risorse della linea di base nel **CONDIVISO** per garantire agli utenti di Brand Portal le informazioni necessarie.

**Per caricare le risorse della linea di base:**

1. Accedi alla tua istanza Experience Manager Assets.

1. Passa a **[!UICONTROL Risorse > File]** e individua la cartella contribuzione.

1. Seleziona la cartella dei contributi e fai clic su per aprirla.

1. Fai clic sul pulsante **[!UICONTROL NUOVO]** cartella.

   ![](assets/upload-new-assets1.png)

1. Fai clic su **[!UICONTROL Crea]** > **[!UICONTROL File]** per caricare singoli file o cartelle (.zip) contenenti più risorse.

   ![](assets/upload-new-assets2.png)

1. Sfoglia e carica le risorse (file o cartelle) nel **[!UICONTROL NUOVO]** cartella.

   ![](assets/upload-asset4.png)

Dopo aver caricato tutte le risorse o le cartelle nella cartella NEW , pubblica la cartella Contribution in Experience Manager Assets.


## Pubblicare la cartella dei contributi in Brand Portal {#publish-contribution-folder-to-brand-portal}

Una volta configurata la cartella dei contributi, l’utente Experience Manager Assets (amministratore/non amministratore) può pubblicare la cartella dei contributi da Experience Manager Assets a Brand Portal. Gli utenti Brand Portal che dispongono dell’autorizzazione per accedere alla cartella dei contributi riceveranno una notifica e-mail/impulso al completamento dell’azione di pubblicazione.


**Per pubblicare la cartella dei contributi:**

1. Accedi alla tua istanza Experience Manager Assets.

1. Passa a **[!UICONTROL Risorse > File]** e individua la cartella dei contributi in cui vuoi pubblicare su Brand Portal.
1. Seleziona la cartella dei contributi e fai clic su **[!UICONTROL Pubblicazione rapida]** > **[!UICONTROL Pubblicare su Brand Portal]**.

   ![](assets/publish-contribution-folder-to-bp.png)

   Dopo la pubblicazione della cartella Contributo in Brand Portal, riceverai un messaggio di successo.

Viene inviata una notifica e-mail/impulso agli utenti Brand Portal assegnati alla cartella dei contributi. Gli utenti Brand Portal possono accedere alla cartella dei contributi e iniziare il contributo. Vedi [Caricare le risorse nella cartella dei contributi e pubblicarle in Experience Manager Assets](brand-portal-publish-contribution-folder-to-aem-assets.md).
