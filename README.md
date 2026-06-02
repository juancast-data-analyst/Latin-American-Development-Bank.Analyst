# Movilidad Urbana y Productividad Económica – Sprint 5

Este repositorio contiene el análisis realizado durante el Sprint 5 del proyecto del American Development Bank (LADB).

Los datasets `tomtom_traffic` y `oecd_city_economy` incluyen datos reales de congestión vehicular y productividad económica de **14 ciudades en 7 países de América Latina**, con registros del año 2024, que combinan fuentes de tráfico en tiempo real con indicadores económicos anuales de la OECD.

---

## 📂 Contenido del repositorio

- `notebooks/S5_ladb_mobility_economy_project.ipynb`
  → Notebook principal con carga, limpieza, integración de datasets, análisis exploratorio, visualizaciones y resumen ejecutivo.

- `data/tomtom_traffic.csv`
  → Datos de congestión vehicular por ciudad: índice de tráfico, retrasos, longitud de embotellamientos y tiempos de viaje (fuente: TomTom Traffic Index).

- `data/oecd_city_economy.csv`
  → Indicadores económicos anuales por ciudad: PIB per cápita, desempleo, contaminación y población (fuente: OECD Cities).

- `data/ladb_mobility_economy_2024_clean.csv`
  → Dataset final exportado: tabla unificada y limpia con una fila por ciudad, lista para análisis posterior.

---

## ▶️ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/juancast-data-analyst/Latin-American-Development-Bank.Analyst/blob/main/S5_ladb_mobility_economy_project_student_(1).ipynb)

O manualmente:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

---

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/S5_ladb_mobility_economy_project.ipynb` en Google Colab o Jupyter
2. Sube los archivos CSV a la carpeta `/datasets/` (o ajusta las rutas según tu entorno)
3. Ejecuta las celdas en orden de arriba hacia abajo
4. Al finalizar, el notebook exporta automáticamente el dataset limpio como `ladb_mobility_economy_2024_clean.csv`

> **Dependencias:** `pandas`, `numpy`, `matplotlib`, `seaborn` — todas disponibles por defecto en Google Colab.

---

## 🧠 Objetivos

### Objetivo del análisis

Evaluar cómo la movilidad urbana (niveles de congestión, tiempos de viaje y retrasos) se relaciona con la productividad económica (PIB per cápita y desempleo) en las principales ciudades latinoamericanas, con el fin de identificar en qué ciudades conviene invertir en infraestructura de transporte para aumentar la productividad y el bienestar de la población.

### Objetivos de aprendizaje

- Crear un dataset único y limpio a partir de dos fuentes de datos diferentes
- Aplicar limpieza, estandarización y validación de tipos de datos
- Filtrar y enfocar el análisis en el año 2024
- Calcular indicadores agregados por ciudad–año mediante agrupaciones
- Integrar ambas fuentes con una unión tipo INNER
- Realizar análisis exploratorios y visualizaciones comparativas entre tráfico y economía
- Exportar el dataset final limpio y documentar todo el proceso en Jupyter Notebook

---

## 🛠️ Herramientas utilizadas

- Python 3.9
- `pandas` · `numpy` · `matplotlib` · `seaborn` · `scipy`
- Jupyter Notebook / Google Colab

---

## 📊 Etapas del análisis

| Paso | Descripción |
|------|-------------|
| 1 | Carga y exploración de los 2 datasets |
| 2 | Limpieza y corrección de formatos (fechas, tipos, snake_case) |
| 3 | Extracción del año y filtrado al período 2024 |
| 4 | Cálculo de promedios de tráfico por ciudad |
| 5 | Integración de datasets (INNER join por ciudad y año) |
| 6 | Visualización: boxplots, histogramas y gráficos de barras comparativos |
| 7 | Exportación del dataset final y resumen ejecutivo |

---

## 💡 Principales hallazgos

- El **PIB per cápita no es directamente proporcional a la congestión vehicular**; no se identificó una relación clara entre ambas variables
- **Montevideo y Ciudad de México** lideran en PIB per cápita (>20,000 USD), pero presentan niveles de congestión opuestos: bajo y muy alto respectivamente
- **Santiago** emerge como ciudad prioritaria para inversión: presenta alta congestión con bajo PIB per cápita relativo al grupo analizado
- **A mayor población, mayor congestión**, aunque esto no se traduce necesariamente en mayor productividad económica
- El análisis cubrió **14 ciudades en 7 países**: México, Brasil, Colombia, Perú, Chile, Argentina y Uruguay

---

👤 Autor
Juan Castelblanco - Analista de Datos 

📝 Licencia
Este proyecto es de uso educativo y forma parte del programa de análisis de datos.

*Análisis basado en datos de tráfico TomTom y economía OECD del año 2024*  
*Fecha de análisis: 2024 | American Development Bank – Data Analytics Team*
