---
lab:
    title: 'Lab 3: Lab di fine modulo per Dynamics 365 Commerce'
    module: 'Modulo 3: Concetti fondamentali su Microsoft Dynamics 365 Commerce'
---

## Lab 3: Lab di fine modulo per Dynamics 365 Commerce

## Obiettivo

Durante questo lab si esamineranno i concetti di base della configurazione di Commerce Headquarters. Le funzionalità di base includono configurazione del canale di vendita, creazione di un assortimento e configurazione di uno sconto per la vendita al dettaglio.

## Configurazione del lab

   - **Tempo stimato**: 30 minuti 

## Istruzioni

## Esercizio 1. Esplorare la configurazione di Commerce nelle sedi centrali

### Creare un nuovo punto vendita

1. Nella pagina di destinazione, in alto a destra, verificare che sia selezionata la società **USRT**.

1. In caso contrario, selezionare la società indicata nell'elenco e immettere **USMF**.

1. Usando il pannello di navigazione, selezionare **Moduli** > **Vendita al dettaglio e commercio** > **Canali** > **Punti vendita** > **Tutti i punti vendita**.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare un nuovo punto vendita.

1. Nella finestra Nuovo record usare le impostazioni nella tabella seguente per aggiornare i valori:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Nome| Seattle Flagship Store|
    | Numero punto vendita| 000098|
    | Magazzino| Seattle|
    | Magazzino di spedizione| Seattle|
    | Fuso orario punto vendita| (GMT-08.00) Fuso costa pacifica|
    | Profilo funzionalità| FN001|
    | Ricerca in magazzino| Sì|
    | Profilo canale| Predefinito|
    | Profilo offline| Predefinito|
    | Fascia IVA| WA|
    | Utilizza imposta basata su destinazione| Sì|
    | Rubrica clienti| RetailCust|
    | Rubrica dipendenti| Seattle|
    | Cliente predefinito| 3002|

1. Nel riquadro azioni selezionare **Salva**.

1. Selezionare la Scheda dettaglio **Rendiconto/Chiusura** e quindi immettere gli aggiornamenti seguenti:

    | Impostazione| Valore|
    | :--- | :--- |
    | Calcolo importo estratto conto| Ultimo|
    | Differenza massima > Registrazione| 100.00|

1. Selezionare la Scheda dettaglio **Dimensioni finanziarie** e quindi immettere gli aggiornamenti seguenti:

    | Impostazione| Valore|
    | :--- | :--- |
    | BusinessUnit| 004|
    | RetailChannel| 000210|

1. Selezionare la Scheda dettaglio **Layout schermo**.

1. Nella casella **ID layout schermo** immettere **A2CP16:9C**.

1. Nel riquadro azioni selezionare **Salva**.

1. Nel riquadro azioni selezionare **Configurazione** e quindi nella scheda **COPIA** selezionare **Copia tutto**.

1. Nel riquadro **Copia tutto** selezionare **Punto vendita origine** e quindi scegliere **ANNAPOL**.

1. Se necessario, selezionare il menu **Punto vendita destinazione** e quindi scegliere **00098**.

1. Selezionare **OK**.

1. Verificare che venga visualizzato il messaggio di esito positivo e quindi chiudere la pagina.

### Aggiungere un gruppo di prodotti a un assortimento e pubblicarlo

1. Usando il pannello di navigazione, selezionare **Moduli** > **Amministrazione organizzazione** > **Organizzazioni** > **Gerarchie organizzative**.

1. Nell'elenco di navigazione selezionare **Punti vendita al dettaglio per stato/regione**.

1. Nel riquadro azioni selezionare **Visualizza**.

1. Nella finestra di progettazione della gerarchia, nel riquadro azioni selezionare **Modifica**.

1. Nel riquadro **Ovest** fare clic sul pulsante con i puntini di sospensione (**...**).

1. Nella finestra di progettazione della gerarchia selezionare **Inserisci** > **Canale di vendita al dettaglio**.

1. Nel riquadro **Canale di vendita al dettaglio** selezionare **Seattle Flagship Store** e quindi scegliere **OK**.

1. Nel riquadro azioni selezionare **Salva**.

1. Nella finestra di dialogo esaminare le informazioni, quindi selezionare **Chiudi**.

1. Nel riquadro azioni selezionare **Pubblica**.

1. Nel riquadro **Pubblica modifiche**, nella casella **Data di validità** selezionare il primo giorno del mese corrente.

1. Nella casella **Descrivi modifiche** immettere **Addition of Seattle Flagship Store** e quindi selezionare **Pubblica**.

1. Nella finestra di dialogo esaminare le informazioni, quindi selezionare **Chiudi**.

1. Nel riquadro azioni selezionare **Salva**.

1. Nella finestra di dialogo esaminare le informazioni, quindi selezionare **Chiudi**.

1. Chiudere la pagina.

1. Usando il pannello di navigazione, selezionare **Moduli** > **Vendita al dettaglio e commercio** > **Cataloghi e assortimenti** > **Assortimenti**.

1. Nella pagina Assortimenti selezionare **AW-Outlet**.

1. Nel riquadro azioni selezionare **Modifica**.

1. Nella finestra di dialogo selezionare **Sì** per confermare la modifica della selezione.

1. Nella pagina AW-Outlet selezionare la Scheda dettaglio **Commerce channel** (Canale di Commerce).

1. Sulla barra degli strumenti selezionare **+ Aggiungi riga**.

1. Nel riquadro **Scegli nodi organizzazione** selezionare il menu **Gerarchia organizzativa** e quindi scegliere **Punti vendita al dettaglio per stato/regione**.

1. In **NODI ORGANIZZAZIONE DISPONIBILI** selezionare **Seattle Flagship Store** e quindi selezionare l'icona freccia DESTRA **Aggiungi** per l'aggiunta in **NODI ORGANIZZAZIONE SELEZIONATI**.

1. Selezionare **OK**.

1. Nel riquadro azioni selezionare **Pubblica**.

1. Nella finestra di dialogo esaminare le informazioni e quindi selezionare **Sì**.

1. Nel riquadro azioni selezionare **Modifica**.

1. Nella finestra di dialogo **Conferma** selezionare **Sì**.

1. Nella pagina AW-Outlet selezionare la scheda **Prodotti**.

1. Nella pagina AW-Outlet selezionare **+ Aggiungi riga**.

1. Selezionare il menu **Categoria**, selezionare **Team Sports** e quindi selezionare **OK**.

1. Nel riquadro azioni selezionare **Pubblica**.  

### Eseguire il processo Retail Scheduler per i prodotti

1. Usando il pannello di navigazione, selezionare **Moduli** > **Vendita al dettaglio e commercio** > **Vendita al dettaglio e commercio IT** > **Programmazione della distribuzione**.

1. Nell'elenco di spostamento selezionare **1040 (Prodotti)**.

1. Nel riquadro azioni selezionare **Esegui ora**.

1. Nel riquadro **Sincronizzazione incrementale con pianificazione "1040"** esaminare le informazioni, quindi scegliere **OK**.

### Creare un nuovo sconto prodotti

1. Usando il pannello di navigazione, selezionare **Moduli** > **Vendita al dettaglio e commercio** > **Prezzi e sconti** > **Tutti gli sconti**.

1. Nel riquadro azioni selezionare **Nuovo** > **Sconto**.

1. Nella pagina Sconti, nella casella **Nome** immettere **Store Opening**.

1. Nella Scheda dettaglio **Dettagli**, nella casella **Descrizione** immettere **Store Opening 20% Off**.

1. Nella Scheda dettaglio **Prezzo/Sconto**, nella casella **Percentuale sconto** immettere **20.00**.

1. Nella Scheda dettaglio **Periodo di convalida**, nella casella **Data di validità** immettere una data del mese precedente.

1. Nella casella **Data di scadenza** immettere una data a una settimana dalla data corrente.

1. Nella Scheda dettaglio **Righe** sulla barra degli strumenti selezionare **+ Aggiungi**.

1. Nella colonna **Categoria** selezionare il menu, selezionare **Team Sports** e quindi selezionare **OK**.

1. Nel riquadro azioni selezionare **Salva**.

1. Nel riquadro azioni selezionare **Gruppi di prezzi**.

1. Nella pagina Gruppi di prezzi selezionare il menu **Gruppi di prezzi** e quindi selezionare **Ovest**.

1. Nel riquadro azioni selezionare **Salva**.

1. Usando il pannello di navigazione, selezionare **Moduli** > **Vendita al dettaglio e commercio** > **Prezzi e sconti** > **Tutti gli sconti**.

1. Nell'elenco di navigazione selezionare **ST100101**.

1. Nella Scheda dettaglio **Generale** selezionare il menu **Stato** e quindi selezionare **Abilitato**.

1. Nel riquadro azioni selezionare **Salva**.

1. Chiudere il modulo.

1. Usando il pannello di navigazione, selezionare **Moduli** > **Vendita al dettaglio e commercio** > **Vendita al dettaglio e commercio IT** > **Programmazione della distribuzione**.

1. Nell'elenco di spostamento selezionare **1020 (Prodotti)**.

1. Nel riquadro azioni selezionare **Esegui ora**.

1. Nel riquadro **Sincronizzazione incrementale con pianificazione "1020"** esaminare le informazioni, quindi scegliere **OK**.
