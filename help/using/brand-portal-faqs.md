---
title: Domande frequenti
seo-title: null
description: Ottenete informazioni approfondite sulle domande frequenti nel portale del marchio Risorse del Adobe Experience Manager .
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: f763917659b5c1b9b37662d963484f4e84caa109
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 0%

---


# Domande frequenti {#frequently-asked-questions}

Le domande frequenti sul Portale del marchio riguardano principalmente le domande e i problemi che gli utenti finali potrebbero incontrare durante l’utilizzo della versione più recente del Portale del marchio AEM Assets 6.4.6 o versioni precedenti.


## Domande frequenti su Brand Portal 6.4.6  {#faqs-bp646}

**Ques. L&#39;endpoint OAuth esistente (`https://legacy-oauth.cloud.adobe.io/login`) non funziona. Quale potrebbe essere la ragione possibile?**

**Ans.** La configurazione OAuth precedente è obsoleta. È necessario aggiornare le istanze degli AEM Assets autori al service pack più recente e configurarlo tramite Adobe Developer Console. Per informazioni dettagliate, consultate [Configurare i AEM Assets con Brand Portal](configure-aem-assets-with-brand-portal.md) . Tuttavia, affinché la configurazione OAuth legacy funzioni fino all&#39;aggiornamento, aggiornate l&#39;endpoint OAuth legacy a `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

**Ques. Dopo l’aggiornamento ad Adobe Developer Console, non è possibile pubblicare le risorse della cartella dei contributi da Brand Portal ai AEM Assets. L’istanza dell’autore si trova in AEM 6.5.4. Quale potrebbe essere la ragione possibile?**

**Ans.** Sì, si verifica un problema noto durante la pubblicazione delle risorse della cartella dei contributi ai AEM Assets in AEM 6.5.4 tramite Adobe Developer Console.

Il problema è stato risolto in AEM 6.5.5. Puoi aggiornare l’istanza AEM Assets al service pack AEM 6.5.5 più recente e [aggiornare le configurazioni](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) in Adobe Developer Console.

Per una correzione immediata su AEM 6.5.4, si consiglia di [scaricare l’hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e installarlo nell’istanza di creazione di AEM.

**Ques. Il contenuto della cartella dei contributi non viene visualizzato nel AEM Assets del portale dei marchi. Quale potrebbe essere la ragione possibile?**

**Ans.** Contattate l’amministratore di AEM Assets per verificare le configurazioni e verificare che il tenant del Brand Portal sia configurato con una sola istanza di autore AEM Assets.

Questo problema potrebbe verificarsi se hai configurato un tenant Brand Portal su più istanze di creazione di AEM Assets. Ad esempio, l&#39;amministratore configura lo stesso tenant Brand Portal nell&#39;istanza di creazione AEM Assets dell&#39;ambiente di staging e di produzione. In questo caso, l&#39;attivazione della pubblicazione delle risorse in Brand Portal ma l&#39;istanza di creazione degli AEM Assets non è riuscita a importare la risorsa, perché l&#39;agente di replica non riceve il token richiesto.


**Ques. Non è possibile pubblicare risorse da AEM Assets al Brand Portal. Il registro di replica indica che la connessione è scaduta per timeout. C&#39;è una correzione rapida?**

**Ans.** In genere la pubblicazione non riesce con un errore di timeout se nella coda di replica sono presenti più richieste in sospeso. Per risolvere il problema, assicurarsi che gli agenti di replica siano configurati in modo da evitare il timeout.

Effettuate le seguenti operazioni per configurare l&#39;agente di replica:
1. Accedete all’istanza di creazione AEM Assets.
1. Dal pannello **Strumenti** , passare a **[!UICONTROL Distribuzione]** > **[!UICONTROL Replica]**.
1. Nella pagina Replica, fate clic su **[!UICONTROL Agenti sull’autore]**. Potete visualizzare i quattro agenti di replica per il tenant del Brand Portal.
1. Fate clic sull&#39;URL dell&#39;agente di replica per aprire i dettagli dell&#39;agente.
1. Fate clic su **[!UICONTROL Modifica]** per modificare le impostazioni dell&#39;agente di replica.
1. In Impostazioni agente, fai clic sulla scheda **[!UICONTROL Estese]** .
1. Selezionate la casella di controllo **[!UICONTROL Chiudi connessione]** .
1. Ripetere i passaggi da 4 a 7 per configurare tutti e quattro gli agenti di replica.
1. Riavviate il server e verificate la connessione.


## Domande frequenti su Brand Portal 6.4.5  {#faqs-bp645}

**Ques. Qual è la modifica principale nella versione 6.4.5 di Brand Portal?**

**Ans.** AEM Assets Brand Portal 6.4.5 è una release che consente agli utenti del Brand Portal di caricare contenuti dall’istanza Brand Portal e di pubblicare nuovamente la cartella Contribution agli AEM Assets senza richiedere diritti di amministratore.
Per ulteriori informazioni, consultate [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).



**Ques. Perderò l’accesso a risorse, funzionalità o configurazioni già esistenti?**

**Ans.** Tutte le funzioni e le configurazioni esistenti rimangono intatte. Gli utenti finali non sono interessati e il contenuto rimane intatto.



**Ques. Quando si passa alla nuova versione di Brand Portal?**

**Ans.** Brand Portal 6.4.5 è stato rilasciato in produzione a ottobre 2019. La prossima versione di Brand Portal verrà rilasciata nel 3° trimestre 2020.
Per aggiornamenti e modifiche di versione, si consiglia di tenere traccia delle note [di](brand-portal-release-notes.md) rilascio e delle [novità di Brand Portal](whats-new.md).



**Ques. I miei utenti saranno interessati?**

**Ans.** La versione di Brand Portal 6.4.5 è disponibile esclusivamente all’interno di Brand Portal, pertanto non ha alcun impatto sugli utenti finali.



**Ques. In qualità di utente del Brand Portal, è necessaria un&#39;azione?**

**Ans.** La versione di Brand Portal 6.4.5 include una nuova funzione denominata Asset Sourcing. L’amministratore di AEM deve configurare la funzione di origine delle risorse in AEM Assets per abilitare la funzione per gli utenti del Brand Portal. Per ulteriori informazioni, consultate [Abilita origine](brand-portal-configure-asset-sourcing.md)risorse.



**Ques. Chi può creare una cartella Contribution?**

**Ans.** Qualsiasi utente AEM che disponga delle autorizzazioni necessarie per creare una nuova cartella in AEM Assets, può creare una cartella **Contribution** . Per creare una cartella **Contribution** , create una nuova cartella di tipo **Asset Contribution**.
Questa cartella viene condivisa con gli utenti attivi di Brand Portal per ottenere un contributo.



**Ques. Cosa contiene una cartella Contribution?**

**Ans.** **La cartella Contribution** contiene due sottocartelle **NEW** e **SHARED**. Inizialmente, la cartella NEW è vuota e la cartella SHARED contiene il contenuto di riferimento (risorse riutilizzabili) per gli utenti di Brand Portal.
Gli utenti di Brand Portal accedono alla cartella **Contribution** e caricano il contenuto nella cartella **NEW** .



**Ques.  È possibile modificare il nome di una cartella di contributi esistente?**

**Ans.** **No**, non è possibile modificare il nome di una cartella **Contributo** esistente.



**Ques. Che cos&#39;è il requisito patrimoniale con il contributo?**

**Ans.** Il documento **Breve** allegato alla cartella **Contribution** e al contenuto di riferimento (risorse riutilizzabili) caricato nella cartella **SHARED** aiuta l’utente del Brand Portal a comprendere la necessità di contributi e aspettative come collaboratore ed è collettivamente chiamato come requisiti delle risorse.



**Ques. Posso caricare le risorse in una qualsiasi cartella consentita?**

**Ans.** Non tutte le cartelle consentite. Un utente di Brand Portal può caricare contenuto solo nella cartella **Contribution** condivisa dall’amministratore AEM o Brand Portal.



**Ques. Come posso accedere a una cartella Contribution?**

**Ans.** Potete accedere a una cartella **Contribution** solo se è stata condivisa con voi. Riceverai una notifica e-mail/impulso ogni volta che una cartella Contribution viene condivisa con te. Potete accedere alla cartella Contribution tramite il collegamento condiviso nell’e-mail oppure accedere all’istanza Brand Portal e passare all’icona Bell per la notifica e accedere alla cartella Contribution.

>[!NOTE]
>
>Se non siete già utenti di Brand Portal, chiedete all’amministratore AEM di creare l’utente nella console di amministrazione di AEM e di aggiungere il vostro profilo al file di configurazione dell’utente nell’elenco degli utenti di Brand Portal. Fate riferimento a [Aggiunta di utenti](brand-portal-configure-asset-sourcing.md)del portale dei marchi.




**Ques. Qual è il formato del file CSV per l’importazione da parte degli utenti?**

**Ans.** Il formato è lo stesso di quello supportato da  Admin Console per l&#39;importazione in massa di utenti. E-mail, nome e cognome sono obbligatori.



**Ques. Cosa compila l’elenco di utenti (collaboratori di Brand Portal) nel menu a discesa degli utenti Contribution?**

**Ans.** Gli utenti nel menu a discesa vengono popolati dal file di configurazione utente (.csv) del Portale marchio caricato in AEM.



**Ques. Dove è possibile visualizzare lo stato dei processi di importazione e pubblicazione?**

**Ans.** In AEM, potete visualizzare lo stato di un’importazione nella pagina del processo **asincrono** . In Brand Portal, potete visualizzare lo stato di un processo di pubblicazione in **[!UICONTROL Strumenti > Stato]** contributo risorsa.



**Ques. Qual è la frequenza di un processo di importazione che viene eseguito periodicamente in AEM?**

**Ans.** In AEM, il sondaggio viene eseguito ogni 5 minuti.



**Ques. Esiste una riduzione del numero di volte in cui è possibile pubblicare una cartella da Brand Portal ai AEM Assets?**

**Ans.** No, tutte le risorse presenti nella cartella **NEW** vengono pubblicate sui AEM Assets, indipendentemente dal fatto che siano state pubblicate in precedenza. Ogni volta che una cartella **Contribution** viene pubblicata da Brand Portal ai AEM Assets, questa viene ignorata e viene sostituita dal contenuto della cartella **NEW** .



**Ques. Come caricare nuove risorse in una cartella Contribution?**

**Ans.** Consultate la documentazione dettagliata per il [caricamento delle risorse nella cartella](brand-portal-upload-assets-to-contribution-folder.md)Contribution.



**Ques. Non vengono visualizzate miniature/anteprime delle risorse caricate nella cartella NEW da un utente di Brand Portal?**

**Ans.** È così come è stato progettato, poiché non è in esecuzione alcun flusso di lavoro alla fine del Brand Portal.



**Ques. Cosa succede se una cartella viene pubblicata dai AEM Assets al Portale del marchio che si trova in pieno flusso?**

**Ans.** In AEM, i file di registro vengono conservati ogni volta che una cartella viene pubblicata nel Brand Portal. Al momento della pubblicazione, tutte le risorse che non vengono pubblicate in Brand Portal vengono messe in coda di replica. Eventuali risorse aggiunte alla cartella dopo l’attivazione del processo di pubblicazione non vengono pubblicate in Brand Portal. Quando l’utente AEM pubblica nuovamente la cartella, solo le risorse che non erano state pubblicate in precedenza (esistenti nella coda di replica) vengono pubblicate nel Brand Portal.
Ciò vale per qualsiasi cartella pubblicata da AEM Assets al Portale del marchio e cartella CONDIVISA all’interno di una cartella Contribution.



**Ques. Chi ho a che fare con le domande?**

**Ans.** Contatta il tuo Adobe Account Manager o l&#39;Assistenza clienti.


>[!NOTE]
>
>Il programma di rilascio è provvisorio e soggetto a modifiche. Contatta il tuo Adobe Account Manager o l&#39;Assistenza clienti per ottenere la pianificazione della versione aggiornata.




## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se siete un cliente e richiedete l&#39;accesso, contattate il vostro account manager Adobe.

* [](https://daycare.day.com) [Accesso al prodotto](https://login.marketing.adobe.com)

* [Assistenza clienti Adobe](https://helpx.adobe.com/contact.html)
