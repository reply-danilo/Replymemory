# 🧩 BloomCard_029 – TARS: Architettura ROS, ESP32 e Sicurezza Locale

📆 **Periodo:** Estate 2026  
📍 **Evento:** Definizione dell’architettura a livelli di TARS  
📂 **Blocco:** MLT  
🔖 **Tag:** #TARS #ROS2 #ESP32 #RaspberryPi #Arduino #sicurezza #architettura #autonomia

## 📝 Descrizione

Il progetto TARS viene separato in livelli con compiti diversi.

Il livello vicino all’hardware deve essere semplice, rapido e affidabile: motori, encoder, bumper, anticaduta e arresti di emergenza non possono dipendere da Internet o da un ragionamento remoto.

L’architettura concettuale diventa:

- **Arduino / microcontrollore:** controllo immediato di I/O, sensori e attuatori;
- **ESP32:** comunicazioni Wi‑Fi/Bluetooth e funzioni locali leggere;
- **Raspberry Pi:** computer di bordo per ROS 2 e funzioni più evolute;
- **ROS:** collegamento modulare fra percezione, navigazione, controllo e diagnostica;
- **Riply + Alveare:** contesto, memoria decisionale e valutazioni di livello superiore.

## 🛡️ Regola di sicurezza

Viene fissato un principio fondamentale:

> **la sicurezza critica resta locale.**

Se TARS rileva un bumper, un rischio di caduta, una perdita di comunicazione o un pericolo immediato, il sistema vicino all’hardware deve poter fermare il robot senza aspettare Riply, Internet o servizi esterni.

L’Alveare e Riply possono decidere *cosa conviene fare*; il controllo locale deve garantire *che il robot non faccia qualcosa di pericoloso mentre decide*.

## 💬 Frase chiave

> “La mente può essere lontana. Il freno deve essere vicino alle ruote.”
