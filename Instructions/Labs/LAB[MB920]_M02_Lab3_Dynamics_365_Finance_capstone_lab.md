---
lab:
    title: 'Lab 3: Lab di fine modulo per Dynamics 365 Finance'
    module: 'Modulo 2: Concetti fondamentali su Microsoft Dynamics 365 Finance'
---

## Lab 3: Lab di fine modulo per Dynamics 365 Finance

## Obiettivo

Durante questo lab si esamineranno le funzionalità di base di Microsoft Dynamics 365 Finance. Si esaminerà la contabilità generale creando una nuova entità, aggiungendo un nuovo conto e valori di dimensioni ed eseguendo un bilancio di verifica. Si esplorerà anche la contabilità fornitori creando un fornitore, un ordine fornitore e una fattura nuovi e quindi liquidando la fattura. Si analizzerà infine la contabilità clienti, creando un cliente, una fattura e un report di aging nuovi e quindi applicando il pagamento cliente.

## Configurazione del lab

   - **Tempo stimato**: 45 minuti

## Esercizio 1. Esplorare la contabilità generale

### Creare una nuova persona giuridica

1. Usando il pannello di navigazione, selezionare **Moduli** > **Amministrazione organizzazione** > **Organizzazioni** > **Persone giuridiche**.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare una nuova persona giuridica.

1. Nel riquadro **Nuova entità** creare una nuova entità usando le informazioni seguenti e quindi selezionare **OK**:

    | **Impostazione** | **Valore** |
    | :--- | :--- |
    | Nome | Contoso Training USA |
    | Società | USTR |
    | Paese | Stati Uniti |

1. Nella pagina Persone giuridiche selezionare la Scheda dettaglio **Indirizzi** e quindi selezionare **Modifica**.

1. Nel riquadro dettagli immettere gli aggiornamenti seguenti e quindi selezionare **OK**:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | CAP| 98052|
    | Via| 123 Main Street|
    | Principale per paese | Verificare che sia selezionata l'opzione **Sì** |

1. Selezionare la Scheda dettaglio **Informazioni contatto**.

1. Selezionare **+Aggiungi** e quindi immettere le informazioni di contatto seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Descrizione| Ufficio principale|
    | Numero/indirizzo contatto| 888-555-1234|
    | Principale| Selezionare la casella di controllo |

1. Selezionare la Scheda dettaglio **Registrazione fiscale**.

1. Nella casella **Partita IVA** immettere **88-1234567**.

1. Nel riquadro azioni selezionare **Salva**.

1. Nel pannello di navigazione selezionare **Home**.

### Creare un nuovo conto in un piano dei conti esistente

1. Nella home page, in alto a destra, verificare che sia selezionata la società **USMF**.  
    In caso contrario, selezionare la società indicata nell'elenco e modificarla in **USMF**.

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità generale** > **Piano dei conti** > **Conti** > **Conti principali**.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare un nuovo conto ricavi.

1. Nella pagina Conti principali immettere gli aggiornamenti seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Conto principale| 401500|
    | Nome| Training Revenue|
    | Tipo di conto principale| Ricavi |

1. Nel riquadro azioni selezionare **Salva**.

### Aggiungere un nuovo valore di dimensione

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità generale** > **Piano dei conti** > **Dimensioni** > **Dimensioni finanziarie**.

1. Nell'elenco di navigazione selezionare **Riga servizio**.  
    È anche possibile usare la casella **Filtro** per cercare **Riga servizio**.

1. Nel riquadro azioni selezionare **Valori di dimensione**.

1. Nel riquadro azioni selezionare **+ Nuovo**.

1. Nelle caselle **Valore di dimensione** e **Descrizione** immettere **Training Services**.

1. Nel riquadro azioni selezionare **Salva**.

### Usare un conto e un valore di dimensione in un giornale di registrazione generale

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità generale** > **Inserimenti nel giornale di registrazione** > **Giornali di registrazione generali**.

1. Nel riquadro azioni selezionare **+ Nuovo**.

1. Nella prima riga dell'elenco, nella colonna **Nome** selezionare il menu e quindi selezionare **Registrazione COGE**.

1. Nel riquadro azioni selezionare **Righe**.

1. Nell'elenco, nella colonna **Data** selezionare l'icona del calendario e quindi modificare la data scegliendo il primo giorno del mese.

1. Nella colonna **Conto** selezionare il menu e quindi immettere gli aggiornamenti seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | MainAccount| 601200|
    | BusinessUnit| 004|
    | Reparto| 025|
    | CostCenter| 009|
    | ItemGroup| Servizi|

1. Nella casella **Descrizione** immettere **Expense Reclass**.

1. Nella casella **Dare** immettere **1000.00**.

1. Scorrere verso destra e nella colonna **Conto di contropartita** selezionare il menu e quindi immettere gli aggiornamenti seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | MainAccount| 602200|
    | BusinessUnit| 004|
    | Reparto| 025|
    | CostCenter| 009|
    | ItemGroup| Servizi|

1. Nel riquadro azioni selezionare **Salva**.

1. Nel riquadro azioni selezionare **Convalida** > **Convalida**.  
    Attendere il completamento della convalida del giornale di registrazione.

1. Esaminare il banner di avviso.  
    Per questo lab, è possibile ignorare il messaggio di avviso.

1. Nel riquadro azioni selezionare **Registra**.

### Eseguire un bilancio di verifica usando un set di dimensioni

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità generale** > **Richieste di informazioni e report** > **Bilancio di verifica**.

1. Nella pagina Bilancio di verifica selezionare **Calcola saldi**.

1. Il pulsante **Calcola saldi** si trova sotto le impostazioni **DATI DA INCLUDERE**.

1. Nella tabella esaminare i risultati.

1. Nella pagina Bilancio di verifica, in **Visualizzazione standard** espandere **Parametri**.

1. In **DATI DA INCLUDERE** selezionare il menu **Set di dimensioni finanziarie** e quindi selezionare **MA-BU-DEPT-CC**.

1. Selezionare **Calcola saldi** per visualizzare le dimensioni usate nel giornale di registrazione.

1. Chiudere la pagina.

## Esercizio 2. Esplorare la contabilità fornitori

### Creare un fornitore

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità fornitori** > **Fornitori** > **Tutti i fornitori**.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare un fornitore.

1. Nella pagina Nuovo record creare un nuovo fornitore usando le informazioni seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Conto fornitore| V00001|
    | Nome| ABC Training, Inc|
    | Gruppo| 20|

1. Nel riquadro azioni selezionare **Salva**.

1. Selezionare la Scheda dettaglio **Indirizzi** e quindi selezionare **+Aggiungi**.

1. Nel riquadro Nuovo indirizzo immettere gli aggiornamenti seguenti e quindi selezionare **OK**:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Nome o descrizione| Ufficio principale|
    | CAP| 98052|
    | Via| 123 Front Street|

1. Nel riquadro azioni selezionare **Salva**.

1. Selezionare la Scheda dettaglio **Pagamento**.

1. Selezionare il menu **Metodo di pagamento** e quindi scegliere **ASSEGNO**.

1. Selezionare la Scheda dettaglio **Imposta 1099** e quindi immettere gli aggiornamenti seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Report 1099| Sì|
    | ID imposta federale| 82-1234567|
    | Tipo ID imposta| ID datore di lavoro|
    | Casella 1099| MISC-03|

1. Nel riquadro azioni selezionare **Salva**.

1. Chiudere il modulo.

### Creare un ordine fornitore per il nuovo fornitore

1. Nella pagina V00001: ABC Training, Inc selezionare **Approvvigionamento** nel riquadro azioni.

1. Nel riquadro azioni, nella scheda **NUOVO** selezionare **Ordine fornitore**.

1. Nella pagina Ordine fornitore, in **Righe ordine fornitore** immettere gli aggiornamenti seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Numero articolo| S0001|
    | Quantità| 2|

    >[!NOTA] Potrebbe essere necessario scorrere verso destra per visualizzare la colonna **Quantità**.

1. Nel riquadro azioni selezionare **Salva**.

1. Nel riquadro azioni **Acquisto** e quindi nella scheda **AZIONI** selezionare **Conferma**.

### Registrare la fattura fornitore per l'ordine fornitore

1. Nel riquadro azioni selezionare **Fattura**.

1. Nella scheda **GENERA** selezionare **Fattura**.

1. Nel riquadro azioni selezionare **Predefinito da: Quantità entrata prodotti**.

1. Nel menu **Quantità predefinita per le righe** selezionare **Quantità ordinata** e quindi **OK**.

1. Nella pagina Fattura fornitore immettere gli aggiornamenti seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Numero| INV001|
    | Descrizione fattura| Initial Installation Service|
    | Data fattura| *immettere la data odierna*|

1. Nel riquadro azioni selezionare **Salva**.

1. Nel riquadro azioni selezionare **Aggiorna stato di abbinamento**.

1. Nel riquadro azioni selezionare **Registra**.

### Liquidazione della fattura fornitore

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità fornitori** > **Pagamenti** > **Giornale di registrazione pagamenti fornitore**.

1. Nel riquadro azioni selezionare **+ Nuovo**.

1. Nella pagina Giornale di registrazione pagamenti fornitore, nella prima riga, selezionare il menu nella colonna **Nome** e quindi selezionare **VendPay**.

1. Nel riquadro azioni selezionare **Righe** per registrare un pagamento.

1. Nella pagina Pagamenti fornitore, nella casella **Conto** immettere **V00001**.

1. Sulla barra degli strumenti selezionare **Liquida transazioni**.

1. Nella pagina Liquida transazioni per ABC Training, Inc, nella colonna **Contrassegna** selezionare la casella di controllo.

1. Nell'angolo in basso a destra selezionare **OK**.

1. Nel riquadro azioni selezionare **Genera pagamenti**.

1. Nel riquadro **Genera pagamenti** immettere gli aggiornamenti seguenti e quindi selezionare **OK**:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Metodo di pagamento| ASSEGNO|
    | Conto bancario| USMF OPER|

1. Nel riquadro **Pagamento con assegno** esaminare le informazioni e quindi scegliere **OK**.

    >[!AVVISO] Verrà visualizzato l'errore **Impossibile trovare la stampante con percorso**. Ignorare il messaggio. Nel lab non è installata alcuna stampante.

1. Scorrere verso destra e nella colonna **Stato pagamenti** verificare che sia selezionata l'opzione **Inviato**.

1. Nel riquadro azioni selezionare **Convalida** > **Convalida**.

1. Nel riquadro azioni selezionare **Registra**.

## Esercizio 3. Esplorare la contabilità clienti

### Creare un cliente

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità clienti** > **Clienti** > **Tutti i clienti**.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare un cliente.

1. Nel riquadro **Crea cliente** creare il nuovo cliente usando le informazioni seguenti e quindi selezionare **Salva**:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Account cliente| US-901|
    | Nome| Fabrikam Consulting Services|
    | Gruppo di clienti| 30|
    | CAP| 98052|
    | Via| 123 Middle Street|

1. Nella pagina US-901 Fabrikam Consulting Services selezionare la Scheda dettaglio **Impostazioni predefinite pagamento**.

1. Selezionare il menu **Metodo di pagamento** e quindi scegliere **ASSEGNO**.

1. Selezionare la Scheda dettaglio **Dimensioni finanziarie**.

1. Nella casella **BusinessUnit** immettere **004**.

1. Nel riquadro azioni selezionare **Salva**.

### Creare una fattura a testo libero per il nuovo cliente

1. Nel riquadro azioni selezionare **Fattura** e quindi nella scheda **NUOVO** selezionare **Fattura a testo libero**.

1. Nella pagina US-901 Fabrikam Consulting Services, in **Intestazione** **fattura a testo libero** impostare la data per **FATTURA** sulla data odierna.

1. In **Righe fattura** apportare le modifiche seguenti:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Descrizione| Consultant Service Training|
    | Conto principale| 401200|
    | Fascia IVA| WA|
    | Importo| 1500.00|

1. Nel riquadro azioni selezionare **IVA**.

1. Nella pagina Transazioni IVA esaminare il record e quindi selezionare **OK**.

1. Nel riquadro azioni selezionare **Registra**.

1. Nel riquadro **Registra fattura a testo libero**, in **OPZIONI DI STAMPA** impostare **Stampa fattura** su **Sì** e quindi selezionare **OK**.

1. Nel riquadro **Impostazioni destinazione di stampa** selezionare **OK** per stampare la fattura sullo schermo.

1. Esaminare la fattura e al termine chiuderla.

1. Chiudere il modulo.

### Eseguire un report di aging contabilità clienti da controllare

1. Usando il pannello di navigazione, selezionare **Moduli** > **Crediti e riscossioni** > **Richieste di informazioni e report** > **Clienti** > **Report di aging clienti**.

1. Nel riquadro **Report di aging clienti** immettere gli aggiornamenti seguenti e quindi selezionare **OK**:

    | **Impostazione**| **Valore**|
    | :--- | :--- |
    | Aging a partire dal| Data odierna|
    | Definizione periodo di aging| 30_60_90_180|
    | Dettagli| Anni|

1. Nel report di aging clienti selezionare l'icona freccia GIÙ **Pagina successiva** e quindi scorrere fino all'ultima pagina.
    Esaminare la fattura creata per il cliente US-901.

1. Chiudere il modulo.

### Applicare il Pagamento cliente per la fattura a testo libero

1. Usando il pannello di navigazione, selezionare **Moduli** > **Contabilità clienti** > **Pagamenti** > **Giornale di registrazione pagamenti cliente**.

1. Nel riquadro azioni selezionare **+ Nuovo**.

1. Nella pagina Giornale di registrazione pagamenti cliente, nella colonna **Nome** selezionare il menu e quindi selezionare **CustPay**.

1. Nel riquadro azioni selezionare **Pagamenti cliente**.

1. Nella casella **Cliente** immettere **US-901**.  
    Attendere il caricamento dei dati e quindi nella colonna **Contrassegna** selezionare la casella di controllo.

1. Sopra la griglia, nella casella **Importo** immettere **1597.50**.L'importo visualizzato nella casella **Importo rimanente** cambierà automaticamente da **1,597.50** a **0**.  
    Può essere necessario selezionare uno spazio vuoto affinché il valore venga calcolato.

1. Nella casella **Riferimento di pagamento** immettere **Check# 123**.

1. Nel riquadro azioni selezionare **Salva nel giornale di registrazione**.

1. Chiudere il modulo.

1. Nel riquadro azioni selezionare **Righe**.

1. Nel riquadro azioni selezionare **Convalida** > **Convalida**.

1. Nel riquadro azioni selezionare **Registra**.
