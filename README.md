# 🧠 Proiect Data Science cu Spark, MLlib, TensorFlow și Streaming

Acest proiect implementează un flux complet de analiză a datelor folosind Apache Spark, în combinație cu tehnici de Machine Learning (ML), Deep Learning (DL) și procesare în timp real prin Spark Streaming.  

## 📌 Cerințe și Rezolvare

---

### ✅ 2. Procesarea și transformarea datelor cu Spark (DataFrames + Spark SQL)

- ✔️ Curățarea datelor (detectarea și eliminarea valorilor `null` și duplicate)
- ✔️ Grupări și agregări folosind:
  - ✅ `groupBy()` + `.agg()` cu `avg`, `count`
  - ✅ Spark SQL (`createOrReplaceTempView`, `spark.sql(...)`)
- ✔️ Exerciții:
  - Procentul bolnavilor de inimă în funcție de gen
  - Procent în funcție de presiune arterială și diabet
  - Grupare pe categorii de vârstă

---

### ✅ 3. Aplicarea a două metode ML (MLlib)

- ✔️ Clasificare binară cu Logistic Regression
- ✔️ Clasificare cu Random Forest (opțional)
- ✔️ Fiecare metodă include:
  - ✅ Enunțul problemei și justificarea
  - ✅ Construirea pipeline-ului cu `StringIndexer`, `VectorAssembler`, `Pipeline`
  - ✅ Împărțirea datelor în `train/test` (70%/30%)
  - ✅ Evaluare cu `BinaryClassificationEvaluator` (AUC)

---

### ✅ 4. Utilizarea unui Data Pipeline

- ✔️ Implementare completă cu `Pipeline` din `pyspark.ml`
- ✔️ Etape: Indexare → Asamblare vectori → Antrenare model → Predictie

---

### ✅ 5. Utilizarea UDF + Optimizare hiperparametri

- ✔️ UDF definit și folosit pentru preprocesare (ex. transformare categorii)
- ✔️ Optimizare cu `ParamGridBuilder` și `CrossValidator` (`numFolds=5`)

---

### ✅ 6. Aplicarea unei metode DL (TensorFlow)

- ✔️ Antrenare model DL folosind TensorFlow (Sequential + Dense)
- ✔️ Evaluare model cu `accuracy`, `loss`
- ✔️ Datele procesate în Spark au fost convertite în Pandas pentru DL

---

### ✅ 7. Spark Streaming 🛰️

- ✔️ Proces de streaming cu `readStream`
- ✔️ Aplicație simplă: citirea datelor din fișier CSV cu streaming
- ✔️ Aplicarea unui model ML deja antrenat pentru inferență în timp real
- ✔️ ✅ Bonus: Se poate adapta ușor pentru camere video sau alte surse distribuite

---

## 📦 Tehnologii utilizate

- 🔥 Apache Spark (DataFrames, SQL, MLlib, Streaming)
- 🤖 TensorFlow
- 📈 Pandas, Matplotlib, Seaborn
- 🐍 Python 3.11

---