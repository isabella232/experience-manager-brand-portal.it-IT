---
title: Condivisione di una raccolta
seo-title: Condivisione di una raccolta
description: Gli amministratori del Brand Portal di AEM Assets possono condividere e annullare la condivisione di una raccolta o di una raccolta dinamica con utenti autorizzati. Gli editor possono visualizzare e condividere solo le raccolte create da loro, condivise con loro e le raccolte pubbliche.
seo-description: Gli amministratori del Brand Portal di AEM Assets possono condividere e annullare la condivisione di una raccolta o di una raccolta dinamica con utenti autorizzati. Gli editor possono visualizzare e condividere solo le raccolte create da loro, condivise con loro e le raccolte pubbliche.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: riferimento
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Condividere le raccolte in Brand Portal {#share-collections-bp}

Gli amministratori del Brand Portal di AEM Assets possono condividere e annullare la condivisione di una raccolta o di una raccolta dinamica con utenti autorizzati. Gli editor possono visualizzare e condividere solo le raccolte create da loro, condivise con loro e le raccolte pubbliche. Tuttavia, gli editor non possono modificare una raccolta pubblica in una raccolta non pubblica.

>[!NOTE]
>
>Gli editor non possono modificare una raccolta pubblica in una raccolta non pubblica e, pertanto, non dispongono della casella di controllo Raccolta  pubblica disponibile nella finestra di dialogo Impostazioni  raccolta.

## Condivisione di una raccolta {#share-collection}

Per condividere una raccolta, effettuate le seguenti operazioni:

1. Fate clic sull'icona della sovrapposizione a sinistra, quindi scegliete **[!UICONTROL Navigazione]**.

   ![](assets/contenttree-1.png)

2. Dal lato laterale a sinistra, fate clic su **[!UICONTROL Raccolte]**.

   ![](assets/access_collections.png)

3. Dalla console **[!UICONTROL Raccolte]** , effettuate una delle seguenti operazioni:

   * Passate il puntatore del mouse sulla raccolta da condividere. Dalle miniature delle azioni rapide disponibili per la raccolta, fate clic sull'icona **[!UICONTROL Impostazioni]** .
   ![](assets/settings_thumbnail.png)

   * Selezionate la raccolta da condividere. Dalla barra degli strumenti nella parte superiore, fate clic su **[!UICONTROL Impostazioni]**.
   ![](assets/collection-sharing.png)

4. Nella finestra di dialogo Impostazioni  raccolta, selezionate gli utenti o i gruppi con i quali desiderate condividere la raccolta e selezionate il ruolo per un utente o un gruppo affinché corrisponda al ruolo globale. Ad esempio, assegnate il ruolo Editor a un editor globale, il ruolo Visualizzatore a un visualizzatore globale.

   In alternativa, per rendere la raccolta disponibile a tutti gli utenti a prescindere dall'appartenenza e dal ruolo del gruppo, rendetela pubblica selezionando la casella di controllo Raccolta **** pubblica.

   >[!NOTE]
   >
   >Tuttavia, agli utenti non amministratori può essere impedito di creare raccolte pubbliche, per evitare di avere numerose raccolte pubbliche in modo da poter risparmiare spazio sul sistema. Le organizzazioni possono disattivare la configurazione **[!UICONTROL Consenti creazione]** raccolte pubbliche dalle impostazioni [!UICONTROL Generali] disponibili nel pannello degli strumenti di amministrazione.

   ![](assets/collection_sharingadduser.png)

   Editors cannot change a public collection to a non-public collection and, therefore, do not have [!UICONTROL Public Collection] check-box available in [!UICONTROL Collection Settings] dialog.

   ![](assets/collection-setting-editor.png)

5. Selezionate **[!UICONTROL Aggiungi]**, quindi **[!UICONTROL Salva]**. La raccolta viene condivisa con gli utenti selezionati.

   >[!NOTE]
   >
   >Il ruolo di un utente regola l'accesso alle risorse e alle cartelle all'interno di una raccolta. Se un utente non ha accesso alle risorse, viene condivisa con l'utente una raccolta vuota. Inoltre, il ruolo di un utente regola le azioni disponibili per le raccolte.

## Annullamento della condivisione di una raccolta {#unshare-a-collection}

Per annullare la condivisione di una raccolta precedentemente condivisa, effettuate le seguenti operazioni:

1. Dalla console [!UICONTROL Raccolte] , selezionate la raccolta da annullare la condivisione.

   Nella barra degli strumenti, fate clic su **[!UICONTROL Impostazioni]**.

   ![](assets/collection_settings.png)

2. Nella finestra di dialogo Impostazioni  raccolta, in [!UICONTROL Membri], fate clic sul simbolo **[!UICONTROL x]** accanto a utenti o gruppi per rimuoverli dall'elenco di utenti con cui avete condiviso la raccolta.

   ![](assets/unshare_collection.png)

3. Nella finestra del messaggio di avviso, fare clic su **[!UICONTROL Conferma]** per confermare l'annullamento della condivisione.

   Fai clic su **[!UICONTROL Salva]**.

4. Accedete al Portale del marchio con le credenziali dell'utente rimosso dall'elenco condiviso. La raccolta viene rimossa dalla console **[!UICONTROL Raccolte]** .
