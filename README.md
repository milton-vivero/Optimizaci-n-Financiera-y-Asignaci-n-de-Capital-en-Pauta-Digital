# 📈 SEM Market Intelligence: Optimización Financiera y Asignación de Capital

> Pipeline analítico desarrollado para transformar datos de mercado SEM en **inteligencia comercial y financiera**, permitiendo identificar oportunidades de inversión, controlar el impacto del CPC y optimizar la asignación de presupuesto publicitario en el mercado financiero de Ecuador.

---

## 🎯 Objetivo

Desarrollar un modelo analítico que permita evaluar la relación entre **demanda de búsqueda, costo por clic (CPC) y pertinencia del mercado ecuatoriano**, facilitando la toma de decisiones para la asignación eficiente del presupuesto de pauta digital.

El proyecto permite:

* Identificar términos de búsqueda con alta demanda y bajo costo.
* Detectar palabras clave con **alto CPC y potencial riesgo presupuestario**.
* Clasificar oportunidades mediante una matriz de **Demanda vs. CPC**.
* Identificar términos relevantes para el sector financiero ecuatoriano.
* Detectar términos internacionales o de baja pertinencia para el mercado objetivo.
* Proporcionar criterios cuantitativos para la priorización de inversión publicitaria.

---

## 📸 Vista del Análisis

<p align="center">
  <img width="100%" alt="Matriz estratégica de Demanda vs CPC" src="https://github.com/user-attachments/assets/f7afe7d8-576b-4d65-b861-41f452c137ae" />
</p>

---

## 🏆 Indicadores Principales

| Indicador                       | Descripción                                                                    |
| ------------------------------- | ------------------------------------------------------------------------------ |
| **Demanda de Mercado**          | Volumen potencial asociado a los términos de búsqueda analizados.              |
| **CPC Promedio (USD)**          | Costo promedio estimado por clic dentro del conjunto analizado.                |
| **CPC Máximo (USD)**            | Mayor costo por clic identificado en el dataset.                               |
| **Umbral Financiero (USD)**     | Valor de referencia establecido para clasificar el nivel de presión de costos. |
| **Términos de Alta Eficiencia** | Keywords que combinan demanda relevante con CPC controlado.                    |
| **Términos de Alto Riesgo**     | Keywords cuyo CPC supera significativamente el umbral definido.                |

---

## 📁 Estructura de Datos

### Archivo base: `Data_financiera.xlsx`

El dataset contiene información relacionada con términos de búsqueda y variables de mercado utilizadas para evaluar el comportamiento económico de la pauta digital.

| Campo           | Tipo       | Descripción                                          |
| --------------- | ---------- | ---------------------------------------------------- |
| **Keyword**     | Texto      | Término o intención de búsqueda analizada.           |
| **Demanda**     | Numérico   | Volumen potencial asociado al término.               |
| **CPC**         | Decimal    | Costo estimado por clic expresado en USD.            |
| **Mercado**     | Texto      | Segmentación geográfica o de mercado.                |
| **Categoría**   | Texto      | Clasificación temática del término.                  |
| **Pertinencia** | Categórico | Nivel de relevancia respecto al mercado ecuatoriano. |

---

## 📐 Métricas y Lógica Analítica

### Umbral de control financiero

Se estableció un umbral analítico de:

> **USD 1,30 por clic**

Este valor permite diferenciar términos con una presión de costos relativamente controlada de aquellos que requieren una evaluación presupuestaria adicional.

### Matriz Demanda vs. CPC

El modelo utiliza dos dimensiones principales:

**Demanda de mercado + Costo por clic**

A partir de esta relación se identifican diferentes escenarios de decisión:

| Segmento               | Característica                      | Interpretación                  |
| ---------------------- | ----------------------------------- | ------------------------------- |
| 🟢 **Alta eficiencia** | Alta demanda + CPC bajo             | Potencial de priorización       |
| 🟡 **Evaluación**      | Demanda o CPC intermedio            | Requiere análisis adicional     |
| 🔴 **Alto riesgo**     | CPC elevado                         | Requiere control presupuestario |
| ⚪ **Baja pertinencia** | Términos fuera del mercado objetivo | Candidatos a exclusión          |

---

## 🔎 Principales Hallazgos

### 🟢 Términos de alta eficiencia

Dentro del dataset se identificaron términos institucionales relacionados con el sistema financiero ecuatoriano, entre ellos:

* `superintendencia de bancos ecuador`
* `cooperativas de ahorro y crédito seps`

Estos términos presentan una combinación favorable de **demanda y CPC**, registrando valores promedio inferiores a **USD 0,65 por clic** dentro del análisis.

### 🔴 Términos de alto CPC

También se identificaron términos genéricos asociados al mercado de servicios financieros.

Por ejemplo:

`empresas de servicios financieros`

presentó valores superiores a **USD 3,38 por clic** dentro del dataset analizado.

Esta diferencia evidencia la importancia de considerar el **costo marginal de adquisición de tráfico**, además del volumen de búsquedas.

---

## 📊 Visualizaciones Incluidas

| Visualización                | Tipo                         | Objetivo analítico                                                                    |
| ---------------------------- | ---------------------------- | ------------------------------------------------------------------------------------- |
| **Matriz Demanda vs. CPC**   | Scatter Plot                 | Identificar oportunidades y zonas de riesgo financiero.                               |
| **Segmentación de Keywords** | Clasificación por cuadrantes | Priorizar términos según demanda y costo.                                             |
| **Análisis de CPC**          | Comparativo                  | Identificar términos con mayor presión presupuestaria.                                |
| **Pertinencia de Mercado**   | Segmentación                 | Diferenciar términos relevantes para Ecuador de búsquedas externas o poco relevantes. |

---

## 💰 Aplicación Financiera

El análisis busca cambiar el enfoque tradicional de asignación presupuestaria:

### Enfoque tradicional

**Volumen de búsquedas → Presupuesto**

### Enfoque propuesto

**Demanda + CPC + Pertinencia → Priorización → Asignación de capital**

Este enfoque permite que la inversión publicitaria sea evaluada desde una perspectiva de **eficiencia económica**, y no únicamente desde el volumen potencial de tráfico.

---

## 📈 Recomendaciones Estratégicas

### 1. Priorizar términos eficientes

Concentrar una mayor proporción de la inversión en términos que presenten:

* Alta demanda.
* CPC controlado.
* Alta pertinencia para Ecuador.
* Intención comercial compatible con el objetivo de adquisición.

### 2. Controlar términos de CPC elevado

Los términos que superen el umbral financiero deberían someterse a una evaluación adicional antes de incrementar su presupuesto.

### 3. Aplicar palabras clave negativas

Identificar términos internacionales, irrelevantes o de baja intención comercial para reducir el riesgo de consumir presupuesto en tráfico no estratégico.

### 4. Incorporar métricas de conversión

Para evolucionar el modelo hacia una herramienta integral de optimización financiera, se recomienda incorporar:

* **CTR**
* **Conversion Rate**
* **CPA**
* **CAC**
* **ROAS**
* **Conversiones**
* **Valor generado por cliente**

De esta forma, el modelo podría pasar de analizar únicamente el **costo del tráfico** a medir el **valor económico generado por la inversión**.

---

## 🧠 Insight Estratégico

> **El mayor volumen de búsquedas no necesariamente representa la mejor oportunidad de inversión.**

Una estrategia eficiente de SEM debe considerar simultáneamente:

**Demanda + Costo + Pertinencia + Conversión + Valor económico**

La matriz desarrollada permite convertir datos de búsqueda en un **framework de decisión para la asignación de capital publicitario**.

---

## 🛠️ Tecnologías Utilizadas

<p align="left">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Pandas-Data_Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
  <img src="https://img.shields.io/badge/NumPy-Data_Processing-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-11557C?style=for-the-badge&logo=python&logoColor=white" alt="Matplotlib" />
  <img src="https://img.shields.io/badge/Excel-Data_Source-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel" />
  <img src="https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
  <img src="https://img.shields.io/badge/Markdown-Documentation-000000?style=for-the-badge&logo=markdown&logoColor=white" alt="Markdown" />
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
</p>

### Herramientas y enfoques aplicados

* Limpieza y preparación de datos.
* Exploración y análisis estadístico.
* Ingeniería de características.
* Segmentación de mercado.
* Análisis de CPC.
* Análisis de demanda.
* Visualización de datos.
* Inteligencia comercial.
* Análisis financiero aplicado a marketing.
* Toma de decisiones basada en datos.

---

## 📁 Estructura del Proyecto

```text
SEM-Market-Intelligence/
│
├── 📂 data/
│   └── Data_financiera.xlsx
│
├── 📂 notebooks/
│   └── SEM_Market_Intelligence.ipynb
│
├── 📂 outputs/
│   └── visualizaciones/
│
├── 📂 src/
│   └── analysis.py
│
├── 📄 README.md
└── 📄 requirements.txt
```

---

## 🚀 Flujo Analítico

```text
Data_financiera.xlsx
        │
        ▼
Limpieza y validación
        │
        ▼
Transformación de variables
        │
        ▼
Análisis de Demanda + CPC
        │
        ▼
Segmentación estratégica
        │
        ▼
Matriz de decisión
        │
        ▼
Recomendaciones de inversión
```

---

## 👤 Autor

**Milton Vivero**
*Data Science & Business Intelligence*

> Proyecto de analítica aplicada orientado a transformar datos de mercado en información estratégica para la optimización financiera, comercial y presupuestaria de campañas digitales.

---

## 📄 Licencia

Este proyecto es de carácter demostrativo y forma parte del portafolio profesional del autor.

El dataset utilizado puede contener información estructurada con fines académicos o de simulación y no representa necesariamente información financiera real de una institución específica.

---

<p align="center">
  <i>“Los datos no solo permiten entender el mercado; permiten decidir dónde tiene sentido invertir.”</i>
</p>
