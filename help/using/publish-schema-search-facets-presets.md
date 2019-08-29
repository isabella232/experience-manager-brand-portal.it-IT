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
source-git-commit: 770c353b1143d879280df310012ce9d4d30b40c9

---


# Pubblicare predefiniti, schema e facet su Brand Portal {#publish-presets-schema-and-facets-to-brand-portal}

L'articolo consente di pubblicare predefiniti per immagini, schemi di metadati e facet di ricerca personalizzati a [!DNL AEM][!DNL Brand Portal]partire da Istanza autore. La funzionalità di pubblicazione consente alle organizzazioni di riutilizzare i predefiniti immagine, gli schemi di metadati e i facet di ricerca creati/modificati nell'istanza [!DNL AEM] Author, riducendo così le attività duplicate.

>[!NOTE]
>
>La funzionalità di pubblicare i predefiniti per immagini, di metadati e di ricerca da [!DNL AEM] Istanza autore è [!DNL Brand Portal] disponibile [!DNL AEM 6.2 SP1-CFP7] e [!DNL AEM 6.3 SP 1-CFP 1 (6.3.1.1)] a partire da tale istanza.

## Pubblicare i predefiniti per immagini su Brand Portal {#publish-image-presets-to-brand-portal}

I predefiniti per immagini sono un insieme di comandi di ridimensionamento e formattazione applicati all'immagine al momento della distribuzione delle immagini. I predefiniti per immagini possono essere creati e modificati in [!DNL Brand Portal]. In alternativa, se [!DNL AEM] l'istanza Autore è in esecuzione in modalità media dinamica, gli utenti possono creare dei predefiniti presso l' [!DNL AEM] autore e pubblicarli [!DNL AEM Assets Brand Portal], evitando [!DNL Brand Portal]di ricreare gli stessi predefiniti.\
Una volta creato il predefinito, questo viene elencato come rappresentazione dinamica sulla barra delle rappresentazioni dei dettagli delle risorse e sul relativo dialogo.

>[!NOTE]
>
>Se [!DNL AEM] l'istanza Autore non è in esecuzione [!DNL Dynamic Media] in modalità (il cliente non è stato acquistato [!DNL Dynamic Media]), la [!UICONTROL rappresentazione TIFF] piramidale delle risorse non viene creata al momento del caricamento. I predefiniti immagine o dinamiche funzionano su [!UICONTROL TIFF piramidale] di una risorsa, pertanto se [!UICONTROL TIFF] piramidale non è disponibile nell'istanza [!DNL AEM] Autore, non è disponibile anche. [!DNL Brand Portal] Di conseguenza, nelle rappresentazioni delle pagine dei dettagli della risorsa e nei dialoghi di download non sono presenti rappresentazioni dinamiche.

Per pubblicare i predefiniti per immagini:[!DNL Brand Portal]

1. Nell'istanza [!DNL AEM] Autore, toccate o fate clic sul [!DNL AEM] logo per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Risorse]** &gt; **[!UICONTROL Predefiniti immagine]**.
2. Selezionate i predefiniti per immagini o più immagini dall'elenco dei predefiniti per immagini, quindi fate clic o toccate **[!UICONTROL Pubblica su Portale marchio]**.

![](assets/publishpreset.png)

>[!NOTE]
>
>Quando gli utenti fanno clic **[!UICONTROL su Pubblica sul portale]** marchio, i predefiniti per immagini vengono messi in coda per la pubblicazione. Agli utenti viene richiesto di monitorare il registro degli agenti di replica per confermare se la pubblicazione è stata completata correttamente.

Per annullare la pubblicazione di un predefinito per immagini da [!DNL Brand Portal]:

1. Nell'istanza [!DNL AEM] Autore, toccate o fate clic sul [!DNL AEM] logo per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Risorse]** &gt; **[!UICONTROL Predefiniti immagine]**.
2. Selezionate un predefinito per immagini e selezionate **[!UICONTROL Rimuovi dal portale]** marchio dalle opzioni disponibili nella parte superiore.

## Pubblicare schema di metadati su Brand Portal {#publish-metadata-schema-to-brand-portal}

Schema di metadati descrive il layout e le proprietà visualizzate nella pagina proprietà di risorse/raccolte.

![](assets/metadata-schema-editor.png) ![](assets/asset-properties-1.png)

Se gli utenti hanno modificato lo schema predefinito nell'istanza [!DNL AEM] Author e sono disposti a utilizzare lo schema predefinito per uno schema predefinito, [!DNL Brand Portal]possono semplicemente pubblicare i moduli schema metadati in [!DNL Brand Portal]. In uno scenario di questo tipo, lo schema predefinito viene [!DNL Brand Portal] ignorato dagli schemi predefiniti pubblicati dall'istanza [!DNL AEM] Author.

Se gli utenti hanno creato uno schema personalizzato nell'istanza [!DNL AEM] Author, possono pubblicare lo schema personalizzato al [!DNL Brand Portal] posto di ricreare lo stesso schema personalizzato. Gli utenti possono quindi applicare lo schema personalizzato a qualsiasi cartella/raccolta in [!DNL Brand Portal].

>[!NOTE]
>
>Gli schemi predefiniti non possono essere pubblicati in [!DNL Brand Portal] caso siano bloccati nell' [!DNL AEM] istanza (ovvero non modificati).

![](assets/default-schema-form.png)

>[!NOTE]
>
>Se una cartella ha uno schema applicato all'istanza [!DNL AEM] Author, lo stesso schema deve esistere anche per [!DNL Brand Portal] mantenere la coerenza nella pagina delle proprietà della risorsa su [!DNL AEM] Autore e [!DNL Brand portal].

Per pubblicare uno schema di metadati dall'istanza [!DNL AEM] Autore a [!DNL Brand Portal]:

1. Nell'istanza [!DNL AEM] Autore, toccate o fate clic sul logo AEM per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Risorse]** &gt; **[!UICONTROL Schemi metadati]**.
2. Selezionate uno schema di metadati e selezionate **[!UICONTROL Pubblica sul portale marchio]** dalle opzioni disponibili nella parte superiore.

>[!NOTE]
>
>Quando gli utenti fanno clic **[!UICONTROL su Pubblica sul portale del brand]**, gli schemi di metadati vengono messi in coda per la pubblicazione. Agli utenti viene richiesto di monitorare il registro degli agenti di replica per confermare se la pubblicazione è stata completata correttamente.

Per annullare la pubblicazione di uno schema di metadati da [!DNL Brand Portal]:

1. Nell'istanza [!DNL AEM] Autore, toccate o fate clic sul [!DNL AEM] logo per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Risorse]** &gt; **[!UICONTROL Schemi metadati]**.
2. Selezionate uno schema di metadati e selezionate **[!UICONTROL Rimuovi dal portale marchio]** dalle opzioni disponibili nella parte superiore.

## Pubblicare facet di ricerca su Brand Portal {#publish-search-facets-to-brand-portal}

I moduli di ricerca consentono agli utenti [di effettuare ricerche](../using/brand-portal-search-facets.md) con facet [!DNL Brand Portal]. I facet di ricerca consentono una granularità maggiore per effettuare ricerche [!DNL Brand Portal]. Tutti [i predicati aggiunti](https://helpx.adobe.com/experience-manager/6-5/assets/using/search-facets.html#AddingaPredicate) nel modulo di ricerca sono disponibili per gli utenti come facet di ricerca nei filtri di ricerca.

![](assets/property-predicate-removed.png)
![](assets/search-form.png)

Se sei disposto a utilizzare la barra di ricerca di Risorse amministratore **[!UICONTROL Risorse amministratore]** dall'istanza [!DNL AEM] Autore, invece di ricreare lo stesso modulo, [!DNL Brand Portal] puoi pubblicare il modulo di ricerca personalizzato [!DNL AEM] a [!DNL Brand Portal]tale istanza.

>[!NOTE]
>
>Non è possibile pubblicare **[!UICONTROL su Risorse AEM la barra]** di ricerca del modulo di ricerca delle risorse in AEM Assets [!DNL Brand Portal] a meno che non venga modificata. Una volta modificato e pubblicato su [!DNL Brand Portal], questo modulo di ricerca sostituisce il modulo di ricerca.[!DNL Brand Portal]

Per pubblicare il facet di ricerca modificato dall'istanza [!DNL AEM] Author a [!DNL Brand Portal]:

1. Toccate/fate clic sul [!DNL AEM] logo, quindi passate **[!UICONTROL a Strumenti]** &gt; **[!UICONTROL Generale]** &gt; **[!UICONTROL Ricerca moduli]**.
2. Selezionate il modulo di ricerca modificato e selezionate **[!UICONTROL Pubblica sul portale del marchio]**.

   >[!NOTE]
   >
   >Quando gli utenti fanno clic **[!UICONTROL su Pubblica sul portale del marchio]**, i facet di ricerca vengono messi in coda per la pubblicazione. Agli utenti viene richiesto di monitorare il registro degli agenti di replica per confermare se la pubblicazione è stata completata correttamente.

Per annullare la pubblicazione di moduli di ricerca da [!DNL Brand Portal]:

1. Nell'istanza [!DNL AEM] Autore, toccate o fate clic sul [!DNL AEM] logo per accedere alla console di navigazione globale, toccate o fate clic sull'icona Strumenti e passate a **[!UICONTROL Generale]** &gt; **[!UICONTROL Ricerca moduli]**.
2. Selezionate il modulo di ricerca e selezionate **[!UICONTROL Rimuovi dal portale marchio]** dalle opzioni disponibili nella parte superiore.

>[!NOTE]
>
>L'azione **[!UICONTROL Annulla pubblicazione da Brand Portal]** lascia il modulo di ricerca predefinito su Brand Portal e non ripristina l'ultimo modulo di ricerca utilizzato prima della pubblicazione.

### Limiti {#limitations}

1. Alcuni predicati di ricerca non sono applicabili per i filtri [!DNL Brand Portal]di ricerca. Quando i predicati di ricerca vengono pubblicati come parte del modulo di ricerca a [!DNL AEM] istanza Autore, [!DNL Brand Portal]vengono filtrati. Gli utenti, quindi, vedono un numero minore di predicati nel modulo [!DNL Brand Portal]pubblicato. Consultate [predicati di ricerca applicabili ai filtri sul portale brand](../using/brand-portal-search-facets.md#list-of-search-predicates).

2. Per [!UICONTROL Predicato opzioni] , se un utente utilizza un percorso personalizzato per le opzioni nell'istanza AEM Author, non funzionerà sul portale marchio. Questi percorsi e opzioni aggiuntivi non vengono pubblicati sul portale marchio con il modulo di ricerca. In questo caso, gli utenti possono selezionare **[!UICONTROL l'opzione Manuale]** in **[!UICONTROL Aggiungi opzioni]** all'interno **[!UICONTROL dell'predicato Opzioni]** per aggiungere manualmente queste opzioni.[!DNL Brand Portal]

![](assets/options-predicate-manual.png)
