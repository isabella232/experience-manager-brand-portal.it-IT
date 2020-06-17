---
title: Crea cartella contributi
seo-title: Crea cartella contributi
description: 'Scopri come creare una cartella di contributi in AEM Assets. '
seo-description: Scopri come creare una cartella di contributi in AEM Assets.
uuid: null
content-type: reference
contentOwner: Vishabh Gupta
topic-tags: brand-portal
products: SG_EXPERIENCEMANAGER/Brand_Portal
discoiquuid: null
translation-type: tm+mt
source-git-commit: ac5952c318baae8400928592d9a372ab966191cf
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---


# Create contribution folder {#create-contribution-folder}

Gli amministratori di AEM e gli utenti non amministratori che dispongono dell’autorizzazione per creare una nuova cartella possono creare una cartella **Contribution** in AEM Assets.
Per creare una cartella **Contribution** , create una nuova cartella di tipo **Asset Contribution**, in modo che la nuova cartella creata sia aperta all’invio delle risorse da parte degli utenti del Brand Portal.  Questo attiva automaticamente un flusso di lavoro che crea due sottocartelle aggiuntive, denominate **SHARED** e **NEW**, all’interno della cartella **Contribution** appena creata.

**Per creare una nuova cartella di contributi:**
1. Accedi all’istanza di creazione AEMURL predefinito: http:// localhost:4502/aem/start.html
1. Passa a **[!UICONTROL Risorse > File]** Elenca tutte le cartelle esistenti nell&#39;archivio AEM Assets.
1. Click **[!UICONTROL Create]** to create a new folder. Viene aperta la finestra a comparsa Crea cartella.
1. Immettete **[!UICONTROL Titolo]** e **[!UICONTROL Nome]** della cartella e contrassegnate la casella di controllo Contributo ****risorsa.
Si consiglia di utilizzare alfabeti di piccole dimensioni senza spazio per denominare la cartella.
1. Fai clic su **[!UICONTROL Crea]**.
   ![](assets/create-contribution-folder.png)
1. Nella directory archivio dei AEM Assets è elencata la cartella dei contributi appena creata.
1. Fate clic per aprire la cartella dei contributi. Potete vedere due sottocartelle:**[!UICONTROL SHARED]** e **[!UICONTROL NEW]** vengono create automaticamente nella cartella dei contributi.\
   ![](assets/contribution-folder.png)

Ora puoi configurare le proprietà della cartella Contribution. Consultate [Configurare le proprietà](brand-portal-configure-contribution-folder-properties.md)della cartella Contribution.

>[!NOTE]
>
>Assicuratevi di fornire un nome appropriato alla cartella Contribution, poiché non potete modificare il nome della cartella dopo la creazione.
>
>La nidificazione della cartella Contribution non è supportata. Non create una cartella Contribution all’interno di un’altra cartella Contribution.

