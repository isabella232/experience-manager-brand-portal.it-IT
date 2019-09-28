---
title: Risoluzione dei problemi relativi alla pubblicazione parallela a Brand Portal
seo-title: Risoluzione dei problemi relativi alla pubblicazione parallela a Brand Portal
description: Risoluzione di problemi relativi alla pubblicazione parallela.
seo-description: Risoluzione di problemi relativi alla pubblicazione parallela.
uuid: 51e45cca-8c96-4c69-84ef-2ef34f3bcde2
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: riferimento
topic-tags: brand-Portal
discoiquuid: a4801024-b509-4c51-afd8-e337417e658b
translation-type: tm+mt
source-git-commit: 86d4d5c358ea795e35db2dce8c9529ed14e9ee2d

---


# Risoluzione dei problemi relativi alla pubblicazione parallela a Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Brand Portal supporta l’integrazione con AEM Assets per disporre di risorse di marchio approvate da assimilare (o pubblicare) direttamente dall’istanza di creazione di AEM Assets. Una volta [integrata](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html), AEM Author utilizza un agente di replica per replicare le risorse selezionate nel servizio cloud Brand Portal per l'utilizzo approvato dagli utenti del Brand Portal. Più agenti di replica vengono utilizzati AEM 6.2 SP1-CFP5], AEM CFP 6.3.0.2 e versioni successive per consentire la pubblicazione parallela ad alta velocità.

>[!NOTE]
>
>Adobe consiglia di effettuare l’aggiornamento ad AEM 6.4.1.0 per garantire che AEM Assets Brand Portal sia integrato con AEM Assets. Una limitazione in AEM 6.4 genera un errore durante la configurazione dell'integrazione con Brand Portal e la replica non riesce.

Quando si configura il servizio cloud per il portale del marchio in [!UICONTROL /etc/cloud service], tutti gli utenti e i token necessari vengono generati automaticamente e salvati nell'archivio. Viene creata la configurazione del servizio cloud, vengono creati anche gli utenti del servizio necessari per gli agenti di replica e replica per replicare il contenuto. Vengono creati quattro agenti di replica. Quando pubblicate numerose risorse da AEM al Brand Portal, queste vengono messe in coda e distribuite tra questi agenti di replica tramite Round Robin.

Tuttavia, la pubblicazione può non riuscire in modo intermittente a causa di lavori di sling di grandi dimensioni, dell'aumento dell'I/O di rete e [!UICONTROL disco] nell'istanza di AEM Author o di prestazioni rallentate dell'istanza di AEM Author. È quindi consigliabile verificare la connessione con gli agenti di replica prima di iniziare la pubblicazione.

![](assets/test-connection.png)

## Risoluzione di errori nella prima pubblicazione: convalida della configurazione di pubblicazione {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Per convalidare le configurazioni di pubblicazione:

1. Controllare i registri degli errori
1. Verificare se l'agente di replica è stato creato
1. Test connessione

**Registri di coda durante la creazione del servizio cloud**

Controllare i registri di coda. Verificare se l'agente di replica è stato creato o meno. Se la creazione dell'agente di replica non riesce, modificate il servizio cloud apportando lievi modifiche al servizio cloud. Convalida e verifica nuovamente se l'agente di replica è stato creato o meno. In caso contrario, modificate nuovamente il servizio.

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

La maggior parte delle volte in cui la pubblicazione non funziona, il motivo può essere dovuto al fatto che l’utente che la pubblica (ad esempio: La replica mac-&lt;tenantid&gt; non dispone della chiave privata più recente, pertanto la pubblicazione non riesce con l'errore "401 non autorizzato" e nessun altro errore viene segnalato nei registri degli agenti di replica. Potreste voler evitare la risoluzione dei problemi e creare una nuova configurazione. Affinché la nuova configurazione funzioni correttamente, pulite le seguenti informazioni dalla configurazione dell’autore di AEM:

1. andate a [!UICONTROL localhost:4502/crx/de] (se state eseguendo l’istanza di autore in [!UICONTROL localhost:4502]):\
   i. delete /etc/replication/agents.author/mp_replica*\
   ii) delete /etc/cloudservices/mediaportal/&lt;nome_configurazione&gt;

1. andate a [!UICONTROL localhost:4502/useradmin]:\
   i cercare l'utente [!UICONTROL mac-&lt;tenantid&gt;-replicationii eliminare questo utente

Ora il sistema è completamente pulito. Ora potete provare a creare una nuova configurazione del servizio cloud e utilizzare comunque l'applicazione JWT già esistente in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). Non è necessario creare una nuova applicazione, ma solo la chiave pubblica deve essere aggiornata dalla configurazione cloud appena creata.

## Problema di visibilità tenant dell'applicazione JWT della connessione sviluppatore {#developer-connection-jwt-application-tenant-visibility-issue}

Se si trova su [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), vengono elencate tutte le organizzazioni (tenant) per le quali gli utenti correnti detengono l'amministratore di sistema. Se non trovi il nome dell'organizzazione qui o non riesci a creare un'applicazione per un tenant richiesto qui, verifica di disporre di diritti (amministratore di sistema) sufficienti per farlo.

Esiste un problema noto in questa interfaccia utente che per ogni tenant sono visibili solo le prime 10 applicazioni. Quando create l’applicazione, rimanete sulla pagina e segnalate l’URL. Non è necessario andare alla pagina di elenco dell'applicazione e trovare l'applicazione creata. Potete accedere direttamente a questo URL con segnalibro e aggiornare/eliminare l’applicazione ogni volta che necessario.

L'applicazione JWT potrebbe non essere elencata correttamente. Si consiglia pertanto di notare/contrassegnare l’URL durante la creazione dell’applicazione JWT.

## L'esecuzione della configurazione interrompe il funzionamento {#running-configuration-stops-working}

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

Se un agente di replica (che pubblicava correttamente nel portale del marchio) interrompe l'elaborazione dei processi di pubblicazione, controllate i registri di replica. In AEM è stato incorporato un nuovo tentativo automatico, pertanto se la pubblicazione di una risorsa non riesce, viene ritentata automaticamente. Se si verifica un problema intermittente come l'errore di rete, potrebbe verificarsi nuovamente durante il tentativo.

Se si verificano continui errori di pubblicazione e la coda è bloccata, controllate la connessione **[!UICONTROL di]** prova e provate a risolvere gli errori segnalati.

In base agli errori, si consiglia di registrare un ticket di assistenza, in modo che il team di progettazione di Brand Portal possa aiutarti a risolvere i problemi.
