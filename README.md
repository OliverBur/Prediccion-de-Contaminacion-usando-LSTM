# Predicción de Contaminación usando LSTM

Este proyecto utiliza un modelo de red neuronal **LSTM** para predecir los niveles de contaminación atmosférica (PM2.5) en Beijing, China, basado en un conjunto de datos que reporta las condiciones climáticas y de calidad del aire cada hora durante cinco años. El dataset fue recopilado en la embajada de EE.UU. en Beijing y contiene variables como la fecha, concentración de PM2.5, y datos meteorológicos. Este problema es relevante porque permite anticipar niveles de contaminación basados en patrones meteorológicos previos, contribuyendo así a la **salud pública** al permitir alertas tempranas y una planificación urbana más informada.

## Objetivo del Proyecto
El objetivo es predecir la concentración de PM2.5 en las próximas horas, considerando la contaminación y condiciones meteorológicas anteriores. Con estas predicciones, se pueden tomar **medidas preventivas** para reducir actividades contaminantes y emitir alertas tempranas. El modelo se enfoca en mejorar la precisión de las predicciones para optimizar la respuesta ante riesgos ambientales y mejorar la calidad de vida en zonas urbanas.

## Enfoque del Modelo
Se entrenan modelos LSTM tanto **univariables** (solo utilizando la variable de contaminación) como **multivariables** (considerando variables meteorológicas adicionales). Esto permite evaluar si el contexto adicional mejora la precisión de las predicciones de contaminación. Las redes LSTM son adecuadas para este tipo de predicción ya que pueden "recordar" patrones en secuencias de datos, aprovechando la información de las horas previas para hacer predicciones más informadas.

## Dataset
El dataset utilizado está disponible en Kaggle: [Beijing Pollution Dataset](https://www.kaggle.com/datasets/rupakroy/lstm-datasets-multivariate-univariate/data).

## Tecnologías
- **TensorFlow** / **Keras** para la creación y entrenamiento del modelo LSTM.
- **Python** para la preparación de datos y análisis.

## Estructura del Proyecto
- `data/`: Contiene el dataset en formato CSV.
- `notebooks/`: Jupyter notebooks con el análisis exploratorio y el entrenamiento del modelo.
- `model/`: Contiene los modelos LSTM entrenados en formatos `.h5` y `.keras`.
- `results/`: Métricas y visualizaciones de los resultados de los modelos.

## Resultados
Comparación entre los modelos univariables y multivariables para observar el impacto de incluir contexto meteorológico en la precisión de las predicciones.
