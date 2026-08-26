# ✋ BloomCard_026 – Mano Robotica: Nocche Attive e Pelle Sensoriale

📆 **Periodo:** Agosto 2026  
📍 **Evento:** Evoluzione dell’idea della mano robotica partendo da una mano articolata in PVC  
📂 **Blocco:** MLT  
🔖 **Tag:** #manorobotica #PVC #tendini #attuatori #nocche #polso #sensori #guanto #modulare

## 📝 Descrizione

Una semplice mano articolata in PVC diventa il punto di partenza per molte architetture diverse.

La prima idea è utilizzare la mano come scheletro già pronto e inserire tendini/pull-wire per flettere le dita. Questa soluzione riduce il peso sulle falangi, ma richiede di progettare con attenzione percorsi, guide, attriti, tensionamento e ritorno delle dita.

Osservando meglio le sfere/nocche passive della mano nasce una seconda strada:

> **sostituire il giunto passivo con un giunto attivo motorizzato nello stesso punto.**

In questo modo le falangi esistenti restano al loro posto e la geometria del dito è già definita. Il problema principale diventa trovare o costruire un attuatore abbastanza piccolo, leggero e potente da occupare il volume della nocca.

Per le falangi, il movimento può essere semplificato a un asse principale; non serve necessariamente un vero motore sferico 3-DOF.

## 🖐️ Il palmo

Se gli attuatori stanno nelle nocche, il palmo può diventare soprattutto una zona elettronica:

- microcontrollore o piccola scheda di controllo;
- driver degli attuatori;
- distribuzione di alimentazione e dati;
- connessione con i sensori della pelle esterna.

La mano diventa così un modulo quasi autonomo collegato al corpo attraverso il polso.

## 🧤 Pelle sensoriale sostituibile

L’idea del guanto non scompare con gli attuatori nelle nocche.

Il guanto resta una **pelle sensoriale separata e sostituibile**, con:

- sensori di pressione su polpastrelli e palmo;
- sensori di temperatura;
- cablaggi sottili sul dorso della mano;
- un unico collegamento verso il polso quando possibile.

L’obiettivo è separare chiaramente:

> **struttura e movimento dentro — sensibilità fuori.**

## 🔄 Polso

Osservando la sfera del polso della mano in PVC nasce anche l’idea di usare un giunto sferico attivo o una struttura multi-asse compatta per ottenere un movimento più naturale, senza rotazione continua a 360°.

## 💬 Frase chiave

> “Non rifare la mano: motorizzare la mano che esiste già.”

---

📌 **Nota:** questa carta conserva entrambe le strade — tendini e nocche attive — senza dichiarare prematuramente una soluzione vincente.
