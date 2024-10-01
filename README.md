# Hackaton_Salon_Ocupacion
Prueba técnica para el salón de Ocupacion de Barcelona 2024
# Hackaton_Salon_Ocupacion
Prueba técnica para el salón de Ocupacion de Barcelona 2024
# Prueba-Tecnica-IT
Prueba técnica IT para actualizar conocimiento sobre Data Science

# Algoritmos de Aprendizaje Supervisado: Clasificación 
Predicción sobre el turno en el que se producen accidentes de tránsito en Barcelona

## 1. Introducción

El presente repositorio se centra en el análisis de datos de accidentes gestionados por la Guàrdia Urbana en la ciudad de Barcelona, recopilados entre los años 2021 y 2023. El objetivo principal es predecir el momento del día en el que se producirán los accidentes, utilizando técnicas de aprendizaje supervisado de clasificación. Si bien la base de datos pública consultada provee registros desde 2016, es a partir de 2021 que el campo que se utilizará como target (turno en el que se produce el accidente) tiene los datos registrados con la consistencia necesaria. Se ha seleccionado el siguiente conjunto de variables para este propósito: distrito, mes y día de la semana.

## 2. Depuración de datos

Para preparar los datos para el análisis, se llevaron a cabo varias técnicas de preprocesamiento. En primer lugar, se realizó un casteo de los datos transformándolos a variables categóricas . Luego se realizó un análisis exploratorio mediante visualizaciones gráficas, tablas de contingencia y test de chi-cuadrado para entender la distribución y correlación de las variables seleccionadas. Posteriormente, se transformaron las variables categóricas en representaciones numéricas adecuadas para el modelado, utilizando técnicas como la codificación One-Hot.


## 3. Resultados

La muestra se dividió en conjuntos de entrenamiento y prueba, y se entrenaron cuatro modelos de clasificación: KNN, LR, SVC y RF. Aunque LR y SVC mostraron una mayor precisión (0.51), al examinar la matriz de confusión, se observó que los modelos RF y KNN se acercaban más a las predicciones deseadas. Se ajustaron los parámetros de estos modelos, resultando en una leve mejora en KNN al establecer el número de vecinos en 13. A pesar de los esfuerzos por balancear la muestra del conjunto de prueba, los resultados no mostraron cambios significativos.

Se utilizaron métricas como precisión (accuracy), F1-score, recall y validación cruzada (CV) para evaluar el rendimiento de los modelos. El mejor rendimiento se logró con el modelo KNN tras ajustar sus parámetros, obteniendo una precisión del 0.46, un F1-score de 0.35, un recall de 0.35 y una validación cruzada de 0.33.

## 4. Conclusiones

Los resultados obtenidos son útiles tanto para la comunidad como para los agentes cívicos en tareas de prevención de accidentes. La capacidad de prever los momentos del día en los que son más probables los accidentes puede contribuir significativamente a la planificación de medidas preventivas. Aunque se logró una precisión modesta, los modelos desarrollados proporcionan una base sólida para futuros análisis y mejoras en la predicción de accidentes en la ciudad de Barcelona.

**Nota:** Este README proporciona una visión general del trabajo realizado y sus resultados clave. Para obtener más detalles, consulte la documentación y el código fuente en el repositorio correspondiente.
