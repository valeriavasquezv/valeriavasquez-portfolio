
# 📊 Proyecto ETL – Análisis de Evasión de Clientes (Churn)

## 🧠 Introducción

La evasión de clientes (**Churn**) es uno de los principales desafíos en empresas de telecomunicaciones, ya que impacta directamente en los ingresos y la sostenibilidad del negocio.

El objetivo de este proyecto es desarrollar un **proceso ETL (Extract, Transform, Load)** que permita preparar datos confiables y validarlos mediante un análisis exploratorio enfocado en churn.

---

## 🎯 Objetivo del Proyecto

- Implementar un pipeline ETL completo.
- Limpiar y transformar datos de clientes.
- Corregir inconsistencias y errores.
- Preparar un dataset listo para análisis.
- Identificar patrones asociados a la evasión de clientes.

---

## 🔄 Proceso ETL

### 1️⃣ Extract (Extracción)
- Carga del dataset original.
- Revisión de estructura, columnas y tipos de datos.
- Identificación de datos anidados y campos complejos.

---

### 2️⃣ Transform (Transformación)

Durante esta etapa se realizaron las siguientes acciones:

- Limpieza de valores vacíos en la variable `Churn`.
- Normalización de variables categóricas.
- Conversión de variables numéricas:
  - `Charges.Monthly`
  - `Charges.Total`
- Manejo de valores nulos.
- Validación de tipos de datos.
- Selección de variables relevantes para el análisis.

Resultado: **dataset final limpio y consistente (`df_final`)**.

---

### 3️⃣ Load (Carga)

- Dataset final listo para:
  - Análisis exploratorio
  - Visualización de datos
  - Modelos predictivos
  - Integración con herramientas de BI

---

## 🔍 Análisis Exploratorio de Datos (EDA)

### 📌 Distribución de la Variable Churn 

- Aproximadamente **73%** de los clientes permanecen.
- Cerca de **27%** de los clientes presentan evasión.

Esto confirma que el churn es un fenómeno significativo y relevante para el negocio.

---

### 📊 Análisis de Variables Numéricas

**Cargos Mensuales y Gasto Total**
- Los clientes que cancelan presentan **mayores cargos mensuales promedio**.
- Los clientes que permanecen tienen **mayor gasto total acumulado**, lo que indica mayor permanencia.

---

### 📊 Análisis de Variables Categóricas

#### 🔹 Tipo de Contrato
- **Month-to-month:** mayor tasa de evasión.
- **One year y Two year:** tasas de churn significativamente menores.

#### 🔹 Método de Pago
- **Electronic check** presenta la mayor tasa de evasión.
- Métodos automáticos reducen el churn.

#### 🔹 Facturación Electrónica
- Los clientes con **PaperlessBilling = Yes** muestran mayor evasión.

---

## 📈 Principales Insights

- El tipo de contrato es el factor más influyente en la evasión.
- Clientes con cargos mensuales altos presentan mayor riesgo de churn.
- El gasto total acumulado es un indicador de fidelización.
- Existen perfiles claros de clientes con mayor probabilidad de cancelar.

---

## 🧩 Conclusiones

El proceso ETL permitió transformar datos con inconsistencias en un dataset confiable y apto para análisis.  
El análisis exploratorio validó la calidad del pipeline y reveló patrones relevantes de evasión.

Este proyecto demuestra la importancia de un ETL sólido como base para la analítica y la toma de decisiones.

---

## 💡 Recomendaciones

- Incentivar contratos de mayor duración.
- Diseñar campañas de retención para clientes con altos cargos mensuales.
- Promover métodos de pago automáticos.
- Implementar monitoreo temprano de clientes con perfil de alto churn.

---

## 🛠️ Tecnologías Utilizadas

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Google Colab  

---

📌 *Proyecto desarrollado como ejercicio práctico de ETL y análisis exploratorio de datos.*
