---
lab:
    title: 'Lab 1: Creare una dimensione finanziaria'
    module: 'Modulo 2: Concetti fondamentali su Microsoft Dynamics 365 Finance'
---

## Lab 1: Creare una dimensione finanziaria

## Obiettivi

Usare la pagina Dimensioni finanziarie per creare dimensioni finanziarie che è possibile usare come segmenti di conto per i piani dei conti. Esistono due tipi di dimensioni finanziarie: dimensioni personalizzate e dimensioni supportate da entità. Le dimensioni personalizzate sono condivise tra persone giuridiche e i valori vengono immessi e gestiti dagli utenti. Per le dimensioni supportate da entità, i valori vengono definiti in un'altra posizione nel sistema, ad esempio nelle entità Clienti o Punti vendita. Alcune dimensioni supportate da entità sono condivise tra persone giuridiche, mentre altre sono specifiche della società.

È necessario creare una dimensione finanziaria personalizzata che verrà usata dalla società.

## Configurazione del lab

   - **Tempo stimato**: 5 minuti

## Istruzioni

1. Nella home page Finance and Operations, in alto a destra, verificare di lavorare con la società USMF.

1. Se necessario, selezionare la società e scegliere **USMF** dal menu.

1. Nel pannello di navigazione a sinistra selezionare **Moduli** > **Contabilità generale** > **Piano dei conti** > **Dimensioni** > **Dimensioni finanziarie**.

1. Nel menu superiore selezionare **+ Nuovo**.

1. Nella pagina Dimensioni finanziarie selezionare il menu **Usa valori da** e quindi selezionare **< Dimensione personalizzata >**.

1. Nella casella **Nome dimensione** immettere **Affliate_Revenue**.

1. Nella casella **Nome colonna report** immettere **Afflt**.

1. Nel menu in alto selezionare **Attiva**.

    ![Screenshot che mostra la nuova dimensione finanziaria personalizzata con gli elementi Usa valori da, Nome dimensione, Nome colonna report e Attiva evidenziati](./media/lp2-m3-new-financial-dimension.png)

1. Esaminare le informazioni nella finestra di dialogo e quindi selezionare **Chiudi**.

1. Esaminare il banner di notifica di avviso.

    ![Screenshot che mostra il banner di informazioni di avviso che fa riferimento al requisito della modalità manutenzione per l'attivazione di una nuova dimensione.](./media/lp2-m3-activation-warning-banner.png)

    >[!NOTA] La modalità manutenzione può essere attivata e disattivata direttamente tramite Lifecycle Services (LCS) negli ambienti sandbox e di produzione. Per altre informazioni sulla gestione di Lifecycle Services, vedere [https://docs.microsoft.com/it-it/dynamics365/fin-ops-core/dev-itpro/deployment/maintenanceoperationsguide-newinfrastructure](https://docs.microsoft.com/it-it/dynamics365/fin-ops-core/dev-itpro/deployment/maintenanceoperationsguide-newinfrastructure).
