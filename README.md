# Urban Mobility and Economic Productivity in Latin American Cities Analysis – Proyecto Sprint 5 

Este repositorio contiene el análisis realizado durante el Proyecto del Sprint 5 del caso *Movilidad urbana y productividad económica en ciudades de LATAM* datos de Latin American Development Bank.

Este proyecto analiza datos de tráfico urbano (`tomtom_traffic`) y variables económicas (`oecd_city_economy`) para explorar cómo se relacionan las condiciones económicas con la movilidad en diferentes ciudades. El proceso incluye la carga y revisión preliminar de los datasets, la corrección de tipos de datos, la estandarización de columnas y la conversión adecuada de fechas y valores numéricos.

Posteriormente, se identifican los registros correspondientes al año 2024, se consolida el tráfico promedio por ciudad y se integra esta información con indicadores económicos. El objetivo es obtener una vista limpia, reproducible y lista para análisis posteriores, complementada con visualizaciones y un resumen ejecutivo que sintetiza los hallazgos principales.


## 📂 Contenido del repositorio

- `notebooks/S5_ladb_mobility_economy_project_student_(1).ipynb`
  → Notebook principal con limpieza, unión datasets, analisis y resumen ejecutivo.

## ▶ Cómo abrir el notebook en Google Colab

Haz clic en el siguiente botón:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([[URL_DEL_NOTEBOOK_EN_GITHUB](https://github.com/juancast-data-analyst/Latin-American-Development-Bank.Analyst/blob/main/S5_ladb_mobility_economy_project_student_(1).ipynb))

O:

1. Abre el archivo `.ipynb` en GitHub
2. Haz clic en **Open in Colab**

## 📘 Cómo reproducir el análisis

1. Abre `notebooks/S5_ladb_mobility_economy_project_student_(1).ipynb`
2. Ejecuta las celdas en orden
3. El notebook carga automáticamente el dataset desde `/data/` o desde un enlace público (según corresponda)

## 🧠 Objetivos del proyecto de análisis

- Cargar y revisar los datasets para entender su estructura y calidad.
- Detectar tipos incorrectos, valores nulos y columnas que requieren conversión.
- Estandarizar nombres de columnas y asegurar formatos correctos en fechas y valores numéricos.
- Filtrar los registros correspondientes al año 2024.
- Calcular el tráfico promedio por ciudad y obtener una vista consolidada del año.
- Integrar datos de tráfico y economía en un único DataFrame para análisis conjunto.
- Explorar visualmente la relación entre indicadores económicos y movilidad urbana en 2024.
- Generar un CSV limpio y reproducible para análisis posteriores.
- Elaborar un resumen ejecutivo con los hallazgos principales.
