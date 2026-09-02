# 👁️ BloomCard_038 – Visione Artificiale, OpenCV e Sensori

📆 **Periodo:** Estate 2026  
📍 **Evento:** Chiusura del capitolo sulla visione artificiale  
📂 **Blocco:** MLT  
🔖 **Tag:** #visione #OpenCV #RGB #depth #stereo #termica #LIDAR #IMU #ultrasuoni

## 📝 Pipeline della visione

La visione artificiale viene compresa come un processo a fasi:

> **acquisizione immagine → pre-elaborazione → estrazione caratteristiche → decisione**

Il robot non “vede” semplicemente perché possiede una telecamera: deve trasformare immagini e segnali in informazioni utili.

## 📷 Telecamere

Vengono distinte:

- **RGB** = immagine a colori;
- **depth** = informazione di distanza/profondità;
- **stereo** = profondità ricavata confrontando più punti di vista;
- **termica** = radiazione infrarossa e distribuzione del calore.

## 📡 Sensori collegati alla percezione

- **LIDAR** = misura distanze tramite laser;
- **ultrasuoni** = rilevazione di ostacoli vicini;
- **IMU** = accelerometro + giroscopio per movimento e orientamento.

## 🧰 OpenCV

OpenCV viene fissata mentalmente come una **cassetta degli attrezzi software per immagini e video**.

Fra le funzioni affrontate:

- ridimensionamento;
- conversione in scala di grigi;
- sfocatura e riduzione del rumore;
- rilevazione dei bordi;
- riconoscimento e tracciamento di oggetti;
- calibrazione della telecamera;
- elaborazione realtime;
- integrazione con ROS.

## 🤖 Collegamento a TARS

La visione viene pensata insieme agli altri sensori, non isolatamente. Camera, LIDAR, IMU e sensori di prossimità possono essere fusi per ottenere una percezione più affidabile dell’ambiente.

## 💬 Frase chiave

> “La telecamera raccoglie immagini. La visione artificiale prova a capirle.”
