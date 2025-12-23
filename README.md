# 📊 Criminalità e Sicurezza in Italia (2008-2023)
### Analisi statistica, modellazione predittiva e Business Intelligence

<p align="center">
  <img src="Images/Logo Team/Logo_DATI_per_spacciati.png" alt="Logo Team DATI per spacciati" width="300">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
  <img src="https://img.shields.io/badge/Source-ISTAT-E12C2C?style=for-the-badge&logoColor=white" alt="ISTAT Red Badge">
</p>

---

## 📝 Overview del Progetto
L'obiettivo di questo progetto è fornire un resoconto scientifico e oggettivo della **sicurezza pubblica in Italia**, basato sull'analisi dei dati ufficiali **ISTAT**. Lo studio analizza la situazione attuale dei reati e del sistema carcerario, con una visione granulare focalizzata sulle **singole regioni italiane**.

Il workflow integra **Data Engineering** per il trattamento dei dati, **Data Science** per l'analisi dei trend e **Business Intelligence** per visualizzare fenomeni sociali complessi e il loro impatto sul territorio.

---

## 📈 Sintesi dello Storytelling Scientifico
L'indagine analizza criticamente l'andamento della sicurezza nazionale attraverso tre direttrici:

1.  **Analisi Regionale dei Reati (2008-2023):** Studio quantitativo dei reati denunciati, con focus su **furti, rapine e omicidi**. La mappatura regionale permette di osservare le variazioni storiche e l'impatto di fattori esterni (es. lockdown 2020) sulle diverse aree del Paese.
2.  **Evoluzione del Sistema Carcerario:** Un'analisi della popolazione detenuta che valuta l'equilibrio tra la componente italiana e quella straniera. L'attenzione è posta sugli indici di sovrappopolazione e sulla capacità ricettiva delle strutture regionali.
3.  **Predictive Modeling - Orizzonte 2030:** Utilizzo della modellazione statistica per prevedere il ritorno della popolazione carceraria a **livelli di pressione strutturale**. Lo studio evidenzia la necessità di interventi sistemici entro il prossimo decennio per prevenire criticità legate alla saturazione delle strutture.

---

## 🛠️ Metodologia e Workflow Tecnico

### 1. Data Engineering (Python)
* **Data Shaping & Unpivoting:** Consolidamento dei dataset ISTAT (Popolazione Residente, Popolazione Straniera, Criminalità e sicurezza) per garantire la massima granularità regionale (v. file [unpivot_df_powerbi.csv](./unpivot_df_powerbi.csv)).
* **Normalizzazione:** Calcolo delle misure pro-capite per rendere i dati confrontabili tra regioni con diverse densità demografiche.

### 2. Modellazione Predittiva (Validazione Scientifica)
In questa fase è stata applicata la **Regressione Lineare** per proiettare i dati al 2030. Seguendo un approccio rigoroso:
* **Detenuti Totali e Stranieri:** I modelli hanno mostrato rilevanza statistica e sono stati utilizzati per le predizioni (v. file [df_con_predizioni.csv](./df_con_predizioni.csv)).
* **Rischio Percepito:** Nonostante il tentativo di modellazione, i risultati sulla percezione della popolazione non sono risultati statisticamente significativi; pertanto, per correttezza scientifica, sono stati esclusi dalle predizioni finali.

### 3. Business Intelligence (Power BI)
* **Logica DAX:** Utilizzo di misure personalizzate per ricavare dati complementari non presenti nei dataset originali (es. calcolo derivato della popolazione e dei detenuti di nazionalità italiana) e per la gestione delle metriche pro-capite regionali.
* **Storytelling Interattivo:** Dashboard progettata per esplorare i dati di ogni regione, facilitando l'identificazione di trend locali e il confronto tra criminalità reale e percezione del rischio.

---

## 📂 Struttura della Repository

* 📂 [**Python**](./Python/) : Il core tecnico con il codice di Data Cleaning e Machine Learning ([Criminalità e sicurezza.ipynb](./Criminalità%20e%20sicurezza.ipynb)).
* 📂 [**CSV**](./Data/CSV/) : I file CSV pronti per l'analisi (tra cui `unpivot_df_powerbi.csv` e `df_con_predizioni.csv`).
* 📂 [**Power BI**](./Power%20BI/) : Il file sorgente `.pbix` per Power BI.
* 📂 [**Images**](./Images/) : Loghi del team, asset grafici e documentazione visiva dei risultati.

---

## 👥 Il Team: "DATI per spacciati"

* **Fabio De Bartolomeo** [GitHub](https://github.com/debaef)
* **Matteo Incamicia** [GitHub](https://github.com/incamiciamatteo)
* **Alessio Massaro** [GitHub](https://github.com/saiba12)
* **Fernanda Macchiarella** [GitHub](https://github.com/)
* **Giuseppe Esposito** [GitHub](https://github.com/giuseppeesposito98-cmd)
