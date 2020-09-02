---
title: Domande frequenti
seo-title: null
description: Ottieni informazioni approfondite sulle domande frequenti nel portale dei marchi di Adobe Experience Manager Assets.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: a32eed22ebfbc683fca96950fc2e08bf5cfaccb3
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---


# Domande frequenti {#frequently-asked-questions}

Le domande frequenti sul Portale di marchi riguardano principalmente le domande e i problemi che gli utenti finali potrebbero incontrare durante l&#39;utilizzo della versione più recente  di AEM Assets Brand Portal 6.4.6 o versioni precedenti.


## Domande frequenti su Brand Portal 6.4.6  {#faqs-bp646}

**Ques. L&#39;endpoint OAuth esistente (`https://legacy-oauth.cloud.adobe.io/login`) non funziona. Quale potrebbe essere la ragione possibile?**

**Ans.** La configurazione OAuth precedente è obsoleta. È necessario aggiornare  istanze di creazione AEM Assets al service pack più recente e configurarlo tramite  Adobe Developer Console. Per informazioni, consultate [Configurare  AEM Assets con Brand Portal](configure-aem-assets-with-brand-portal.md) . Tuttavia, affinché la configurazione OAuth legacy funzioni fino all&#39;aggiornamento, aggiornate l&#39;endpoint OAuth legacy a `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. Non è possibile pubblicare le risorse della cartella dei contributi da Brand Portal a  AEM Assets dopo l’aggiornamento  Adobe Developer Console. L’istanza dell’autore è AEM 6.5.4. Quale potrebbe essere la ragione possibile?**

**Ans.** Sì, si verifica un problema noto durante la pubblicazione delle risorse della cartella dei contributi in  AEM Assets su AEM 6.5.4 tramite  Developer Console.

Il problema è stato risolto nella AEM 6.5.5. È possibile aggiornare l&#39;istanza di  AEM Assets al service pack più recente AEM 6.5.5 e [aggiornare le configurazioni](https://docs.adobe.com/content/help/en/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) su  Developer Console.

Per la correzione immediata del AEM 6.5.4, si consiglia di [scaricare l’hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) e installarlo nell’istanza di AEM autore.

**Ques. Non vedo il contenuto della cartella dei contributi pubblicato da Brand Portal in  AEM Assets. Quale potrebbe essere la ragione possibile?**

**Ans.** Contattate il vostro amministratore  AEM Assets per verificare le configurazioni e verificare che il tenant del Portale marchio sia configurato con una sola istanza  autore AEM Assets.

Questo problema potrebbe verificarsi se avete configurato un tenant di Brand Portal su più istanze di creazione di AEM Assets . Ad esempio, l&#39;amministratore configura lo stesso tenant del Portale marchio nell&#39;istanza di authoring  AEM Assets dell&#39;ambiente di produzione e di staging. In questo caso, la pubblicazione delle risorse viene attivata in Brand Portal, ma l’istanza di creazione di AEM Assets  non è stata in grado di importare la risorsa perché l’agente di replica non riceve il token richiesto.


**Ques. Non è possibile pubblicare risorse da  AEM Assets a Brand Portal. Il registro di replica indica che la connessione è scaduta per timeout. C&#39;è una correzione rapida?**

**Ans.** In genere la pubblicazione non riesce con un errore di timeout se nella coda di replica sono presenti più richieste in sospeso. Per risolvere il problema, assicurarsi che gli agenti di replica siano configurati in modo da evitare il timeout.

Effettuate le seguenti operazioni per configurare l&#39;agente di replica:
1. Accedete all’istanza di creazione  AEM Assets.
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

**Ans.**  AEM Assets Brand Portal 6.4.5 è una release che consente agli utenti di Brand Portal di caricare contenuti dall’istanza Brand Portal e pubblicare nuovamente la cartella Contribution su  AEM Assets senza richiedere diritti di amministratore.
Per ulteriori informazioni, consultate [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).



**Ques. Perderò l’accesso a risorse, funzionalità o configurazioni già esistenti?**

**Ans.** Tutte le funzioni e le configurazioni esistenti rimangono intatte. Gli utenti finali non sono interessati e il contenuto rimane intatto.



**Ques. Quando si passa alla nuova versione di Brand Portal?**

**Ans.** Brand Portal 6.4.5 è stato rilasciato in produzione a ottobre 2019. La prossima versione di Brand Portal verrà rilasciata nel 3° trimestre 2020.
Per aggiornamenti e modifiche di versione, si consiglia di tenere traccia delle note [di](brand-portal-release-notes.md) rilascio e delle [novità di Brand Portal](whats-new.md).



**Ques. I miei utenti saranno interessati?**

**Ans.** La versione di Brand Portal 6.4.5 è disponibile esclusivamente all’interno di Brand Portal, pertanto non ha alcun impatto sugli utenti finali.



**Ques. In qualità di utente del Brand Portal, è necessaria un&#39;azione?**

**Ans.** La versione di Brand Portal 6.4.5 include una nuova funzione denominata Asset Sourcing. AEM amministratore deve configurare la funzione di origine delle risorse in  AEM Assets per abilitare la funzione per gli utenti di Brand Portal. Per ulteriori informazioni, consultate [Abilita origine](brand-portal-configure-asset-sourcing.md)risorse.



**Ques. Chi può creare una cartella Contribution?**

**Ans.** Ogni utente AEM che dispone delle autorizzazioni per creare una nuova cartella in  AEM Assets può creare una cartella **Contribution** . Per creare una cartella **Contribution** , create una nuova cartella di tipo **Asset Contribution**.
Questa cartella viene condivisa con gli utenti attivi di Brand Portal per ottenere un contributo.



**Ques. Cosa contiene una cartella Contribution?**

**Ans.** **La cartella Contribution** contiene due sottocartelle **NEW** e **SHARED**. Inizialmente, la cartella NEW è vuota e la cartella SHARED contiene il contenuto di riferimento (risorse riutilizzabili) per gli utenti di Brand Portal.
Gli utenti di Brand Portal accedono alla cartella **Contribution** e caricano il contenuto nella cartella **NEW** .



**Ques.  È possibile modificare il nome di una cartella di contributi esistente?**

**Ans.** **No**, non è possibile modificare il nome di una cartella **Contributo** esistente.



**Ques. Che cos&#39;è il requisito patrimoniale con il contributo?**

**Ans.** Il documento **Breve** allegato alla cartella **Contribution** e al contenuto di riferimento (risorse riutilizzabili) caricato nella cartella **SHARED** aiuta l’utente del Brand Portal a comprendere la necessità di contributi e aspettative come collaboratore ed è collettivamente chiamato come requisiti delle risorse.



**Ques. Posso caricare le risorse in una qualsiasi cartella consentita?**

**Ans.** Non tutte le cartelle consentite. Un utente di Brand Portal può caricare il contenuto solo nella cartella **Contribution** condivisa dall’amministratore di AEM o Brand Portal.



**Ques. Come posso accedere a una cartella Contribution?**

**Ans.** Puoi accedere a una cartella **Contribution** solo se è stata condivisa con te. Riceverai una notifica e-mail/impulso ogni volta che una cartella Contribution viene condivisa con te. Potete accedere alla cartella Contribution tramite il collegamento condiviso nell’e-mail oppure accedere all’istanza Brand Portal e passare all’icona Bell per la notifica e accedere alla cartella Contribution.

>[!NOTE]
>
>Se non siete già utenti di Brand Portal, chiedete all’amministratore AEM di creare l’utente nella console di amministrazione AEM e aggiungere il vostro profilo al file di configurazione dell’utente nell’elenco degli utenti di Brand Portal. Fate riferimento a [Aggiunta di utenti](brand-portal-configure-asset-sourcing.md)del portale dei marchi.

**Ques. Qual è il formato del file CSV per l’importazione da parte degli utenti?**

**Ans.** Il formato è lo stesso di quello supportato dal Admin Console  per l&#39;importazione in massa di utenti. E-mail, nome e cognome sono obbligatori.



**Ques. Cosa compila l’elenco di utenti (collaboratori di Brand Portal) nel menu a discesa degli utenti Contribution?**

**Ans.** Gli utenti nel menu a discesa vengono popolati dal file di configurazione utente (.csv) del Brand Portal caricato in AEM.



**Ques. Dove è possibile visualizzare lo stato dei processi di importazione e pubblicazione?**

**Ans.** In AEM potete visualizzare lo stato di un&#39;importazione nella pagina del processo **asincrono** . In Brand Portal, potete visualizzare lo stato di un processo di pubblicazione in **[!UICONTROL Strumenti > Stato]** contributo risorsa.



**Ques. Qual è la frequenza di un processo di importazione che viene eseguito periodicamente in AEM?**

**Ans.** In AEM, il sondaggio viene eseguito ogni 5 minuti.



**Ques. Esiste una riduzione del numero di volte in cui è possibile pubblicare una cartella da Brand Portal a  AEM Assets?**

**Ans.** No, tutte le risorse presenti nella cartella **NEW** vengono pubblicate su  AEM Assets indipendentemente dal fatto che siano state pubblicate in precedenza. Ogni volta che una cartella **Contribution** viene pubblicata da Brand Portal a  AEM Assets, sostituisce il contenuto della cartella **NEW** .



**Ques. Come caricare nuove risorse in una cartella Contribution?**

**Ans.** Consultate la documentazione dettagliata per il [caricamento delle risorse nella cartella](brand-portal-upload-assets-to-contribution-folder.md)Contribution.



**Ques. Non vengono visualizzate miniature/anteprime delle risorse caricate nella cartella NEW da un utente di Brand Portal?**

**Ans.** È così come è stato progettato, poiché non è in esecuzione alcun flusso di lavoro alla fine del Portale marchio.



**Ques. Cosa succede se una cartella viene pubblicata da  AEM Assets al Portale del marchio che si trova in pieno flusso?**

**Ans.** In AEM, i file di registro vengono conservati ogni volta che una cartella viene pubblicata nel Brand Portal. Al momento della pubblicazione, tutte le risorse che non vengono pubblicate in Brand Portal vengono messe in coda di replica. Eventuali risorse aggiunte alla cartella dopo l’attivazione del processo di pubblicazione non vengono pubblicate in Brand Portal. Quando l&#39;utente AEM pubblica nuovamente la cartella, solo le risorse che non erano state pubblicate in precedenza (esistenti nella coda di replica) vengono pubblicate in Brand Portal.
Ciò vale per qualsiasi cartella pubblicata da  AEM Assets al Portale del marchio e cartella CONDIVISA all’interno di una cartella Contribution.



**Ques. Chi ho a che fare con le domande?**

**Ans.** Contatta il tuo Account Manager  Adobe o l&#39;Assistenza clienti.


>[!NOTE]
>
>Il programma di rilascio è provvisorio e soggetto a modifiche. Contatta il tuo Account Manager  Adobe o l&#39;Assistenza clienti per ottenere la pianificazione aggiornata della versione.





## Product Access and Support (Restricted Sites) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se siete un cliente e richiedete l&#39;accesso, contattate il vostro responsabile commerciale  Adobe.

* [](https://daycare.day.com) [Accesso al prodotto](https://login.marketing.adobe.com)

* [Assistenza clienti  Adobe](https://helpx.adobe.com/contact.html)
