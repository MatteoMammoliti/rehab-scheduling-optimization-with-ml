# 🏥 Ottimizzazione delle Schedulazioni ASP dei Turni Riabilitativi mediante Predizioni di Machine Learning
*Un approccio neuro-simbolico per i turni di riabilitazione integrando Machine Learning e Answer Set Programming (ASP).*

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Engineering-150458.svg)
![Machine Learning](https://img.shields.io/badge/Machine_Learning-Regression-FF6F00.svg)
![ASP](https://img.shields.io/badge/Solver-Answer_Set_Programming-success.svg)

## 📌 Descrizione del Progetto
Questo repository contiene il codice sorgente e la pipeline di dati sviluppata per il mio progetto di tesi. L'obiettivo principale è superare i limiti computazionali dei classici risolutori logici (come ASP) nella schedulazione ospedaliera, integrandoli con modelli predittivi basati sui dati.

Attraverso algoritmi di regressione, il modello stima il numero di assegnamenti giornalieri (`totalAssignments`) nei reparti di riabilitazione, analizzando la complessità clinica dei pazienti e la disponibilità degli operatori, fungendo da "oracolo" per ottimizzare il carico di lavoro della struttura.

## 🗂️ Struttura del Repository
```text
├── data/
│   ├── raw/                  # Dataset originali grezzi (JSON)
│   ├── processed/            # Design Matrix pulita e aggregata (CSV)
├── notebooks/                
│   ├── 01_EDA_and_Outliers.ipynb  # Analisi di correlazione (Pearson) e Boxplot (IQR)
│   ├── 02_Model_Training.ipynb    # Addestramento e validazione (Train/Test cronologico)
├── src/                      
│   ├── data_engineering.py   # Script di parsing, deduplicazione e feature extraction
│   └── utils.py              # Funzioni di supporto
├── requirements.txt          # Dipendenze del progetto
└── README.md
