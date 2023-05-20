---
title: Condividere le cartelle
seo-title: Share folders
description: Brand Portal non supporta l’acquisizione delle risorse, pertanto le risorse devono essere pubblicate in Brand Portal da un’istanza Experience Manager Assets Author preconfigurata. Le risorse pubblicate non sono accessibili agli utenti non amministratori di Brand Portal, a meno che non siano configurate durante la configurazione della replica con l’istanza Experience Manager e debbano essere condivise con loro.
seo-description: Brand Portal does not support asset ingestion so assets must be published to Brand Portal from a pre-configured Experience Manager Assets Author instance. Published assets are not accessible to non-admin users of Brand Portal, unless configured while configuring replication with Experience Manager instance, and need to be shared with them.
uuid: 340d0a49-b708-4f0e-9fb8-99c824942f34
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: 2332c16f-40be-4673-8cc6-2360d5b74116
exl-id: d28cf927-60e8-437e-9cba-92f7e19020e7
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 2%

---

# Condividere cartelle su Brand Portal {#share-folders}

È necessario pubblicare le risorse in Brand Portal da un’istanza Experience Manager Author preconfigurata, in quanto Brand Portal non supporta l’inserimento delle risorse.

## Flusso di lavoro di condivisione cartelle in Brand Portal {#folder-sharing-workflow-in-brand-portal}

Di seguito sono descritti il flusso di lavoro di condivisione cartelle e l&#39;accesso utente:

* Per impostazione predefinita, tutte le cartelle pubblicate da Experience Manager Assets a Brand Portal sono visibili solo all’amministratore di Brand Portal, a meno che non siano contrassegnate come pubbliche durante la configurazione della replica.
* L’amministratore utilizza **[!UICONTROL Proprietà cartella]** per condividere una cartella con utenti o gruppi selettivi. Solo gli utenti o i gruppi con cui è condivisa la cartella potranno visualizzarla dopo l&#39;accesso a Brand Portal. La cartella non è visibile ad altri utenti.
* L’amministratore può anche scegliere di rendere pubblica una cartella tramite il **[!UICONTROL Cartella pubblica]** casella di controllo in **[!UICONTROL Proprietà cartella]** console. Una cartella pubblica è visibile a tutti gli utenti.

* Indipendentemente dai ruoli utente e dai privilegi, quando gli utenti accedono a Brand Portal, visualizzano tutte le cartelle pubbliche e le cartelle condivise direttamente con loro o con un gruppo a cui appartengono. Le cartelle private o condivise con altri utenti non sono visibili a tutti gli utenti.

### Condividere cartelle con gruppi di utenti su Brand Portal {#sharing-folders-with-user-groups-on-brand-portal}

I diritti di accesso alle risorse di una cartella dipendono dai diritti di accesso della relativa cartella principale, indipendentemente dalle impostazioni delle cartelle secondarie. Questo comportamento è gestito da [ACL](https://experienceleague.adobe.com/docs/experience-manager-65/administering/security/security.html?lang=it) in AEM, poiché le cartelle secondarie ereditano gli ACL dalle cartelle principali. Ad esempio, se una cartella A contiene la cartella B che contiene la cartella C, anche un gruppo di utenti (o utenti) con diritti di accesso alla cartella A dispone degli stessi diritti di accesso per la cartella B e la cartella C. La cartella B, che è la cartella secondaria di A, eredita i propri ACL, mentre la cartella C, che è la cartella secondaria di B, ne eredita gli ACL.

Analogamente, i gruppi di utenti (o gli utenti) che dispongono delle autorizzazioni per accedere solo alla cartella B dispongono delle stesse autorizzazioni di accesso per la cartella C ma non per la cartella A. È consigliabile, pertanto, che le organizzazioni dispongano i propri contenuti in modo che la maggior parte delle risorse esposte vengano posizionate nella cartella secondaria e che l’accesso dalle cartelle secondarie a quelle principali possa essere limitato.

### Pubblicazione cartella pubblica {#public-folder-publish}

A meno che **[!UICONTROL Pubblicazione cartella pubblica]** L’opzione è selezionata durante la configurazione della replica di Brand Portal e gli utenti non amministratori (come Editor e Visualizzatori) non hanno accesso alle risorse pubblicate da AEM Assets a Brand Portal.

![](assets/assetbpreplication.png)

Se il **[!UICONTROL Pubblicazione cartella pubblica]** se l’opzione è disattivata, gli amministratori devono condividere queste risorse con utenti non amministratori utilizzando la funzionalità di condivisione.

>[!NOTE]
>
>L’opzione per abilitare **[!UICONTROL Pubblicazione cartella pubblica]** è disponibile in AEM 6.3.2.1 e versioni successive.

## Accesso alle cartelle condivise {#access-to-shared-folders}

La matrice seguente illustra i diritti di accesso e i diritti di condivisione/annullamento della condivisione delle risorse per vari ruoli utente:

|  | Accesso a tutte le cartelle pubblicate da AEM Assets a Brand Portal | Accesso alle cartelle condivise | Condividere/annullare la condivisione dei diritti delle cartelle |
|---------------|-----------|-----------|------------|
| Amministratore | Sì | Sì | Sì |
| Editor | No* | Sì, solo se condiviso con loro o con il gruppo a cui appartengono | Sì, solo per le cartelle condivise con loro o con il gruppo a cui appartengono |
| Visualizzatore | No* | Sì, solo se condiviso con loro o con il gruppo a cui appartengono | No |
| Utente ospite | No* | Sì, solo se condiviso con loro o con il gruppo a cui appartengono | No |

>[!NOTE]
>
>Per impostazione predefinita, il **[!UICONTROL Pubblicazione cartella pubblica]** L’opzione è disabilitata durante la configurazione della replica di Brand Portal con AEM Author. Se l’opzione è abilitata, le cartelle pubblicate in Brand Portal saranno accessibili a tutti gli utenti (anche a quelli non amministratori) per impostazione predefinita.

### Accesso degli utenti non amministratori alle cartelle condivise {#non-admin-user-access-to-shared-folders}

Gli utenti non amministratori possono accedere solo alle cartelle condivise con loro su Brand Portal. Tuttavia, la modalità di visualizzazione di queste cartelle nel portale all&#39;accesso dipende dalle impostazioni di **[!UICONTROL Abilita gerarchia cartelle]** configurazione.

**Se la configurazione è disabilitata**

Gli utenti non amministratori visualizzano tutte le cartelle condivise con loro nella pagina di destinazione al momento dell’accesso a Brand Portal.

![](assets/disabled-folder-hierarchy1-1.png)

**Se la configurazione è abilitata**

Al momento dell’accesso a Brand Portal, gli utenti non amministratori visualizzano la struttura delle cartelle (a partire dalla cartella principale) e le cartelle condivise organizzate all’interno delle rispettive cartelle principali.

Queste cartelle principali sono le cartelle virtuali e non è possibile eseguire alcuna azione su di esse. È possibile riconoscere queste cartelle virtuali con un&#39;icona di blocco.

Nessuna attività di azione visibile al passaggio del mouse o selezionando le attività **[!UICONTROL Vista a schede]**, a differenza delle cartelle condivise. **[!UICONTROL Panoramica]** quando si seleziona una cartella virtuale in **[!UICONTROL Vista a colonne]** e **[!UICONTROL Vista a elenco]**.

>[!NOTE]
>
>La miniatura predefinita delle cartelle virtuali è l&#39;immagine miniatura della prima cartella condivisa.

![](assets/enabled-hierarchy1-1.png) ![](assets/hierarchy1-nonadmin-1.png) ![](assets/hierarchy-nonadmin-1.png) ![](assets/hierarchy2-nonadmin-1.png)

## Condividere le cartelle {#how-to-share-folders}

Per condividere una cartella con gli utenti su Brand Portal, effettua le seguenti operazioni:

1. Fai clic sull’icona della sovrapposizione a sinistra, quindi scegli **[!UICONTROL Navigazione]**.

   ![](assets/selectorrail.png)

1. Dal siderale a sinistra, seleziona **[!UICONTROL File]**.

   ![](assets/access_files.png)

1. Dall’interfaccia di Brand Portal, seleziona la cartella da condividere.

   ![](assets/share-folders.png)

1. Dalla barra degli strumenti nella parte superiore, seleziona **[!UICONTROL Condividi]**.

   ![](assets/share_icon.png)

   Il [!UICONTROL Proprietà cartella] viene visualizzata la console.

   ![](assets/folder_properties.png)

1. In **[!UICONTROL Proprietà cartella]** , specifica il titolo della cartella nel **[!UICONTROL Titolo cartella]** se non si desidera che il nome predefinito venga visualizzato agli utenti.
1. Dalla sezione **[!UICONTROL Aggiungi utente]** selezionare gli utenti o i gruppi con cui si desidera condividere la cartella e fare clic su **[!UICONTROL Aggiungi]**.
Per condividere la cartella solo con utenti guest e nessun altro utente, selezionare **[!UICONTROL Utenti anonimi]** dal **[!UICONTROL Membri]** a discesa.

   ![](assets/only-anonymous.png)

   >[!NOTE]
   >
   >Per rendere la cartella disponibile a tutti gli utenti, indipendentemente dall’appartenenza al gruppo e dal ruolo, rendila pubblica selezionando la **[!UICONTROL Cartella pubblica]** casella di controllo.

1. Se necessario, fai clic su **[!UICONTROL Cambia miniatura]** per modificare l&#39;immagine miniatura per la cartella.
1. Fai clic su **[!UICONTROL Salva]**.

1. Per accedere alla cartella condivisa, accedi a Brand Portal con le credenziali dell’utente con cui hai condiviso la cartella. Controlla la cartella condivisa nell’interfaccia.

## Annullare la condivisione delle cartelle {#unshare-the-folders}

Per annullare la condivisione di una cartella condivisa in precedenza, effettua le seguenti operazioni:

1. Dall’interfaccia di Brand Portal, seleziona la cartella di cui vuoi annullare la condivisione.

   ![](assets/share-folders-1.png)

1. Dalla barra degli strumenti nella parte superiore, fai clic su **[!UICONTROL Condividi]**.
1. In **[!UICONTROL Proprietà cartella]** console, sotto **[!UICONTROL Membri]**, fare clic su **[!UICONTROL x]** accanto a un utente per rimuoverli dall’elenco degli utenti con cui hai condiviso la cartella.

   ![](assets/folder_propertiesunshare.png)

1. Nella finestra di messaggio di avviso, fare clic su **[!UICONTROL Conferma]** per confermare l’annullamento della condivisione.
Fai clic su **[!UICONTROL Salva]**.

1. Accedi a Brand Portal con le credenziali dell’utente rimosso dall’elenco condiviso. La cartella non è più disponibile per l’utente nell’interfaccia di Brand Portal.
