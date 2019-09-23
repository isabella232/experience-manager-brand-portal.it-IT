---
title: Condividere le cartelle
seo-title: Condividere le cartelle
description: Il Brand Portal non supporta l’assimilazione delle risorse. Pertanto, le risorse devono essere pubblicate nel Brand Portal da un’istanza AEM Author preconfigurata. Le risorse pubblicate non sono accessibili agli utenti non amministratori di Brand Portal, a meno che non siano configurate durante la configurazione della replica con l’istanza AEM, e devono essere condivise con loro.
seo-description: Il Brand Portal non supporta l’assimilazione delle risorse. Pertanto, le risorse devono essere pubblicate nel Brand Portal da un’istanza AEM Author preconfigurata. Le risorse pubblicate non sono accessibili agli utenti non amministratori di Brand Portal, a meno che non siano configurate durante la configurazione della replica con l’istanza AEM, e devono essere condivise con loro.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: riferimento
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Condivisione di cartelle sul Brand Portal {#share-folders}

Le risorse devono essere pubblicate su Brand Portal da un’istanza di AEM Author preconfigurata, in quanto Brand Portal non supporta l’assimilazione delle risorse.

## Flusso di lavoro per la condivisione di cartelle in Brand Portal {#folder-sharing-workflow-in-brand-portal}

Di seguito viene descritto il flusso di lavoro di condivisione delle cartelle e l’accesso degli utenti:

* Per impostazione predefinita, tutte le cartelle pubblicate da AEM Assets al Portale marchio sono visibili solo all’amministratore del Portale marchio, a meno che non siano contrassegnate come pubbliche durante la configurazione della replica.
* L’amministratore utilizza la console Proprietà  cartella per condividere una cartella con utenti o gruppi selettivi. Solo gli utenti o i gruppi con i quali la cartella è condivisa possono visualizzarla dopo l’accesso al Portale marchio. La cartella non è visibile agli altri utenti.
* L’amministratore può anche scegliere di rendere pubblica una cartella tramite la casella di controllo Cartella  pubblica nella console Proprietà  cartella. Una cartella pubblica è visibile a tutti gli utenti.

* Irrespective of user roles and privileges, when users log in to Brand Portal, they see all the public folders, and the folders directly shared with them or with a group to which they belong. Private folders, or folders shared with other users, are not visible to all users.

### Share folders with user groups on Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

Access rights on assets of a folder are dependant on the access rights on its parent folder, irrespective of the settings of children folders. Questo comportamento è regolato dagli [ACL](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM) in AEM, poiché le cartelle figlie ereditano gli ACL dalle cartelle principali. For example, if a folder A contains folder B which contains folder C, then a user group (or users) having access rights on folder A also have the same access rights on folder B and folder C. Folder B being the child folder of A inherits its ACLs, and folder C being the child folder of B inherits its ACLs.

Allo stesso modo, i gruppi di utenti (o utenti) che dispongono delle autorizzazioni per accedere solo alla cartella B hanno le stesse autorizzazioni di accesso nella cartella C ma non nella cartella A. Si consiglia pertanto alle organizzazioni di disporre il contenuto in modo che le risorse più esposte vengano inserite nella cartella figlio e che l’accesso alle cartelle principali possa essere limitato dagli elementi secondari.

### Public folder publish {#public-folder-publish}

A meno che l’opzione Pubblica [!UICONTROL nella cartella] pubblica non sia selezionata durante la configurazione della replica del Portale marchio, gli utenti non amministratori (come editor e visualizzatori) non hanno accesso alle risorse pubblicate da AEM Assets al Portale marchio.

![](assets/assetbpreplication.png)

Se l’opzione Pubblica [!UICONTROL nella cartella] pubblica è disabilitata, gli amministratori devono condividere in modo specifico queste risorse con utenti non amministratori che utilizzano la funzionalità di condivisione.

>[!NOTE]
>
>L’opzione per attivare la pubblicazione [!UICONTROL delle cartelle] pubbliche è disponibile a partire da AEM 6.3.2.1.

## Accesso alle cartelle condivise {#access-to-shared-folders}

Nella seguente matrice vengono descritti i diritti di accesso e i diritti di condivisione o annullamento della condivisione delle risorse per vari ruoli utente:

|  | Accesso a tutte le cartelle pubblicate da AEM Assets al Portale marchio | Accesso alle cartelle condivise | Condividere/annullare la condivisione dei diritti di cartella |
|---------------|-----------|-----------|------------|
| Amministratore | Sì | Sì | Sì |
| Editor | No* | Sì, solo se condiviso con loro o con il gruppo al quale appartengono | Sì, solo per le cartelle condivise con loro o con il gruppo al quale appartengono |
| Visualizzatore | No* | Sì, solo se condiviso con loro o con il gruppo al quale appartengono | No |
| Utente ospite | No* | Sì, solo se condiviso con loro o con il gruppo al quale appartengono | No |

**Per impostazione predefinita, l'opzione Pubblica[!UICONTROL cartella]pubblica è disattivata durante la configurazione della replica di Brand Portal con AEM Author. Se l’opzione è abilitata, per impostazione predefinita le cartelle pubblicate su Brand Portal saranno accessibili a tutti gli utenti (anche agli utenti non amministratori).*

### Accesso utente non amministratore alle cartelle condivise {#non-admin-user-access-to-shared-folders}

Gli utenti non amministratori possono accedere solo alle cartelle condivise con loro sul Brand Portal. Tuttavia, la modalità di visualizzazione di queste cartelle sul portale al momento dell'accesso dipende dalle impostazioni di [!UICONTROL Abilita configurazione gerarchia] cartelle.

**Se la configurazione è disabilitata**

Gli utenti non amministratori visualizzano tutte le cartelle condivise con loro sulla pagina di destinazione, al momento dell’accesso al Portale marchio.

![](assets/disabled-folder-hierarchy1-1.png)

**Se la configurazione è abilitata**

Gli utenti non amministratori visualizzano la struttura delle cartelle (a partire dalla cartella principale) e le cartelle condivise disposte all’interno delle rispettive cartelle principali, al momento dell’accesso al Portale marchio.

Queste cartelle principali sono le cartelle virtuali e non è possibile eseguire alcuna azione su di esse. È possibile riconoscere queste cartelle virtuali con un'icona a forma di lucchetto.

A differenza delle cartelle condivise, non è visibile alcuna attività di azione al passaggio del mouse o alla selezione in vista a schede. [!UICONTROL Il pulsante Panoramica] viene visualizzato quando si seleziona una cartella virtuale in Visualizzazione [!UICONTROL a] colonne e Visualizzazione elenco.

>[!NOTE]
>
>La miniatura predefinita delle cartelle virtuali è la miniatura della prima cartella condivisa.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Condividere le cartelle {#how-to-share-folders}

Per condividere una cartella con gli utenti sul Brand Portal, effettuate le seguenti operazioni:

1. Fate clic sull'icona della sovrapposizione a sinistra, quindi scegliete **[!UICONTROL Navigazione]**.

   ![](assets/selectorrail.png)

2. Dall'area laterale a sinistra, selezionate **[!UICONTROL File]**.

   ![](assets/access_files.png)

3. Dall’interfaccia Brand Portal, selezionate la cartella da condividere.

   ![](assets/share-folders.png)

4. Dalla barra degli strumenti nella parte superiore, selezionate **[!UICONTROL Condividi]**.

   ![](assets/share_icon.png)

   Viene visualizzata la console Proprietà  cartella.

   ![](assets/folder_properties.png)

5. Nella console Proprietà  cartella, specificate il titolo della cartella nel campo Titolo  cartella se non desiderate che il nome predefinito venga visualizzato agli utenti.
6. Dall’elenco [!UICONTROL Aggiungi utente] , selezionate gli utenti o i gruppi con i quali desiderate condividere la cartella e fate clic su **[!UICONTROL Aggiungi]**.
Per condividere la cartella solo con gli utenti ospiti e nessun altro utente, selezionate Utenti **** anonimi dal menu a discesa [!UICONTROL Membri] .

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Per rendere la cartella disponibile a tutti gli utenti, indipendentemente dall’appartenenza e dal ruolo del gruppo, rendetela pubblica selezionando la casella di controllo Cartella **** pubblica.

7. Se necessario, fate clic su **[!UICONTROL Cambia miniatura]** per modificare l’immagine in miniatura della cartella.
8. Fai clic su **[!UICONTROL Salva]**.
9. Per accedere alla cartella condivisa, accedete a Brand Portal con le credenziali dell’utente con cui avete condiviso la cartella. Rivedete la cartella condivisa nell'interfaccia.

## Annulla condivisione cartelle {#unshare-the-folders}

Per annullare la condivisione di una cartella precedentemente condivisa, effettuate le seguenti operazioni:

1. Dall’interfaccia Brand Portal, selezionate la cartella da annullare la condivisione.

   ![](assets/share-folders-1.png)

2. Dalla barra degli strumenti nella parte superiore, fate clic su **[!UICONTROL Condividi]**.
3. Nella console Proprietà  cartella, in [!UICONTROL Membri], fate clic sul simbolo **[!UICONTROL x]** accanto all’utente per rimuoverlo dall’elenco degli utenti con cui avete condiviso la cartella.

   ![](assets/folder_propertiesunshare.png)

4. Nella finestra del messaggio di avviso, fare clic su **[!UICONTROL Conferma]** per confermare l'annullamento della condivisione.
Fai clic su **[!UICONTROL Salva]**.

5. Accedete al Portale del marchio con le credenziali dell'utente rimosso dall'elenco condiviso. La cartella non è più disponibile nell’interfaccia Brand Portal per l’utente.
