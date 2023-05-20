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

L’articolo approfondisce la pubblicazione di predefiniti immagine, schemi di metadati e facet di ricerca personalizzati dall’istanza Autore AEM a Brand Portal. La funzionalità di pubblicazione consente alle organizzazioni di riutilizzare i predefiniti immagine, gli schemi di metadati e i facet di ricerca creati/modificati nell’istanza di AEM Author, riducendo in tal modo le attività di duplicazione.

>[!NOTE]
>
>La funzionalità per pubblicare i predefiniti immagine, lo schema metadati e i facet di ricerca dall’istanza di AEM Author a Brand Portal è disponibile da AEM 6.2 SP1-CFP7 e AEM 6.3 SP 1-CFP 1 (6.3.1.1) in poi.

## Pubblicare predefiniti immagine in Brand Portal {#publish-image-presets-to-brand-portal}

I predefiniti per immagini sono un set di comandi di ridimensionamento e formattazione applicati all’immagine al momento della consegna. I predefiniti per immagini possono essere creati e modificati in Brand Portal. In alternativa, se l’istanza di AEM Author è in esecuzione in modalità Dynamic Media, gli utenti possono creare i predefiniti in AEM Author e pubblicarli in AEM Assets Brand Portal, evitando di ricrearli in Brand Portal.\
Una volta creato, il predefinito viene elencato come rappresentazione dinamica nella barra delle rappresentazioni dei dettagli delle risorse e nella finestra di dialogo per il download.

>[!NOTE]
>
>Se l’istanza di AEM Author non è in esecuzione in **[!UICONTROL Modalità Dynamic Media]** (il cliente non ha acquistato Dynamic Media), il **[!UICONTROL Pyramid TIFF]**  la rappresentazione delle risorse non viene creata al momento del caricamento. Predefiniti immagine o rappresentazioni dinamiche su cui lavorare **[!UICONTROL Pyramid TIFF]** di una risorsa, quindi se **[!UICONTROL Pyramid TIFF]** non è disponibile nell’istanza di AEM Author, quindi non è disponibile anche in Brand Portal. Di conseguenza, nella barra delle rappresentazioni della pagina dei dettagli delle risorse e nella finestra di dialogo per il download non sono presenti rappresentazioni dinamiche.

Per pubblicare i predefiniti immagine in Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e vai a **[!UICONTROL Risorse > Predefiniti immagine]**.
1. Seleziona il predefinito immagine o più predefiniti immagine dall’elenco e tocca o fai clic su **[!UICONTROL Pubblica su Brand Portal]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]** i predefiniti immagine sono in coda per la pubblicazione. Si consiglia agli utenti di monitorare il registro degli agenti di replica per verificare se la pubblicazione è stata eseguita correttamente.

Per annullare la pubblicazione di un predefinito immagine da Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sul pulsante **[!UICONTROL Strumenti]** e passa a **[!UICONTROL Risorse > Predefiniti immagine]**.
1. Seleziona un predefinito immagine e fai clic su **[!UICONTROL Rimuovi da Brand Portal]** dalle opzioni disponibili nella parte superiore.

## Pubblicare schema metadati in Brand Portal  {#publish-metadata-schema-to-brand-portal}

Lo schema metadati descrive il layout e le proprietà visualizzati nella pagina delle proprietà di risorse/raccolte.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se gli utenti hanno modificato lo schema predefinito sull’istanza di AEM Author e sono disposti a utilizzare lo stesso schema come schema predefinito in Brand Portal, possono semplicemente pubblicare i moduli schema metadati in Brand Portal. In questo caso, lo schema predefinito in Brand Portal viene sostituito dagli schemi predefiniti pubblicati dall’istanza di AEM Author.

Se gli utenti hanno creato uno schema personalizzato nell’istanza di AEM Author, possono pubblicarlo in Brand Portal anziché ricreare lo stesso schema personalizzato. Gli utenti possono quindi applicare questo schema personalizzato a qualsiasi cartella/raccolta in Brand Portal.

>[!NOTE]
>
>Gli schemi predefiniti non possono essere pubblicati in Brand Portal se sono bloccati nell’istanza AEM (ossia se non sono modificati).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se a una cartella è applicato uno schema nell’istanza di AEM Author, lo stesso schema deve esistere anche in Brand Portal per mantenere la coerenza nella pagina delle proprietà delle risorse in AEM Author e Brand Portal.

Per pubblicare uno schema di metadati dall’istanza di AEM Author a Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e vai a **[!UICONTROL Assets > Schemi metadati]**.
1. Seleziona uno schema di metadati e seleziona **[!UICONTROL Pubblica su Brand Portal]** dalle opzioni disponibili nella parte superiore.

>[!NOTE]
>
>Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]**, gli schemi di metadati vengono inseriti nella coda per la pubblicazione. Si consiglia agli utenti di monitorare il registro degli agenti di replica per verificare se la pubblicazione è stata eseguita correttamente.

Per annullare la pubblicazione di uno schema di metadati da Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e vai a **[!UICONTROL Assets > Schemi metadati]**.
1. Seleziona uno schema di metadati e seleziona **[!UICONTROL Rimuovi da Brand Portal]** dalle opzioni disponibili nella parte superiore.

## Pubblicare i facet di ricerca in Brand Portal {#publish-search-facets-to-brand-portal}

I moduli di ricerca offrono le funzionalità di [ricerca sfaccettata](../using/brand-portal-search-facets.md) agli utenti su Brand Portal. I facet di ricerca conferiscono maggiore granularità alle ricerche su Brand Portal. Tutte le [predicati aggiunti](https://experienceleague.adobe.com/docs/experience-manager-65/assets/administer/search-facets.html) nel modulo di ricerca sono disponibili per gli utenti come facet di ricerca nei filtri di ricerca.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se desideri utilizzare un modulo di ricerca personalizzato **[!UICONTROL Barra di ricerca amministrazione risorse]** dall’istanza Autore AEM, invece di ricreare lo stesso modulo su Brand Portal, puoi pubblicare il modulo di ricerca personalizzato dall’istanza Autore AEM a Brand Portal.

>[!NOTE]
>
>Modulo di ricerca bloccato **[!UICONTROL Barra di ricerca amministrazione risorse]** su AEM Assets non può essere pubblicato su Brand Portal a meno che non venga modificato. Dopo essere stato modificato e pubblicato in Brand Portal, questo modulo di ricerca ha la precedenza su quello in Brand Portal.

Per pubblicare il facet di ricerca modificato dall’istanza di AEM Author a Brand Portal:

1. Tocca/fai clic sul logo AEM, quindi vai a **[!UICONTROL Strumenti > Generale > Moduli di ricerca]**.
1. Seleziona il modulo di ricerca modificato e seleziona **[!UICONTROL Pubblica su Brand Portal]**.

   >[!NOTE]
   >
   >Quando gli utenti fanno clic su **[!UICONTROL Pubblica su Brand Portal]**, i facet di ricerca sono accodati per la pubblicazione. Si consiglia agli utenti di monitorare il registro degli agenti di replica per verificare se la pubblicazione è stata eseguita correttamente.

Per annullare la pubblicazione dei moduli di ricerca da Brand Portal:

1. Nell’istanza di AEM Author, tocca o fai clic sul logo AEM per accedere alla console di navigazione globale, quindi tocca o fai clic sull’icona Strumenti e vai a **[!UICONTROL Generale > Cerca in Forms]**.
1. Seleziona il modulo di ricerca e seleziona **[!UICONTROL Rimuovi da Brand Portal]** dalle opzioni disponibili nella parte superiore.

>[!NOTE]
>
>Il **[!UICONTROL Annulla pubblicazione da Brand Portal]** L’azione lascia il modulo di ricerca predefinito su Brand Portal e non ripristina l’ultimo modulo di ricerca utilizzato prima della pubblicazione.

### Limitazioni {#limitations}

1. Pochi predicati di ricerca non sono applicabili ai filtri di ricerca sul Brand Portal. Quando questi predicati di ricerca vengono pubblicati come parte del modulo di ricerca dall’istanza di AEM Author a Brand Portal, vengono filtrati. Gli utenti, pertanto, visualizzano meno predicati nel modulo pubblicato in Brand Portal. Consulta [predicati di ricerca applicabili ai filtri su Brand Portal](../using/brand-portal-search-facets.md#list-of-search-predicates).

1. Per [!UICONTROL Predicato opzioni], se un utente utilizza un percorso personalizzato per leggere le opzioni nell’istanza di AEM Author, non funzionerà in Brand Portal. Questi percorsi e opzioni aggiuntivi non vengono pubblicati in Brand Portal con il modulo di ricerca. In questo caso, gli utenti possono selezionare **[!UICONTROL Manuale]** opzione in **[!UICONTROL Aggiungi opzioni]** entro **[!UICONTROL Predicato opzioni]** per aggiungere queste opzioni manualmente in Brand Portal.

![](assets/options-predicate-manual.png)
