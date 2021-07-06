---
lab:
    title: 'Lab 1: Creare un prodotto con sconto'
    module: 'Modulo 3: Concetti fondamentali su Microsoft Dynamics 365 Commerce'
---

## Lab 1: Creare un prodotto con sconto

## Obiettivi

Il punto vendita di Boston della società desidera incentivare le vendite di alcuni prodotti per far spazio alla nuova linea. È necessario creare e attivare un nuovo sconto prodotti.

## Configurazione del lab

   - **Tempo stimato**: 10 minuti

## Istruzioni

1. Nella pagina Finance and Operations, in alto a sinistra, selezionare il menu hamburger **Espandere il pannello di navigazione**.

1. Nel pannello di navigazione selezionare **Aree di lavoro** > **Gestione prezzi e sconti**.

1. Nella pagina Gestione prezzi e sconti esaminare i valori visualizzati per **Sconti attivi**.

1. Nel menu selezionare **Nuovo**, esaminare le opzioni disponibili e quindi selezionare **Sconto**.

1. Nella pagina Sconti, nella casella **Nome** immettere un nome per lo sconto. Ad esempio, New Year 20%.

1. Nella scheda Generale verificare che lo stato sia impostato su **Disabilitato**.

1. Lo sconto può essere modificato solo quando è impostato come disabilitato.

1. Selezionare il menu **Modalità di concorrenza sconti**, esaminare le opzioni disponibili e quindi selezionare **Prezzo migliore**.

    >[!NOTA] Quando si sceglie tra le opzioni per la modalità di concorrenza, tenere presente quanto segue:
    >
    >  - Quando sono applicabili più sconti composti, quello più alto viene sempre calcolato per primo.  Il successivo sconto più alto viene quindi calcolato sull'importo rimanente.  Questa gerarchia di calcolo continua fino a quando non sono stati applicati tutti gli sconti composti.  
    >    **Calcolo corretto**: 40% di sconto + 20% di sconto = 52% di sconto  
    >      - (40% di sconto su $ 100 = $ 40. Importo rimanente = $ 60.  20% di sconto su $ 60 = 12. Importo rimanente = $48)  
    >
    >    **Calcolo errato**: 40% di sconto + 20% di sconto = 60% di sconto
    >
    >  - Gli sconti esclusivi si applicano sempre sul prezzo migliore o sullo sconto composto, anche se si tratta della percentuale di sconto più bassa.
    >    - Quando sono applicabili più sconti esclusivi, viene usato il più alto.
    >  - Quando sono applicabili sia il prezzo migliore sia lo sconto composto, oppure se sono applicabili più opzioni dello stesso sconto, viene applicato lo sconto più alto.

1. Selezionare il menu **Conto sconti** ed esaminare l'elenco.

1. Nella casella Conto sconti immettere **sconto**.

1. L'elenco verrà filtrato automaticamente.

1. Nei risultati selezionare il numero di conto sconti **403200**.

1. Esaminare le altre opzioni e quindi espandere **Dettagli**.

1. Nella casella **Descrizione** immettere una descrizione per lo sconto. Ad esempio, New Year discount offering 20% off.

1. Espandere **Prezzo/Sconto**.

1. Nella casella Percentuale sconto immettere **20.00**.

1. Espandere **Periodo di convalida**.

1. Impostare **Data di validità** e **Data di scadenza** per lo sconto.

1. Assicurarsi di impostare la data di scadenza nel futuro, altrimenti lo sconto non verrà visualizzato nell'elenco Sconti attivi.

1. Espandere **Righe**.

1. Nel menu selezionare **+ Aggiungi**.

1. Selezionare il menu **Categoria** e quindi selezionare **Fashion (Fashion)**.

1. In questo modo, lo sconto verrà applicato a tutti i prodotti nella categoria Abbigliamento.

1. Espandere **Dettagli riga** e quindi nella casella **Descrizione** immettere una descrizione per la linea di prodotti. Ad esempio, All products in the Fashion category will be included in the discount.

1. Nella parte superiore della pagina scegliere **Gruppi di prezzi** dal menu.

1. Nella pagina Gruppi di prezzi selezionare il menu **Gruppo di prezzi**.

1. Analizzare i gruppi di prezzi disponibili, selezionare **Boston price group** e quindi selezionare **Salva**.

1. Nell'angolo in alto a destra della pagina Gruppi di prezzi selezionare l'icona **Chiudi**.

1. Nella scheda Dettagli della pagina Sconti selezionare il menu **Stato** e quindi **Abilitato**.

1. Osservare che non è più possibile modificare le impostazioni dello sconto.

1. Salvare le modifiche e quindi chiudere la pagina Sconto.

1. Nella pagina Gestione prezzi e sconti esaminare la scheda Sconti attivi e verificare che il nuovo sconto aggiunto sia visualizzato nella parte inferiore dell'elenco.

1. Se necessario, in alto a destra selezionare l'icona **Aggiorna** per aggiornare l'elenco di sconti.
