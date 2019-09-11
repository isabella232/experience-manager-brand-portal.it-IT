---
title: Accelerare i download di Brand Portal
seo-title: Accelerare i download di Brand Portal
description: Migliorate le prestazioni di download dal portale brand e dai collegamenti condivisi.
seo-description: Migliorate le prestazioni di download dal portale brand e dai collegamenti condivisi.
uuid: 2871137 e -6471-49 a 7-872 a -841 bd 92543 d 1
contentOwner: mgulati
topic-tags: download-install
content-type: riferimento
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 301 f 7 a 0 b -5527-4 aac-b 731-bfc 145 fed 0 c 0
translation-type: tm+mt
source-git-commit: fb8243ea896d39b324a69ea534271ee3015c076f

---


# Accelerare i download di Brand Portal {#guide-to-accelerate-downloads-from-brand-portal}

Brand Portal consente di migliorare le prestazioni di download dei file di risorse di grandi dimensioni mediante l'integrazione con IBM Aspera Connect, un'applicazione di installazione. L'applicazione utilizza tecnologie proprietarie per rimuovere i sovraccarichi TCP e migliorare la velocità di trasferimento dei file di risorse. Questa integrazione garantisce un'esperienza di download avanzata.

>[!NOTE]
>
>La velocità di download varia a seconda degli utenti che dipendono da fattori quali larghezza di banda, latenza server e posizione geografica dei client.

Se abilitata, gli utenti del portale marchio possono ridurre notevolmente il tempo necessario per scaricare i file di risorse desiderati da Brand Portal o tramite il collegamento Condiviso installando il client Aspera Connect.

![](assets/enable-fast-file-download.png)

## Prerequisiti per accelerare il download dei file {#prerequisites-to-accelerate-file-download}

Per scaricare i file più rapidamente, assicurati che:

* **[!UICONTROL Attiva accelerazione download]** (disattivata per impostazione predefinita) da [!UICONTROL Impostazioni generali] nel pannello Strumenti di amministrazione.
* La porta 33001 (sia TCP che UDP) è aperta sul firewall. Per ulteriori informazioni sui prerequisiti, consultate [la documentazione Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).
* Installate Aspera Connect mediante i privilegi di amministratore.
* Per il supporto piattaforma del client di trasferimento Aspera, consultate [Matrice di supporto della piattaforma Aspera Connect](https://www.asperasoft.com/company/support/transfer-clients/).

## Download dei domini {#download-domains}

Di seguito sono indicati i domini di download per diverse aree geografiche:

| Codice regione | Dominio |
|---|---|
| NA OR 1 | downloads-na1.brand-portal.adobe.com |
| NA VA 5 | downloads-na2.brand-portal.adobe.com |
| EMEA LON 5 | downloads-emea1.brand-portal.adobe.com |
| APAC SIN 2 | downloads-apac1.brand-portal.adobe.com |

## Prestazioni di download di esempio utilizzando acceleratore file {#expected-download-performance-using-file-accelerator}

La tabella seguente mostra le prestazioni di download per file 2 GB utilizzando l'acceleratore di download del file Aspera Connect:

**I risultati osservati variano a causa di fattori quali larghezza di banda di rete, latenza server e posizione client, considerando il server Brand Portal in Oregon (Stati Uniti).*

| Percorso cliente | Latenza tra client e server (millisecondi) | Velocità con Aspera Connect File Transfer Accelerator (MBps) | Tempo impiegato per scaricare file 2 GB con Aspera File Transfer Accelerator (secondi) |
|---------------------------|-----------------------------------|---------------------------------------------|-------------------------------------------------------------------------|
| Occidentale Occidentale (N. California) | 18 | 36 | 57 |
| Occidentale (Oregon) | 42 | 36 | 57 |
| U.S. East (N. Virginia) | 85 | 35 | 58 |
| APAC (Tokyo) | 124 | 36 | 57 |
| Noida (India) | 275 | 13.36 | 153 |
| Sydney | 175 | 29 | 70 |
| Londra | 179 | 35 | 58 |
| Singapore | 196 | 34 | 60 |

## Download del flusso di lavoro utilizzando l'acceleratore del file {#download-workflow-using-file-accelerator}

Per scaricare più rapidamente le risorse dal portale brand:

1. Effettuate l'accesso al portale marchio utilizzando un browser supportato.
2. Sfogliate e selezionate il file, la cartella o la raccolta desiderati per il download. Toccate/fate clic sul pulsante di download.
Viene visualizzata la finestra di dialogo di download con [l'opzione Abilita accelerazione] download selezionata.
   ![](assets/download-assetsbp.png)

   >[!NOTE]
   >
   >La funzionalità per inviare una notifica e-mail con il collegamento per scaricare le risorse non è attualmente supportata, mentre i download più rapidi sono abilitati.

   ![](assets/fast-download-emailchk.png)

3. Toccate o fate clic sull'opzione **[!UICONTROL Scarica]** .
Per velocizzare l'esperienza di download sull'account tenant di Brand Portal, nel sistema deve essere installato l'applicazione client Aspera Connect.

4. **Download del client Aspera Connect Client**
Se il client Aspera Connect non è installato sul sistema o il client Aspera Connect esistente non è aggiornato, nella pagina del browser viene visualizzato un prompt da dove è possibile scaricare il client Aspera Connect specifico del sistema selezionando **[!UICONTROL Scarica versione più recente]**.

   ![](assets/aspera-not-launched.png)

   Per scaricare la versione più recente di Aspera Connect da [https://downloads.asperasoft.com/connect2/](https://downloads.asperasoft.com/connect2/), selezionate **[!UICONTROL Scarica ora]** e seguite le istruzioni.

5. **Installa il client Aspera Connect Per**
installare la configurazione client IBM Aspera Connect, eseguite l'impostazione dal file. msi dell'applicazione client IBM Aspera Connect e seguite la procedura guidata di installazione.

6. Una volta installato il client, aggiornate la pagina del browser e avviate nuovamente i passaggi di download oppure selezionate **[!UICONTROL Riavvia]** nella finestra **[!UICONTROL di]** dialogo Download delle risorse (passaggio # 2).
Quando si utilizza Aspera Connect per la prima volta, viene richiesto di aprire il collegamento tramite **[!UICONTROL IBM Aspera Connect]**. Per saltare la finestra di dialogo in futuro, abilita **[!UICONTROL Ricorda scelta per i collegamenti FASP]**.

   >[!NOTE]
   >
   >Questo messaggio è diverso sui diversi browser.

7. Una finestra di dialogo conferma se spostare o meno il trasferimento. Selezionate **[!UICONTROL Consenti]** inizio.
Per saltare questa finestra di dialogo in futuro, abilitate **[!UICONTROL la scelta personale per tutte le connessioni con l'host]**.
Il download inizia. Una finestra di dialogo mostra l'avanzamento del download. Utilizzare la finestra di dialogo **[!UICONTROL per sospendere]**, **[!UICONTROL riprendere]** o **[!UICONTROL annullare]** il download.
L'applicazione Aspera Connect fornisce una finestra Attività nel sistema in cui l'utente può visualizzare e gestire tutte le sessioni di trasferimento. Per ulteriori informazioni, fate riferimento [alla documentazione Aspera Connect Client](https://downloads.asperasoft.com/en/documentation/8).

![](assets/aspera-activity-window.png)

Al termine del download, una finestra di dialogo mostra il percorso in cui le risorse vengono scaricate nel sistema dell'utente. Se si verifica un errore, viene visualizzato un errore.

>[!NOTE]
>
>Esiste un limite noto nell'applicazione client Aspera Connect che non viene richiesto di selezionare la posizione di download se **[!UICONTROL viene richiesto sempre dove salvare i file]** scaricati nella scheda [!UICONTROL Trasferimenti] di schede all'interno [!UICONTROL delle Preferenze]. Prima di iniziare il download, indicate la posizione nella casella di testo in **[!UICONTROL cui salvare i file scaricati]**.

## Utilizzo acceleratore file nel browser Microsoft Edge {#using-file-accelerator-on-microsoft-edge-browser}

Microsoft Edge viene eseguito in modalità protetta avanzata (EPM), che impedisce la comunicazione con il server Aspera Connect, nella stessa rete privata o con un sito affidabile. Di conseguenza, viene visualizzata una finestra popup ogni volta che viene stabilita una connessione con il server.

![](assets/switchapps-msedge.png)

Per utilizzare la funzionalità di download accelerata su Microsoft Edge, rimuovete il sito Brand Portal dall'elenco dei siti affidabili.

1. Aprite il Pannello di controllo (premete **[!UICONTROL Finestra + X]**, quindi selezionate **[!UICONTROL Pannello di controllo]**).
2. Andate a **[!UICONTROL Rete e Internet &gt; Opzioni Internet]**. Fate clic sulla scheda **[!UICONTROL Protezione]** .
3. Fate clic sulla **[!UICONTROL zona Siti affidabili]**, quindi su **[!UICONTROL Siti]**.
4. Rimuovere il sito Brand Portal dall'elenco.

## Preferenze client Aspera Connect {#aspera-connect-client-preferences}

Alcune preferenze utili possono essere impostate nella preferenza Client Aspera IBM Aspera facendo clic con il pulsante destro del mouse sull'icona e selezionando **[!UICONTROL Preferenze]**.

![](assets/download_assets_frombrandportalimg19.png)

Potete impostare il percorso di download predefinito.

![](assets/aspera-preferences.png)

Inoltre, il client Aspera Connect può essere contrassegnato automaticamente all'avvio del sistema in modo che il client Connect sia in esecuzione e sia disponibile affinché il download inizi più rapidamente.

![](assets/aspera-automaticallylaunch.png)

## Risoluzione dei problemi con l'accelerazione del download {#troubleshoot-issues-with-download-acceleration}

Se l'accelerazione del download non funziona per voi, effettuate le seguenti operazioni per risolvere i problemi:

1. Verificate che le porte non vengano bloccate, visitando [https://test-connect.asperasoft.com](https://test-connect.asperasoft.com/) dal computer.

   Se le porte non vanno a buon fine, rivolgetevi al team di rete e assicuratevi che Porte 33001 (sia TCP e UDP) sia bloccata nel firewall.

2. Se le porte sono OK, controllate che la rete non sia lenta, misurando la larghezza di banda disponibile tramite [https://www.speedtest.net/](https://www.speedtest.net/).

   Se la larghezza di banda è di pochi (1-10 Mbps) o in Kbps, utilizzate le preferenze Aspera e provate a limitare la larghezza di banda pari all'ampiezza di banda disponibile.

3. Per confermare se i download dal server Aspera demo funzionano, utilizzate [https://demo.asperasoft.com/aspera/user](https://demo.asperasoft.com/aspera/user).\
   (login: asperaweb, password: demoaspera)

4. Se non funzionano i passaggi di risoluzione dei problemi, deselezionate l'opzione Abilita accelerazione download e utilizzate il download normale.
