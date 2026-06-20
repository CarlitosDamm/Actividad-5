# Actividad 5 - Entrenamiento, Evaluación y Registro de Modelos con MLflow

## Descripción del proyecto

Este proyecto tiene como objetivo comparar diferentes algoritmos de aprendizaje automático para predecir la supervivencia de pasajeros del Titanic utilizando técnicas de clasificación supervisada y herramientas de MLOps.

Para garantizar la trazabilidad y reproducibilidad del experimento se utilizó MLflow como plataforma de seguimiento de experimentos, registro de parámetros, métricas y artefactos generados durante el entrenamiento.

## Dataset

Se utilizó el dataset Titanic disponible a través de la biblioteca Seaborn.

Variable objetivo:

* survived

  * 0 = No sobrevivió
  * 1 = Sobrevivió

Variables predictoras principales:

* pclass
* sex
* age
* sibsp
* parch
* fare
* embarked
* alone

## Modelos evaluados

Se entrenaron y compararon los siguientes algoritmos:

1. Logistic Regression
2. Random Forest
3. Support Vector Machine (SVM)
4. Gradient Boosting

## Proceso de preparación de datos

Las principales actividades realizadas fueron:

* Eliminación de variables redundantes.
* Tratamiento de valores nulos mediante imputación.
* Codificación de variables categóricas mediante One-Hot Encoding.
* Escalado de variables numéricas cuando fue requerido.
* División de datos en conjuntos de entrenamiento y prueba.

## Validación

Se utilizó GridSearchCV con validación cruzada estratificada de 5 particiones para optimizar hiperparámetros y reducir sesgos en la evaluación.

## Métricas utilizadas

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

## Uso de MLflow

Durante cada ejecución se registraron:

* Hiperparámetros
* Métricas de desempeño
* Modelos entrenados
* Matrices de confusión
* Artefactos generados

## Estructura del repositorio

Actividad5/
│
├── Actividad_5_Gestion_de_Proyectos_de_IA.ipynb
├── README.md
├── evidencias/
└── reporte_tecnico.pdf

## Reproducción

1. Abrir el notebook en Google Colab.
2. Instalar dependencias requeridas.
3. Ejecutar todas las celdas en orden.
4. Revisar los resultados generados en MLflow.
5. Consultar las evidencias almacenadas en la carpeta correspondiente.

## Autor

Carlos Damm
Tecnológico de Monterrey - Universidad Tecmilenio

