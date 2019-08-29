---
title: Utilizzo dei rapporti
seo-title: Utilizzo dei rapporti
description: Gli amministratori di AEM Assets Brand Portal possono visualizzare il rapporto sull'utilizzo di Brand Portal e creare, gestire e visualizzare i rapporti sulle risorse scaricate, scadute, pubblicate e collegate tramite Brand Portal.
seo-description: Gli amministratori di AEM Assets Brand Portal possono visualizzare il rapporto sull'utilizzo di Brand Portal e creare, gestire e visualizzare i rapporti sulle risorse scaricate, scadute, pubblicate e collegate tramite Brand Portal.
uuid: dc 4 e 5275-a 614-4 b 95-8 c 70-2 b 7 e 470 c 50 a 7
content-type: riferimento
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 7683074 f-b 6 ea -42 e 0-a 411-3 b 13 eb 88 d 1 f 2
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Utilizzo dei rapporti {#work-with-reports}

La funzionalità di reporting è fondamentale per valutare [!DNL Brand Portal] l'utilizzo e conoscere il modo in cui gli utenti interni e esterni interagiscono con le risorse approvate. Gli amministratori possono visualizzare [!DNL Brand Portal] il rapporto Utilizzo, disponibile sempre nella pagina Rapporti risorse. Tuttavia, i rapporti per accessi utente e risorse scaricate, scadute, pubblicate e condivise tramite i collegamenti possono essere generati e visualizzati dalla pagina Rapporti risorse. Questi report sono utili per analizzare la distribuzione delle risorse, che consente di derivare metriche chiave di successo per misurare l'adozione delle risorse approvate all'interno e all'esterno dell'organizzazione.

L'interfaccia di gestione dei report è intuitiva e include opzioni e controlli ben grassetto per accedere ai rapporti salvati. Potete visualizzare, scaricare o eliminare i rapporti dalla pagina Rapporti risorse, in cui vengono elencati tutti i rapporti precedentemente generati.

## Visualizzare i rapporti {#view-reports}

Per visualizzare un rapporto, effettuate le seguenti operazioni:

1. Nella barra degli strumenti in alto, toccate o fate clic sul [!DNL AEM] logo per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

2. Dal pannello Strumenti di amministrazione, fate clic su **Crea/Gestisci rapporti** per aprire** Report risorse**.

   ![](assets/access-asset-reports.png)

3. Rapporto **Utilizzo** accesso e altri rapporti generati dalla pagina Rapporti risorse.

   >[!NOTE]
   >
   >Il rapporto Utilizzo è presente per impostazione predefinita. [!DNL Brand Portal] Non può essere creato o eliminato. Tuttavia, potete creare, scaricare ed eliminare i rapporti Scarica, Scadenza, Pubblica, Condividi collegamento e Login utente.

   Per visualizzare un rapporto, tocca o fai clic sul collegamento del rapporto. In alternativa, selezionate il rapporto e toccate o fate clic sull'icona Visualizza dalla barra degli strumenti.

   **Il rapporto** sull'utilizzo visualizza informazioni sul numero di [!DNL Brand Portal] utenti correnti, lo spazio di archiviazione occupato da tutte le risorse e il totale delle risorse in. [!DNL Brand Portal] Il rapporto mostra inoltre la capacità consentita per ciascuna di queste metriche di informazioni.

   ![](assets/usage-report.png)

   **Il rapporto Login** utente fornisce informazioni sugli utenti a cui [!DNL Brand Portal]ha effettuato l'accesso. Il rapporto mostra i nomi visualizzati, gli ID e-mail, le personalizzazioni (amministratore, visualizzatore, editor, ospite), gruppi, ultimo login, stato dell'attività e conteggio di accesso di ciascun utente dalla [!DNL Brand Portal] distribuzione 6.4.2 fino alla data e all'ora della generazione dei report.

   ![](assets/user-logins.png)

   **Scaricare** elenchi di rapporti e dettagli su tutte le risorse scaricate in una data e nell'intervallo di tempo specifici.

   ![](assets/download-report.png)

   >[!NOTE]
   >
   >Le risorse** Download** mostrano solo le risorse selezionate e scaricate singolarmente. [!DNL Brand Portal] Se un utente ha scaricato una cartella contenente delle risorse, il rapporto non visualizza la cartella o le risorse all'interno della cartella.

   **Elenchi** di rapporti di scadenza e dettagli su tutte le risorse scadute in un intervallo specifico.

   ![](assets/expiration-report.png)

   **Pubblica** elenchi di rapporti e fornisce informazioni su tutte le risorse pubblicate [!DNL AEM] in [!DNL Brand Portal] un intervallo di tempo specificato.

   ![](assets/publish-report.png)

   >[!NOTE]
   >
   >Il rapporto Pubblica non visualizza informazioni sui frammenti di contenuto, in quanto i frammenti di contenuto non possono essere pubblicati in [!DNL Brand Portal].

   **Il rapporto Condividi condivisione** elenca tutte le risorse condivise tramite collegamenti dall [!DNL Brand Portal] 'interfaccia in un intervallo specifico. Il rapporto informa anche quando è stata condivisa la risorsa tramite collegamento, tramite quale utente, quando è scaduto il collegamento e quanti collegamenti condivisi per il tenant (e gli utenti con cui è stato condiviso il collegamento). Le colonne di Collegamento condivisione non sono personalizzabili.

   ![](assets/link-share-report.png)

   >[!NOTE]
   >
   >Il rapporto Condivisione collegamento non visualizza gli utenti che hanno accesso alla risorsa condivisa tramite il collegamento o che hanno scaricato la risorsa tramite il collegamento.
   >
   >
   >Per tenere traccia dei download tramite il collegamento condiviso, è necessario generare il rapporto di download dopo aver selezionato **l'opzione Solo condivisione collegamenti** nella **pagina Crea rapporto** . Tuttavia, l'utente (scaricato da) è anonimo in questo caso.

## Generazione di rapporti {#generate-reports}

Gli amministratori possono generare e gestire i seguenti rapporti standard, una volta generati, [salvati](../using/brand-portal-reports.md#main-pars-header) in un secondo momento:

* Accessi utenti
* Scarica
* Scadenza
* Pubblicazione
* Condivisione collegamenti

Le colonne nei rapporti Scarica, Scadenza e Pubblica possono essere personalizzate per la visualizzazione. Per generare un rapporto, effettuate le seguenti operazioni:

1. Da barra degli strumenti nella parte superiore, toccate o fate clic sul [!DNL AEM] logo per accedere agli strumenti di amministrazione.

   ![](assets/aemlogo.png)

2. Nel pannello Strumenti di amministrazione, toccate/fate clic **su Crea/Gestisci rapporti** per aprire** Report risorse**.

   ![](assets/asset-reports.png)

3. Nella pagina Rapporti risorse, toccate o fate clic **su Crea**.
4. Nella pagina **Crea rapporto** , selezionate un rapporto da creare e toccate o fate clic **su Avanti**.

   ![](assets/crete-report.png)

5. Configurare i dettagli del rapporto. Specifica titolo, descrizione, struttura delle cartelle (dove è necessario eseguire il rapporto e genera statistiche), e intervallo di date per **i rapporti Scarica**, **Scadenza** e **Pubblica** .

   ![](assets/create-report-page.png)

   Tuttavia **, per il report** Condividi condivisione sono necessari solo i parametri titolo, descrizione e intervallo di date.

   ![](assets/create-link-share-report.png)

   >[!NOTE]
   >
   >I caratteri speciali # e % nel titolo del rapporto vengono sostituiti da un trattino (-) sulla generazione dei report.

6. Tocca o fai clic **su Avanti**, per configurare le colonne dei rapporti Scarica, Scadenza e Pubblica.
7. Seleziona o deseleziona le caselle di controllo appropriate, a seconda delle necessità. Ad esempio, per visualizzare i nomi degli utenti (che hanno scaricato le risorse) nel **rapporto Download** , selezionate **Scaricato da**. L'immagine seguente illustra la selezione delle colonne predefinite nel rapporto Download.

   ![](assets/createdownloadreport.png)

   Potete inoltre aggiungere colonne personalizzate a tali rapporti per visualizzare più dati in base ai requisiti personalizzati.

   Per aggiungere colonne personalizzate al rapporto Scarica, Pubblica o Scadenza, effettuate le seguenti operazioni:

   1. Per visualizzare una colonna personalizzata, toccate o fate clic **su Aggiungi** all'interno **delle colonne personalizzate**.
   2. Specificate il nome della colonna nel **campo Nome** colonna.
   3. Selezionate la proprietà a cui deve essere mappata la colonna, utilizzando il selettore delle proprietà.

      ![](assets/property-picker.png)In alternativa, digitate il percorso nel campo percorso proprietà.

      ![](assets/property-path.png)

      Per aggiungere altre colonne personalizzate, toccate o fate clic **su Aggiungi** e ripetete i passaggi 2 e 3.

8. Tocca o fai clic su **Crea**. Un messaggio notifica che è stata avviata la generazione dei report.

## Download dei rapporti {#download-reports}

Per salvare e scaricare un rapporto come file. csv, effettua una delle operazioni seguenti:

* Selezionate un rapporto sulla pagina Rapporti risorsa e toccate o fate clic **su Scarica** nella barra degli strumenti in alto.

![](assets/download-asset-report.png)

* Dalla pagina Rapporti risorse, apri un rapporto. Selezionate **Scarica** nella parte superiore della pagina del rapporto.

![](assets/download-report-fromwithin.png)

## Eliminare i rapporti {#delete-reports}

Per eliminare un rapporto esistente, selezionate il rapporto dalla **pagina Rapporti** risorse e toccate o fate clic **su Elimina** nella barra degli strumenti in alto.

>[!NOTE]
>
>**Il rapporto Utilizzo** non può essere eliminato.
