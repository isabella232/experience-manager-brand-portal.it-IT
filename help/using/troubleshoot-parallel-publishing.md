---
title: Risoluzione dei problemi nella pubblicazione parallela su Brand Portal
seo-title: Risoluzione dei problemi nella pubblicazione parallela su Brand Portal
description: Risoluzione dei problemi pubblicazione parallela.
seo-description: Risoluzione dei problemi pubblicazione parallela.
uuid: 51 e 45 cca -8 c 96-4 c 69-84 ef -2 ef 34 f 3 bcde 2
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: riferimento
topic-tags: brand-portal
discoiquuid: a 4801024-b 509-4 c 51-afd 8-e 337417 e 658 b
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Risoluzione dei problemi nella pubblicazione parallela su Brand Portal {#troubleshoot-issues-in-parallel-publishing-to-brand-portal}

Il portale brand supporta l'integrazione con AEM Assets affinché le risorse del marchio approvate vengano trasferite (o pubblicate) direttamente dall'istanza autore di AEM Assets. Una volta [integrata](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html), AEM Author utilizza un agente di replica per replicare le risorse selezionate nel servizio cloud Brand Portal per l'utilizzo approvato dagli utenti del portale marchio. Più agenti di replica vengono utilizzati AEM 6.2 SP 1-CFP 5], AEM CFP 6.3.0.2 e successivi per consentire la pubblicazione parallela ad alta velocità.

>[!NOTE]
>
>Adobe consiglia di effettuare l'aggiornamento ad AEM 6.4.1.0 per garantire che AEM Assets Brand Portal sia integrato correttamente con AEM Assets. Una limitazione in AEM 6.4 genera un errore durante la configurazione dell'integrazione con Brand Portal e la replica non riesce.

Quando si configura il servizio cloud per brand portal in [!UICONTROL /etc/cloudservice], tutti gli utenti e token necessari vengono generati automaticamente e salvati nella directory archivio. La configurazione del servizio cloud viene creata, gli utenti del servizio richiesti per gli agenti di replica e replica per replicare il contenuto vengono creati. Vengono creati quattro agenti di replica. Quindi, quando pubblicate numerose risorse da AEM a Brand Portal, queste vengono messe in coda e distribuite tra questi agenti di replica attraverso Round Robin.

Tuttavia, la pubblicazione può non riuscire in modo intermittente a causa di processi sling di grandi dimensioni, aumento della rete e [!UICONTROL I/O] del disco sull'istanza AEM Author o delle prestazioni rallentate dell'istanza AEM Author. Si consiglia quindi di verificare la connessione con gli agenti di replica prima di iniziare la pubblicazione.

![](assets/test-connection.png)

## Risoluzione dei problemi relativi alla prima pubblicazione: convalida della configurazione di pubblicazione {#troubleshoot-failures-in-first-time-publishing-validating-your-publish-configuration}

Per convalidare le configurazioni di pubblicazione:

1. Verificate i registri di errore
2. Verificare se l'agente di replica è stato creato
3. Connessione testuale

**Registri di coda durante la creazione del servizio cloud**

Controllate i registri di coda. Verificate che l'agente di replica sia stato creato o meno. Se la creazione dell'agente di replica non riesce, modificate il servizio cloud apportate modifiche minori nel servizio cloud. Convalidate e verificate nuovamente se l'agente di replica viene creato o meno. In caso contrario, modificate nuovamente il servizio.

Se la modifica del servizio cloud non è configurata in modo corretto, segnalate un ticket legale.

**Verifica connessione con agenti di replica**

Visualizza registro, se si verificano errori nel registro di replica:

1. Contattate il supporto Adobe.

2. Riprovate [a pulire](../using/troubleshoot-parallel-publishing.md#clean-up-existing-config) e create di nuovo la configurazione di pubblicazione.

<!--
Comment Type: remark
Last Modified By: Mini Gulati (mgulati)
Last Modified Date: 2018-06-21T22:56:21.256-0400
<p>?? check and compare public key. At times public key is different</p>
<p>?? another thing to check in /useradmin</p>
-->

### Pulizia delle configurazioni di pubblicazione di Brand Portal esistente {#clean-up-existing-config}

La maggior parte delle volte in cui la pubblicazione non funziona, può essere necessario che l'utente che pubblica (ad esempio: [!UICONTROL mac-&lt; tenantid &gt;-replica]) non dispone della chiave privata più recente, pertanto la pubblicazione non riesce con l'errore "401 unautorizzato" e non viene segnalato nessun altro errore nei registri degli agenti di replica. Potrebbe essere utile evitare la risoluzione dei problemi e creare una nuova configurazione. Affinché la nuova configurazione funzioni correttamente, ripulite quanto segue dalla configurazione dell'autore di AEM:

1. vai a [!UICONTROL localhost: 4502/crx/de] (considerando che state eseguendo istanza di authoring su [!UICONTROL localhost: 4502]):\
   i. delete /etc/replication/agents.author/mp_replication *\
   ii. delete /etc/cloudservices/mediaportal/ &lt; config_ name &gt;

2. vai a [!UICONTROL localhost: 4502/useradmin]:\
   i search for user [! UICONTROL mac-&lt; tenantid &gt;-replication
ii delete this user

Ora il sistema è tutto pulito. Ora potete tentare di creare una nuova configurazione cloud e continuare a utilizzare l'applicazione JWT esistente in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/). Non è necessario creare una nuova applicazione, ma è necessario aggiornare solo la chiave pubblica dalla nuova configurazione cloud creata.

## Problema di visibilità tenant dell'applicazione JWT per sviluppatore {#developer-connection-jwt-application-tenant-visibility-issue}

Se in [https://legacy-oauth.cloud.adobe.io/](https://legacy-oauth.cloud.adobe.io/), vengono elencate tutte le organizzazioni (tenant) per cui gli utenti correnti detengono l'amministratore di sistema. Se non trovate qui il nome organizzazione oppure non potete creare un'applicazione per un tenant obbligatorio qui, verificate che disponiate dei diritti sufficienti (amministratore di sistema) per farlo.

Esiste un problema noto su questa interfaccia utente che per ogni tenant sono visibili solo le prime 10 applicazioni. Quando create l'applicazione, usate la pagina e segnalibri sull'URL. Non è necessario passare alla pagina di elenco dell'applicazione e trovare l'applicazione che hai creato. Potete accedere direttamente a questo URL con segnalibro e aggiornare o eliminare l'applicazione ogni volta che necessario.

L'applicazione JWT potrebbe non essere elencata correttamente. Si consiglia quindi di inserire/aggiungere un segnalibro all'URL durante la creazione dell'applicazione JWT.

## La configurazione della configurazione si interrompe {#running-configuration-stops-working}

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

Se un agente di replica (che stava pubblicando il brand portal è sufficiente) interrompe i processi di pubblicazione, controllate i registri di replica. AEM dispone di un nuovo tentativo di ripristino automatico, quindi se una particolare pubblicazione di risorse non riesce, viene riprovata automaticamente. Se si verifica un problema intermittente come l'errore di rete, potrebbe riuscire durante il ritentativo.

Se sono presenti errori di pubblicazione continui e la coda è bloccata, è necessario controllare **[!UICONTROL la connessione]** di prova e tentare di risolvere gli errori segnalati.

In base agli errori, vi viene richiesto di registrare un ticket di supporto, in modo che il team tecnico di Brand Portal possa aiutarti a risolvere i problemi.
