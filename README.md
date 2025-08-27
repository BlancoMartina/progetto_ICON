# 🧠 Sistema di Supporto alla Diagnosi del Diabete

Questo progetto integra tecniche di **Intelligenza Artificiale simbolica** (sistemi esperti basati su regole) e di **Machine Learning supervisionato** per supportare la diagnosi del diabete.  
Il sistema è stato sviluppato come progetto accademico e combina una **knowledge base** con modelli predittivi allenati su dataset reali.


## 📝 Descrizione del Progetto
Il sistema è in grado di:
- Porre **domande all’utente** e, tramite un sistema esperto rule-based, generare proposizioni (*facts*) utili al processo diagnostico.  
- Applicare **algoritmi di classificazione supervisionata** sui dati clinici per predire la probabilità di diabete.  
- Integrare una **base di conoscenza strutturata** (ontologia) e semplici **CSP (Constraint Satisfaction Problem)** per la gestione di vincoli, come ad esempio la disponibilità dei laboratori.  

---

## 🏗 Architettura del Sistema
L’architettura si compone di tre moduli principali:
1. **Sistema esperto (rule-based)**: realizzato con la libreria `Experta`, gestisce fatti e regole per produrre diagnosi logiche.  
2. **Modulo di Machine Learning**: implementato con `scikit-learn`, comprende modelli supervisionati per la classificazione.  
3. **Gestione CSP e Ontologie**: utilizzando le librerie `constraint` e `Owlready2`, il sistema è in grado di ragionare su vincoli e concetti strutturati del dominio.  

---

## 📊 Dataset
È stato utilizzato il dataset **Pima Indians Diabetes Database**, disponibile su Kaggle:  
👉 [Link al dataset](https://www.kaggle.com/uciml/pima-indians-diabetes-database)

Le feature considerate includono:
- Concentrazione di glucosio  
- Pressione arteriosa diastolica  
- Spessore della piega cutanea  
- Livelli di insulina sierica  
- BMI (Body Mass Index)  
- Funzione pedigree del diabete  
- Età  

La variabile target (*Outcome*) indica la presenza o meno di diabete.

---

## 🤖 Algoritmi Utilizzati
Gli algoritmi implementati e confrontati sono:
- 🌳 **Decision Tree**  
- 📈 **Regressione Logistica**  
- 👥 **K-Nearest Neighbors (K-NN)**  

Il confronto delle performance è stato effettuato tramite:
- Matrici di confusione  
- Metriche: *accuracy, precision, recall, F1-score*  