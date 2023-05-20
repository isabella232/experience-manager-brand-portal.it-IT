---
title: Domande frequenti
seo-title: null
description: Ottieni informazioni sulle domande frequenti in Adobe Experience Manager Assets Brand Portal.
seo-description: null
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: frequently-asked-questions
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
exl-id: 4a8f7fbd-7485-421d-a8db-755324d2dbef
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1509'
ht-degree: 0%

---

# Domande frequenti {#frequently-asked-questions}

Le domande frequenti su Brand Portal sono incentrate sulle query e sui problemi che gli utenti finali potrebbero incontrare durante l’utilizzo della versione più recente di Experience Manager Assets Brand Portal 6.4.6 o di versioni precedenti.


## Domande frequenti su Brand Portal 6.4.6  {#faqs-bp646}

**Ques. Endpoint OAuth legacy esistente (`https://legacy-oauth.cloud.adobe.io/login`) non funziona. Quale potrebbe essere la ragione?**

**Ans.** La configurazione legacy di OAuth è obsoleta. È necessario aggiornare le istanze Autore Experience Manager Assets al service pack più recente e configurarlo tramite la console Adobe Developer. Consulta [Configurare Experience Manager Assets con Brand Portal](configure-aem-assets-with-brand-portal.md) per i dettagli. Tuttavia, affinché la configurazione OAuth legacy funzioni fino all’aggiornamento, aggiorna l’endpoint OAuth legacy a `https://hypnosisprod.ethos11-prod-or1.ethos.adobe.net/`.

<!--
**Ques. I have created a collection using the asset link shared by the administrator. But I am unable to create a share link for my collection. Do I need special permissions to do this?**

**Ans.** The functionality is by design, the viewer users are not permitted to share link for collections as they have limited privileges due to which they cannot add users to create a share link. It is a known issue that the share link for collections is currently visible to the viewer users. This issue will be fixed in the upcoming release, the option to share link for the collections will not be available to the viewer users.    
-->

**Ques. Dopo l’aggiornamento alla console Adobe Developer, non riesco a pubblicare le risorse della cartella Contributi da Brand Portal a Experience Manager Assets. La mia istanza di authoring è su Experience Manager Assets 6.5.4. Quale potrebbe essere la ragione?**

**Ans.** Sì, si è verificato un problema noto durante la pubblicazione delle risorse della cartella dei contributi in Experience Manager Assets 6.5.4 tramite la console Adobe Developer.

Il problema è risolto in Experience Manager Assets 6.5.5. È possibile aggiornare l’istanza di Experience Manager Assets al service pack più recente e [aggiornare le configurazioni](https://experienceleague.adobe.com/docs/experience-manager-65/assets/brandportal/configure-aem-assets-with-brand-portal.html#upgrade-integration-65) sulla console Adobe Developer.

<!--
Broken link of download hotfix, comment out this section until we have the latest URL.

For immediate fix on AEM 6.5.4, it is recommended to [download the hotfix](https://www.adobeaemcloud.com/content/marketplace/marketplaceProxy.html?packagePath=/content/companies/public/adobe/packages/cq650/hotfix/cq-6.5.0-hotfix-33041) and install on your AEM author instance.
-->

**Ques. Non viene visualizzato il contenuto della cartella Contributi pubblicato da Brand Portal in Experience Manager Assets. Quale potrebbe essere la ragione?**

**Ans.** Contatta l’amministratore di Experience Manager Assets per verificare le configurazioni e assicurarti che il tuo tenant Brand Portal sia configurato con una sola istanza di authoring Experience Manager Assets.

Questo problema può verificarsi quando hai configurato un tenant Brand Portal su più istanze di authoring Experience Manager Assets. Ad esempio, l’amministratore configura lo stesso tenant Brand Portal nell’istanza di authoring Experience Manager Assets dell’ambiente di staging e produzione. In questo caso, i trigger di pubblicazione delle risorse in Brand Portal ma l’istanza di authoring di Experience Manager Assets non ha potuto importare il codice risorsa che l’agente di replica non riceve il token richiedente.


**Ques. Non è possibile pubblicare risorse da Experience Manager Assets a Brand Portal. Il registro di replica indica che la connessione è scaduta. C&#39;è una correzione rapida?**

**Ans.** In genere, la pubblicazione non riesce e genera un errore di timeout se nella coda di replica sono presenti più richieste in sospeso. Per risolvere questo problema, assicurati che gli agenti di replica siano configurati in modo da evitare il timeout.

Per configurare l’agente di replica, effettua le seguenti operazioni:

1. Accedi all’istanza Autore Experience Manager Assets.
1. Dalla sezione **Strumenti** , passa a **[!UICONTROL Distribuzione]** > **[!UICONTROL Replica]**.
1. Nella pagina Replica, fai clic su **[!UICONTROL Agenti per creazione]**. Puoi visualizzare i quattro agenti di replica per il tenant Brand Portal.
1. Fai clic sull’URL dell’agente di replica per aprire i dettagli dell’agente.
1. Clic **[!UICONTROL Modifica]** per modificare le impostazioni dell&#39;agente di replica.
1. In Impostazioni agente, fare clic su **[!UICONTROL Esteso]** scheda.
1. Seleziona la **[!UICONTROL Chiudi connessione]** casella di controllo.
1. Ripeti i passaggi da 4 a 7 per configurare tutti e quattro gli agenti di replica.
1. Riavvia il server e verifica la connessione.


## Domande frequenti su Brand Portal 6.4.5  {#faqs-bp645}

**Ques. Qual è la modifica principale nella versione 6.4.5 di Brand Portal?**

**Ans.** Experience Manager Assets Brand Portal 6.4.5 è una versione con nuove funzioni che consente agli utenti di Brand Portal di caricare contenuti dall’istanza di Brand Portal e pubblicare nuovamente la cartella Contributi in Experience Manager Assets senza bisogno di diritti di amministratore.
Per ulteriori informazioni, consulta [Asset Sourcing in Brand Portal](brand-portal-asset-sourcing.md).



**Ques. Perderò l’accesso alle risorse, alle funzioni o alle configurazioni esistenti create?**

**Ans.** Tutte le funzioni e le configurazioni esistenti rimangono intatte. Gli utenti finali non sono interessati e il contenuto rimane intatto.



**Ques. Quando si passa alla nuova versione di Brand Portal?**

**Ans.** Brand Portal 6.4.5 è stato rilasciato in produzione a ottobre 2019. La prossima versione di Brand Portal dovrebbe essere rilasciata nel terzo trimestre del 2020.
Per gli aggiornamenti e la modifica della versione, si consiglia di tenere traccia di [Note sulla versione](brand-portal-release-notes.md) e [Novità di Brand Portal](whats-new.md).



**Ques. Saranno interessati i miei utenti?**

**Ans.** La versione di Brand Portal 6.4.5 è disponibile esclusivamente in Brand Portal, quindi non ha alcun impatto sugli utenti finali.



**Ques. È necessaria un&#39;azione da parte mia in qualità di utente di Brand Portal?**

**Ans.** Brand Portal versione 6.4.5 viene fornito con una nuova funzione denominata Asset Sourcing. L’amministratore deve configurare la funzione Asset Sourcing in Experience Manager Assets per abilitare tale funzione per gli utenti di Brand Portal. Per ulteriori informazioni, consulta [Abilita Asset Sourcing](brand-portal-asset-sourcing.md).



**Ques. Chi può creare una cartella Contributi?**

**Ans.** Qualsiasi utente di Experience Manager Assets autorizzato a creare una nuova cartella in Experience Manager Assets può creare un **Contributo** cartella. Per creare un **Contributo** cartella, crea una nuova cartella di tipo **Contributo risorse**.
Questa cartella è condivisa con gli utenti Brand Portal attivi per il contributo.



**Ques. Cosa contiene una cartella Contributi?**

**Ans.** **Contributo** la cartella contiene due sottocartelle **NUOVO** e **CONDIVISO**. Inizialmente, la cartella NEW è vuota e la cartella SHARED contiene il contenuto di riferimento (risorse riutilizzabili) per gli utenti di Brand Portal.
Gli utenti di Brand Portal accedono a **Contributo** cartella e caricare il contenuto in **NUOVO** cartella.



**Ques.  Posso modificare il nome di una cartella Contributi esistente?**

**Ans.** **No**, non è possibile modificare il nome di un **Contributo** cartella.



**Ques. Cos&#39;è il contributo w.r.t per i requisiti degli asset?**

**Ans.** Il **Descrizione** documento allegato al **Contributo** e il contenuto di riferimento (risorse riutilizzabili) caricati nella **CONDIVISO** La cartella aiuta l’utente di Brand Portal a comprendere le esigenze di contributo e aspettative in qualità di collaboratore ed è collettivamente chiamata come requisito della risorsa.



**Ques. Posso caricare risorse in una cartella consentita?**

**Ans.** Non tutte le cartelle consentite. Un utente di Brand Portal può caricare contenuti solo in **Contributo** cartella condivisa dall&#39;amministratore di Experience Manager Assets o Brand Portal.



**Ques. Come posso accedere a una cartella Contributi?**

**Ans.** È possibile accedere a un **Contributo** solo se è stata condivisa con te. Riceverai una notifica e-mail/impulso ogni volta che una cartella Contributi viene condivisa con te. Puoi accedere alla cartella Contributi tramite il collegamento condiviso nell’e-mail oppure alla tua istanza di Brand Portal e passare all’icona a forma di campanello per la notifica di accesso alla cartella Contributi.

>[!NOTE]
>
>Se non sei un utente Brand Portal esistente, richiedi all’amministratore di Experience Manager Assets di creare l’utente in Admin Console e di aggiungere il tuo profilo al file di configurazione utente nell’elenco Utenti di Brand Portal.

**Ques. Qual è il formato del file CSV da importare?**

**Ans.** Il formato è uguale a quello supportato da Admin Console per l’importazione in blocco da parte dell’utente. E-mail, nome e cognome sono obbligatori.



**Ques. Cosa popola l’elenco di utenti (collaboratori Brand Portal) nel menu a discesa degli utenti di Asset Contribution?**

**Ans.** Gli utenti nel menu a discesa sono compilati dal file di configurazione utente di Brand Portal (con estensione csv) caricato in Experience Manager Assets.



**Ques. Dove posso visualizzare lo stato dei processi di importazione e pubblicazione?**

**Ans.** In Experience Manager Assets, puoi visualizzare lo stato di un’importazione in **asincrono** pagina del processo. In Brand Portal, puoi visualizzare lo stato di un processo di pubblicazione in **[!UICONTROL Strumenti > Stato contributo risorsa]**.



**Ques. Qual è la frequenza di un processo di importazione eseguito periodicamente in Experience Manager?**

**Ans.** In Experience Manager Assets, il polling viene eseguito ogni 5 minuti.



**Ques. Esiste un limite al numero di volte in cui una cartella può essere pubblicata da Brand Portal a Experience Manager Assets?**

**Ans.** No, tutte le risorse in **NUOVO** vengono pubblicati in Experience Manager Assets indipendentemente dal fatto che siano stati pubblicati in precedenza. Ogni volta che **Contributo** viene pubblicata da Brand Portal a Experience Manager Assets, sostituisce il contenuto della cartella **NUOVO** cartella.



**Ques. Come si caricano le nuove risorse in una cartella Contributi?**

**Ans.** Consulta la documentazione dettagliata per [Caricamento delle risorse nella cartella Contributi](brand-portal-publish-contribution-folder-to-brand-portal.md).



**Ques. Non visualizzo miniature/anteprime sulle risorse caricate nella NUOVA cartella da un utente di Brand Portal?**

**Ans.** È progettato per evitare l’esecuzione di flussi di lavoro all’estremità Brand Portal.



**Ques. Cosa succede se una cartella è pubblicata da Experience Manager Assets a Brand Portal in continua evoluzione?**

**Ans.** In Experience Manager Assets, i registri vengono mantenuti per ogni volta che una cartella viene pubblicata in Brand Portal. Al momento della pubblicazione, tutte le risorse non pubblicate in Brand Portal vengono inserite in una coda di replica. Tutte le risorse aggiunte alla cartella dopo l’attivazione del processo di pubblicazione non vengono pubblicate in Brand Portal. Quando l’utente di Experience Manager Assets pubblica nuovamente la cartella, in Brand Portal vengono pubblicate solo le risorse non pubblicate in precedenza (esistenti nella coda di replica).
Ciò vale per tutte le cartelle pubblicate da Experience Manager Assets a Brand Portal e per le cartelle CONDIVISE all’interno di una cartella Contributi.

**Ques. Chi devo contattare per le domande?**

**Ans.** Contatta il tuo Adobe Account Manager o l’Assistenza clienti.

>[!NOTE]
>
>La pianificazione del rilascio è provvisoria e soggetta a modifiche. Per ottenere la pianificazione aggiornata del rilascio, contatta il tuo Adobe Account Manager o l’Assistenza clienti.


## Accesso e supporto ai prodotti (siti con restrizioni) {#product-access-and-support-restricted-sites}

Questi siti sono disponibili solo per i clienti. Se sei un cliente e vuoi accedervi, contatta il tuo account manager Adobe.

<!--
* [](https://daycare.day.com) [Product Access](https://login.marketing.adobe.com)

* [Adobe Customer Support]()
-->
