---
title: Pubblicare predefiniti, schema e facet su Brand Portal
seo-title: Pubblicare predefiniti, schema e facet su Brand Portal
description: Scoprite come pubblicare predefiniti, schema e facet su Brand Portal.
seo-description: Scoprite come pubblicare predefiniti, schema e facet su Brand Portal.
uuid: c 836 d 9 bb -074 a -4113-9 c 91-b 2 bf 7658 b 88 d
topic-tags: pubblicazione
products: SG_ EXPERIENCEMANAGER/Brand_ Portal
content-type: riferimento
discoiquuid: bc 305 abc -9373-4 d 33-9179-0 a 5 f 3904 b 352
translation-type: tm+mt
source-git-commit: 068ce845c51de48fb677f7bd09a2f6d20ff6f1a5

---


# Pubblicare predefiniti, schema e facet su Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

L'articolo consente di pubblicare predefiniti per immagini, schemi di metadati e facet di ricerca personalizzati dall'istanza AEM Author a Brand Portal. La funzionalità di pubblicazione consente alle organizzazioni di riutilizzare i predefiniti immagine, gli schemi di metadati e i facet di ricerca creati/modificati nell'istanza AEM Author, riducendo così le attività duplicate.

>[!NOTE]
>
>La funzionalità di pubblicazione di predefiniti per immagini, schema di metadati e facet di ricerca dall'istanza AEM Author a Brand Portal è disponibile su AEM 6.2 SP 1-CFP 7 e AEM 6.3 SP 1-CFP 1 (6.3.1.1).

## Pubblicare i predefiniti per immagini su Brand Portal {#publish-image-presets-to-brand-portal}

I predefiniti per immagini sono un insieme di comandi di ridimensionamento e formattazione applicati all'immagine al momento della distribuzione delle immagini. I predefiniti per immagini possono essere creati e modificati sul portale del brand. In alternativa, se l'istanza AEM Author è in esecuzione in modalità media dinamica, gli utenti possono creare predefiniti in AEM Author e pubblicarli sul portale di AEM Assets Brand ed evitare di ricreare gli stessi predefiniti sul portale del brand.\
Una volta creato il predefinito, questo viene elencato come rappresentazione dinamica sulla barra delle rappresentazioni dei dettagli delle risorse e sul relativo dialogo.

>[!NOTE]
>
>Se l'istanza AEM Author non è in esecuzione in [!UICONTROL modalità File multimediali dinamici] (il cliente non ha acquistato elementi multimediali dinamici), al momento del caricamento la [!UICONTROL rappresentazione TIFF] piramidale delle risorse non viene creata. I predefiniti immagine o dinamiche funzionano su [!UICONTROL TIFF piramidale] di una risorsa, pertanto se [!UICONTROL TIFF] piramidale non è disponibile nell'istanza AEM Author, non è disponibile anche sul portale marchio. Di conseguenza, nelle rappresentazioni delle pagine dei dettagli della risorsa e nei dialoghi di download non sono presenti rappresentazioni dinamiche.

Per pubblicare i predefiniti immagine su Brand Portal:

1. Nell'istanza AEM Author, toccate o fate clic sul logo AEM per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Risorse]** &gt; **[!UICONTROL Predefiniti immagine]**.
2. Selezionate i predefiniti per immagini o più immagini dall'elenco dei predefiniti per immagini, quindi fate clic o toccate **[!UICONTROL Pubblica su Portale marchio]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando gli utenti fanno clic **[!UICONTROL su Pubblica sul portale]** marchio, i predefiniti per immagini vengono messi in coda per la pubblicazione. Agli utenti viene richiesto di monitorare il registro degli agenti di replica per confermare se la pubblicazione è stata completata correttamente.

Per annullare la pubblicazione di un predefinito per immagini da Brand Portal:

1. Nell'istanza AEM Author, toccate o fate clic sul logo AEM per accedere alla console di navigazione globale, toccate o fate clic sull'icona **[!UICONTROL Strumenti]** e passate a **[!UICONTROL Risorse &gt; Predefiniti immagine]**.
2. Selezionate un predefinito per immagini e selezionate **[!UICONTROL Rimuovi dal portale]** marchio dalle opzioni disponibili nella parte superiore.

## Pubblicare schema di metadati su Brand Portal {#publish-metadata-schema-to-brand-portal}

Schema di metadati descrive il layout e le proprietà visualizzate nella pagina proprietà di risorse/raccolte.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se gli utenti hanno modificato lo schema predefinito sull'istanza AEM Author e sono disposti a utilizzare lo schema predefinito per il portale marchio, possono semplicemente pubblicare i moduli schema metadati su Brand Portal. In questo scenario, lo schema predefinito di Brand Portal viene ignorato dagli schemi predefiniti pubblicati dall'istanza AEM Author.

Se gli utenti hanno creato uno schema personalizzato sull'istanza AEM Author, possono pubblicare lo schema personalizzato su Brand Portal invece di ricreare lo stesso schema personalizzato. Gli utenti possono quindi applicare questo schema personalizzato a qualsiasi cartella/raccolta in Brand Portal.

>[!NOTE]
>
>Gli schemi predefiniti non possono essere pubblicati sul portale brand se sono bloccati nell'istanza di AEM (ovvero non modificati).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se una cartella ha uno schema applicato all'istanza AEM Author, lo schema deve esistere anche sul portale marchio per mantenere la coerenza nella pagina delle proprietà della risorsa su AEM Author e Brand Portal.

Per pubblicare uno schema di metadati dall'istanza AEM Author su Brand Portal:

1. Nell'istanza AEM Author, toccate o fate clic sul logo AEM per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Risorse &gt; Schemi metadati]**.
2. Selezionate uno schema di metadati e selezionate **[!UICONTROL Pubblica sul portale marchio]** dalle opzioni disponibili nella parte superiore.

>[!NOTE]
>
>Quando gli utenti fanno clic **[!UICONTROL su Pubblica sul portale del brand]**, gli schemi di metadati vengono messi in coda per la pubblicazione. Agli utenti viene richiesto di monitorare il registro degli agenti di replica per confermare se la pubblicazione è stata completata correttamente.

Per annullare la pubblicazione di uno schema di metadati da Brand Portal:

1. Nell'istanza AEM Author, toccate o fate clic sul logo AEM per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Risorse &gt; Schemi metadati]**.
2. Selezionate uno schema di metadati e selezionate **[!UICONTROL Rimuovi dal portale marchio]** dalle opzioni disponibili nella parte superiore.

## Pubblicare facet di ricerca su Brand Portal {#publish-search-facets-to-brand-portal}

I moduli di ricerca consentono di effettuare ricerche [con facet](../using/brand-portal-search-facets.md) agli utenti sul portale del brand. I facet di ricerca rendono più granularità la granularità su Brand Portal. Tutti [i predicati aggiunti](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) nel modulo di ricerca sono disponibili per gli utenti come facet di ricerca nei filtri di ricerca.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se sei disposto a utilizzare la barra di ricerca di Risorse amministratore **[!UICONTROL Risorse AEM]** dall'istanza AEM Author, invece di ricreare lo stesso modulo su Brand Portal puoi pubblicare il modulo di ricerca personalizzato da AEM Author Instance to Brand Portal.

>[!NOTE]
>
>La barra di ricerca del modulo **[!UICONTROL di ricerca Risorse di ricerca Risorse]** su AEM Assets non può essere pubblicata sul portale marchio a meno che non venga modificata. Una volta modificato e pubblicato sul portale brand, questo modulo di ricerca sostituisce il modulo di ricerca sul portale del brand.

Per pubblicare il facet di ricerca modificato dall'istanza AEM Author su Brand Portal:

1. Toccate/fate clic sul logo AEM, quindi andate a **[!UICONTROL Strumenti]** &gt; **[!UICONTROL Generale]** &gt; **[!UICONTROL Ricerca moduli]**.
2. Selezionate il modulo di ricerca modificato e selezionate **[!UICONTROL Pubblica sul portale del marchio]**.

   >[!NOTE]
   >
   >Quando gli utenti fanno clic **[!UICONTROL su Pubblica sul portale del marchio]**, i facet di ricerca vengono messi in coda per la pubblicazione. Agli utenti viene richiesto di monitorare il registro degli agenti di replica per confermare se la pubblicazione è stata completata correttamente.

Per annullare la pubblicazione di moduli di ricerca da Brand Portal:

1. Nell'istanza di AEM Author, toccate o fate clic sul logo AEM per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Generale &gt; Ricerca moduli]**.
2. Selezionate il modulo di ricerca e selezionate **[!UICONTROL Rimuovi dal portale marchio]** dalle opzioni disponibili nella parte superiore.

>[!NOTE]
>
>L'azione **[!UICONTROL Annulla pubblicazione da Brand Portal]** lascia il modulo di ricerca predefinito su Brand Portal e non ripristina l'ultimo modulo di ricerca utilizzato prima della pubblicazione.

### Limiti {#limitations}

1. Alcuni predicati di ricerca non sono applicabili per i filtri di ricerca sul portale brand. Quando questi predicati di ricerca vengono pubblicati come parte del modulo di ricerca da AEM Author Instance to Brand Portal, vengono filtrati. Gli utenti, quindi, vedono un numero minore di predicati nel modulo pubblicato sul portale brand. Consultate [predicati di ricerca applicabili ai filtri sul portale brand](../using/brand-portal-search-facets.md#list-of-search-predicates).

2. Per [!UICONTROL Predicato opzioni], se un utente utilizza un percorso personalizzato per le opzioni nell'istanza AEM Author, non funzionerà sul portale marchio. Questi percorsi e opzioni aggiuntivi non vengono pubblicati sul portale marchio con il modulo di ricerca. In questo caso, gli utenti possono selezionare l'opzione **[!UICONTROL Manuale]** in **[!UICONTROL Aggiungi opzioni]** all'interno **[!UICONTROL dell'predicato Opzioni]** per aggiungere manualmente queste opzioni al portale del brand.

![](assets/options-predicate-manual.png)
