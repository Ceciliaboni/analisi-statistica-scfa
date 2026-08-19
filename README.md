# Analisi Statistica degli Acidi Grassi a Catena Corta (SCFA)

### Studio multi-malattia su campioni paralleli di plasma e feci

Questa repository contiene l'analisi statistica sviluppata per la mia tesi di Laurea Triennale in Statistica presso l'Università degli Studi di Firenze durante l'Anno Accademico 2024/2025.

Lo studio analizza le concentrazioni di sette acidi grassi a catena corta (SCFA) misurate in campioni di plasma e feci provenienti da quattro gruppi clinici.

Gli obiettivi principali sono:

- confrontare le concentrazioni di SCFA tra i diversi gruppi clinici;
- valutare la loro capacità discriminante rispetto alle diverse condizioni cliniche;
- indagare la relazione tra le concentrazioni di SCFA plasmatiche e fecali.

---

## Gruppi Clinici

L'analisi prende in esame quattro gruppi clinici:

- **CD** — Celiachia (Celiac Disease)
- **CRC** — Carcinoma del colon-retto (Colorectal Cancer)
- **HC** — Controlli sani (Healthy Controls)
- **Obesi** — Obesità

Per ciascun paziente, le concentrazioni dei sette SCFA sono state misurate sia su campioni plasmatici che fecali.

---

## Metodologie Statistiche

L'analisi comprende:

- Statistica descrittiva
- Analisi di correlazione
- Analisi delle Componenti Principali (PCA)
- Analisi dei Cluster Gerarchica (Hierarchical Cluster Analysis)
- Metodo di Ward
- Test di Kruskal-Wallis
- Test post-hoc di Dunn
- Regressione Logistica Multinomiale
- Cross-Validation 10-fold
- Analisi Discriminante Lineare di Fisher (LDA)

Questi metodi sono stati impiegati per indagare le differenze tra i gruppi clinici e valutare il potere discriminante delle concentrazioni di SCFA.

---

## Risultati Principali

L'analisi evidenzia che **le concentrazioni plasmatiche di SCFA risultano più informative rispetto a quelle fecali nella discriminazione tra i gruppi clinici**.

In particolare, le misurazioni plasmatiche garantiscono una separazione più netta dei controlli sani rispetto ai gruppi patologici.

L'analisi di regressione logistica multinomiale identifica inoltre l'**acido valerico** come biomarcatore significativamente associato all'appartenenza ai gruppi clinici nei dati plasmatici.

Il modello congiunto su dati plasmatici e fecali fornisce buone prestazioni di classificazione, pur senza mostrare un incremento sostanziale rispetto al modello basato unicamente sul plasma.

La cluster analysis gerarchica basata sul metodo di Ward non separa completamente tutti e quattro i gruppi clinici, sebbene i campioni plasmatici e fecali mostrino informazioni tra loro complementari.

---

## Flusso di Lavoro dell'Analisi (Workflow)

```text
Dati
 │
 ├── Campioni di plasma
 │
 └── Campioni di feci
        │
        ▼
Analisi Esplorativa
        │
        ├── Statistica descrittiva
        ├── Correlazioni
        └── PCA
        │
        ▼
Cluster Analysis
   └── Metodo di Ward
        │
        ▼
Confronto tra Gruppi
   ├── Kruskal-Wallis
   └── Test di Dunn
        │
        ▼
Regressione Logistica Multinomiale
   ├── Plasma
   ├── Feci
   └── Dati combinati
        │
        ▼
Cross-Validation 10-Fold
        │
        ▼
Classificazione
   └── LDA di Fisher
```
## Tecnologie

L'analisi è stata sviluppata in **R**.

Le principali metodologie statistiche e tematiche affrontate nel progetto sono:

- Inferenza statistica
- Analisi esplorativa dei dati (EDA)
- Analisi multivariata
- Analisi delle Componenti Principali (PCA)
- Cluster analysis
- Classificazione
- Regressione logistica
- Analisi Discriminante Lineare (LDA)
- Cross-validation
- Data visualization

---

## Struttura della Repository
```text
.
├── README.md
├── analisi.R
└── tesi.pdf
```
- ```analisi.R``` — Script R contenente l'intera pipeline di analisi statistica..
- ```tesi.pdf``` — Tesi di laurea completa.
- ```README.md``` — Tesi di laurea completa.
---
## Contesto Accademico

**Corso di Laurea Triennale in Statistica**
Università degli Studi di Firenze
Scuola di Economia e Management

**Anno Accademico**: 2024/2025

**Titolo della tesi**:

*Un'analisi statistica degli acidi grassi a catena corta: studio multi-malattia su due campioni paralleli*

**Relatore**: Prof. Francesco Claudio Stingo

**Autrice**: Cecilia Boni
