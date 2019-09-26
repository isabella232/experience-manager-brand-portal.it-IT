---
title: Utilizzo dei rapporti
seo-title: Utilizzo dei rapporti
description: Gli amministratori del Brand Portal di AEM Assets possono visualizzare rapporti sull’utilizzo del Brand Portal e creare, gestire e visualizzare rapporti sulle risorse scaricate, scadute, pubblicate e sui collegamenti condivisi tramite il Brand Portal.
seo-description: Gli amministratori del Brand Portal di AEM Assets possono visualizzare rapporti sull’utilizzo del Brand Portal e creare, gestire e visualizzare rapporti sulle risorse scaricate, scadute, pubblicate e sui collegamenti condivisi tramite il Brand Portal.
uuid: dc4e5275-a614-4b95-8c70-2b7e470c50a7
content-type: riferimento
topic-tags: administration
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 7683074f-b6ea-42e0-a411-3b13eb88d1f2
translation-type: tm+mt
source-git-commit: 9763a57a83db22cd6686701dcbd8fcde16bcbb31

---


# Utilizzo dei rapporti {#work-with-reports}

La funzionalità di reporting è fondamentale per valutare l’utilizzo del Brand Portal e sapere in che modo gli utenti interni ed esterni interagiscono con le risorse approvate. Gli amministratori possono visualizzare il rapporto Utilizzo del Brand Portal, sempre disponibile nella pagina Rapporti risorse. Tuttavia, i rapporti per accessi utente e risorse scaricate, scadute, pubblicate e condivise tramite i collegamenti possono essere generati e visualizzati dalla pagina Rapporti risorse. Questi rapporti sono utili per analizzare la distribuzione delle risorse, per derivare le metriche di successo chiave per misurare l’adozione di risorse approvate all’interno e all’esterno dell’organizzazione.

L'interfaccia di gestione dei report è intuitiva e include opzioni e controlli di granulometria per accedere ai report salvati. Potete visualizzare, scaricare o eliminare i rapporti dalla pagina Rapporti risorse, in cui sono elencati tutti i rapporti generati in precedenza.

## Visualizzare i rapporti {#view-reports}

Per visualizzare un rapporto, effettuate le seguenti operazioni:

1. Dalla barra degli strumenti nella parte superiore, tocca o fai clic sul logo AEM per accedere agli strumenti amministrativi.

   ![](assets/aemlogo.png)

2. Dal pannello degli strumenti di amministrazione, fate clic su **[!UICONTROL Crea/gestisci rapporti]** per aprire la pagina Rapporti **** risorse.

   ![](assets/access-asset-reports.png)

3. Accedete al rapporto **[!UICONTROL Utilizzo]** e ad altri rapporti generati dalla pagina Rapporti risorse.

   >[!NOTE]
   >
   >Il rapporto sull'utilizzo è presente per impostazione predefinita in Brand Portal. Non può essere creato o eliminato. Tuttavia, potete creare, scaricare ed eliminare i rapporti Download, Scadenza, Pubblica, Condivisione collegamenti e Login utente.

   Per visualizzare un rapporto, toccate o fate clic sul collegamento del rapporto. In alternativa, seleziona il rapporto e tocca o fai clic sull’icona Visualizza nella barra degli strumenti.

   [!UICONTROL Report] sull’utilizzo visualizza informazioni sul numero di utenti correnti del Brand Portal, sullo spazio di archiviazione occupato da tutte le risorse e sul totale delle risorse conteggiate nel Brand Portal. Il rapporto mostra anche la capacità consentita per ciascuna di queste metriche di informazioni.

   ![](assets/usage-report.png)

   [!UICONTROL Il rapporto Login] utente fornisce informazioni sugli utenti che hanno eseguito l'accesso al Portale marchio. Il rapporto mostra i nomi visualizzati, gli ID e-mail, le persone (amministratore, visualizzatore, editor, ospite), i gruppi, l'ultimo login, lo stato dell'attività e il conteggio di login di ciascun utente dalla distribuzione di Brand Portal 6.4.2 fino al momento della generazione del rapporto.

   ![](assets/user-logins.png)

   [!UICONTROL Scaricate] elenchi di rapporti e dettagli su tutte le risorse scaricate in un intervallo di date e ore specifico.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >Il rapporto [!UICONTROL Scarica] risorse visualizza solo le risorse che sono state selezionate singolarmente e scaricate dal Brand Portal. Se un utente ha scaricato una cartella contenente delle risorse, il rapporto non visualizza la cartella o le risorse all’interno della cartella.

   [!UICONTROL Il rapporto Scadenza] elenca e fornisce dettagli a tutte le risorse scadute in un intervallo di tempo specifico.

   ![](assets/expiration-report.png)

   [!UICONTROL Il rapporto Pubblica] elenca e fornisce informazioni su tutte le risorse pubblicate da AEM a Brand Portal in un intervallo di tempo specificato.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Pubblica rapporto non visualizza informazioni sui frammenti di contenuto, in quanto non è possibile pubblicare i frammenti di contenuto nel Brand Portal.

   [!UICONTROL Nel rapporto] Condivisione collegamenti sono elencate tutte le risorse condivise tramite collegamenti dall’interfaccia del Portale marchio in un intervallo di tempo specifico. Il rapporto informa anche quando la risorsa è stata condivisa tramite collegamento, da quale utente, quando scade il collegamento, e quanti collegamenti condivisi per il tenant (e gli utenti con cui è stato condiviso il collegamento della risorsa). Le colonne del Rapporto condivisione collegamenti non sono personalizzabili.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Il rapporto Condivisione collegamenti non visualizza gli utenti che hanno accesso alla risorsa condivisa tramite il collegamento o che hanno scaricato la risorsa tramite il collegamento.
   >
   >
   >Per tenere traccia dei download tramite il collegamento condiviso, è necessario generare un rapporto di download dopo aver selezionato l'opzione **[!UICONTROL Solo download]** condivisione collegamento nella pagina **[!UICONTROL Crea rapporto]** . Tuttavia, l'utente (Scaricato da) è anonimo in questo caso.

## Generazione di rapporti {#generate-reports}

Una volta generati, gli amministratori possono generare e gestire i seguenti rapporti standard, per poi [accedervi](../using/brand-portal-reports.md#main-pars-header) in un secondo momento:

* Accessi utenti
* Scarica
* Scadenza
* Pubblicazione
* Condivisione collegamenti

Le colonne nel rapporto Download, Scadenza e Pubblica possono essere personalizzate per la visualizzazione. Per generare un rapporto, effettuate le seguenti operazioni:

1. Dalla barra degli strumenti nella parte superiore, tocca o fai clic sul logo AEM per accedere agli strumenti amministrativi.

   ![](assets/aemlogo.png)

2. Dal pannello degli strumenti di amministrazione, toccate/fate clic su **[!UICONTROL Crea/Gestisci rapporti]** per aprire la pagina Rapporti **** risorse.

   ![](assets/asset-reports.png)

3. Nella pagina Rapporti risorse, toccate o fate clic su **[!UICONTROL Crea]**.
4. Dalla pagina **[!UICONTROL Crea rapporto]** , selezionate un rapporto da creare e toccate o fate clic su **[!UICONTROL Avanti]**.

   ![](assets/crete-report.png)

5. Configurare i dettagli del rapporto. Specificate titolo, descrizione, struttura delle cartelle (dove il rapporto deve essere eseguito e generare statistiche) e intervallo di date per i rapporti [!UICONTROL Download], [!UICONTROL Scadenza]e [!UICONTROL Pubblica] .

   ![](assets/create-report-page.png)

   Al contrario, [!UICONTROL Collega rapporto] condivisione richiede solo i parametri di titolo, descrizione e intervallo di date.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >I caratteri speciali # e % nel titolo del rapporto sono sostituiti da un trattino (-) nella generazione del rapporto.

6. Toccate/fate clic su **[!UICONTROL Avanti]** per configurare le colonne dei rapporti Download, Scadenza e Pubblica.
7. Selezionate o deselezionate le caselle di controllo appropriate a seconda delle necessità. Ad esempio, per visualizzare i nomi degli utenti (che hanno scaricato delle risorse) nel rapporto [!UICONTROL Download] , selezionate **[!UICONTROL Scaricato da]**. L'immagine seguente illustra la selezione di colonne predefinite nel rapporto Download.

   ![](assets/createdownloadreport.png)

   Puoi anche aggiungere colonne personalizzate a questi rapporti per visualizzare più dati per i tuoi requisiti personalizzati.

   Per aggiungere colonne personalizzate al rapporto Download, Publish o Expiration, effettuate le seguenti operazioni:

   1. Per visualizzare una colonna personalizzata, toccate o fate clic su **[!UICONTROL Aggiungi]** in Colonne personalizzate.
   2. Specificare il nome della colonna nel campo Nome **** colonna.
   3. Selezionate la proprietà a cui deve essere associata la colonna utilizzando il selettore delle proprietà.

      ![](assets/property-picker.png)
In alternativa, digitare il percorso nel campo percorso della proprietà.

      ![](assets/property-path.png)

      Per aggiungere altre colonne personalizzate, toccate/fate clic su **Aggiungi** e ripetete i passaggi 2 e 3.

8. Tocca o fai clic su **[!UICONTROL Crea]**. Un messaggio notifica che è stata avviata la generazione del report.

## Download dei rapporti {#download-reports}

Per salvare e scaricare un rapporto come file .csv, effettuare una delle seguenti operazioni:

* Selezionate un rapporto nella pagina Rapporti risorse, quindi toccate o fate clic su **[!UICONTROL Scarica]** dalla barra degli strumenti nella parte superiore.

![](assets/download-asset-report.png)

* Dalla pagina Rapporti risorse, aprite un rapporto. Selezionate **[!UICONTROL Scarica]** opzione nella parte superiore della pagina del rapporto.

![](assets/download-report-fromwithin.png)

## Eliminare i rapporti {#delete-reports}

Per eliminare un rapporto esistente, selezionatelo dalla pagina Rapporti **** risorse e toccate o fate clic su **[!UICONTROL Elimina]** dalla barra degli strumenti nella parte superiore.

>[!NOTE]
>
>[!UICONTROL Impossibile eliminare il rapporto sull'utilizzo] .
