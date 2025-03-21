# 📊 Informe Integral de Análisis de Datos: Eficiencia Operativa y Visualización Estratégica
### 🏆 Caso de estudio: **Plataforma de Apuestas**

---
## 📌 Introducción
Este informe analiza datos operativos sobre **jugadores, depósitos y rendimiento de fuentes de tráfico**. Mediante un enfoque basado en datos, buscamos:

✅ **Identificar patrones de comportamiento** de los jugadores.  
✅ **Evaluar la eficiencia** de las fuentes de adquisición.  
✅ **Detectar discrepancias** en los registros internos.  

💡 **Objetivo**: Mejorar la rentabilidad mediante decisiones estratégicas basadas en datos.

---
## 📍 Contexto
La empresa opera en un mercado competitivo donde **comprender el comportamiento del usuario** y **optimizar estrategias de adquisición** son claves. Este análisis se enfoca en:

1. **Evaluar métricas mensuales de FTD (Primer Depósito) y CPA (Costo por Adquisición).**
2. **Detectar y analizar discrepancias en registros internos.**
3. **Identificar las fuentes de tráfico más eficientes.**  

---
## 🛠️ Metodología
🔹 **Python y SQLite** para procesamiento y estructuración de datos.  
🔹 **Power BI** para visualización de resultados clave.  
🔹 **Jupyter Notebook** como entorno principal de desarrollo.  

Este informe documenta los pasos realizados, hallazgos clave y conclusiones del análisis.

---
## 🗂️ Base de Datos y Análisis Preliminar con Jupyter

### 🏗️ 1. Creación de la Base de Datos
Para centralizar y organizar los datos, se creó una **base de datos en SQLite**, lo que permite análisis estructurados y conexiones con herramientas externas.

### 📥 2. Carga de Datos
Se importaron archivos CSV para estructurar la información en el Notebook y la base de datos.

### 🔍 3. Consultas Iniciales
Se generaron DataFrames clave para el análisis:
- **Estado de Jugadores**: Clasificación según FTD/CPA.
- **FTD y CPA por Mes**: Comparación con el reporte interno.

### ⚖️ 4. Comparativa con Reporte Interno
Se analizaron diferencias entre datos esperados y datos reales obtenidos del archivo `deposits.csv`.

### 📊 5. Análisis y Visualizaciones

#### FTD y CPA Esperado vs. Real
Se detectaron diferencias iniciales, con una tendencia a mejorar la alineación en registros internos con el tiempo.

#### Proporción CPA vs. No CPA
- **83.3%** de los jugadores son **CPA**.  
- **16.7%** son **No CPA**.  

✅ Esto indica un **buen desempeño en captación y retención**.

#### Histórico de Depósitos por Mes
Crecimiento sostenido, con picos recientes ligados al aumento de jugadores FTD/CPA.

#### Jugador con Mayor Depósito
**Blake Edwards** lidera con **$2,156.42** depositados.

#### Jugadores por Fuente de Tráfico
**Trafficker_2, Trafficker_4 y Trafficker_9** destacan como las fuentes más efectivas.

### 📤 6. Exportación de Resultados
Los DataFrames finales fueron exportados como CSV y se cerró la conexión con la base de datos.

---
## 📊 Análisis de Datos y Power BI

### 🏛️ Modelo de Datos
Se integraron tablas originales (`deposits`, `players`, `traffic_sources`) con tablas procesadas (`player_status`, `combined_records`).

### 🔢 Medidas DAX
Se crearon **medidas DAX** para visualizaciones dinámicas.

### 📊 Dashboard
Se desarrolló un **tablero interactivo** con:

- **FTD/CPA Real vs. Esperado por Mes**
- **Costos por Registro, FTD y CPA**
- **Análisis de Fuentes de Tráfico**
- **Conteo de Depósitos por Mes**
- **Top 10 Jugadores por Depósito Total**  

**Vista previa del Dashboard**:
![Dashboard](dashboard%20image.png)

### Filtros e Interactividad
Se implementaron **filtros por fecha** y botones de **reinicio de vistas** para facilitar el análisis.

---
## 🔍 Conclusiones y Recomendaciones

### ⚙️ Flujo de Trabajo Automatizado
El script en **Jupyter Notebook** permitió consolidar un **flujo automatizado y replicable** para el análisis de datos.

### 📊 Hallazgos Clave
✅ **Crecimiento sostenido** en depósitos y CPA.  
✅ **Estabilidad en costos de adquisición**.  
✅ **Diversificación de jugadores de alto valor**.  
✅ **Eficiencia variable en fuentes de tráfico**.  

### 🚀 Recomendaciones
📌 Replicar estrategias de tráfico exitosas.  
📌 Profundizar en motivaciones de jugadores de alto valor.  
📌 Optimizar costos de CPA/FTD.  
📌 Monitorear patrones de crecimiento continuamente.  

---
## 📂 Archivos Adjuntos
📄 [Jupyter Notebook](bca_operations.ipynb)  
📊 [Power BI](BCA_Operations_PALS.pbix)  

🚀 **¡Análisis basado en datos para decisiones estratégicas!**
