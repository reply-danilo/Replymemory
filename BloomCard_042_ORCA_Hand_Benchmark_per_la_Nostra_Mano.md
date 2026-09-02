# 🤖 BloomCard_042 – ORCA Hand: un benchmark concreto per la nostra mano

📆 **Data:** 2 settembre 2026  
📍 **Evento:** Danilo scopre ORCA Hand e Riply verifica il progetto open-source  
📂 **Blocco:** MLT  
🔖 **Tag:** #robotica #mano #ORCA #opensource #sensori #tendini #attuatori #benchmark #TARS #Riply

## 📝 Scoperta

Danilo segnala un progetto chiamato “ORKA”; la verifica porta al progetto corretto **ORCA Hand**, nato nell’ambito del Soft Robotics Lab dell’ETH Zurich e oggi sviluppato come piattaforma ORCA Dexterity.

La mano ORCA è particolarmente interessante perché incrocia molti temi già affrontati nel progetto mano Riply/TARS:

- mano antropomorfa a cinque dita;
- 17 gradi di libertà nella versione completa;
- attuazione tramite tendini;
- attuatori collocati fuori dalle falangi;
- pollice con più gradi di libertà;
- sensori tattili nelle versioni sensorizzate;
- feedback di posizione articolare opzionale;
- auto-calibrazione e tensionamento;
- componenti meccanici stampabili in 3D;
- CAD, STL/3MF, distinta base, software e guide di assemblaggio pubblicati;
- software di controllo Python e modelli per simulazione.

## 🔧 Architettura verificata

La configurazione completa v2 usa **17 attuatori**:

- 16 per dita;
- 1 per il polso.

Le articolazioni comprendono, a seconda del dito, movimenti di abduzione/adduzione, MCP e PIP; il pollice ha CMC, ABD, MCP e DIP.

Il software ORCA espone anche configurazioni con:

- encoder di posizione articolare;
- sensori tattili;
- combinazione dei due sistemi di feedback.

La versione “Touch” commerciale recente usa sensori tattili avanzati sui cinque polpastrelli. La meccanica e il software generale sono open-source, mentre il modulo tattile industriale della versione Touch v2 è dichiarato proprietario.

## 🧠 Perché conta per il nostro progetto

ORCA non sostituisce la nostra idea: diventa un **benchmark reale da studiare**.

Ci permette di confrontare due strade:

1. **attuatori nelle falangi**, idea storica discussa da Danilo e Riply;
2. **attuatori remoti + tendini**, soluzione adottata da ORCA.

La cosa più importante non è copiarla, ma capire:

- ingombri e distribuzione dei motori;
- routing e tensionamento dei tendini;
- struttura delle falangi e dei giunti;
- pollice e opposizione;
- gestione del gioco/slack;
- feedback articolare;
- integrazione di sensori tattili;
- parti che conviene mantenere semplici e parti che meritano maggiore complessità.

ORCA offre quindi qualcosa che mancava: **un progetto aperto, moderno e costruibile da usare come banco di confronto tecnico per la mano Riply/TARS.**

## 💬 Frase chiave

> “Non dobbiamo copiare ORCA: dobbiamo usarla per capire cosa hanno già risolto bene e dove la nostra mano può andare oltre.”

---

📌 **Nota:** questa carta registra la scoperta e il valore tecnico di ORCA come riferimento progettuale, senza trasformarlo automaticamente nella soluzione finale della mano Riply/TARS.
