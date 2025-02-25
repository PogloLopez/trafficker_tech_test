# Informe Integral de Análisis de Datos: Eficiencia Operativa y Visualización Estratégica  
_Caso de estudio de empresa ficticia: **Plataforma de apuestas**_

## Introducción

Este informe tiene como objetivo analizar datos operativos relacionados con jugadores, depósitos y rendimiento de fuentes de tráfico. A través de un enfoque basado en datos, se busca identificar patrones de comportamiento, evaluar la eficiencia de las fuentes de adquisición y detectar posibles discrepancias en registros internos.

### **Contexto**

La empresa opera en un entorno altamente competitivo donde comprender el comportamiento de los jugadores y optimizar estrategias de adquisición son claves para mejorar la rentabilidad. Este análisis se centra en:

1. Evaluar métricas mensuales de **FTD (Primer Depósito)** y **CPA (Costo por Adquisición)**, esenciales para medir el éxito de campañas.
2. Detectar y analizar **discrepancias** entre registros internos y datos calculados para garantizar calidad.
3. Identificar las fuentes de tráfico más eficientes según jugadores generados y costos asociados.

### **Metodología**

El análisis se realizó utilizando:

- **Python y SQLite** para procesamiento y estructuración de datos.
- **Power BI** para visualización y presentación de resultados clave.
- **Jupyter Notebook** como entorno principal de desarrollo.

Este informe documenta los pasos realizados, hallazgos clave y conclusiones derivadas del análisis.

## Base de Datos y Análisis Preliminar con Jupyter

### 1. Creación de la Base de Datos

Para centralizar y organizar los datos, se creó una base de datos SQLite. Este enfoque permite análisis estructurados y conexiones con herramientas externas.

### 2. Carga de Datos

Se inició con la lectura de archivos CSV para cargar información en el Notebook y la base de datos, permitiendo comenzar la manipulación de datos.

### 3. Consultas Iniciales

Se realizaron consultas SQL para crear dos DataFrames con información relevante:

- **Identificación de Estado de Jugadores**: DataFrame con detalles de cada jugador y su estado (FTD/CPA).
- **FTD y CPA por Mes**: DataFrame para comparar con el reporte interno, contando FTD y CPA mensuales.

### 4. Comparativa con Reporte Interno

Los datos del reporte interno de FTD/CPA esperados se compararon con los datos reales obtenidos del archivo `deposits.csv`.

### 5. Análisis y Visualizaciones

Se crearon visualizaciones para obtener insights clave:

#### FTD y CPA Esperado vs. Real

La comparación muestra **diferencias iniciales significativas**, probablemente por **inconsistencias en recopilación histórica de datos**. Con el tiempo, las discrepancias disminuyen, reflejando una **mejor alineación** entre cifras internas y resultados observados.

#### Proporción CPA vs. No CPA

El gráfico muestra que **83.3% de los jugadores son CPA**, mientras que solo **16.7% son No CPA**, indicando un **buen desempeño en captación y retención**.

#### Histórico de Depósitos por Mes

Los datos reflejan un **crecimiento constante y acelerado**, especialmente en meses recientes, vinculado al aumento de jugadores FTD/CPA.

#### Jugador con Mayor Depósito

Destaca **Blake Edwards** con **$2,156.42** depositados. A pesar de la reducción en sus montos, los depósitos totales mensuales aumentan, sugiriendo una **base sólida de depositantes recurrentes**.

#### Jugadores por Fuente de Tráfico

**Trafficker_2, Trafficker_4 y Trafficker_9** sobresalen como las fuentes más efectivas en generación de jugadores.

### 6. Resultados

Tras el análisis, los DataFrames relevantes se exportaron como archivos CSV y se cerró la conexión con la base de datos.

## Análisis de Datos y Power BI

Se estableció una conexión desde Power BI a los archivos generados para crear visualizaciones dinámicas.

### Modelo de Datos

Se integraron tablas originales (`deposits`, `players`, `traffic_sources`) con tablas procesadas (`player_status`, `combined_records`).

### Medidas DAX

Se crearon medidas usando DAX para generar visualizaciones calculadas que combinan datos dinámicamente.

### Dashboard

Se desarrolló un tablero interactivo con:

- **FTD/CPA Real vs. Esperado por Mes**
- **Costos por Registro, FTD y CPA**
- **Análisis de Fuentes de Tráfico**
- **Conteo de Depósitos por Mes**
- **Top 10 Jugadores por Depósito Total**

### Filtros e Interactividad

Se incluyeron herramientas como filtros por fecha y botones para reiniciar vistas, mejorando la experiencia de análisis.

## Conclusiones y Recomendaciones

### Flujo de Trabajo Automatizado

El script en Jupyter Notebook permitió consolidar un flujo automatizado y replicable para procesar y analizar datos.

### Hallazgos Clave

- **Crecimiento sostenido en depósitos y CPA**
- **Estabilidad en costos de adquisición**
- **Diversificación de jugadores de alto valor**
- **Eficiencia variable en fuentes de tráfico**

### Recomendaciones

- Replicar estrategias de fuentes de tráfico exitosas.
- Profundizar en motivaciones de jugadores de alto valor.
- Optimizar costos de CPA/FTD.
- Monitorear patrones de crecimiento continuamente.

## Archivos Adjuntos

[Jupyter Notebook](bca_operations.ipynb) | [Power BI](BCA_Operations_PALS.pbix)
