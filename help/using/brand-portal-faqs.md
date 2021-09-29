---
title: 'Domande frequenti '
seo-title: null
description: Ottieni informazioni approfondite sulle domande frequenti in Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 67a745fed6a13cfdb30e26062eecc3c8d1775e36
workflow-type: tm+mt
source-wordcount: '1468'
ht-degree: 0%

---

# Domande frequenti  {#frequently-asked-questions}

Le domande frequenti su Brand Portal si concentrano sulle query e sui problemi che gli utenti finali potrebbero incontrare durante l&#39;utilizzo dell&#39;ultima versione di AEM Assets Brand Portal 6.4.6 o delle versioni precedenti.


## Domande frequenti su Brand Portal 6.4.6  {#faqs-bp646}

**Si fermi. L’endpoint OAuth esistente (`https://legacy-oauth.cloud.adobe.io/login`) non funziona. Quale potrebbe essere il motivo?**

**Ans.** La configurazione OAuth legacy è obsoleta. È necessario aggiornare le istanze di authoring di AEM Assets al service pack più recente e configurarlo tramite Adobe Developer Console. Per ulteriori informazioni, consulta [Configurare AEM Assets con Brand Portal](configure-aem-assets-with-brand-portal.md) . Tuttavia, affinché la configurazione OAuth legacy funzioni fino all’aggiornamento, aggiorna l’endpoint OAuth legacy a `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Si fermi. Dopo l’aggiornamento ad Adobe Developer Console, non è possibile pubblicare le risorse della cartella dei contributi da Brand Portal ad AEM Assets. L&#39;istanza del mio autore è in AEM 6.5.4. Quale potrebbe essere il motivo?**

**Ans.** Sì, si verifica un problema noto durante la pubblicazione delle risorse della cartella dei contributi in AEM Assets in AEM 6.5.4 tramite Adobe Developer Console.

Il problema è risolto in AEM 6.5.5. È possibile aggiornare l&#39;istanza AEM Assets all&#39;ultimo service pack AEM 6.5.5 e [aggiornare le configurazioni](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) in Adobe Developer Console.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Si fermi. Non visualizzo il contenuto della cartella dei contributi pubblicato da Brand Portal in AEM Assets. Quale potrebbe essere il motivo?**

**Ans.** Contatta il tuo amministratore AEM Assets per verificare le configurazioni e verificare che il tenant Brand Portal sia configurato con una sola istanza di authoring AEM Assets.

Questo problema può verificarsi quando hai configurato un tenant Brand Portal su più istanze di authoring di AEM Assets. Ad esempio, l’amministratore configura lo stesso tenant Brand Portal nell’istanza di authoring AEM Assets dell’ambiente di staging e produzione. In questo caso, la pubblicazione delle risorse viene attivata in Brand Portal ma l’istanza di authoring di AEM Assets non è riuscita a importare la risorsa, perché l’agente di replica non riceve il token richiedente.


**Si fermi. Non sono in grado di pubblicare risorse da AEM Assets a Brand Portal. Il registro di replica indica che la connessione è scaduta per timeout. Esiste una correzione rapida?**

**Ans.** Di solito la pubblicazione non riesce con un errore di timeout se ci sono più richieste in sospeso nella coda di replica. Per risolvere questo problema, assicurati che gli agenti di replica siano configurati per evitare timeout.

Esegui i seguenti passaggi per configurare l’agente di replica:

1. Accedi alla tua istanza di authoring di AEM Assets.
1. Dal pannello **Strumenti**, passa a **[!UICONTROL Implementazione]** > **[!UICONTROL Replica]**.
1. Nella pagina Replica, fai clic su **[!UICONTROL Agenti sull&#39;autore]**. Puoi visualizzare i quattro agenti di replica per il tenant Brand Portal.
1. Fai clic sull&#39;URL dell&#39;agente di replica per aprire i dettagli dell&#39;agente.
1. Fare clic su **[!UICONTROL Modifica]** per modificare le impostazioni dell&#39;agente di replica.
1. In Impostazioni agente, fai clic sulla scheda **[!UICONTROL Extended]** .
1. Selezionare la casella di controllo **[!UICONTROL Chiudi connessione]**.
1. Ripetere i passaggi da 4 a 7 per configurare tutti e quattro gli agenti di replica.
1. Riavvia il server e verifica la connessione.


## Domande frequenti su Brand Portal 6.4.5  {#faqs-bp645}

**Si fermi. Qual è la principale modifica nella versione Brand Portal 6.4.5?**

**Ans.** AEM Assets Brand Portal 6.4.5 è una versione con nuove funzioni che consente agli utenti di Brand Portal di caricare contenuti dall’istanza di Brand Portal e pubblicare nuovamente la cartella Contribution in AEM Assets senza disporre dei diritti di amministratore.
Per ulteriori informazioni, consulta [Origine risorse in Brand Portal](brand-portal-asset-sourcing.md).



**Si fermi. Perderò l&#39;accesso a risorse, funzionalità o configurazioni esistenti create?**

**Ans.** Tutte le funzioni e le configurazioni esistenti rimangono intatte. Gli utenti finali non sono interessati e il contenuto rimane intatto.



**Si fermi. Quando passerò alla nuova versione di Brand Portal?**

**Ans.** Brand Portal 6.4.5 è stato rilasciato in produzione a ottobre 2019. E la prossima versione di Brand Portal dovrebbe essere rilasciata nel terzo trimestre del 2020.
Per aggiornamenti e modifiche alla versione, si consiglia di tenere traccia delle [Note sulla versione](brand-portal-release-notes.md) e [Novità di Brand Portal](whats-new.md).



**Si fermi. I miei utenti saranno interessati?**

**Ans.** La versione 6.4.5 di Brand Portal è esclusivamente in Brand Portal, quindi non vi è alcun impatto per gli utenti finali.



**Si fermi. È necessaria un&#39;azione da parte mia come utente Brand Portal?**

**Ans.** La versione 6.4.5 di Brand Portal include una nuova funzione denominata Asset Sourcing. AEM amministratore deve configurare la funzione Origine risorse in AEM Assets per abilitare la funzione per gli utenti di Brand Portal. Per ulteriori informazioni, consulta [Abilita Asset Sourcing](brand-portal-asset-sourcing.md).



**Si fermi. Chi può creare una cartella Contribution?**

**Ans.** Qualsiasi utente AEM con autorizzazioni per creare una nuova cartella in AEM Assets può creare una cartella  **** Contributo. Per creare una cartella **Contributo**, crea una nuova cartella di tipo **Contributo risorsa**.
Questa cartella viene condivisa con gli utenti Brand Portal attivi per il contributo.



**Si fermi. Cosa contiene una cartella Contribution?**

**Ans.** **** La cartella Contributo contiene due sottocartelle  **** NEWe  **SHARED**. Inizialmente, la cartella NEW è vuota e la cartella SHARED contiene il contenuto di riferimento (risorse riutilizzabili) per gli utenti Brand Portal.
Gli utenti Brand Portal accedono alla cartella **Contribution** e caricano il contenuto nella cartella **NEW** .



**Si fermi.  Posso modificare il nome di una cartella Contribution esistente?**

**Ans.** **No**, non è possibile modificare il nome di una cartella di  **** contributo esistente.



**Si fermi. Qual è il fabbisogno di risorse con il contributo?**

**Ans.** Il  **** Documento di sintesi allegato alla cartella  **** Contributo e il contenuto di riferimento (risorse riutilizzabili) caricato nella cartella  **** SHARED aiuta l’utente Brand Portal a comprendere la necessità di contributi e aspettative come collaboratore e viene collettivamente chiamato come requisiti di risorse.



**Si fermi. Posso caricare le risorse in qualsiasi cartella consentita?**

**Ans.** Non tutte le cartelle consentite. Un utente Brand Portal può caricare il contenuto solo nella cartella **Contribution** condivisa dall’amministratore AEM o Brand Portal.



**Si fermi. Come posso accedere a una cartella Contribution?**

**Ans.** Puoi accedere a una cartella  **** Contributo solo se è stata condivisa con te. Riceverai una notifica e-mail/impulso ogni volta che una cartella Contribution viene condivisa con te. Puoi accedere alla cartella Contribution tramite il collegamento condiviso nell’e-mail oppure all’istanza Brand Portal e passare all’icona bell per la notifica e accedere alla cartella Contribution.

>[!NOTE]
>
>Se non sei un utente Brand Portal esistente, chiedi all’amministratore AEM di creare il tuo utente nella console di amministrazione AEM e di aggiungere il tuo profilo al file di configurazione dell’utente nell’elenco degli utenti di Brand Portal.

**Si fermi. Qual è il formato del file CSV per l&#39;importazione da parte dell&#39;utente?**

**Ans.** Il formato è lo stesso supportato da Admin Console per l’importazione in massa di utenti. E-mail, nome e cognome sono obbligatori.



**Si fermi. Cosa compila l’elenco di utenti (collaboratori di Brand Portal) nel menu a discesa dell’utente Contributo risorse?**

**Ans.** Gli utenti nel menu a discesa vengono compilati dal file di configurazione utente (.csv) di Brand Portal caricato in AEM.



**Si fermi. Dove posso visualizzare lo stato dei processi di importazione e pubblicazione?**

**Ans.** In AEM, puoi visualizzare lo stato di un’importazione nella pagina  **** asincrona. In Brand Portal, puoi visualizzare lo stato di un processo di pubblicazione in **[!UICONTROL Strumenti > Stato contributo risorsa]**.



**Si fermi. Qual è la frequenza di un processo di importazione che viene eseguito periodicamente in AEM?**

**Ans.** In AEM, le votazioni vengono eseguite ogni 5 minuti.



**Si fermi. Esiste una minaccia per il numero di volte in cui una cartella può essere pubblicata da Brand Portal ad AEM Assets?**

**Ans.** No, tutte le risorse presenti nella cartella  **** NEWfolder vengono pubblicate in AEM Assets indipendentemente dal fatto che siano state pubblicate in precedenza. Ogni volta che una cartella **Contribution** viene pubblicata da Brand Portal ad AEM Assets, sostituisce il contenuto della cartella **NEW**.



**Si fermi. Come caricare nuove risorse in una cartella Contribution?**

**Ans.** Consulta la documentazione dettagliata per il  [caricamento delle risorse nella cartella Contribution](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Si fermi. Non vedo miniature/anteprime sulle risorse caricate nella NUOVA cartella da un utente Brand Portal?**

**Ans.** È così come è stato progettato, perché non è in corso alcun flusso di lavoro all’estremità di Brand Portal.



**Si fermi. Cosa succede se una cartella viene pubblicata da AEM Assets a Brand Portal in flusso?**

**Ans.** In AEM, i registri vengono mantenuti ogni volta che una cartella viene pubblicata in Brand Portal. Al momento della pubblicazione, tutte le risorse che non vengono pubblicate in Brand Portal vengono messe in coda di replica. Le risorse aggiunte alla cartella dopo l’attivazione del processo di pubblicazione non vengono pubblicate in Brand Portal. Quando l’utente AEM pubblica nuovamente la cartella, solo le risorse che non sono state pubblicate in precedenza (esistenti nella coda di replica) vengono pubblicate in Brand Portal.
Ciò vale per qualsiasi cartella pubblicata da AEM Assets a Brand Portal e cartella CONDIVISA all’interno di una cartella Contribution.

**Si fermi. A chi posso rivolgermi per le domande?**

**Ans.** Contatta il tuo Adobe Account Manager o l&#39;Assistenza clienti.

>[!NOTE]
>
>La pianificazione del rilascio è provvisoria e soggetta a modifiche. Contatta il tuo Adobe Account Manager o l&#39;Assistenza clienti per ottenere la pianificazione aggiornata della versione.


## Accesso e supporto ai prodotti (siti con restrizioni) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se sei un cliente e hai bisogno di accedervi, contatta il tuo account manager Adobe.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Care](https://helpx.adobe.com/contact.html)
-->
