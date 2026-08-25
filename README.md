# 🚗 Análisis de Accidentes de Tránsito en Brasil (2020–2022)

Proyecto de análisis de datos y modelado predictivo sobre accidentes de tránsito en Brasil, planteado a partir de un problema real de seguridad vial.

---

## Contexto de Negocio

Las autoridades de seguridad vial necesitan información basada en datos para diseñar políticas de prevención más efectivas. Este proyecto analiza los registros de accidentes de tránsito en Brasil desde 2020 hasta mediados de 2023, con el objetivo de identificar patrones y factores de riesgo que puedan orientar decisiones de seguridad vial.

## Preguntas de Interés

- ¿Cuál es la tendencia en el número total de accidentes a lo largo de los años?
- ¿Existe estacionalidad en la ocurrencia de accidentes según mes o estación del año?
- ¿Cuáles son las condiciones meteorológicas más comunes en los accidentes y cómo afectan su gravedad?
- ¿Qué días de la semana tienen mayor cantidad de accidentes?
- ¿Cómo se distribuyen los tipos de carreteras en relación con los accidentes?
- ¿En qué horario del día ocurren más accidentes?
- ¿Cuáles son las Unidades Federales (estados) con mayores índices de accidentes?

## Principales Insights

- La cantidad de accidentes se mantuvo relativamente constante entre meses/estaciones, sin un efecto estacional fuerte.
- Los fines de semana mostraron más accidentes de lo esperado, sugiriendo que los viajes de ocio (no laborales) son un factor relevante.
- La mayoría de los accidentes ocurrieron con cielo despejado, no en condiciones climáticas adversas — lo que podría indicar exceso de confianza o mayor volumen de tráfico en esos días.
- Las horas de la tarde y la noche concentraron la mayor cantidad de accidentes.
- Minas Gerais, Santa Catarina y Paraná se destacaron con los mayores índices de accidentes, sugiriendo la necesidad de políticas de seguridad específicas por región.

## Modelado Predictivo

Además del análisis exploratorio, el proyecto aplica un análisis de **Information Value (IV)** para selección de variables, y luego construye y compara dos modelos de clasificación para predecir la gravedad de los accidentes:

- **Árbol de Decisión** — ~82% de precisión en entrenamiento, ~79% en test
- **Random Forest** (con optimización de hiperparámetros vía GridSearchCV) — 82.25% de precisión en test

El análisis también aborda con honestidad las limitaciones del modelo (desbalance de clases que afecta la detección de la clase minoritaria), reflejando un enfoque realista y riguroso en la evaluación de modelos, sin sobrevender los resultados.

---

## 📁 Archivos

- [**Proyecto_final_DS.ipynb**](https://github.com/Luovelar/Brazil-Road-Accidents-Analysis/blob/main/Proyecto_final_DS.ipynb) — Notebook completo del análisis (EDA, prueba de hipótesis, selección de variables, modelado)
- [**Proyecto final.pdf**](<https://github.com/Luovelar/Brazil-Road-Accidents-Analysis/blob/main/Proyecto%20final.pdf>) — Presentación / informe del proyecto
- [**Acidentes_Brasil_2020-2022.csv**](https://github.com/Luovelar/Brazil-Road-Accidents-Analysis/blob/main/Acidentes_Brasil_2020-2022.csv) — Dataset original

---

*Desarrollado con Python (pandas, scikit-learn, seaborn) | Proyecto de Análisis de Datos y Data Science.*
