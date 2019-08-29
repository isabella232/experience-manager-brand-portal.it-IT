---
title: Gestione di utenti, gruppi e ruoli utente
seo-title: Gestione di utenti, gruppi e ruoli utente
description: Gli amministratori possono utilizzare Adobe Admin Console per creare utenti di AEM Assets Brand Portal e profili di prodotto e gestire i propri ruoli utilizzando l'interfaccia utente Brand Portal. Questo privilegio non è disponibile per i visualizzatori e gli editor.
seo-description: Gli amministratori possono utilizzare Adobe Admin Console per creare utenti di AEM Assets Brand Portal e profili di prodotto e gestire i propri ruoli utilizzando l'interfaccia utente Brand Portal. Questo privilegio non è disponibile per i visualizzatori e gli editor.
uuid: 0 dc 1867 c -6 d 1 b -4 d 0 d-a 25 e -0 df 207 c 269 b 8
content-type: riferimento
topic-tags: administration
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: ba 468 e 80-d 077-4 af 6-b 782-238 fc 557 e 22 b
translation-type: tm+mt
source-git-commit: 32c3cdb8e3fafd74cfb36e6bcfe0811e7152b2d0

---


# Gestione di utenti, gruppi e ruoli utente {#manage-users-groups-and-user-roles}

Gli amministratori possono utilizzare [!DNL Adobe Admin Console] per creare [!DNL AEM Assets Brand Portal] utenti e profili di prodotto e gestire i propri ruoli utilizzando l'interfaccia utente Brand Portal. Questo privilegio non è disponibile per i visualizzatori e gli editor.

In [Admin Console](http://adminconsole.adobe.com/enterprise/overview), puoi visualizzare tutti i prodotti associati alla tua organizzazione. Un prodotto potrebbe essere una [!DNL Experience Cloud] qualsiasi soluzione, ad esempio [!DNL Adobe Analytics], [!DNL Adobe Target]o [!DNL AEM Brand Portal]. Devi scegliere il prodotto AEM Brand Portal e creare profili di prodotto.

<!--
Comment Type: draft

<note type="note">
<p>Product Profiles (formerly known as product configurations*). </p>
<p>* The nomenclature has changed from product configurations to product profiles in the new Adobe Admin Console.</p>
</note>
-->
![](assets/create-user-group.png)

Questi profili di prodotto vengono sincronizzati con l'interfaccia [!DNL Brand Portal] utente ogni 8 ore e visibili come gruppi. [!DNL Brand Portal] Dopo aver aggiunto utenti e creato profili di prodotto e aggiunto utenti a tali profili di prodotto, puoi assegnare ruoli a utenti e gruppi in [!DNL Brand Portal].

>[!NOTE]
>
>Per creare gruppi in [!DNL Brand Portal], dalla [!DNL Adobe Admin Console]pagina **Prodotti** &gt; Profili **** di prodotto, anziché Pagina **utente** &gt; Gruppi **di utenti**. I profili di prodotto in [!DNL Adobe Admin Console] vengono utilizzati per creare gruppi.[!DNL Brand Portal]

## Aggiungere un utente {#add-a-user}

Se siete un amministratore di prodotto, utilizzate [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) per creare utenti e assegnarli a profili di prodotto (*precedentemente noti come configurazioni di prodotto*), [!DNL Brand Portal]che vengono visualizzati come gruppi. Potete usare i gruppi per eseguire operazioni in massa quali gestione dei ruoli e condivisione delle risorse.

>[!NOTE]
I nuovi utenti che non dispongono dell'accesso possono [!DNL Brand Portal] richiedere l'accesso dalla schermata di accesso. [!DNL Brand Portal] Per ulteriori informazioni, consulta [Richiedere l'accesso a [! DNL Brand Portal]](../using/brand-portal.md#request-access-to-brand-portal). Dopo aver ricevuto le notifiche di richiesta di accesso nell'area di notifica, fate clic sulla notifica interessata e quindi su **Concedi accesso**. In alternativa, segui il collegamento presente nel messaggio e-mail di richiesta di accesso ricevuto. Successivamente, per aggiungere un utente tramite [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview), segui i passaggi 4-7 nella procedura seguente.

>[!NOTE]
Potete accedere a [[! DNL Adobe Admin Console]](http://adminconsole.adobe.com/enterprise/overview) direttamente o da [!DNL Brand Portal]. Se accedete direttamente, seguite i passaggi 4-7 nella procedura seguente per aggiungere un utente.

1. Nella [!DNL AEM] barra degli strumenti in alto, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![Logo AEM](assets/aemlogo.png)

2. Dal pannello degli strumenti di amministrazione, fate clic **su Utenti**.

   ![Pannello Strumenti amministratore](assets/admin-tools-panel-5.png)

3. Nella **pagina Ruoli** utente, fai clic sulla **scheda Gestione** , quindi su **Avvia Admin Console**.

   ![Ruoli utente per avviare Admin Console](assets/launch_admin_console.png)

4. In Admin Console, effettuate una delle seguenti operazioni per creare un nuovo utente:

   * Nella barra degli strumenti in alto, fate clic **su Panoramica**. Nella pagina **Panoramica** , fai clic **su Assegna utenti** dalla scheda **[!DNL AEM Brand Portal]** Prodotto.
   ![Panoramica di Admin Console](assets/admin_console_overviewadduser.png)

   * Nella barra degli strumenti in alto, fate clic **su Utenti**. Nella pagina **Utenti** , **per impostazione predefinita gli utenti** nella barra a sinistra sono selezionati. Fate clic **su Aggiungi utente**.
   ![Aggiunta di utenti Admin Console](assets/admin_console_adduseruserpage.png)

5. Nella finestra di dialogo Aggiungi utente, digitate l'ID e-mail dell'utente che desiderate aggiungere o selezionate dall'elenco dei suggerimenti che vengono visualizzati durante il digitazione.

   ![Aggiungere utenti a Brand Portal](assets/add_user_to_aem_bp.png)

6. Assegna l'utente ad almeno un profilo di prodotto (precedentemente denominato configurazioni di prodotto) in modo che l'utente possa accedere a Brand Portal. Seleziona il profilo di prodotto appropriato dall' **elenco Selezionate un profilo per il** campo di prodotto.
7. Fai clic su **Salva**. Viene inviato un messaggio e-mail di benvenuto all'utente aggiunto. L'utente invitato può accedere [!DNL Brand Portal] facendo clic sul collegamento nel messaggio e-mail di benvenuto e effettuando l'accesso con un [!UICONTROL Adobe ID]. Per ulteriori informazioni, consultate [Esperienze di accesso per la prima volta](../using/brand-portal-onboarding.md).

   >[!NOTE]
   Se un utente non è in grado di eseguire [!DNL Brand Portal]l'accesso, l'amministratore dell'organizzazione deve visitare Adobe [!UICONTROL Admin Console] e controllare se l'utente è presente ed è stato aggiunto ad almeno un profilo di prodotto.

   Per informazioni sulla concessione di privilegi di amministratore all'utente, consultate [Fornire privilegi di amministratore agli utenti](../using/brand-portal-adding-users.md#provideadministratorprivilegestousers).

## Aggiunta di un profilo di prodotto {#add-a-product-profile}

I profili di prodotto (precedentemente noti come configurazioni di prodotto) in [!UICONTROL Admin Console] sono utilizzati per creare gruppi in [!DNL Brand Portal] modo da poter eseguire operazioni in massa quali gestione dei ruoli e condivisione delle risorse. [!DNL Brand Portal] **[!DNL Brand Portal]** è il profilo di prodotto predefinito disponibile; puoi creare altri profili di prodotto e aggiungere utenti ai nuovi profili di prodotto.

>[!NOTE]
Potete accedere a [[! UICONTROL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) direttamente o da [!DNL Brand Portal]. Se accedi direttamente ad [!UICONTROL Admin Console] , segui i passaggi 4-7 nella procedura seguente per aggiungere un profilo di prodotto.

1. Nella [!DNL AEM] barra degli strumenti in alto, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![[!DNL AEM] Logo](assets/aemlogo.png)

2. Dal pannello degli strumenti di amministrazione, fate clic **su Utenti**.

   ![Pannello Strumenti amministratore](assets/admin-tools-panel-6.png)

3. Nella **pagina Ruoli** utente, fai clic sulla **scheda Gestione** , quindi su **Avvia Admin Console**.

   ![Avviare Admin Console](assets/launch_admin_console.png)

4. Dalla barra degli strumenti in alto, fate clic **su Prodotti**.
5. Nella pagina **Prodotti** , **per impostazione predefinita viene** selezionato Profilo di prodotto. Fate clic su **Nuovo profilo**.

   ![Aggiungi nuovo profilo di prodotto](assets/admin_console_addproductprofile.png)

6. Nella pagina **Crea nuovo profilo** , indicate il nome, il nome visualizzato, la descrizione del profilo e scegliete se inviare un messaggio e-mail agli utenti quando vengono aggiunti o rimossi dal profilo.

   ![Crea profilo di prodotto](assets/admin_console_addaproductprofilecreatenewprofile.png)

7. Fate clic su **Fine**. Il gruppo di configurazione di prodotto, ad esempio **Gruppo vendite**, viene aggiunto al portale marchio.

   ![Profili di prodotto](assets/admin_console_productprofileadded.png)

## Aggiunta di utenti a un profilo di prodotto {#add-users-to-a-product-profile}

Per aggiungere utenti a [!DNL Brand Portal] un gruppo, aggiungili al profilo di prodotto corrispondente (precedentemente denominato configurazioni di prodotto) in [!UICONTROL Admin Console]. Potete aggiungere utenti singolarmente o in gruppo.

>[!NOTE]
Potete accedere a [[! DNL Admin Console]](http://adminconsole.adobe.com/enterprise/overview) direttamente o da [!DNL Brand Portal]. Se accedi direttamente ad Admin Console, segui i passaggi 4-7 nella procedura seguente per aggiungere utenti a un profilo di prodotto.

1. Nella [!DNL AEM] barra degli strumenti in alto, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![[!DNL AEM] Logo](assets/aemlogo.png)

2. Dal pannello degli strumenti di amministrazione, fate clic **su Utenti**.

   ![Pannello Strumenti amministratore](assets/admin-tools-panel-7.png)

3. Nella **pagina Ruoli** utente, fai clic sulla **scheda Gestione** , quindi su **Avvia Admin Console**.

   ![Launch [!DNL Admin Console]](assets/launch_admin_console.png)

4. Dalla barra degli strumenti in alto, fate clic **su Prodotti**.
5. Nella pagina **Prodotti** , **per impostazione predefinita viene** selezionato Profilo di prodotto. Apri il profilo di prodotto a cui vuoi aggiungere un utente, ad esempio **, Gruppo vendite**.

   ![Profili di prodotto](assets/admin_console_productprofileadded.png)

6. Per aggiungere singoli utenti al profilo di prodotto, effettua le seguenti operazioni:

   * Fate clic **su Aggiungi utente**.
   ![Gruppo per la mappatura Profilo di prodotto in [!DNL Brand Portal]](assets/admin_console_productprofilesalesgroup.png)

   * Nella pagina **Aggiungi utente alla** vendita, digitate l'ID e-mail dell'utente che desiderate aggiungere o selezionate dall'elenco dei suggerimenti che vengono visualizzati durante il digitazione.
   ![Aggiungere utenti a un gruppo](assets/admin_console_addusertosalesgroup.png)

   * Fai clic su **Salva**.



7. Per aggiungere utenti in massa al profilo di prodotto, effettua le seguenti operazioni:

   * Scegliete le ellissi(...)****&gt; **Aggiungi utenti in base al CSV**.
   ![Aggiunta di utenti in gruppo](assets/admin_console_addbulkusers.png)

   * Nella pagina **Aggiungi utenti per CSV** , scaricate un modello CSV o trascinate un file CSV.
   ![Aggiunta di utenti in base a CSV](assets/admin_console_addbulkuserscsv.png)

   * Click **Upload**.
   Se avete aggiunto utenti al profilo di prodotto predefinito, viene inviato [!DNL Brand Portal]un messaggio e-mail di benvenuto all'ID e-mail degli utenti che avete aggiunto. Gli utenti invitati possono accedere [!DNL Brand Portal] facendo clic sul collegamento nel messaggio e-mail di benvenuto e effettuando l'accesso con un [!UICONTROL Adobe ID]. Per ulteriori informazioni, consultate [Esperienze di accesso per la prima volta](../using/brand-portal-onboarding.md).

   Gli utenti aggiunti a un profilo di prodotto personalizzato o nuovo non ricevono notifiche e-mail.

## Fornire privilegi di amministratore agli utenti {#provide-administrator-privileges-to-users}

Potete fornire l'amministratore di sistema o il privilegio di amministratore di un prodotto a un [!DNL Brand Portal] utente. Non fornire altri diritti amministrativi disponibili in [!UICONTROL Admin Console], ad esempio amministratore di profilo di prodotto, amministratore di gruppo di utenti e amministratore del supporto. Per ulteriori informazioni su questi ruoli, consultate [Ruoli amministrativi](https://helpx.adobe.com/enterprise/using/admin-roles.html).

>[!NOTE]
Potete accedere a [[! UICONTROL Admin Console]](https://adminconsole.adobe.com/enterprise/overview) direttamente o da [!DNL Brand Portal]. Se accedi direttamente ad [!UICONTROL Admin Console] , segui i passaggi 4-8 nella procedura seguente per aggiungere un utente a un profilo di prodotto.

1. Nella [!DNL AEM] barra degli strumenti in alto, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![Aemlogo](assets/aemlogo.png)

2. Dal pannello degli strumenti di amministrazione, fate clic **su Utenti**.

   ![Pannello Strumenti amministratore](assets/admin-tools-panel-8.png)

3. Nella **pagina Ruoli** utente, fai clic sulla **scheda Gestione** , quindi su **Avvia Admin Console**.

   ![Avviare Admin Console](assets/launch_admin_console.png)

4. Nella barra degli strumenti in alto, fate clic **su Utenti**.
5. Nella pagina **Utenti** , **per impostazione predefinita gli utenti** nella barra a sinistra sono selezionati. Fate clic sul nome utente dell'utente al quale desiderate fornire i privilegi di amministratore.

   ![Aggiungi utenti in Admin Console](assets/admin_console_adduseruserpage.png)

6. Nella pagina del profilo utente, individuate la **sezione Diritti** amministrativi nella parte inferiore e scegliete puntini di sospensione(...)****&gt; **Modifica diritti di amministratore**.
   ![Diritti di amministratore in Admin Console](assets/admin_console_editadminrights.png)

7. Nella pagina **Modifica amministratore** , seleziona Amministratore di sistema o Amministratore di prodotto.

   ![Modifica dei diritti di amministratore in Admin Console](assets/admin_console_editadminrightsselection.png)

   >[!NOTE]
   [!DNL Brand Portal] supporta solo i ruoli di amministratore di sistema e amministratore prodotto.
   [!DNL Adobe] consiglia di evitare di utilizzare il ruolo di amministratore di sistema perché garantisce privilegi amministrativi a livello dell'organizzazione per tutti i prodotti di un'organizzazione. Ad esempio, un amministratore di sistema di un'organizzazione che include tre prodotti Marketing Cloud dispone dell'intero set di privilegi per tutti e tre i prodotti. Solo un amministratore di sistema può configurare [!DNL AEM] le risorse in modo che le risorse possano essere pubblicate da [!DNL AEM] Risorse a [!DNL Brand Portal]. Per ulteriori informazioni, consulta [Configurazione dell'integrazione di AEM Assets con [! DNL Brand Portal]](https://helpx.adobe.com/experience-manager/6-5/assets/using/brand-portal-configuring-integration.html).
   Al contrario, il ruolo di amministratore di prodotto concede i privilegi di amministratore solo a un prodotto specifico. Per applicare un controllo più dettagliato all'accesso, [!DNL Brand Portal]usa il ruolo di amministratore di prodotto e seleziona il prodotto come **[!DNL AEM Brand Portal]**.

   >[!NOTE]
   [!DNL Brand Portal] non supporta privilegi di amministratore di profilo di prodotto (precedentemente noti come amministratore di configurazione). Evita di assegnare diritti di amministratore del profilo di prodotto a un utente.

8. Rivedete il tipo di amministratore e fate clic **su Salva**.

   >[!NOTE]
   Per revocare i privilegi di amministratore di un utente, apportate le modifiche appropriate nella pagina **Modifica amministratore** , quindi fate clic **su Salva**.

## Gestire i ruoli utente {#manage-user-roles}

Un amministratore può modificare i ruoli per [!DNL Brand Portal]gli utenti.

Oltre al ruolo Amministratore [!DNL Brand Portal] , supporta i seguenti ruoli:

* **Visualizzatore**: Gli utenti con questo ruolo possono visualizzare i file e le cartelle che un amministratore condivide con loro. I visualizzatori possono inoltre cercare e scaricare le risorse. Tuttavia, i visualizzatori non possono condividere contenuto (file, cartelle, [!UICONTROL raccolte]) con altri utenti.
* **Editor**: Gli utenti con questo ruolo dispongono di tutti i privilegi di un visualizzatore. Inoltre, gli editor possono condividere contenuto (cartelle, [!UICONTROL raccolte], collegamenti) con altri utenti.

1. Nella [!DNL AEM] barra degli strumenti in alto, fate clic sul logo Adobe per accedere agli strumenti di amministrazione.

   ![Aemlogo](assets/aemlogo.png)

2. Dal pannello degli strumenti di amministrazione, fate clic **su Utenti**.

   ![Pannello Strumenti amministratore](assets/admin-tools-panel-9.png)

3. Nella pagina **Ruoli** utente, la scheda **Utenti** è selezionata per impostazione predefinita. Per l'utente di cui desiderate cambiare il ruolo, selezionate **Editor** o **Visualizzatore** dal menu **a** discesa Ruolo.

   ![Modifica dei ruoli degli utenti](assets/modify_user_role.png)

   Per modificare il ruolo di più utenti contemporaneamente, seleziona gli utenti e scegli il ruolo appropriato dal menu **a** discesa Ruolo.

   >[!NOTE]
   L'elenco **Ruolo** per gli utenti amministratore è disattivato. Non potete selezionare questi utenti per modificarne i ruoli.

   >[!NOTE]
   Il ruolo utente viene disattivato anche se l'utente è un membro del gruppo Editor. Per revocare i privilegi di modifica dall'utente, rimuovete l'utente dal gruppo Editor o modificate il ruolo dell'intero gruppo nel visualizzatore.

4. Fai clic su **Salva**. Il ruolo viene modificato per l'utente corrispondente. Se avete selezionato più utenti, i ruoli per tutti gli utenti vengono modificati contemporaneamente.

   >[!NOTE]
   Le modifiche nelle autorizzazioni dell'utente vengono riportate nella pagina Ruoli **utente** solo dopo che gli utenti hanno eseguito nuovamente il login al portale marchio.

## Gestione dei ruoli e dei privilegi dei gruppi {#manage-group-roles-and-privileges}

Un amministratore può associare privilegi specifici a un [gruppo](../using/brand-portal-adding-users.md#main-pars-title-278567577) di utenti sul portale brand. La **scheda Gruppi** nella **pagina Ruoli** utente consente agli amministratori di:

* Assegnazione di ruoli a gruppi di utenti
* Limita i gruppi di utenti per scaricare rappresentazioni originali di file immagine (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portatile-bitmap, x-portable-graymap, x-portable-graymap, x-rgb, x-icon, image/photoshop, x-icon, image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) da Brand Portal.

>[!NOTE]
Per le risorse condivise come collegamento, l'autorizzazione per accedere alle rappresentazioni originali dei file di immagine si applica in base alle autorizzazioni dell'utente che condivide le risorse.

Per modificare il ruolo e il diritto di accesso alle rappresentazioni originali per determinati membri del gruppo, effettuate le seguenti operazioni:

1. Nella **pagina Ruoli** utente, passate alla **scheda Gruppi** .
2. Selezionate i gruppi per i quali desiderate modificare i ruoli.
3. Seleziona il ruolo appropriato dall'elenco **a** discesa Ruolo.

   Per consentire ai membri di un gruppo di accedere a rappresentazioni originali di file immagine (.jpeg. tiff. png. bmp. gif. pjpeg, x-portable-anymap, x-portatile-bitmap, x-portable-graymap, x-portable-graymap, x-display-pixmap, x-xpixel, x-icon, x-icon, image/photoshop, image/x-photoshop. psd, image/vnd. adobe. photoshop) che vengono scaricati dal portale o da un collegamento condiviso, mantenere l'opzione **Accesso all'originale** selezionata per quel gruppo. Per impostazione predefinita, **l'opzione Accesso all'originale** è selezionata per tutti gli utenti. Per impedire a un gruppo di utenti di accedere alle rappresentazioni originali, deselezionate l'opzione corrispondente a tale gruppo.

   ![Ruoli dei gruppi di utenti](assets/access-original-rend.png)

   >[!NOTE]
   Se un utente viene aggiunto a più gruppi e uno di questi dispone di restrizioni, queste vengono applicate a quell'utente.
   Inoltre, le limitazioni per accedere alle rappresentazioni originali dei file di immagine non sono applicabili agli amministratori, anche se sono membri di gruppi limitati.

4. Fai clic su **Salva**. Il ruolo viene modificato per i gruppi corrispondenti.

   >[!NOTE]
   L'associazione utente-gruppo, o l'appartenenza al gruppo di un utente, viene sincronizzata [!DNL Brand Portal] con ogni 8 ore. Le modifiche apportate ai ruoli di utenti o gruppi sono effettive dopo l'esecuzione del processo di sincronizzazione successivo.
