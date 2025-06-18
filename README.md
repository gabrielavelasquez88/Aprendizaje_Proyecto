**COVID-19 - Predicción de Nuevas Dosis de Vacunas Administradas en Argentina**

**Objetivo General**

Desarrollar un modelo de Aprendizaje Automático que permita predecir la cantidad diaria de nuevas dosis de vacunas administradas en Argentina, a partir de variables climáticas, de movilidad y estacionales.

**Objetivos Específicos**

- Preprocesar los datos de vacunación, movilidad y clima.
- Construir un modelo de regresión supervisada para predecir la variable `new_vaccine_doses_administered`.
- Evaluar el rendimiento de distintos algoritmos de regresión (Regresión Lineal, Random Forest, SVR).
- Analizar la importancia relativa de cada variable en la predicción.
- Aplicar el modelo sobre datos futuros para anticipar variaciones estacionales y asistir la planificación sanitaria.

**Contexto y Relevancia**

Durante y después de la pandemia del COVID-19, el seguimiento de las campañas de vacunación se ha convertido en una herramienta clave para los sistemas de salud.

Prever cuántas dosis se aplicarán diariamente, en función de factores como el clima, la movilidad o la época del año, permite:

- Organizar mejor los recursos.
- Optimizar la logística de distribución.
- Priorizar zonas de mayor demanda.
- Focalizar estrategias de comunicación sanitaria.

Este proyecto se enfoca en Argentina, utilizando:

- Variables climáticas: temperatura, precipitación, humedad.
- Variables de movilidad: hacia lugares de trabajo y en el hogar.
- Variables temporales: mes y año.
- Datos históricos de vacunación.

**Tipo de Problema**

Regresión Supervisada  
Se busca predecir una variable continua (`new_vaccine_doses_administered`) en función de un conjunto de características independientes.

**Modelos de Aprendizaje Automático Considerados**

- Regresión Lineal Múltiple: modelo base por su sencillez e interpretabilidad.
- Random Forest Regressor: robusto ante relaciones no lineales y valores atípicos.
- Support Vector Regressor (SVR): útil para capturar relaciones no lineales con kernel RBF.

**Estructura del Proyecto**

**Estructura del Proyecto**

├── data/                # Datos originales y derivados

│   ├── raw/             # Datos sin procesar (brutos)
│   ├── processed/       # Datos listos para el modelado
│   └── interim/         # Datos intermedios (transformaciones)

├── docs/                # Documentación del proyecto
│   └── 1. Proceso del codigo realizado.pdf

└──2. Informe del proyecto.pdf

├── models/              # Modelos entrenados y serializados

├── notebooks/           # Notebooks de análisis y entrenamiento
│   └── 2025\_AA\_Proyecto.ipynb.ipynb

├── references/          # Artículos, papers o benchmarks usados como base

├── reports/             # Reportes y visualizaciones │   ├── figures/         # Imágenes generadas │

├── src/                 # Código fuente del proyecto
│   ├── preprocess/      # Scripts de limpieza y preparación de datos
│   ├── train/           # Scripts de entrenamiento
│   └── predict/         # Scripts de predicción con modelos entrenados

├── .gitignore           # Archivos y carpetas excluidos del control de versiones
├── LICENSE              # Licencia del proyecto
├── README.md            # Descripción general del proyecto
└── requirements.txt     # Dependencias necesarias para reproducir el entorno




Gabriela Velasquez
Proyecto final - Aprendizaje Automático 2025

