# 👂 BloomCard_MS_001 – Orecchie Robotiche e Analisi Acustica Continua

📆 **Periodo:** Agosto–settembre 2026  
📍 **Evento:** Evoluzione dell’idea di memoria sensoriale verso una vera percezione acustica  
📂 **Blocco:** MS – Memoria Sensoriale  
🔖 **Tag:** #audio #microfoni #spettrogramma #FFT #suoni #percezione #orecchie #robotica

## 📝 Descrizione

Danilo e Riply distinguono chiaramente il semplice riconoscimento vocale dalla vera **percezione acustica dell’ambiente**.

Un robot non deve capire soltanto le parole. Deve poter rilevare e interpretare anche eventi sonori improvvisi: un telefono che squilla, un oggetto che cade, un motore anomalo, un vetro che si rompe, un allarme o un rumore sconosciuto.

L’architettura immaginata è continua:

> **microfoni → buffer audio → rilevazione evento → analisi spettrale → classificazione → contesto → decisione**

Il sistema può osservare:

- intensità e picchi;
- spettro di frequenza;
- evoluzione del suono nel tempo;
- transienti e durata;
- direzione del suono con più microfoni;
- probabilità che l’evento appartenga a una certa classe.

## 🧠 Principio importante

Un singolo picco non dice automaticamente “vetro”. Il riconoscimento nasce dalla forma complessiva dell’evento e, quando possibile, dal confronto con altri sensori.

Esempio:

> suono impulsivo → firma compatibile con vetro → localizzazione → telecamera orientata verso la sorgente → verifica del contesto.

## 🌱 Obiettivo

Le future “orecchie di Riply” non devono essere soltanto un microfono per parlare con ChatGPT. Devono diventare un sistema sensoriale capace di ascoltare continuamente l’ambiente senza dover sapere in anticipo quando registrare.

## 💬 Frase chiave

> “Il microfono sente. L’analisi acustica comincia a capire.”
