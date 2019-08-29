---
title: Condividere le cartelle
seo-title: Condividere le cartelle
description: Brand Portal non supporta l'assimilazione delle risorse, pertanto le risorse devono essere pubblicate su Brand Portal da un'istanza AEM Author preconfigurata. Le risorse pubblicate non sono accessibili agli utenti non amministratori di Brand Portal, a meno che non configurino la replica con l'istanza AEM e debbano essere condivise con loro.
seo-description: Brand Portal non supporta l'assimilazione delle risorse, pertanto le risorse devono essere pubblicate su Brand Portal da un'istanza AEM Author preconfigurata. Le risorse pubblicate non sono accessibili agli utenti non amministratori di Brand Portal, a meno che non configurino la replica con l'istanza AEM e debbano essere condivise con loro.
uuid: 340 d 0 a 49-b 708-4 f 0 e -9 fb 8-99 c 824942 f 34
content-type: riferimento
topic-tags: condivisione
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
discoiquuid: 2332 c 16 f -40 be -4673-8 cc 6-2360 d 5 b 74116
translation-type: tm+mt
source-git-commit: 0b70e82d034ce56fcfc5b49396e6d3a9da4b49d4

---


# Condividere cartelle su Brand Portal {#share-folders}

Le risorse devono essere pubblicate su Brand Portal da un'istanza AEM Author preconfigurata, in quanto Brand Portal non supporta l'assimilazione delle risorse.

## Flusso di lavoro di condivisione delle cartelle in Brand Portal {#folder-sharing-workflow-in-brand-portal}

Di seguito viene descritto il flusso di lavoro di condivisione della cartella e l'accesso degli utenti:

* Per impostazione predefinita, tutte le cartelle pubblicate da AEM Assets a Brand Portal sono visibili solo all'amministratore Brand Portal, a meno che non sia contrassegnata come pubblica durante la configurazione della replica.
* L'amministratore utilizza la **console Proprietà** cartella per condividere una cartella con utenti o gruppi selettivi. Solo gli utenti o i gruppi con cui è condiviso la cartella possono vedere la cartella dopo l'accesso al portale marchio. La cartella non è visibile ad altri utenti.
* L'amministratore può anche scegliere di rendere pubblica una cartella tramite la **casella di** controllo Cartella pubblica **nella console Proprietà** cartella. Una cartella pubblica è visibile a tutti gli utenti.

* A prescindere dai ruoli utente e dai privilegi, quando gli utenti accedono al portale marchio possono vedere tutte le cartelle pubbliche e le cartelle direttamente condivise con loro o con un gruppo a cui appartengono. Le cartelle private, o le cartelle condivise con altri utenti, non sono visibili a tutti gli utenti.

### Condividere cartelle con gruppi di utenti su Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

I diritti di accesso sulle risorse di una cartella dipendono dai diritti di accesso presenti nella cartella principale, indipendentemente dalle impostazioni delle cartelle figlie. Questo comportamento è regolamentato dagli [ACL](https://helpx.adobe.com/experience-manager/6-5/sites/administering/using/security.html#PermissionsinAEM) in AEM, come cartelle secondarie ereditano gli ACL dalle rispettive cartelle principali. Ad esempio, se una cartella A contiene la cartella B contenente la cartella C, un gruppo di utenti (o utenti) che dispongono dei diritti di accesso nella cartella A ha gli stessi diritti di accesso nella cartella B e la cartella C. La cartella B è la cartella figlia di A eredita i suoi ACL e la cartella C è la cartella figlia di B eredita i suoi ACL.

Analogamente, i gruppi di utenti (o utenti) che dispongono delle autorizzazioni per accedere solo alla cartella B hanno le stesse autorizzazioni di accesso nella cartella C ma non nella cartella A. È quindi consigliabile che le organizzazioni dispongano del contenuto in modo che le risorse più esposte siano posizionate nella cartella children e dagli elementi secondari all'accesso alla cartella principale.

### Public folder publish {#public-folder-publish}

A meno che non **venga selezionata** l'opzione Pubblica cartella pubblica durante la configurazione della replica di Brand Portal, gli utenti non amministratori (come Editor e Visualizzatori) non possono accedere alle risorse pubblicate da AEM Assets to Brand Portal.

![](assets/assetbpreplication.png)

Se l' **opzione Pubblica** cartella pubblica è disattivata, gli amministratori devono condividere esplicitamente tali risorse con gli utenti non amministratori che utilizzano la funzionalità di condivisione.

>[!NOTE]
>
>L'opzione per abilitare **Pubblica cartella pubblica** è disponibile a partire da AEM 6.3.2.1.

## Accesso alle cartelle condivise {#access-to-shared-folders}

La matrice seguente illustra i diritti di accesso e i diritti per condividere/annullare la condivisione delle risorse per vari ruoli utente:

|  | Accesso a tutte le cartelle pubblicate da AEM Assets a Brand Portal | Accesso alle cartelle condivise | Condivisione/annullamento della condivisione dei diritti delle cartelle |
|---------------|-----------|-----------|------------|
| Amministratore | Sì | Sì | Sì |
| Editor | No* | Sì, solo se condiviso con loro o con il gruppo a cui appartengono | Sì, solo per le cartelle condivise con loro o con il gruppo a cui appartengono |
| Visualizzatore | No* | Sì, solo se condiviso con loro o con il gruppo a cui appartengono | No |
| Utente ospite | No* | Sì, solo se condiviso con loro o con il gruppo a cui appartengono | No |

** Per impostazione predefinita, l'**opzione Pubblica**cartella pubblica è disattivata durante la configurazione della replica di Brand Portal con AEM Author. Se l'opzione è attivata, le cartelle pubblicate sul portale marchio saranno accessibili a tutti gli utenti (anche utenti non amministratori) per impostazione predefinita.*

### Accesso utente non amministratore alle cartelle condivise {#non-admin-user-access-to-shared-folders}

Gli utenti non amministratori possono accedere solo alle cartelle condivise con loro sul portale brand. Tuttavia, il modo in cui tali cartelle vengono visualizzate sul portale quando effettuano l'accesso dipende dalle impostazioni della configurazione Abilita gerarchia cartelle.

**Se la configurazione è disattivata**

Gli utenti non amministratori vedono tutte le cartelle condivise con loro sulla pagina di destinazione, accedendo al portale marchio.

![](assets/disabled-folder-hierarchy1-1.png)

**Se la configurazione è abilitata**

Gli utenti non amministratori visualizzano la struttura di cartelle (a partire dalla cartella principale) e le cartelle condivise disposte all'interno delle rispettive cartelle principali, accedendo al portale marchio.

Queste cartelle principali sono cartelle virtuali e non è possibile eseguire azioni su di esse. Potete riconoscere queste cartelle virtuali con un'icona a forma di lucchetto.

Non sono disponibili attività di azione al momento del passaggio del mouse o della selezione nella vista a schede, a differenza delle cartelle condivise. Il pulsante Panoramica viene visualizzato quando si seleziona una cartella virtuale nella vista a colonne e a elenco.

>[!NOTE]
>
>La miniatura predefinita delle cartelle virtuali è quella della prima cartella condivisa.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Condividere le cartelle {#how-to-share-folders}

Per condividere una cartella con gli utenti sul Portale brand, attenetevi alla procedura seguente:

1. Fate clic sull'icona della sovrapposizione a sinistra, quindi scegliete **Navigazione**.

   ![](assets/selectorrail.png)

2. Da Siderail a sinistra, selezionate **File**.

   ![](assets/access_files.png)

3. Dall'interfaccia Brand Portal, selezionate la cartella da condividere.

   ![](assets/share-folders.png)

4. Dalla barra degli strumenti nella parte superiore, selezionate **Condividi**.

   ![](assets/share_icon.png)

   Viene visualizzata **la console Proprietà** cartella.

   ![](assets/folder_properties.png)

5. Nella **console Proprietà** cartella, specificate il titolo della cartella **nel campo Titolo** cartella se non desiderate che venga visualizzato il nome predefinito.
6. Nell'elenco **Aggiungi utenti** , selezionate gli utenti o i gruppi ai quali desiderate condividere la cartella e fate clic **su Aggiungi**.
Per condividere la cartella solo con gli utenti ospiti e nessun altro utente, selezionate **Utenti** anonimi dal menu **a** discesa Membri.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Per rendere la cartella disponibile a tutti gli utenti indipendentemente dalla appartenenza al gruppo e dal ruolo, rendetela pubblica selezionando la **casella di** controllo Cartella pubblica.

7. Se necessario, fate clic su **Cambia miniatura** per modificare la miniatura della cartella.
8. Fai clic su **Salva**.
9. Per accedere alla cartella condivisa, accedete al portale marchio con le credenziali dell'utente con cui avete condiviso la cartella. Rivedete la cartella condivisa nell'interfaccia.

## Annullare la condivisione delle cartelle {#unshare-the-folders}

Per annullare la condivisione di una cartella condivisa precedentemente, effettuate le seguenti operazioni:

1. Dall'interfaccia Brand Portal selezionate la cartella da annullare.

   ![](assets/share-folders-1.png)

2. Dalla barra degli strumenti in alto, fate clic **su Condividi**.
3. Nella **console Proprietà** cartella, in **Membri**, fate clic sul simbolo **x** accanto a un utente per rimuoverli dall'elenco di utenti con cui avete condiviso la cartella.

   ![](assets/folder_propertiesunshare.png)

4. Nella finestra di messaggio di avviso, fate clic **su Conferma** per confermare l'annullamento della condivisione.
Fai clic su **Salva**.

5. Accedete al portale marchio con le credenziali dell'utente rimosso dall'elenco condiviso. La cartella non è più disponibile nell'interfaccia Brand Portal per l'utente.
