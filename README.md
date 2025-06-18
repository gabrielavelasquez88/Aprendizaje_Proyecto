COVID19 - Predicción de Nuevas Dosis de Vacunas Administradas en Argentina

*Objetivo General

Desarrollar un modelo de Aprendizaje Automático que permita predecir la cantidad diaria de nuevas dosis de vacunas administradas en Argentina, a partir de variables climáticas, de movilidad y estacionales.

*Objetivos Específicos

* Preprocesar los datos de vacunación, movilidad y clima.
* Construir un modelo de regresión supervisada para predecir la variable" new_vaccine_doses_administered".
* Evaluar el rendimiento de distintos algoritmos de regresión (Regresión Lineal, Random Forest, SVR).
* Analizar la importancia relativa de cada variable en la predicción.
* Aplicar el modelo sobre datos futuros para anticipar variaciones estacionales y asistir la planificación sanitaria.

*Contexto y Relevancia

Durante y después de la pandemia del COVID-19, el seguimiento de las campañas de vacunación se ha convertido en una herramienta clave para los sistemas de salud. Prever cuántas dosis se aplicarán diariamente, en función de factores contextuales como el clima, la movilidad o la temporalidad del año, permite organizar mejor los recursos, definir estrategias de comunicación, optimizar la logística y priorizar zonas con mayor demanda esperada.
Este proyecto se enfoca en Argentina y utiliza datos climáticos (temperatura, precipitación, humedad), de movilidad poblacional (hacia lugares de trabajo y en el hogar) y variables temporales (mes y año), en combinación con datos históricos de vacunación para predecir el volumen diario de dosis aplicadas.

*Tipo de Problema

El problema abordado corresponde a una regresión supervisada, dado que la variable objetivo es continua y numérica.

*Modelos de Aprendizaje Automático Considerados

  - Regresión Lineal Múltiple: como línea base, por su interpretabilidad.
  - Random Forest Regressor: por su robustez ante relaciones no lineales, outliers y su capacidad de estimar importancia de variables.
  - Support Vector Regressor (SVR): adecuado para problemas con complejidad no lineal en los datos.

Estructura del proyecto
├── data/                                
│   ├── raw/                  # Datos originales sin procesar
│   ├── processed/            # Datos listos para entrenar
│   └── interim/              # Datos intermedios
│
├── docs/                     # Documentación del proyecto
│   └── dataset_description.md
│
├── models/                   # Modelos entrenados y serializados
│
├── notebooks/                # Jupyter notebooks para análisis exploratorio, entrenamiento y pruebas
│    
│
├── references/               # Artículos, papers, papers técnicos o benchmarks
│
├── reports/                  # Reporte final generado
│   ├── figures/              # Gráficos 
│   └── Análisis de Resultados          # Reportes de evaluación del modelo
│
├── .gitignore
├── LICENSE
├── README.md
└── requirements.txt

