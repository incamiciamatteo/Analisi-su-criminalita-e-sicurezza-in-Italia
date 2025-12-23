# Analisi della Criminalità e della Situazione Carceraria in Italia (2008-2023)

## 📌 Obiettivo del Progetto
Questo progetto analizza l'evoluzione della sicurezza e della giustizia in Italia attraverso tre lenti: la **criminalità reale** (denunce), la **percezione del rischio** da parte delle famiglie e la **risposta del sistema sanzionatorio** (popolazione carceraria). L'analisi copre un arco temporale di 15 anni, evidenziando come eventi straordinari, riforme legislative e dinamiche sociali abbiano modellato il panorama attuale.

---

## 📈 Analisi delle Serie Storiche e Fenomeni Chiave

Dall'analisi dei dati ISTAT emergono evidenze cruciali che spiegano le fluttuazioni dei grafici:

### 1. L'Effetto Pandemia e il "Rimbalzo" (2020-2022)
* **Crollo dei reati predatori:** Il grafico dei furti e delle rapine mostra un minimo storico nel biennio 2020-2021. Le restrizioni alla mobilità (Lockdown) hanno drasticamente ridotto le opportunità per i reati di strada.
* **Recupero post-Covid:** A partire dal 2022, si osserva una risalita dei reati che sta riportando le statistiche verso i livelli pre-pandemici, confermando che il calo era un'anomalia congiunturale e non un trend strutturale di lungo periodo.

### 2. La Dinamica degli Omicidi: Il "Gender Gap"
Confrontando le vittime per genere emerge una divergenza sociale allarmante:
* **Calo Maschile:** Gli omicidi con vittime maschili (spesso legati a criminalità organizzata o comune) sono crollati drasticamente dal 2008 a oggi, seguendo il trend di calo dei reati gravi.
* **Resilienza Femminile:** Al contrario, il numero di vittime femminili rimane tragicamente costante (linea "piatta" nella serie storica). Questo evidenzia come la violenza di genere sia un fenomeno strutturale che non risponde alle fluttuazioni della criminalità generale.

### 3. Sistema Carcerario: Riforme e Sovraffollamento
La curva della popolazione carceraria riflette la storia legislativa del paese:
* **Condoni e Sentenza Torreggiani:** Il netto calo dei detenuti intorno al 2010 e la stabilizzazione (2013-2015) riflettono l'impatto dei provvedimenti "svuota-carceri" e delle sentenze CEDU che hanno imposto all'Italia standard minimi di vivibilità.
* **Emergenza 2030:** Esaurito l'effetto di quelle riforme, l'indice di affollamento è tornato a crescere. Le proiezioni integrate nel modello stimano il superamento di quota **72.000 detenuti entro il 2030**, un valore che riporterebbe il sistema ai livelli di massima criticità del 2008.

---

## 📊 Principali Evidenze (Dati 2023)
* **Volume di reati:** Circa **963K furti** e **26K rapine** denunciati.
* **Percezione del rischio:** Campania (34%) e Lazio (32%) sono le regioni dove le famiglie percepiscono il rischio maggiore, dato coerente con l'alto tasso di criminalità pro-capite.
* **Popolazione carceraria:** 56K detenuti totali (69% italiani, 31% stranieri). In regioni come la Liguria, la quota di detenuti stranieri è proporzionalmente più alta rispetto alla media nazionale.

---

## 🛠️ Data Pipeline & Metodologia

Il progetto segue un flusso di lavoro che separa la preparazione del dato dalla visualizzazione:

1.  **Data Ingestion & Cleaning (Python):** La pulizia e manipolazione dei dati ISTAT sono state effettuate esternamente per garantire massima precisione:
    * **Pandas & Numpy:** Utilizzati per gestire dataset complessi, normalizzare i nomi dei territori e gestire i valori mancanti nelle serie storiche storiche.
    * **Feature Engineering:** Calcolo dei tassi pro-capite (indici per 100 abitanti o 100.000 residenti) per rendere confrontabili regioni con popolazioni diverse (es. Lombardia vs Molise).
2.  **Data Modeling (Power BI):** Architettura a stella per collegare tabelle dei fatti (reati, detenuti) con tabelle dimensionali (calendario, geografia, demografia).
3.  **Analisi Previsionale:** Implementazione di modelli di forecasting per stimare la pressione sulle infrastrutture carcerarie nei prossimi anni.
4.  **UI/UX Design:** Dashboard interattiva con navigazione tra pagine tematiche e funzionalità di *drill-through* per il dettaglio regionale (es. il focus sulla regione Toscana).

---

## 💡 Conclusioni dell'Analista
L'analisi suggerisce che, mentre l'Italia è diventata oggettivamente più sicura in termini di volumi totali di reati comuni, la pressione sul sistema carcerario sta tornando a livelli d'allerta. Inoltre, l'invarianza del dato sugli omicidi femminili sottolinea la necessità di politiche di contrasto specifiche che vadano oltre la gestione della sicurezza pubblica tradizionale.

---
