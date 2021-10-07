---
title: Pubblicare predefiniti, schemi e facet in Brand Portal
seo-title: Publish presets, schema, and facets to Brand Portal
description: Scopri come pubblicare predefiniti, schemi e facet in Brand Portal.
seo-description: Learn how to publish presets, schema, and facets to Brand Portal.
uuid: c836d9bb-074a-4113-9c91-b2bf7658b88d
topic-tags: publish
products: SG_EXPERIENCEMANAGER/Brand_Portal
content-type: reference
discoiquuid: bc305abc-9373-4d33-9179-0a5f3904b352
exl-id: 9b585606-6538-459b-87a9-2e68df0087b3
source-git-commit: 4caa4263bd74b51af7504295161c421524e51f0c
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 2%

---

# Pubblicare predefiniti, schemi e facet in Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

L’articolo descrive come pubblicare predefiniti immagine, schemi di metadati e facet di ricerca personalizzati dall’istanza di AEM Author a Brand Portal. La funzionalità di pubblicazione consente alle organizzazioni di riutilizzare i predefiniti immagine, gli schemi di metadati e i facet di ricerca creati/modificati nell’istanza di AEM Author, riducendo in tal modo gli sforzi duplicati.

>[!NOTE]
>
>La capacità di pubblicare predefiniti immagine, schema metadati e facet di ricerca dall’istanza di AEM Author a Brand Portal è disponibile AEM 6.2 SP1-CFP7 e AEM 6.3 SP 1-CFP 1 (6.3.1.1) in avanti.

## Pubblicare predefiniti immagine in Brand Portal {#publish-image-presets-to-brand-portal}

I predefiniti immagine sono un set di comandi di ridimensionamento e formattazione applicati all’immagine al momento della distribuzione dell’immagine. I predefiniti immagine possono essere creati e modificati in Brand Portal. In alternativa, se l’istanza di AEM Author è in esecuzione in modalità Dynamic Media, gli utenti possono creare dei predefiniti in AEM Author e pubblicarli in AEM Assets Brand Portal, evitando di ricreare gli stessi predefiniti in Brand Portal.\
Una volta creato, il predefinito viene elencato come rendering dinamico nella barra delle rappresentazioni dei dettagli delle risorse e nella finestra di dialogo di download.

>[!NOTE]
>
>Se l&#39;istanza di authoring di AEM non è in esecuzione in **[!UICONTROL Modalità Dynamic Media]** (il cliente non ha acquistato Dynamic Media), il rendering **[!UICONTROL TIFF piramidale]** delle risorse non viene creato al momento del caricamento. I predefiniti immagine o le rappresentazioni dinamiche funzionano su **[!UICONTROL TIFF piramidale]** di una risorsa, quindi se **[!UICONTROL TIFF piramidale]** non è disponibile sull’istanza di AEM Author, non è disponibile anche su Brand Portal. Di conseguenza, nella barra delle rappresentazioni della pagina dei dettagli delle risorse e della finestra di dialogo di download non sono presenti rappresentazioni dinamiche.

Per pubblicare i predefiniti immagine in Brand Portal:

1. Nell’istanza di authoring di AEM, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e passa a **[!UICONTROL Risorse > Predefiniti immagini]**.
1. Seleziona il predefinito per immagini o più predefiniti immagine dall’elenco dei predefiniti per immagini e tocca o fai clic su **[!UICONTROL Pubblica in Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]** i predefiniti per immagini vengono messi in coda per la pubblicazione. Consigliamo agli utenti di monitorare il registro degli agenti di replica per confermare se la pubblicazione è riuscita.

Per annullare la pubblicazione di un predefinito immagine da Brand Portal:

1. Nell’istanza di authoring di AEM, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona **[!UICONTROL Strumenti]** e passa a **[!UICONTROL Risorse > Predefiniti immagini]**.
1. Seleziona un predefinito per immagini e seleziona **[!UICONTROL Rimuovi da Brand Portal]** dalle opzioni disponibili nella parte superiore.

## Pubblicare lo schema metadati su Brand Portal  {#publish-metadata-schema-to-brand-portal}

Lo schema metadati descrive il layout e le proprietà visualizzate nella pagina delle proprietà delle risorse o delle raccolte.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se gli utenti hanno modificato lo schema predefinito nell’istanza di AEM Author e desiderano utilizzare lo stesso schema dello schema predefinito in Brand Portal, possono semplicemente pubblicare i moduli dello schema metadati in Brand Portal. In questo caso, lo schema predefinito di Brand Portal è sostituito dagli schemi predefiniti pubblicati dall’istanza di AEM Author.

Se gli utenti hanno creato uno schema personalizzato sull’istanza di AEM Author, possono pubblicare lo schema personalizzato in Brand Portal anziché ricrearvi lo stesso schema personalizzato. Gli utenti possono quindi applicare questo schema personalizzato a qualsiasi cartella/raccolta in Brand Portal.

>[!NOTE]
>
>Gli schemi predefiniti non possono essere pubblicati in Brand Portal se sono bloccati nell’istanza AEM (ovvero non sono stati modificati).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se una cartella ha uno schema applicato all’istanza di AEM Author, lo stesso schema deve esistere anche in Brand Portal per mantenere la coerenza nella pagina delle proprietà della risorsa in AEM Author e Brand Portal.

Per pubblicare uno schema di metadati dall’istanza di AEM Author a Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e passa a **[!UICONTROL Risorse > Schemi di metadati]**.
1. Seleziona uno schema di metadati e seleziona **[!UICONTROL Pubblica in Brand Portal]** dalle opzioni disponibili nella parte superiore.

>[!NOTE]
>
>Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]**, gli schemi di metadati vengono messi in coda per la pubblicazione. Consigliamo agli utenti di monitorare il registro degli agenti di replica per confermare se la pubblicazione è riuscita.

Per annullare la pubblicazione di uno schema di metadati da Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e passa a **[!UICONTROL Risorse > Schemi di metadati]**.
1. Seleziona uno schema di metadati e seleziona **[!UICONTROL Rimuovi da Brand Portal]** dalle opzioni disponibili nella parte superiore.

## Pubblicare i facet di ricerca in Brand Portal {#publish-search-facets-to-brand-portal}

I moduli di ricerca forniscono agli utenti su Brand Portal la funzionalità di ricerca sfaccettata [a1/>. ](../using/brand-portal-search-facets.md) I facet di ricerca conferiscono maggiore granularità alle ricerche in Brand Portal. Tutti i predicati [aggiunti](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) nel modulo di ricerca sono disponibili agli utenti come facet di ricerca nei filtri di ricerca.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se sei disposto a utilizzare un modulo di ricerca personalizzato **[!UICONTROL Barra di ricerca amministrazione risorse]** dall’istanza di AEM Author, invece di ricreare lo stesso modulo su Brand Portal puoi pubblicare il modulo di ricerca personalizzato dall’istanza di AEM Author a Brand Portal.

>[!NOTE]
>
>Il modulo di ricerca bloccato **[!UICONTROL Barra di ricerca amministrazione risorse]** su AEM Assets non può essere pubblicato in Brand Portal a meno che non venga modificato. Una volta modificato e pubblicato in Brand Portal, questo modulo di ricerca sostituisce il modulo di ricerca in Brand Portal.

Per pubblicare il facet di ricerca modificato dall’istanza di AEM Author in Brand Portal:

1. Tocca/fai clic sul logo AEM, quindi vai a **[!UICONTROL Strumenti > Generale > Moduli di ricerca]**.
1. Selezionare il modulo di ricerca modificato e selezionare **[!UICONTROL Pubblica in Brand Portal]**.

   >[!NOTE]
   >
   >Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]**, i facet di ricerca vengono messi in coda per la pubblicazione. Consigliamo agli utenti di monitorare il registro degli agenti di replica per confermare se la pubblicazione è riuscita.

Per annullare la pubblicazione dei moduli di ricerca da Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e passa a **[!UICONTROL Generale > Cerca Forms]**.
1. Selezionare il modulo di ricerca e selezionare **[!UICONTROL Rimuovi da Brand Portal]** tra le opzioni disponibili nella parte superiore.

>[!NOTE]
>
>L&#39;azione **[!UICONTROL Annulla pubblicazione da Brand Portal]** lascia il modulo di ricerca predefinito su Brand Portal e non viene ripristinato all&#39;ultimo modulo di ricerca utilizzato prima della pubblicazione.

### Limitazioni  {#limitations}

1. Pochi predicati di ricerca non sono applicabili ai filtri di ricerca su Brand Portal. Quando questi predicati di ricerca vengono pubblicati come parte del modulo di ricerca dall’istanza di AEM Author a Brand Portal, vengono filtrati. Gli utenti, quindi, visualizzano un minor numero di predicati nel modulo pubblicato in Brand Portal. Consulta [predicati di ricerca applicabili ai filtri su Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Per [!UICONTROL Predicato opzioni], se un utente utilizza un percorso personalizzato per leggere le opzioni nell&#39;istanza di AEM Author, non funzionerà in Brand Portal. Questi percorsi e opzioni aggiuntivi non vengono pubblicati in Brand Portal con il modulo di ricerca. In questo caso, gli utenti possono selezionare l&#39;opzione **[!UICONTROL Manuale]** in **[!UICONTROL Aggiungi opzioni]** in **[!UICONTROL Predicato opzioni]** per aggiungere manualmente queste opzioni in Brand Portal.

![](assets/options-predicate-manual.png)
