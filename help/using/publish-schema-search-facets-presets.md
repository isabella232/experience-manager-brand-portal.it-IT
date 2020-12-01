---
title: Pubblicare predefiniti, schemi e facet in Brand Portal
seo-title: Pubblicare predefiniti, schemi e facet in Brand Portal
description: Scoprite come pubblicare predefiniti, schemi e facet in Brand Portal.
seo-description: Scoprite come pubblicare predefiniti, schemi e facet in Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
translation-type: tm+mt
source-git-commit: 86078dd07b5d487f8cf5cd08bc46e4745529c873
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 3%

---


# Pubblicare predefiniti, schemi e facet in Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

L&#39;articolo descrive come pubblicare i predefiniti per immagini, gli schemi di metadati e i facet di ricerca personalizzati dall&#39;istanza di AEM Author al Brand Portal. La funzione di pubblicazione consente alle organizzazioni di riutilizzare i predefiniti per immagini, gli schemi di metadati e i facet di ricerca creati/modificati nell’istanza di AEM Author, riducendo in tal modo il rischio di duplicazione.

>[!NOTE]
>
>La possibilità di pubblicare i predefiniti per immagini, lo schema di metadati e i facet di ricerca dall’istanza di AEM Author al Portale del marchio è disponibile AEM 6.2 SP1-CFP7 e AEM 6.3 SP 1-CFP 1 (6.3.1.1) in avanti.

## Pubblicare i predefiniti per immagini su Brand Portal {#publish-image-presets-to-brand-portal}

I predefiniti per immagini sono una serie di comandi di ridimensionamento e formattazione applicati all’immagine al momento della distribuzione. I predefiniti per immagini possono essere creati e modificati in Brand Portal. In alternativa, se l&#39;istanza di AEM Author è in esecuzione in modalità per contenuti multimediali dinamici, gli utenti possono creare dei predefiniti in AEM Author e pubblicarli  Portale del marchio AEM Assets ed evitare di ricreare gli stessi predefiniti in Brand Portal.\
Una volta creato, il predefinito viene elencato come rappresentazione dinamica nella barra delle rappresentazioni dei dettagli delle risorse e nella finestra di dialogo di download.

>[!NOTE]
>
>Se l&#39;istanza di AEM Author non è in esecuzione in **[!UICONTROL Modalità elemento multimediale dinamico]** (il cliente non ha acquistato elementi multimediali dinamici), la rappresentazione **[!UICONTROL TIFF piramidale]** delle risorse non viene creata al momento del caricamento. I predefiniti per immagini o le rappresentazioni dinamiche funzionano su **[!UICONTROL TIFF piramidale]** di una risorsa, pertanto se **[!UICONTROL TIFF piramidale]** non è disponibile nell’istanza di AEM Author, non è disponibile anche sul Portale marchio. Di conseguenza, nella barra delle rappresentazioni della pagina dei dettagli della risorsa e nella finestra di dialogo di download non sono presenti rappresentazioni dinamiche.

Per pubblicare i predefiniti per immagini in Brand Portal:

1. Nell&#39;istanza di AEM Author, toccate o fate clic sul logo AEM per accedere alla console di navigazione globale, quindi toccate o fate clic sull&#39;icona Strumenti e andate a **[!UICONTROL Risorse > Predefiniti immagine]**.
1. Selezionate il predefinito per immagini o più predefiniti per immagini dall’elenco dei predefiniti per immagini e toccate **[!UICONTROL Pubblica su Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]**, i predefiniti per immagini vengono messi in coda per la pubblicazione. Agli utenti viene consigliato di monitorare il registro degli agenti di replica per confermare l’esito della pubblicazione.

Per annullare la pubblicazione di un predefinito per immagini da Brand Portal:

1. Nell&#39;istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull&#39;icona **[!UICONTROL Strumenti]** e passa a **[!UICONTROL Risorse > Predefiniti immagine]**.
1. Selezionate un predefinito per immagini e selezionate **[!UICONTROL Rimuovi da Brand Portal]** tra le opzioni disponibili nella parte superiore.

## Pubblicare lo schema di metadati su Brand Portal {#publish-metadata-schema-to-brand-portal}

Lo schema metadati descrive il layout e le proprietà visualizzati nella pagina delle proprietà delle risorse/raccolte.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se gli utenti hanno modificato lo schema predefinito nell&#39;istanza di AEM Author e sono disposti a utilizzare lo stesso schema dello schema predefinito nel Portale marchio, possono semplicemente pubblicare i moduli dello schema di metadati in Brand Portal. In questo caso, lo schema predefinito in Brand Portal viene sostituito dagli schemi predefiniti pubblicati dall&#39;istanza di AEM Author.

Se gli utenti hanno creato uno schema personalizzato sull&#39;istanza di AEM Author, possono pubblicare lo schema personalizzato su Brand Portal invece di ricreare lo stesso schema personalizzato. Gli utenti possono quindi applicare questo schema personalizzato a qualsiasi cartella/raccolta in Brand Portal.

>[!NOTE]
>
>Gli schemi predefiniti non possono essere pubblicati sul Portale marchio se sono bloccati nell’istanza AEM (ovvero se non sono stati modificati).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se a una cartella è applicato uno schema sull’istanza di AEM Author, lo stesso schema deve esistere anche nel Portale marchio per mantenere la coerenza nella pagina delle proprietà delle risorse su AEM Author e Brand Portal.

Per pubblicare uno schema di metadati dall’istanza di AEM Author al Brand Portal:

1. Nell&#39;istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull&#39;icona Strumenti e passa a **[!UICONTROL Risorse > Schemi di metadati]**.
1. Selezionate uno schema di metadati, quindi selezionate **[!UICONTROL Pubblica su Brand Portal]** tra le opzioni disponibili nella parte superiore.

>[!NOTE]
>
>Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]**, gli schemi di metadati vengono messi in coda per la pubblicazione. Agli utenti viene consigliato di monitorare il registro degli agenti di replica per confermare l’esito della pubblicazione.

Per annullare la pubblicazione di uno schema di metadati da Brand Portal:

1. Nell&#39;istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull&#39;icona Strumenti e passa a **[!UICONTROL Risorse > Schemi di metadati]**.
1. Selezionate uno schema di metadati, quindi selezionate **[!UICONTROL Rimuovi da Brand Portal]** dalle opzioni disponibili nella parte superiore.

## Pubblicare i facet di ricerca nel Portale marchio {#publish-search-facets-to-brand-portal}

I moduli di ricerca forniscono agli utenti la funzionalità di [ricerca sfaccettata](../using/brand-portal-search-facets.md) su Brand Portal. I facet di ricerca conferiscono maggiore granularità alle ricerche sul Portale marchio. Tutti i [predicati aggiunti](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) nel modulo di ricerca sono disponibili per gli utenti come facet di ricerca nei filtri di ricerca.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se sei disposto a utilizzare un modulo di ricerca personalizzato **[!UICONTROL Barra di ricerca Amministratore risorse]** dall&#39;istanza di AEM Author, invece di ricreare lo stesso modulo su Brand Portal puoi pubblicare il modulo di ricerca personalizzato dall&#39;istanza di AEM Author al Brand Portal.

>[!NOTE]
>
>Il modulo di ricerca bloccato **[!UICONTROL Risorse Admin Search Rail]** su  AEM Assets non può essere pubblicato su Brand Portal a meno che non venga modificato. Una volta modificato e pubblicato in Brand Portal, questo modulo di ricerca sostituisce il modulo di ricerca sul Brand Portal.

Per pubblicare il facet di ricerca modificato dall’istanza di AEM Author al Brand Portal:

1. Tocca/fai clic sul logo AEM, quindi vai a **[!UICONTROL Strumenti > Generale > Moduli di ricerca]**.
1. Selezionate il modulo di ricerca modificato e selezionate **[!UICONTROL Pubblica su Brand Portal]**.

   >[!NOTE]
   >
   >Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]**, i facet di ricerca vengono messi in coda per la pubblicazione. Agli utenti viene consigliato di monitorare il registro degli agenti di replica per confermare l’esito della pubblicazione.

Per annullare la pubblicazione dei moduli di ricerca da Brand Portal:

1. Nell&#39;istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull&#39;icona Strumenti e passa a **[!UICONTROL Generale > Cerca Forms]**.
1. Selezionate il modulo di ricerca e selezionate **[!UICONTROL Rimuovi da Brand Portal]** tra le opzioni disponibili nella parte superiore.

>[!NOTE]
>
>L&#39;azione **[!UICONTROL Annulla pubblicazione da Brand Portal]** lascia il modulo di ricerca predefinito su Brand Portal e non ripristina l&#39;ultimo modulo di ricerca utilizzato prima della pubblicazione.

### Limitazioni  {#limitations}

1. Pochi predicati di ricerca non sono applicabili ai filtri di ricerca nel Brand Portal. Quando questi predicati di ricerca vengono pubblicati come parte del modulo di ricerca dall&#39;istanza di AEM Author al Portale del marchio, vengono esclusi. Di conseguenza, gli utenti possono vedere un numero minore di predicati nel modulo pubblicato sul Brand Portal. Consultate i predicati di ricerca [applicabili ai filtri nel portale marchio](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Per [!UICONTROL Options Predicate], se un utente utilizza un percorso personalizzato per le opzioni di lettura nell&#39;istanza di AEM Author, non funzionerà nel Brand Portal. Tali percorsi e opzioni aggiuntivi non vengono pubblicati in Brand Portal con il modulo di ricerca. In questo caso, gli utenti possono selezionare l&#39;opzione **[!UICONTROL Manuale]** in **[!UICONTROL Aggiungi opzioni]** all&#39;interno di **[!UICONTROL Predicato opzioni]** per aggiungere manualmente queste opzioni in Brand Portal.

![](assets/options-predicate-manual.png)
