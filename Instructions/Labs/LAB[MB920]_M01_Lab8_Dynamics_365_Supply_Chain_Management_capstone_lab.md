---
lab:
    title: 'Lab 8: Lab di fine modulo per Dynamics 365 Supply Chain Management'
    module: 'Modulo 1: Concetti fondamentali su Microsoft Dynamics 365 Supply Chain Management'
---

## Lab 8: Lab di fine modulo per Dynamics 365 Supply Chain Management

## Obiettivo

Durante questo lab verranno esaminate la creazione di prodotti e la gestione dei prezzi. Si esamineranno anche i principali processi aziendali delle catene di approvvigionamento, ad esempio gestione articoli, approvvigionamento ed esternalizzazione.

## Configurazione del lab

- **Tempo stimato**: 45 minuti 

## Esercizio 1. Esplorare la gestione dei prodotti

### Creare un prodotto

In Contoso Entertainment System USA (USMF) è necessario creare un nuovo articolo per un alloggiamento per altoparlanti configurato da acquistare dai fornitori.

1. Nella home page, in alto a destra, verificare che sia selezionata la società **USMF**.

1. In caso contrario, selezionare la società indicata nell'elenco e modificarla in **USMF**.

1. Usando il pannello di navigazione, selezionare **Moduli** > **Gestione informazioni sul prodotto** > **Prodotti** > **Prodotti rilasciati**.

1. Nella pagina dettagli Prodotto rilasciato, nel riquadro azioni selezionare **+ Nuovo**.

1. Nel riquadro **Nuovo prodotto rilasciato**, nel menu **Tipo di prodotto** verificare che sia selezionato **Articolo**.

1. Nel menu **Sottotipo di prodotto** verificare che sia selezionato **Prodotto**.

1. Selezionare il menu **Gruppo di dimensioni di tracciabilità**, quindi scegliere **Nessuno**.

1. In **IDENTIFICAZIONE**, nella casella **Numero prodotto** immettere **GTL201**.

1. Nella casella **Nome prodotto** immettere **Speaker Enclosure**.

1. In **TASSAZIONE VENDITE** selezionare il menu **Fascia IVA articoli**, quindi selezionare **TUTTO**.

1. In **TASSAZIONE ACQUISTI** selezionare il menu **Fascia IVA articoli**, quindi selezionare **TUTTO**.

1. In **PREZZI**, nella casella **Prezzo di acquisto** immettere **30.00**.

1. Nella casella **Prezzo di vendita** immettere **30.00**.

1. In **GRUPPI DI RIFERIMENTO** selezionare il menu **Gruppo di modelli di articoli**, quindi selezionare **FIFO (First-In-First-Out)**.

1. Selezionare il menu **Gruppo di articoli** e quindi scegliere **CarAudio**.

1. Selezionare il menu **Gruppo di dimensioni di immagazzinamento**, quindi scegliere **SiteWH**.

1. In **UNITÀ DI MISURA** verificare che siano impostati i valori seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Unità di magazzino| ea|
    | Unità di acquisto| ea|
    | Unità di vendita| ea|
    | Unità DBA| ea|

1. Selezionare **OK**.

1. Per assicurarsi che il prodotto sia finalizzato, nel riquadro azioni selezionare **Prodotto** e quindi in **Gestisci** selezionare **Convalida**.

1. Verificare che venga visualizzato il banner di informazioni che conferma che tutti i valori dei campi richiesti sono stati convalidati.

1. Chiudere tutte le pagine e tornare alla home page.

## Esercizio 2. Esplorare la gestione del magazzino

### Creare un magazzino

1. Nel pannello di navigazione selezionare **Moduli** > **Gestione inventario** > **Configurazione** > **Suddivisione scorte** > **Magazzini**.

1. Nella pagina Magazzini, nel riquadro azioni selezionare **Nuovo**.

1. Nella casella **Magazzino** immettere **150**.

1. Nella casella **Nome** immettere **Outpost Warehouse**.

1. Selezionare il menu **Sito** e quindi selezionare **1 Home speakers production**.

1. Selezionare la Scheda dettaglio **Nomi ubicazioni**.

1. Le opzioni in questa sezione definiscono il formato predefinito per i nomi delle ubicazioni.

1. Impostare le opzioni **Includi sezione** e **Includi scaffale** su **Sì**.

1. Impostare l'opzione **Includi ripiano** su **Sì**.

1. Nella casella **Formato** per il ripiano immettere **-##**.

1. Nel riquadro azioni selezionare **Magazzino**.

1. In **Gestisci** selezionare **Creazione guidata ubicazione**.

1. Nella pagina iniziale esaminare le informazioni e quindi selezionare **Avanti** nell'angolo inferiore destro.

1. Deselezionare le caselle di controllo **Banchine di entrata** e **Ubicazioni di stoccaggio**.

1. Selezionare **Avanti** ed esaminare le informazioni.

1. Procedere alle pagine successive e al termine selezionare **Fine**.

1. Chiudere la pagina e tornare alla home page.

### Creare un accordo commerciale per il prezzo di vendita

1. Usando il pannello di navigazione, selezionare **Moduli** > **Gestione informazioni sul prodotto** > **Prodotti** > **Prodotti rilasciati**.

1. Nella pagina dettagli Prodotti rilasciati cercare il numero di prodotto **GTL201**.

1. A sinistra di **GTL201** selezionare la casella di controllo **Seleziona o deseleziona riga**.

1. Nel riquadro azioni selezionare **Vendi** e quindi in **ACCORDI COMMERCIALI** selezionare **Crea accordi commerciali**.

1. Nel riquadro azioni selezionare **+ Nuovo**.

1. Nella colonna **Nome** selezionare il menu e quindi scegliere **S_Price**.

1. Nel riquadro azioni selezionare **Righe**.

1. Nelle righe di registrazione della pagina dell'accordo commerciale, nella colonna **Relazione articolo** selezionare il menu e quindi **GTL201**.

1. Questo è il numero di articolo del prodotto creato.

1. Nella colonna **Magazzino** selezionare il menu, quindi scegliere **150**.

1. Potrebbe essere necessario scorrere verso destra per visualizzare la colonna.

1. Nella colonna **Importo in valuta** immettere **100.00** nella casella.

1. Nella sezione Dettagli, nella casella **Dal** immettere la prima data dell'anno corrente.

1. Nel riquadro azioni selezionare **Convalida** > **Convalida tutte le righe**.

1. Nel riquadro **Registrazione giornale prezzi/sconti** selezionare **OK**.

1. Verificare che non ci siano errori.

1. Nel riquadro azioni selezionare **Registra**.

1. Nel riquadro **Registrazione giornale prezzi/sconti** selezionare **OK**.

1. Verificare che l'operazione venga completata.

1. Chiudere la pagina.

1. Nella pagina dettagli Prodotto rilasciato, nel riquadro azioni in **Vendi** > **ACCORDI COMMERCIALI** selezionare **Visualizza accordi commerciali**.

1. L'accordo commerciale deve essere registrato. Esaminare la riga e osservare le informazioni sul prezzo.

1. Chiudere le pagine e tornare alla home page.

## Esercizio 3. Esplorare la gestione della produzione

### Creare un ordine di produzione per un prodotto

1. Nel pannello di navigazione a sinistra selezionare **Moduli** > **Controllo produzione** > **Ordini di produzione** > **Tutti gli ordini di produzione**.

1. Nel riquadro azioni selezionare **Nuovo ordine di produzione**.

1. Nel riquadro **Crea ordine di produzione**, in **IDENTIFICAZIONE** immettere **D0004** nella casella **Numero articolo** e quindi selezionare l'articolo identificato.

1. In **PRODUZIONE**, nella casella **Consegna**, selezionare una data a un mese da oggi.

1. La data di consegna indica quando deve terminare l'ordine di produzione per poter consegnare in tempo. Questa data può essere usata nel processo di pianificazione. Ad esempio, è possibile pianificare l'ordine a ritroso dalla data di consegna.

1. Nella casella **Quantità** immettere **30**.

1. Selezionare **Crea**.

1. Chiudere tutte le pagine e tornare alla home page.

## Esercizio 4. Esplorare la gestione dell'inventario

### Creare un giornale di registrazione conteggi con il prodotto per il magazzino creato

1. Usando il pannello di navigazione, selezionare **Moduli** > **Gestione inventario** > **Inserimenti nel giornale di registrazione** > **Conteggio articoli > Conteggio**.

1. Nel riquadro azioni selezionare **+ Nuovo**.

1. Nel riquadro **Crea giornale di registrazione inventario** in **Conteggio per** selezionare l'interruttore **Magazzino** per impostarlo su **Sì**.

1. Selezionare **OK**.

1. Nella pagina Giornale di registrazione conteggio scorte, nella Scheda dettaglio **Dettagli intestazione giornale di registrazione**, in **Righe giornale di registrazione** sulla barra degli strumenti selezionare **+Nuovo**.

1. Nella colonna **Numero articolo** selezionare il menu e quindi scegliere **GTL201**.

1. Nella colonna **Magazzino** selezionare il menu, quindi scegliere **150**.

1. Nella casella **Conteggiato** immettere **100.00**.

1. Questo valore specifica il numero di articoli stoccati in magazzino per questo prodotto.

1. Nel riquadro azioni selezionare **Convalida**.

1. Nel riquadro **Verifica giornale di registrazione** selezionare **OK**.

1. Nel riquadro azioni selezionare **Registra**.

1. Nel riquadro **Registra giornale** selezionare **OK**.

1. Chiudere tutte le pagine e tornare alla home page.

### Controllare le scorte disponibili per il prodotto

1. Usando il pannello di navigazione, selezionare **Moduli** > **Gestione inventario** > **Richieste di informazioni e report** > **Elenco scorte disponibili**.

1. Nel riquadro azioni selezionare **Dimensioni**.

1. Nel riquadro **Visualizzazione dimensioni** in **DIMENSIONI DI IMMAGAZZINAMENTO** selezionare le caselle di controllo **Sito** e **Magazzino** e quindi **OK**.

1. Nel riquadro **Filtri** selezionare **Applica**.

1. Individuare ed esaminare le scorte disponibili per **GTL201**.

1. Chiudere tutte le pagine e tornare alla home page.

## Esercizio 5. Esplorare l'approvvigionamento

### Creare un ordine fornitore con un prodotto

1. Usando il pannello di navigazione, selezionare **Moduli** > **Approvvigionamento** > **Ordini fornitore** > **Tutti gli ordini fornitore**.

1. Nella pagina Tutti gli ordini fornitore, nel riquadro azioni selezionare **+ Nuovo**.

1. Nel riquadro **Crea ordine fornitore** selezionare il menu **Account fornitore** e quindi **US-101**.

1. Quando si seleziona un fornitore, i dettagli del record fornitore, ad esempio indirizzo, conto fatture, termini di consegna e modalità di consegna, verranno copiati come valori predefiniti nell'intestazione dell'ordine. È possibile modificare questi valori in qualsiasi momento.

1. Nella sezione **Generale** in **DIMENSIONI DI IMMAGAZZINAMENTO** selezionare il menu **Sito** e quindi **1 Home speakers production**.

1. In **DATE** selezionare un valore per **Data di consegna** a una settimana dalla data corrente.

1. Selezionare **Amministrazione**.

1. Selezionare il menu **Autore ordine** e quindi selezionare **Lars Giusti** per specificare chi sta effettuando l'ordine.

1. Nel riquadro **Crea ordine fornitore** selezionare **OK**.

1. Sulla barra degli strumenti selezionare **Riga ordine fornitore**.

1. In **VISUALIZZAZIONE** selezionare **Dimensioni**.

1. Nel riquadro **Visualizzazione dimensioni**, in **DIMENSIONI PRODOTTO** selezionare la casella di controllo **Colore**.

1. Selezionare **OK**.

1. Nella colonna **Numero articolo** selezionare il menu e quindi scegliere **T0005**.

1. Nella colonna **Numero variante** selezionare il menu e quindi scegliere uno dei colori.

1. Nella casella **Quantità** immettere **15**.

1. In **Righe ordine fornitore**, nella parte inferiore della pagina, selezionare la Scheda dettaglio **Dettagli riga**.

1. È possibile che questa scheda sia già espansa.

1. Selezionare la scheda **Consegna** e nella casella **Data di consegna** usare la data assegnata o immettere una data futura.  
    È possibile assegnare una data di consegna univoca a ogni riga dell'ordine. La data viene ereditata dal campo nell'intestazione dell'ordine fornitore, ma è possibile modificarla.

1. Annotare il numero di ordine fornitore. Sarà necessario in seguito.

1. Nel riquadro azioni selezionare **Salva**.

1. Chiudere la pagina Riga ordine fornitore.

1. Nella pagina Tutti gli ordini fornitore usare la funzionalità **Filtro** per cercare il nuovo ordine fornitore.

1. Al termine, chiudere la pagina Tutti gli ordini fornitore e tornare alla home page.
