---
lab:
    title: 'Lab 1: Lab di fine modulo per Dynamics 365 Human Resources'
    module: 'Modulo 4: Concetti fondamentali su Microsoft Dynamics 365 Human Resources'
---

## Lab 1: Lab di fine modulo per Dynamics 365 Human Resources

## Obiettivo

In questo lab si esaminerà il processo di inserimento di un nuovo dipendente, inclusa la creazione di un record dipendente. Si esaminerà anche il processo di verifica delle prestazioni che comprende la definizione di un obiettivo e la valutazione delle prestazioni. Si useranno inoltre le funzionalità self-service per inviare una nota spese.

## Configurazione del lab

- **Tempo stimato**: 20 minuti 

## Esercizio 1. Esplorare Human Resources

### Creare un nuovo record di assunzione

1. Usando il pannello di navigazione, selezionare **Moduli** > **Risorse umane** > **Posizioni** > **Posizioni**.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare una nuova posizione.

1. Nella finestra di dialogo **Crea nuova posizione** selezionare il menu **Mansione** e quindi selezionare **Responsabile punto vendita**.

1. Selezionare **Crea posizione**.

1. Usando il pannello di navigazione, selezionare **Moduli** > **Lavoratori** > **Dipendenti**.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare un nuovo dipendente.

1. Nel riquadro **Assumi nuovo lavoratore** immettere gli aggiornamenti seguenti e quindi selezionare **Hire and add details** (Assumi e aggiungi dettagli).

    | **Impostazione** | **Valore** |
    | :--- | :---- |
    | Nome | Bill |
    | Cognome | Smith |
    | Data di inizio impiego | Selezionare la data corrente|

### Creare un obiettivo per la nuova assunzione

1. Nel riquadro azioni selezionare **Lavoratore**.

1. Nella scheda **SVILUPPO** selezionare **Obiettivi**.

1. Potrebbe essere necessario scorrere verso destra per visualizzare la scheda.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare un nuovo obiettivo.

1. Nella Scheda dettaglio **Generale** immettere gli aggiornamenti seguenti:

    | **Impostazione** | **Valore** |
    | :--- | :---- |
    | Nome | Quarterly Sales Goal |
    | Panoramica | Help the store team reach the quarterly sales goal. |
    | Categoria obiettivo | Vendite |
    | Data di inizio | Selezionare una data a una settimana dalla data corrente |
    | Data di fine | Selezionare una data due settimane dopo la data di inizio |

1. Nel riquadro azioni selezionare **Salva**.

1. Chiudere la pagina Quarterly Sales Goal.

1. Chiudere la pagina Obiettivi | Bill.

### Assegnare un corso di formazione alla persona neoassunta

1. Nella pagina Dipendenti per Bill, nel riquadro azioni selezionare **Lavoratore**

1. Nella scheda **COMPETENZE** selezionare **Corsi**.

1. Potrebbe essere necessario scorrere verso destra per visualizzare la scheda.

1. Nel riquadro azioni selezionare **+ Nuovo** per creare un nuovo corso.

1. In visualizzazione Griglia, nella colonna **ID corso** selezionare il menu e quindi scegliere **00004**.

1. Nella finestra di dialogo **Trasferire i dati del corso?** selezionare **Sì**.

1. Nella colonna **Data di inizio** selezionare l'icona del calendario e quindi scegliere la data corrente.

1. Nella colonna **Data di fine** selezionare l'icona del calendario e quindi scegliere una data a due settimane da quella corrente.

1. Nel riquadro azioni selezionare **Salva**.

1. Chiudere la pagina Corsi | Bill.

### Creare una nota spese

1. Usando il pannello di navigazione, selezionare **Moduli** > **Risorse umane** > **Aree di lavoro** > **Dipendente self-service**.

1. Nella sezione **My career information** (Informazioni carriera), nel riquadro **Spese** selezionare **Nuovo report**.

1. Nel riquadro **Nuova nota spese** selezionare il menu **Scopo**, scegliere **Formazione** e quindi selezionare **OK**.

1. Nella griglia **Spese**, nella riga per la nuova spesa immettere gli aggiornamenti seguenti:

    | **Impostazione** | **Valore** |
    | :--- | :---- |
    | Data transazione | Selezionare la data odierna |
    | Categoria di spesa | Noleggio auto |
    | Esercente | LitWare Travel |
    | Importo transazione | 150.00 |

1. Usando la macchina virtuale del lab, aprire **Blocco note**.

1. Nel corpo di Blocco note immettere **LitWare Travel receipt**.

1. Salvare il file sul desktop come **Receipt.txt** e quindi chiudere Blocco note.

1. Questo file verrà usato come ricevuta da allegare alla nota spese.

1. Tornare alla scheda del browser relativa a Microsoft Dynamics 365 Finance and Operations.

1. Nel riquadro azioni selezionare **Entrate intestazioni**.

1. Nel riquadro **Entrate intestazioni** selezionare **Carica e collega nuova ricevuta**.

1. Selezionare **Sfoglia**.

1. Selezionare il file **Receipt.txt** creato in precedenza e quindi scegliere **Apri**.

1. Nella casella **Note** immettere **Car rental** e quindi selezionare **Carica**.

1. Selezionare la casella di controllo **Ricevuta** e quindi scegliere **Seleziona righe**.

1. Nel riquadro **Allega ricevute a righe** selezionare la casella di controllo per **150.00 LitWare Travel** e quindi scegliere **OK**.

1. Selezionare **Chiudi**.

1. Nel riquadro azioni selezionare **Flusso di lavoro** e quindi scegliere **Invia**.

1. Nel riquadro **Nota spese - USMF - Invia**, nella casella **Commenti** immettere **Please review my expense report**.

1. Selezionare **Invia**.

### Registrare una registrazione prestazioni

1. Usando il pannello di navigazione, selezionare **Moduli** > **Risorse umane** > **Prestazioni** > **Registrazione prestazioni**

1. Nel riquadro azioni selezionare **+ Nuovo**.

1. Nella pagina **Nuovo giornale di registrazione** immettere gli aggiornamenti seguenti.


    | **Impostazione** | **Valore** |
    | :--- | :---- |
    | Titolo | Attended Training |
    | Descrizione | Completed business training for Store Manager |
    | Persona | Bill Smith |
    | Data di completamento | Data odierna |

1. Nel riquadro azioni selezionare **Salva**.

1. Nel riquadro azioni selezionare **Aggiungi a obiettivo**.

1. Selezionare **Quarterly Sales Goal** e quindi scegliere **OK**.

1. Chiudere la pagina Registrazione prestazioni.
