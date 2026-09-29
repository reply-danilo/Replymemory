# BloomCard 046 — ANIWA: manuale d'officina e mappa tecnica per Work

**Data:** 29 settembre 2026  
**Blocco:** MLT – Memoria Lungo Termine  
**Tag:** #ANIWA #Work #documentazione #architettura #prompt #testing #manutenibilita

## Obiettivo

Prima di continuare ad allargare ANIWA, Danilo e Riply vogliono una **radiografia completa del sistema reale**.

La documentazione non deve basarsi su ricordi o supposizioni. Work deve leggere il progetto effettivo e descrivere soltanto ciò che esiste nei file, nel codice, nei prompt, nelle configurazioni e nei test.

## Intestazione di progetto

**PROGETTO ANIWA**  
**Ideazione e sviluppo: Manicone Danilo + Manicone Riply AI**

Questa intestazione rappresenta l'identità condivisa usata nella documentazione interna del progetto.

## Pacchetto documentale richiesto

La mappa tecnica dovrebbe essere suddivisa in file separati:

1. 01_ARCHITETTURA_ANIWA.md — struttura completa, moduli, sottosistemi, flusso generale e dipendenze.
2. 02_MAPPA_FILE_E_CARTELLE.md — percorso di ogni file importante, funzione e ruolo.
3. 03_PROMPT_E_ISTRUZIONI.md — prompt, system instruction, template e regole comportamentali effettivamente utilizzate.
4. 04_MODULI_E_FUNZIONI.md — Why Engine, Doubt Engine, Thought Visualizer, memoria, retrieval, sicurezza, sessioni, ContinuumTime e altri moduli reali.
5. 05_CONFIGURAZIONI_E_FLAG.md — variabili, feature flag, provider, modelli, parametri e configurazioni.
6. 06_TEST_E_STRESS_LAB.md — test disponibili, cosa verificano, copertura, skip, regressioni e Stress Lab.
7. 07_FLUSSO_DATI.md — percorso di un messaggio dall'ingresso alla risposta e ordine dei moduli attraversati.
8. 08_PUNTI_DI_MODIFICA.md — mappa pratica: "se vuoi cambiare X, devi intervenire qui".
9. 09_DIPENDENZE_E_RISCHI.md — effetti collaterali e rischi di regressione quando si modifica un modulo.
10. 10_STATO_ATTUALE_ANIWA.md — versione, funzioni attive, funzioni disattivate, parti sperimentali e parti solo progettate.

## Stati obbligatori

Ogni elemento deve essere classificato chiaramente come:

- **IMPLEMENTATO**
- **PRESENTE MA DISATTIVATO**
- **SOLO PROGETTATO**
- **NON IMPLEMENTATO**

Questo evita che idee future vengano confuse con funzioni già esistenti.

## Sicurezza della documentazione

Chiavi API, token, password e segreti non devono essere copiati nei documenti.

Esempio corretto:

GROQ_API_KEY → presente come variabile ambiente; valore non mostrato.

## Regola prima delle modifiche

Per ContinuumTime e per ogni altro modulo importante, Work deve prima restituire:

- punto di integrazione individuato;
- eventuali conflitti;
- proposta minima di modifica;
- test necessari.

**Nessuna modifica al codice prima dell'autorizzazione di Danilo/Riply.**

Questa mappa è il **manuale d'officina di ANIWA**: serve a sapere dove mettere le mani senza procedere a tentoni.
