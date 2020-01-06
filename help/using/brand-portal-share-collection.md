---
title: Condividere una raccolta
seo-title: Condividere una raccolta
description: Gli amministratori del Brand Portal di AEM Assets possono condividere e annullare la condivisione di una raccolta o di una raccolta dinamica con utenti autorizzati. Gli editor possono visualizzare e condividere solo le raccolte create da loro, condivise con loro e le raccolte pubbliche.
seo-description: Gli amministratori del Brand Portal di AEM Assets possono condividere e annullare la condivisione di una raccolta o di una raccolta dinamica con utenti autorizzati. Gli editor possono visualizzare e condividere solo le raccolte create da loro, condivise con loro e le raccolte pubbliche.
uuid: 965f39cd-1378-42c1-a58a-01e1bf825aa3
contentOwner: bdhar
content-type: reference
topic-tags: sharing
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: f053013e-5981-419f-927e-b5bb1d47eae2
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873

---


# Condividere le raccolte in Brand Portal {#share-collections-bp}

Gli amministratori del Brand Portal di AEM Assets possono condividere e annullare la condivisione di una raccolta o di una raccolta dinamica con utenti autorizzati. Gli editor possono visualizzare e condividere solo le raccolte create da loro, condivise con loro e le raccolte pubbliche. Tuttavia, gli editor non possono modificare una raccolta pubblica in una raccolta non pubblica.

>[!NOTE]
>
>Gli editor non possono modificare una raccolta pubblica in una raccolta non pubblica e, pertanto, non dispongono della casella di controllo Raccolta ****pubblica disponibile nella finestra di dialogo Impostazioni**** raccolta.

## Condividere una raccolta {#share-collection}

Per condividere una raccolta, effettuate le seguenti operazioni:

1. Fate clic sull&#39;icona della sovrapposizione a sinistra, quindi scegliete **[!UICONTROL Navigazione]**.

   ![](assets/contenttree-1.png)

1. Dal lato laterale a sinistra, fate clic su **[!UICONTROL Raccolte]**.

   ![](assets/access_collections.png)

1. Dalla console **[!UICONTROL Raccolte]**, effettuate una delle seguenti operazioni:

   * Passate il puntatore del mouse sulla raccolta da condividere. Dalle miniature delle azioni rapide disponibili per la raccolta, fate clic sull&#39;icona **[!UICONTROL Impostazioni]**.
   ![](assets/settings_thumbnail.png)

   * Selezionate la raccolta da condividere. Dalla barra degli strumenti nella parte superiore, fate clic su **[!UICONTROL Impostazioni]**.
   ![](assets/collection-sharing.png)

1. Nella finestra di dialogo Impostazioni  raccolta, selezionate gli utenti o i gruppi con i quali desiderate condividere la raccolta e selezionate il ruolo per un utente o un gruppo affinché corrisponda al ruolo globale. Ad esempio, assegnate il ruolo Editor a un editor globale, il ruolo Visualizzatore a un visualizzatore globale.

   In alternativa, per rendere la raccolta disponibile a tutti gli utenti a prescindere dall&#39;appartenenza e dal ruolo del gruppo, rendetela pubblica selezionando la casella di controllo Raccolta ****pubblica.

   >[!NOTE]
   >
   >Tuttavia, agli utenti non amministratori può essere impedito di creare raccolte pubbliche, per evitare di avere numerose raccolte pubbliche in modo da poter risparmiare spazio sul sistema. Le organizzazioni possono disattivare la configurazione **[!UICONTROL Consenti creazione]**raccolte pubbliche dalle impostazioni[!UICONTROL Generali]disponibili nel pannello degli strumenti di amministrazione.

   ![](assets/collection_sharingadduser.png)

   Gli editor non possono modificare una raccolta pubblica in una raccolta non pubblica e, pertanto, non dispongono della casella di controllo Raccolta ****pubblica disponibile nella finestra di dialogo Impostazioni**** raccolta.

   ![](assets/collection-setting-editor.png)

1. Selezionate **[!UICONTROL Aggiungi]**, quindi**[!UICONTROL  Salva]**. La raccolta viene condivisa con gli utenti selezionati.

   >[!NOTE]
   >
   >Il ruolo di un utente regola l&#39;accesso alle risorse e alle cartelle all&#39;interno di una raccolta. Se un utente non ha accesso alle risorse, viene condivisa con l&#39;utente una raccolta vuota. Inoltre, il ruolo di un utente regola le azioni disponibili per le raccolte.

## Annullamento della condivisione di una raccolta {#unshare-a-collection}

Per annullare la condivisione di una raccolta precedentemente condivisa, effettuate le seguenti operazioni:

1. Dalla console **[!UICONTROL Raccolte]**, selezionate la raccolta da annullare la condivisione.

   In the toolbar, click **[!UICONTROL Settings]**.

   ![](assets/collection_settings.png)

1. Nella finestra di dialogo Impostazioni ****raccolta, in**[!UICONTROL  Membri]**, fate clic sul simbolo **[!UICONTROL x]**accanto a utenti o gruppi per rimuoverli dall&#39;elenco di utenti con cui avete condiviso la raccolta.

   ![](assets/unshare_collection.png)

1. Nella finestra del messaggio di avviso, fare clic su **[!UICONTROL Conferma]**per confermare l&#39;annullamento della condivisione.

   Fai clic su **[!UICONTROL Salva]**.

1. Accedete al Portale del marchio con le credenziali dell&#39;utente rimosso dall&#39;elenco condiviso. La raccolta viene rimossa dalla console **[!UICONTROL Raccolte]**.
