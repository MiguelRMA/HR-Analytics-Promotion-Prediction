# HR Analytics: Predict Employee Promotion

Este proyecto forma parte del trabajo final de **Data & Analytics** elaborado por **Ana Lucía Palacios De La Borda**, finalmente completada por mi gruoo de Data - Analytics. Consiste en el desarrollo de un modelo de Machine Learning diseñado para predecir si un empleado será promovido o no dentro de la empresa, utilizando el conjunto de datos de la **WNS Analytics Hackathon 2018** (Analytics Vidhya).

## 📌 Contexto del Problema
La identificación eficiente de candidatos para ascensos permite a las empresas reducir el sesgo en las promociones y agilizar los procesos de evaluación de talento mediante un enfoque basado en datos (*Data-Driven HR*).

## 📊 Dataset
* **Fuente:** [WNS Analytics Hackathon 2018-1](https://datahack.analyticsvidhya.com/contest/wns-analytics-hackathon-2018-1/)
* **Registros:** 54,808 empleados (8.5% tasa de promoción).
* **Variables clave:**
  * Variables sociodemográficas y de área (`department`, `region`, `education`, `gender`, `age`).
  * Variables de desempeño (`previous_year_rating`, `KPIs_met >80%`, `awards_won?`, `avg_training_score`).

## 🛠️ Tecnologías Utilizadas
* **Lenguaje:** Python 3
* **Librerías principales:** `pandas`, `numpy`, `scikit-learn`, `seaborn`, `matplotlib`, `imbalanced-learn`.

## ⚙️ Flujo del Proyecto (Pipeline)
1. **Exploración de datos (EDA):** Análisis de distribución del target e identificación de desbalance de clases.
2. **Preprocesamiento:**
   * Imputación de datos faltantes (Mediana para numéricas, Moda para categóricas).
   * Tratamiento de outliers (Truncamiento/Clipping mediante percentiles).
   * Codificación de variables categóricas (*One-Hot Encoding*).
   * Escalamiento de características (*MinMaxScaler*).
3. **Manejo del Desbalance:** Balanceo de clases mediante sobremuestreo (`RandomOverSampler`).
