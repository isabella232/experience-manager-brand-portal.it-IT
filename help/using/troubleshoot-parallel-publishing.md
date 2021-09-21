---
title: Risolvere i problemi relativi alla pubblicazione parallela in Brand Portal
seo-title: Troubleshoot issues in parallel publishing to Brand Portal
description: Risolvere i problemi relativi alla pubblicazione parallela.
seo-description: Troubleshoot parallel publishing.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
role: Admin
exl-id: 631beabc-b145-49ba-a8e4-f301497be6da
source-git-commit: fa346d075c6f8c5bd7aeed2318932b1747c388c2
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 1%

---

# Risolvere i problemi relativi alla pubblicazione parallela in Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal è configurato con AEM Assets per disporre di risorse di marchio approvate direttamente assimilate (o pubblicate) dall’istanza di authoring di AEM Assets. Una volta [configurato](../using/configure-aem-assets-with-brand-portal.md), AEM Author utilizza un agente di replica per replicare le risorse selezionate al servizio cloud Brand Portal per l’utilizzo approvato dagli utenti Brand Portal. Gli agenti di replica multipli vengono utilizzati AEM 6.2 SP1-CFP5, AEM CFP 6.3.0.2 e successivi per consentire la pubblicazione parallela ad alta velocità.

>[!NOTE]
>
>Adobe consiglia di effettuare l’aggiornamento a AEM 6.4.1.0 per garantire che AEM Assets Brand Portal sia configurato correttamente con AEM Assets. Una limitazione in AEM 6.4 genera un errore durante la configurazione di AEM Assets con Brand Portal e la replica non riesce.

Durante la configurazione del servizio cloud per il brand portal in **[!UICONTROL /etc/cloudservice]**, tutti gli utenti e i token necessari vengono generati automaticamente e salvati nell&#39;archivio. Viene creata la configurazione del servizio cloud, vengono creati anche gli utenti del servizio necessari per gli agenti di replica e replica per replicare il contenuto. Questo crea quattro agenti di replica. Quindi quando pubblichi numerose risorse da AEM a Brand Portal, queste vengono messe in coda e distribuite tra questi agenti di replica tramite Round Robin.

Tuttavia, la pubblicazione può non riuscire a intermittenza a causa di lavori sling di grandi dimensioni, dell’aumento di Network e di **[!UICONTROL Disk I/O]** sull’istanza di AEM Author o delle prestazioni rallentate dell’istanza di AEM Author. È quindi consigliabile verificare la connessione con gli agenti di replica prima di iniziare la pubblicazione.

![](assets/test-connection.png)

## Risolvere i problemi relativi alla prima pubblicazione: convalida della configurazione di pubblicazione {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Per convalidare le configurazioni di pubblicazione:

1. Controlla i registri degli errori
1. Verifica se l’agente di replica è stato creato
1. Prova connessione

**Log di coda durante la creazione di un Cloud Service**

Controlla i log tail. Controlla se l&#39;agente di replica viene creato o meno. Se la creazione dell’agente di replica non riesce, modifica il servizio cloud effettuando modifiche minori nel servizio cloud. Convalida e controlla nuovamente se l&#39;agente di replica è stato creato o meno. In caso contrario, modifica nuovamente il servizio.

Se si modifica ripetutamente il servizio cloud non è configurato correttamente, segnalare un ticket di assistenza clienti.

**Verifica della connessione con gli agenti di replica**

Visualizza registro, se si verificano errori nel registro di replica:

1. Contatta il supporto Adobe.

1. Riprova [pulizia](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) e crea di nuovo la configurazione di pubblicazione.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Pulizia delle configurazioni di pubblicazione Brand Portal esistenti {#clean-up-existing-config}

Nella maggior parte dei casi in cui la pubblicazione non funziona, il motivo può essere che l’utente che la pubblica (ad esempio: `mac-<tenantid>-replication` non dispone dell&#39;ultima chiave privata, e quindi la pubblicazione non riesce con l&#39;errore &quot;401 non autorizzato&quot; e nessun altro errore viene segnalato nei registri degli agenti di replica. È possibile evitare la risoluzione dei problemi e creare una nuova configurazione. Affinché la nuova configurazione funzioni correttamente, elimina quanto segue dalla configurazione AEM autore:

1. Vai a `localhost:4502/crx/de/` (considerando che stai eseguendo un&#39;istanza dell&#39;autore su localhost:4502:\
   i. elimina `/etc/replication/agents.author/mp_replication`
ii) delete 
`/etc/cloudservices/mediaportal/<config_name>`

1. Vai a localhost:4502/useradmin:\
   i. cerca l&#39;utente `mac-<tenantid>replication`
ii) elimina questo utente

Ora il sistema è completamente pulito. Ora puoi provare a creare una nuova configurazione cloudservice e continuare a utilizzare l&#39;applicazione JWT già esistente in `https://legacy-oauth.cloud.adobe.io/`. Non è necessario creare una nuova applicazione, ma solo la chiave pubblica deve essere aggiornata dalla configurazione cloud appena creata.

## Problema di visibilità tenant dell’applicazione JWT per la connessione sviluppatore {#developer-connection-jwt-application-tenant-visibility-issue}

Se è su `https://legacy-oauth.cloud.adobe.io/`, vengono elencate tutte le organizzazioni (tenant) per le quali gli utenti correnti detengono l’amministratore di sistema. Se non trovi il nome dell’organizzazione qui o non riesci a creare un’applicazione per un tenant obbligatorio qui, verifica di disporre di diritti (amministratore di sistema) sufficienti per eseguire questa operazione.

C&#39;è un problema noto in questa interfaccia utente che per ogni tenant sono visibili solo le prime 10 applicazioni. Quando crei l&#39;applicazione, resta su quella pagina e segnalibro l&#39;URL. Non è necessario passare alla pagina di elenco dell&#39;applicazione e trovare l&#39;applicazione creata. Puoi accedere direttamente a questo URL contrassegnato con segnalibro e aggiornare/eliminare l’applicazione ogni volta che necessario.

L&#39;applicazione JWT potrebbe non essere elencata in modo appropriato. Si consiglia quindi di notare/contrassegnare l’URL durante la creazione dell’applicazione JWT.

## L&#39;esecuzione della configurazione smette di funzionare {#running-configuration-stops-working}

<!--
Comment Type: draft

<p>If the running configuration stops working, either of the following two possibilities
<g class="gr_ gr_15 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar multiReplace" data-gr-id="15" id="15" style="font-size: 12px;">
are
</g> there:</p>
<p>1.
<g class="gr_ gr_14 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="14" id="14">
Connection
</g> has failed, or</p>
<p>2. Publish has failed with permission to dam-replication-service denied, while connection has passed </p>
<p>If the connection has failed [1], the
<g class="gr_ gr_10 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling ins-del multiReplace" data-gr-id="10" id="10">
fail safe
</g> way to fix it is to <a href="../using/troubleshoot-parallel-publishing.md#main-pars-header-1664955658">clean up</a> the existing Brand Portal publish configuration and recreate a publish configuration. </p>
<p>However, if the
<g class="gr_ gr_18 gr-alert gr_spell gr_inline_cards gr_run_anim ContextualSpelling" data-gr-id="18" id="18">
publish
</g> has failed with
<g class="gr_ gr_16 gr-alert gr_gramm gr_inline_cards gr_run_anim Grammar only-ins doubleReplace replaceWithoutSep" data-gr-id="16" id="16">
permission
</g> denied to dam-replication-service, raise a support ticket.</p>
-->

Se un agente di replica (che pubblicava su Brand Portal solo bene) smette di elaborare i processi di pubblicazione, controlla i registri di replica. AEM è stato incorporato un nuovo tentativo automatico, quindi se la pubblicazione di una particolare risorsa non riesce, viene ritentata automaticamente. Se si verifica un problema intermittente come l&#39;errore di rete, potrebbe verificarsi durante un nuovo tentativo.

Se si verificano continui errori di pubblicazione e la coda è bloccata, controlla **[!UICONTROL prova connessione]** e prova a risolvere gli errori che vengono segnalati.

In base agli errori, ti consigliamo di registrare un ticket di assistenza, in modo che il team di progettazione Brand Portal possa aiutarti a risolvere i problemi.


## Configura gli agenti di replica per evitare l’errore di timeout della connessione {#connection-timeout}

Di solito il processo di pubblicazione non riesce con un errore di timeout se ci sono più richieste in sospeso nella coda di replica. Per risolvere questo problema, assicurati che gli agenti di replica siano configurati per evitare timeout.

Esegui i seguenti passaggi per configurare gli agenti di replica:

1. Accedi alla tua istanza di authoring di AEM Assets.
1. Dal pannello **Strumenti**, passa a **[!UICONTROL Implementazione]** > **[!UICONTROL Replica]**.
1. Nella pagina Replica, fai clic su **[!UICONTROL Agenti sull&#39;autore]**. Puoi visualizzare i quattro agenti di replica del tenant Brand Portal.
1. Fai clic sull&#39;URL dell&#39;agente di replica per aprire i dettagli dell&#39;agente.
1. Fare clic su **[!UICONTROL Modifica]** per modificare le impostazioni dell&#39;agente di replica.
1. In Impostazioni agente , fai clic sulla scheda **[!UICONTROL Extended]** .
1. Selezionare la casella di controllo **[!UICONTROL Chiudi connessione]**.
1. Ripetere i passaggi da 4 a 7 per configurare tutti e quattro gli agenti di replica.
1. Riavvia il server.
