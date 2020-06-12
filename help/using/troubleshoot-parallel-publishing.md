---
title: Risolvere i problemi relativi alla pubblicazione parallela in Brand Portal
seo-title: Risolvere i problemi relativi alla pubblicazione parallela in Brand Portal
description: Risoluzione di problemi relativi alla pubblicazione parallela.
seo-description: Risoluzione di problemi relativi alla pubblicazione parallela.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
topic-tags: brand-portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
translation-type: tm+mt
source-git-commit: 2b5d2fabc666a1d98af29c859f22a6d02bce3784
workflow-type: tm+mt
source-wordcount: '914'
ht-degree: 2%

---


# Risolvere i problemi relativi alla pubblicazione parallela in Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal è configurato con Risorse AEM per disporre di risorse del marchio approvate da assimilare (o pubblicare) direttamente dall’istanza di creazione di AEM Assets. Una volta [configurata](../using/configure-aem-assets-with-brand-portal.md), AEM Author utilizza un agente di replica per replicare le risorse selezionate nel servizio cloud Brand Portal per l&#39;utilizzo approvato dagli utenti del Brand Portal. Più agenti di replica vengono utilizzati AEM 6.2 SP1-CFP5, AEM CFP 6.3.0.2 e versioni successive per consentire la pubblicazione parallela ad alta velocità.

>[!NOTE]
>
>Adobe consiglia di effettuare l’aggiornamento ad AEM 6.4.1.0 per garantire che AEM Assets Brand Portal sia configurato correttamente con Risorse AEM. Una limitazione in AEM 6.4 causa un errore durante la configurazione di Risorse AEM con Brand Portal e la replica non riesce.

Quando si configura il servizio cloud per il portale del marchio in **[!UICONTROL /etc/cloud service]**, tutti gli utenti e i token necessari vengono generati automaticamente e salvati nell&#39;archivio. Viene creata la configurazione del servizio cloud, vengono creati anche gli utenti del servizio necessari per gli agenti di replica e replica per replicare il contenuto. Vengono creati quattro agenti di replica. Quando pubblicate numerose risorse da AEM al Brand Portal, queste vengono messe in coda e distribuite tra questi agenti di replica tramite Round Robin.

Tuttavia, la pubblicazione può non riuscire in modo intermittente a causa di lavori di sling di grandi dimensioni, dell&#39;aumento dell&#39;I/O di rete e **[!UICONTROL disco]** nell&#39;istanza di AEM Author o di prestazioni rallentate dell&#39;istanza di AEM Author. Si consiglia pertanto di verificare la connessione con gli agenti di replica prima di iniziare la pubblicazione.

![](assets/test-connection.png)

## Risoluzione dei problemi relativi alla prima pubblicazione: convalida della configurazione di pubblicazione {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Per convalidare le configurazioni di pubblicazione:

1. Controllare i registri degli errori
1. Verificare se l&#39;agente di replica è stato creato
1. Test connessione

**Registri di coda durante la creazione del servizio cloud**

Controllare i registri di coda. Verificare se l&#39;agente di replica è stato creato o meno. Se la creazione dell&#39;agente di replica non riesce, modificate il servizio cloud apportando lievi modifiche al servizio cloud. Convalida e verifica nuovamente se l&#39;agente di replica è stato creato o meno. In caso contrario, modificate nuovamente il servizio.

Se durante la modifica ripetuta del servizio cloud non è configurato correttamente, segnalate un ticket di assistenza legale.

**Verificare la connessione con gli agenti di replica**

Visualizza registro, se si verificano errori nel registro di replica:

1. Contattate il supporto Adobe.

1. Tentate di [ripulire](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) e creare nuovamente la configurazione di pubblicazione.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Pulizia delle configurazioni di pubblicazione esistenti di Brand Portal {#clean-up-existing-config}

La maggior parte delle volte in cui la pubblicazione non funziona, il motivo può essere dovuto al fatto che l’utente che la pubblica (ad esempio: `mac-<tenantid>-replication` non dispone della chiave privata più recente e, di conseguenza, la pubblicazione non riesce con l&#39;errore &quot;401 non autorizzato&quot; e nessun altro errore viene segnalato nei registri dell&#39;agente di replica. Potreste voler evitare la risoluzione dei problemi e creare una nuova configurazione. Affinché la nuova configurazione funzioni correttamente, pulite le seguenti informazioni dalla configurazione dell’autore di AEM:

1. Vai a `localhost:4502/crx/de/` (se stai eseguendo l’istanza di autore in localhost:4502:\
   i. delete `/etc/replication/agents.author/mp_replication`ii. delete `/etc/cloudservices/mediaportal/<config_name>`
`/etc/cloudservices/mediaportal/<config_name>`Vai a localhost:4502/useradmin:

1. i. cercare l’utente `mac-<tenantid>replication`ii. elimina questo utente\
   Ora il sistema è completamente pulito. Ora potete provare a creare una nuova configurazione del servizio cloud e utilizzare comunque l&#39;applicazione JWT già esistente in [https://legacy-oauth.cloud.adobe.io/[#$tu31]. Non è necessario creare una nuova applicazione, ma solo la chiave pubblica deve essere aggiornata dalla configurazione cloud appena creata.



## Se si trova su [https://legacy-oauth.cloud.adobe.io/[#$tu34], vengono elencate tutte le organizzazioni (tenant) per le quali gli utenti correnti detengono l&#39;amministratore di sistema. Se non trovi il nome dell&#39;organizzazione qui o non riesci a creare un&#39;applicazione per un tenant richiesto qui, verifica di disporre di diritti (amministratore di sistema) sufficienti per farlo.



L&#39;applicazione JWT potrebbe non essere elencata correttamente. Si consiglia pertanto di notare/contrassegnare l’URL durante la creazione dell’applicazione JWT.

L&#39;esecuzione della configurazione interrompe il funzionamento {#running-configuration-stops-working}

## Se un agente di replica (che pubblicava correttamente nel portale del marchio) interrompe l&#39;elaborazione dei processi di pubblicazione, controllate i registri di replica. In AEM è stato incorporato un nuovo tentativo automatico, pertanto se la pubblicazione di una risorsa non riesce, viene ritentata automaticamente. Se si verifica un problema intermittente come l&#39;errore di rete, potrebbe verificarsi nuovamente durante il tentativo.{#running-configuration-stops-working}

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

Se si verificano continui errori di pubblicazione e la coda è bloccata, controllate la connessione **[!UICONTROL di]** prova e provate a risolvere gli errori segnalati.

In base agli errori, si consiglia di registrare un ticket di assistenza, in modo che il team di progettazione di Brand Portal possa aiutarti a risolvere i problemi.****

Configurare gli agenti di replica per evitare l&#39;errore di timeout della connessione {#connection-timeout}


## **Problema**: Non è possibile pubblicare risorse da AEM Assets al Brand Portal. Il registro di replica indica che la connessione è scaduta per timeout.

**Risoluzione**: In genere la pubblicazione non riesce con un errore di timeout se nella coda di replica sono presenti più richieste in sospeso. Per risolvere il problema, assicurarsi che gli agenti di replica siano configurati in modo da evitare il timeout.

**Effettuate le seguenti operazioni per configurare l&#39;agente di replica:**

Accedi all’istanza di creazione di Risorse AEM.
1. Dal pannello **Strumenti** , passare a **[!UICONTROL Distribuzione]** > **[!UICONTROL Replica]**.
1. Nella pagina Replica, fate clic su **[!UICONTROL Agenti sull’autore]**. Potete visualizzare i quattro agenti di replica per il tenant del Brand Portal.**]******
1. Fate clic sull&#39;URL dell&#39;agente di replica per aprire i dettagli dell&#39;agente.****
1. Fate clic su **[!UICONTROL Modifica]** per modificare le impostazioni dell&#39;agente di replica.
1. In Impostazioni agente, fai clic sulla scheda **[!UICONTROL Estese]** .
1. Selezionate la casella di controllo **[!UICONTROL Chiudi connessione]** .
1. Ripetere i passaggi da 4 a 7 per configurare tutti e quattro gli agenti di replica.****
1. Riavviate il server.
1. Restart the server.