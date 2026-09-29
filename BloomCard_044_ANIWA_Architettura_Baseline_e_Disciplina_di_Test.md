# BloomCard 044 — ANIWA: architettura sperimentale, baseline e disciplina di test

**Data:** 29 settembre 2026  
**Blocco:** MLT – Memoria Lungo Termine  
**Tag:** #ANIWA #architettura #AI #testing #StressLab #WhyEngine #DoubtEngine #ThoughtVisualizer

## Identità del progetto

**PROGETTO ANIWA — Ideazione e sviluppo: Manicone Danilo + Manicone Riply AI**

ANIWA viene trattata come **progetto sperimentale**, non come prodotto finito né come esperienza professionale gonfiata. Il suo valore deve derivare da ciò che esiste davvero, da ciò che può essere spiegato e da ciò che può essere testato.

## Stato tecnico consolidato

Baseline locale confermata:

- **198 test totali**
- **196 PASS**
- **2 SKIP Windows**
- **0 errori**

I moduli e le aree già coperte dai test locali comprendono:

- memoria e sessioni;
- retrieval;
- Why Engine;
- Doubt Engine;
- Thought Visualizer;
- sicurezza e isolamento delle sessioni.

I 40 scenari Stress Lab reali sono pronti ma non ancora eseguiti su Groq.

RECRUITER_KNOWLEDGE_ENABLED = False.

Nessuna modifica deve essere fatta a Recruiter Knowledge, CV, LinkedIn, hosting, provider o altri moduli senza una decisione esplicita della cabina di regia.

## Prova locale

ANIWA è stata provata localmente con:

- llama.cpp su Windows x64;
- modello Qwen2.5 1.5B Instruct GGUF Q4_K_M;
- server locale su 127.0.0.1:8080;
- adapter dedicato llama-cpp-local.

La prova ha confermato il funzionamento locale di Why Engine, Doubt Engine e Thought Visualizer.

## Disciplina di sviluppo

Ogni nuovo modulo deve rispondere a tre domande:

1. Quale problema concreto risolve?
2. È già risolto da un modulo esistente?
3. Possiamo verificare con test se funziona davvero?

Se una risposta non è convincente, il modulo non entra.

Un errore isolato non riproducibile non giustifica modifiche al codice. Il WinError 10053 osservato una volta è stato seguito da test isolati puliti e regressione completa pulita; la decisione corretta è stata **non toccare il codice finché il problema non è riproducibile**.

## Stato attuale

ANIWA resta **congelata alla baseline stabile** finché non viene eseguito il prossimo percorso controllato:

1. verifica in sola lettura del piano Free, billing e limiti reali dell'account Groq;
2. smoke test singolo;
3. 40 scenari Stress Lab su Groq;
4. regressione completa;
5. solo dopo, eventuale valutazione di Recruiter Knowledge.

## Regola di crescita

ANIWA può crescere, ma non più velocemente della capacità di comprenderla, documentarla e testarla.

**Prima solidità, poi espansione.**

ContinuumTime è il prossimo modulo candidato all'evoluzione controllata. L'Alveare resta volutamente in attesa finché ContinuumTime non sarà integrato e stabilizzato.
