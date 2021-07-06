---
lab:
    title: 'Lab 2: Creare un assortimento di prodotti'
    module: 'Modulo 3: Concetti fondamentali su Microsoft Dynamics 365 Commerce'
---

## Lab 2: Creare un assortimento di prodotti

## Obiettivi

È necessario creare un assortimento di prodotti correlati assegnati a un canale di Commerce specifico che verrà reso disponibile in una data futura.

## Configurazione del lab

   - **Tempo stimato**: 10 minuti

## Istruzioni

1. Nella pagina Finance and Operations, in alto a sinistra, selezionare il menu hamburger **Espandere il pannello di navigazione**.

1. Nel pannello di navigazione selezionare **Vendita al dettaglio e commercio** > **Cataloghi e assortimenti** > **Assortimenti**.

1. Attendere il caricamento della pagina.

1. Nella pagina Assortimenti selezionare **+ Nuovo**.

1. Nel riquadro Nuovo record espandere **Generale**.

1. Selezionare la casella **Data di validità** e quindi selezionare una data futura.

1. Nella casella **Nome assortimento** immettere un nome per il nuovo assortimento. Ad esempio, **New Spring Season**.

1. Impostare **Data di scadenza** su **Mai**.

1. La data di scadenza può essere usata per disattivare automaticamente un assortimento pubblicato.

1. Espandere **Commerce channels** (Canali di Commerce).

1. Nel menu relativo ai canali di Commerce selezionare **+ Aggiungi riga**.

1. In Scegli nodi organizzazione selezionare il menu **Gerarchia organizzativa** e quindi selezionare **Punti vendita al dettaglio per tipo (Fabrikam)**.

1. Nell'elenco NODI ORGANIZZAZIONE DISPONIBILI selezionare Online e quindi selezionare l'icona Aggiungi ![Icona freccia DESTRA](./media/d365-fo-add-org-node-icon.png) per l'aggiunta in **NODI ORGANIZZAZIONE SELEZIONATI**.  
  In questo modo verranno aggiunti il nodo padre e tutti i nodi figlio.

1. Aggiungere il nodo padre **Mall** e quindi selezionare **OK**.

1. Verificare che siano stati aggiunti due nodi ai canali di Commerce.

1. Espandere **Prodotti**.

1. Nel menu Prodotti selezionare **+ Aggiungi riga**.

1. Selezionare il menu **Categoria**, selezionare **Team Sports (Team Sports)** e quindi selezionare **OK**.

1. In questo modo verranno aggiunti tutti gli articoli figlio della categoria padre.

1. Esaminare l'ultima colonna denominata **Tipo di riga**. Per impostazione predefinita, verranno inclusi tutti gli articoli.

1. Selezionare **+ Aggiungi riga**, selezionare il menu **Categoria**, espandere **Team Sports (Team Sports)**, selezionare **Baseball** e quindi selezionare **OK**.

1. Per escludere un articolo da una categoria più ampia già inclusa, in questo caso Team Sports, nella colonna Tipo di riga modificare il valore in **Escludi**.

1. Usando la riga della categoria Baseball, selezionare il menu **Prodotti**.

1. Quando vengono definiti i prodotti di una categoria, è possibile selezionare un prodotto specifico da includere o escludere. Selezionare **AdultBaseballInfield**.

1. Per rimuovere un prodotto aggiunto, eliminare i contenuti della casella del prodotto e quindi premere TAB o selezionare un'altra area nella pagina.

1. Nel menu in alto selezionare **Salva**.

1. Nel menu in alto selezionare **Pubblica**.

1. Esaminare le informazioni nella finestra di dialogo e quindi selezionare **Sì**.

1. Il nuovo assortimento di prodotti creato diventerà disponibile a partire dalla data di validità.
