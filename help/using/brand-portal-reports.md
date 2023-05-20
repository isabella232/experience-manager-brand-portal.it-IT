---
title: Utilizzare i rapporti
seo-title: Work with reports
description: Gli amministratori di Experience Manager Assets Brand Portal possono visualizzare i rapporti sull’utilizzo di Brand Portal e creare, gestire e visualizzare i rapporti sulle risorse scaricate, scadute, pubblicate e condivise tramite Brand Portal.
seo-description: Experience Manager Assets Brand Portal Administrators can view report about Brand Portal usage, and create, manage, and view reports around assets downloaded, expired, published, and link shared through Brand Portal.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: reference
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
role: Admin
exl-id: 03d0292c-23c2-4ea0-9781-eb27768e6c33
source-git-commit: 955cd8afe939ff47e9f08f312505e230e2f38495
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 2%

---

# Utilizzare i rapporti {#work-with-reports}

La funzionalità di reporting è fondamentale per valutare l’utilizzo di Brand Portal e conoscere il modo in cui gli utenti interni ed esterni interagiscono con le risorse approvate. Gli amministratori possono visualizzare il rapporto sull’utilizzo di Brand Portal, sempre disponibile nella pagina Rapporti sulle risorse. Tuttavia, i rapporti per gli accessi degli utenti e le risorse scaricate, scadute, pubblicate e condivise tramite collegamenti possono essere generati e visualizzati dalla pagina Rapporti sulle risorse. Questi rapporti sono utili per l’analisi della distribuzione delle risorse, che consente di derivare metriche di successo chiave per misurare il livello di adozione delle risorse approvate all’interno e all’esterno dell’organizzazione.

L’interfaccia di gestione dei rapporti è intuitiva e include opzioni e controlli dettagliati per accedere ai rapporti salvati. Puoi visualizzare, scaricare o eliminare i rapporti dalla pagina Rapporti su risorse, in cui sono elencati tutti i rapporti generati in precedenza.

## Visualizzare i rapporti {#view-reports}

Per visualizzare un rapporto, effettua le seguenti operazioni:

1. Dalla barra degli strumenti nella parte superiore, tocca o fai clic sul logo dell’Experience Manager per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

1. Nel pannello Strumenti di amministrazione, fate clic su **[!UICONTROL Creare/gestire i rapporti]** per aprire **[!UICONTROL Rapporti su risorse]** pagina.

   ![](assets/access-asset-reports.png)

1. Accesso **[!UICONTROL Utilizzo]** report e altri report generati dalla pagina Report risorse.

   >[!NOTE]
   >
   >Il rapporto di utilizzo è un rapporto predefinito generato in Brand Portal. Non può essere creata o eliminata. Tuttavia, puoi creare, scaricare ed eliminare i rapporti Scarica, Scadenza, Pubblica, Condivisione collegamenti e Accessi utente.

   Per visualizzare un rapporto, fai clic sul collegamento al rapporto. In alternativa, seleziona il rapporto e tocca o fai clic sull’icona Visualizza nella barra degli strumenti.

   **[!UICONTROL Rapporto utilizzo]** visualizza informazioni sul numero di utenti Brand Portal attivi, lo spazio di archiviazione occupato da tutte le risorse e il conteggio totale delle risorse in Brand Portal. Gli utenti di Brand Portal che non sono assegnati ad alcun profilo di prodotto nell’Admin Console vengono considerati utenti inattivi e non si riflettono nel **[!UICONTROL Rapporto utilizzo]**.
Il rapporto mostra anche la capacità consentita per ciascuna di queste metriche informative.

   ![](assets/usage-report.png)

   **[!UICONTROL Accessi utente]** Questo rapporto fornisce informazioni sugli utenti che hanno effettuato l’accesso a Brand Portal. Il rapporto mostra nomi visualizzati, ID e-mail, utenti tipo (amministratore, visualizzatore, editor, ospite), gruppi, ultimo accesso, stato attività e conteggio di accesso di ogni utente dalla distribuzione di Brand Portal 6.4.2 fino al momento della generazione del rapporto.

   ![](assets/user-logins.png)

   **[!UICONTROL Scarica]** il rapporto elenca e fornisce dettagli su tutte le risorse scaricate in un intervallo di date e ore specifico.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >Le risorse **[!UICONTROL Scarica]** Questo rapporto visualizza solo le risorse selezionate e scaricate singolarmente da Brand Portal. Se un utente ha scaricato una cartella contenente risorse, il rapporto non visualizza la cartella o le risorse all’interno della cartella.

   **[!UICONTROL Scade]** il rapporto elenca e fornisce dettagli su tutte le risorse scadute in un intervallo di tempo specifico.

   ![](assets/expiration-report.png)

   **[!UICONTROL Pubblica]** il rapporto elenca e fornisce informazioni su tutte le risorse pubblicate da Experience Manager Assets a Brand Portal in un intervallo di tempo specificato.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Il rapporto di pubblicazione non visualizza informazioni sui frammenti di contenuto, poiché questi non possono essere pubblicati in Brand Portal.

   **[!UICONTROL Rapporto Condivisione collegamenti]** elenca tutte le risorse condivise tramite collegamenti dall’interfaccia di Brand Portal in un intervallo di tempo specifico. Il rapporto indica anche quando la risorsa è stata condivisa tramite collegamento, da quale utente, quando scade il collegamento e il numero di collegamenti condivisi per il tenant (e gli utenti con cui è stato condiviso il collegamento alla risorsa). Le colonne del rapporto Condivisione collegamenti non sono personalizzabili.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Nel rapporto Condivisione collegamenti non vengono visualizzati gli utenti che hanno accesso alla risorsa condivisa tramite il collegamento o che hanno scaricato la risorsa tramite il collegamento.
   >
   >Per tenere traccia dei download tramite il collegamento condiviso, devi generare un rapporto sui download dopo aver selezionato **[!UICONTROL Solo download da condivisione collegamenti]** opzione su **[!UICONTROL Crea rapporto]** pagina. Tuttavia, in questo caso, l’utente (scaricato da) è anonimo.

## Generare rapporti {#generate-reports}

Gli amministratori possono generare e gestire i seguenti rapporti standard: una volta generati, vengono salvati per essere [accesso eseguito](../using/brand-portal-reports.md#main-pars-header) più tardi:

* Accessi utenti
* Scarica
* Scadenza
* Pubblicazione
* Condivisione collegamenti

Le colonne nei rapporti Scarica, Scadenza e Pubblica possono essere personalizzate per la visualizzazione. Per generare un rapporto, effettua le seguenti operazioni:

1. Dalla barra degli strumenti nella parte superiore, tocca o fai clic sul logo dell’Experience Manager per accedere agli strumenti di amministrazione.

1. Dal pannello Strumenti di amministrazione, tocca o fai clic su **[!UICONTROL Creare/gestire i rapporti]** per aprire **[!UICONTROL Rapporti su risorse]** pagina.

   ![](assets/asset-reports.png)

1. Nella pagina Rapporti su risorse, tocca o fai clic su **[!UICONTROL Crea]**.
1. Dalla sezione **[!UICONTROL Crea rapporto]** , seleziona un rapporto da creare e tocca o fai clic su **[!UICONTROL Successivo]**.

   ![](assets/crete-report.png)

1. Configurare i dettagli del rapporto. Specifica il titolo, la descrizione, la struttura delle cartelle (dove il rapporto deve essere eseguito e generare le statistiche) e l’intervallo di date per **[!UICONTROL Scarica]**, **[!UICONTROL Scade]**, e **[!UICONTROL Pubblica]** rapporti.

   ![](assets/create-report-page.png)

   considerando quanto segue: **[!UICONTROL Rapporto condivisione collegamenti]** sono necessari solo i parametri title, description e date range.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >I caratteri speciali # e % nel titolo del rapporto sono sostituiti da un trattino (-) nella generazione del rapporto.

1. Tocca o fai clic **[!UICONTROL Successivo]**, per configurare le colonne dei rapporti Scarica, Scadenza e Pubblica.
1. Seleziona o deseleziona le caselle di controllo appropriate, in base alle esigenze. Ad esempio, per visualizzare i nomi degli utenti (che hanno scaricato le risorse) in **[!UICONTROL Scarica]** report, seleziona **[!UICONTROL Scaricato da]**. L’immagine seguente illustra come selezionare le colonne predefinite nel rapporto di download.

   ![](assets/createdownloadreport.png)

   Puoi anche aggiungere colonne personalizzate a questi rapporti per visualizzare più dati per i requisiti personalizzati.

   Per aggiungere colonne personalizzate ai rapporti Scarica, Pubblica o Scadenza, effettua le seguenti operazioni:

   1. Per visualizzare una colonna personalizzata, tocca o fai clic su **[!UICONTROL Aggiungi]** entro [!UICONTROL Colonne personalizzate].
   1. Specifica il nome della colonna in **[!UICONTROL Nome colonna]** campo.
   1. Seleziona la proprietà a cui mappare la colonna utilizzando il selettore delle proprietà.

      ![](assets/property-picker.png)
In alternativa, digita il percorso nel campo percorso proprietà.

      ![](assets/property-path.png)

      Per aggiungere altre colonne personalizzate, tocca o fai clic su **Aggiungi** e ripetere i passaggi 2 e 3.

1. Tocca o fai clic su **[!UICONTROL Crea]**. Un messaggio notifica che la generazione del rapporto è stata avviata.

## Scaricare i rapporti {#download-reports}

Per salvare e scaricare un report come file .csv, effettuare una delle seguenti operazioni:

* Seleziona un rapporto nella pagina Rapporti su risorse, quindi tocca o fai clic **[!UICONTROL Scarica]** dalla barra degli strumenti nella parte superiore.

![](assets/download-asset-report.png)

* Dalla pagina Rapporti su risorse, apri un rapporto. Seleziona **[!UICONTROL Scarica]** nella parte superiore della pagina del rapporto.

![](assets/download-report-fromwithin.png)

## Eliminare i rapporti {#delete-reports}

Per eliminare un rapporto esistente, selezionalo da **[!UICONTROL Rapporti su risorse]** pagina e tocca o fai clic **[!UICONTROL Elimina]** dalla barra degli strumenti nella parte superiore.

>[!NOTE]
>
>**[!UICONTROL Utilizzo]** il report non può essere eliminato.
