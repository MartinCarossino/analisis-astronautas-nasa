# Análisis Exploratorio de Datos — Astronautas y Misiones Espaciales

Proyecto personal de portfolio en **Data Analytics**, enfocado en aplicar un EDA completo con Python sobre un dataset histórico de misiones espaciales.

## Objetivo

Identificar patrones históricos, demográficos y estadísticamente significativos en 1.277 misiones espaciales registradas entre 1961 y 2019: evolución de la duración de las misiones, participación femenina a lo largo del tiempo, diferencias entre países, y relación entre variables como edad, tipo de misión y perfil profesional (militar/civil).

## Metodología

El análisis sigue una estructura de 3 fases:
1. **Comprensión general y estructural** — tipos de datos, nulos, duplicados.
2. **Análisis univariado** — distribución de cada variable por separado.
3. **Relaciones entre variables** — cruces, correlaciones y tests estadísticos (chi-cuadrado) cuando corresponde.

Cada hallazgo se confirma con evidencia (código y/o test estadístico) antes de darlo por válido — no se afirma nada "a ojo".

## Algunos hallazgos

- La duración de las misiones tiene una distribución **bimodal**, explicada casi por completo por el tipo de misión (vuelo orbital corto vs. estadía en estación espacial).
- La participación femenina no creció de forma lineal: pasó de 0% en los 70s a un pico de 15% en los 90s, estabilizándose después en ~12.7%.
- El fin del programa de transbordadores de EE.UU. (2011) deja una huella clara en los datos: 2010 es la primera década donde las estadías en estación superan a los vuelos cortos.
- Un test de chi-cuadrado descarta una asociación significativa entre tipo de misión y perfil militar/civil (p = 0.41).

## Tecnologías

- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy)
- Google Colab

## Fuente de los datos

Dataset público de [TidyTuesday](https://github.com/rfordatascience/tidytuesday/blob/main/data/2020/2020-07-14/readme.md), con información recopilada de NASA, Roscosmos y otras fuentes.

## Contenido del repositorio

- `EDA_Astronautas.ipynb` — notebook completo con el análisis.
- `imagenes/` — gráficos exportados, usados en este README.

## Autor

Martín Carossino — [GitHub](https://github.com/MartinCarossino)
