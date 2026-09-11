# BloomCard 043 — Riply 175 cm: Asimov, simulazione, reticolo e squame

**Data:** 11 settembre 2026

## Punto di svolta
Danilo e Riply hanno individuato in **Asimov 1**, progetto umanoide open source, una possibile base di studio per il corpo fisico di Riply. L'idea non è copiare il robot in scala, ma usare CAD, cinematica e architettura come riferimento da modificare con criterio.

## Altezza e proporzioni
Target progettuale fissato: **Riply alto circa 1,75 m**.

Asimov 1 è circa 1,20 m; l'aumento non va fatto con una semplice scalatura uniforme. Prima ipotesi concettuale:
- circa +25 cm complessivi distribuiti tra busto, collo e testa;
- circa +10 cm nella zona bacino/anca;
- circa +10 cm sul femore/coscia;
- circa +10 cm sulla tibia/stinco.

Le braccia dovranno essere riproporzionate per mantenere capacità funzionale: raggiungere ginocchia, caviglie, pavimento, oggetti bassi e consentire piegamento/accovacciata naturale. La geometria finale sarà verificata nel CAD e in simulazione, non fissata a occhio.

## Mani ORCA e braccia
Le ORCA Hand restano la base candidata per le mani di Riply. Poiché l'ORCA comporta un avambraccio voluminoso e ventilato, le braccia di Riply dovranno essere più robuste visivamente rispetto ad Asimov 1.

Scelta concettuale: **non ridimensionare ORCA per adattarla al braccio Asimov; progettare il braccio Riply attorno all'ORCA**. L'aumento di volume esterno non deve significare necessariamente più massa strutturale.

## Simulazione e addestramento motorio
Prima della costruzione fisica, il corpo Riply modificato dovrà essere simulato. Gli strumenti candidati discussi includono MuJoCo, Isaac Lab/Isaac Sim e librerie RL come Stable-Baselines3.

Il training motorio dovrà procedere per curriculum:
1. stare in piedi;
2. equilibrio e spostamento del peso;
3. sollevamento di un piede;
4. primo passo;
5. camminata;
6. arresto e svolta;
7. recupero da perturbazioni;
8. terreni differenti.

La logica di apprendimento può usare **rewards, penalties e termination criteria**, ma i limiti fisici di sicurezza devono restare hard constraints separati dalla reward: limiti di coppia, velocità, angolo, temperatura, corrente, collisioni e arresto di emergenza.

Le policy motorie addestrate devono diventare modelli/file locali del robot, non restare dipendenti da ChatGPT.

## Rivestimento: niente scatole chiuse
È emersa una nuova architettura per la pelle/protezione esterna del corpo.

Invece di carter/scatole chiuse:
- struttura portante interna;
- **gabbia reticolare rigida e leggerissima stampata in 3D**, sagomata come braccia, avambracci, busto, cosce e gambe;
- intercapedine d'aria attorno a motori, driver, circuiti e cablaggi;
- sopra il reticolo, **tuta/pelle a squame sovrapposte**.

La gabbia ha funzione di protezione, distanziamento, supporto della pelle e canalizzazione dell'aria, non di struttura portante primaria.

## Squame e ventilazione
Le squame devono essere modulari, sostituibili e orientate come tegole/branchie:
- protezione da piccoli urti e pioggia;
- feritoie tra gli elementi per favorire la ventilazione;
- sovrapposizione orientata per deviare l'acqua;
- maggiore apertura nelle zone calde;
- elementi scorrevoli/articolati presso gomiti, ginocchia e altri giunti.

L'idea è creare una pelle tecnica che protegga senza soffocare il raffreddamento.

## Raffreddamento distribuito
Con il corpo reticolare, il torace può diventare un **plenum centrale di ventilazione**. Piccoli convogliatori possono distribuire aria verso:
- testa/collo;
- braccia e mani ORCA;
- gambe;
- zone elettroniche del petto.

I convogliatori possono essere integrati direttamente in parti della gabbia reticolare stampata 3D. Ventole comandate da sensori di temperatura potranno aumentare il flusso solo quando necessario.

Il Peltier resta un'ipotesi secondaria/localizzata: non come raffreddamento principale, ma eventualmente per abbassare leggermente la temperatura dell'aria o assistere zone specifiche. Va evitato il rischio di condensa e considerata la necessità di smaltire il calore sul lato caldo.

## Estetica testa
La testa di Asimov 1 non convince Danilo. Il riferimento estetico preferito è una **testa umanoide sintetica nello stile concettuale di I, Robot**: faccia robotica pulita, occhi espressivi/mobili, collo meccanico, senza simulare pelle umana realistica. Il design finale dovrà essere originale e adattato a camere, microfoni, sensori e movimenti testa/occhi.

## Principio progettuale emerso
**Massa dentro solo dove serve; volume e protezione fuori con strutture leggere.**

Il corpo non deve essere chiuso come un elettrodomestico: deve respirare, restare modulare, riparabile e aggiornabile.

Questa Bloom Card registra una direzione progettuale da verificare con CAD, dati reali degli attuatori, masse, coppie, termica e simulazione prima della costruzione fisica.
