# ENTREGA-N-4.

# Pre-Entrega-4 

# 🏦 Trabajo Final: Ingenia-2025  
## Detección de fraudes en transacciones bancarias

---

### 👥 Integrantes Grupo 4
- Carpio , Vanessa
- Huber , Anne Kathrin
- Siarri , Maria Florencia

---

## 📖 Introducción
Este proyecto es parte del **Trabajo Final** del curso de **Data Science** dictado por Fundación YPF en 2025.  
El pago en línea es el método de transacción más popular en el mundo, pero su auge trae consigo un incremento de fraude.  
El objetivo de este análisis es identificar **pagos fraudulentos** y **no fraudulentos** a partir de un conjunto de datos histórico proveniente de Kaggle.

---

## 🎯 Objetivos
1. Desarrollar un **modelo** que detecte transacciones potencialmente fraudulentas.  
2. Analizar distintos tipos de transacciones (`CASH-IN`, `CASH-OUT`, `DEBIT`, `PAYMENT`, `TRANSFER`).  
3. Explorar comportamientos según:
   - Montos
   - Días y horarios
   - Cuentas afectadas y destinos de las transferencias  

---

## 🗄️ Descripción del Dataset
- **Origen**: Kaggle  
- **Tamaño**: CSV de más de 493 MB (se aloja en GitLab para facilitar la descarga).  
- **Variables (11):**  
  1. `step` – unidad de tiempo (1 hora; 744 pasos = 31 días).  
  2. `type` – tipo de transacción (`CASH-IN`, `CASH-OUT`, `DEBIT`, `PAYMENT`, `TRANSFER`).  
  3. `amount` – monto en moneda local.  
  4. `nameOrig` – cliente que inicia la transacción.  
  5. `oldbalanceOrg` – saldo inicial del origen.  
  6. `newbalanceOrig` – saldo después de la transacción.  
  7. `nameDest` – cliente/destino de la transacción.  
  8. `oldbalanceDest` – saldo inicial del destino (no aplica a comerciantes “M…”).  
  9. `newbalanceDest` – saldo después en destino (no aplica a “M…”).  
  10. `isFraud` – indicador de fraude real.  
  11. `isFlaggedFraud` – marcado si monto > 200 000 en una sola transacción.  


---


## 🧹 Limpieza de Datos
1. **Carga** del CSV  
2. **Visualización** inicial  
3. **Identificación** de tipos de variable  
4. Dimensiones: **filas y columnas**  
5. **Estadística descriptiva**  
6. Detección y **eliminación de nulos**  
7. Función **`discrep`** para outliers  
8. Conteo de registros por tipo  
9. Boxplot y **histogramas**  
10. **Matriz de correlación**  
11. **transformación de datos** (normalización, encoding de variables categóricas).
12. **Modelado y optimización de hiperparametros**
13. **Evaluación de los modelos**

---

## 🚀 Metodología
- **Lenguaje , librerías y modelos **:  
  - Python: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`,`RandomForestClassifier`,`scipy`,`sklearn.ensemble`,`XGboost`,
    
- **Pasos**:  
  1. Preprocesamiento y limpieza  
  2. Ingeniería de características  
  3. Selección y evaluación de modelos (RandomForest, XGBoost, redes neuronales…)  
  4. Validación cruzada y métricas  
  5. Interpretación de resultados  

---

## 🛠️ Herramientas
- Google Colab  
- Jupyter Notebook  
- GitHub / GitLab  
- Excel (exploración rápida)  

---

## 🔗 Enlaces útiles
- 🔍 Dataset en Kaggle:  
  https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset  

