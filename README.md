# Celebrity-face-classification-deep-learning
Clasificación de imágenes con Deep Learning (TensorFlow)
# Celebrity Face Classification – Deep Learning

Proyecto de **Clasificación de Imágenes** desarrollado como parte de la  
**Tarea 5 – Inteligencia Artificial (UDH-B1-001-IMP-42A-25-03-G3)**.

El objetivo del proyecto es realizar un análisis completo de un dataset de imágenes
y aplicar técnicas de **Deep Learning** para clasificar rostros de celebridades,
utilizando **TensorFlow/Keras** y sin hacer uso de la librería `sklearn`.

---

## Dataset

Se utiliza el dataset público de Kaggle:

**Celebrity Face Image Dataset**  
https://www.kaggle.com/datasets/vishesh1412/celebrity-face-image-dataset

Del dataset original se seleccionan únicamente las siguientes clases:
- Natalie Portman  
- Scarlett Johansson  

---

## Objetivos del Proyecto

- Realizar una exploración general del dataset
- Analizar la distribución de imágenes por clase
- Evaluar tamaños, resoluciones y formatos de imagen
- Detectar imágenes corruptas o vacías
- Evaluar el balance de clases
- Realizar análisis estadístico por canal RGB
- Detectar valores atípicos en las imágenes
- Aplicar preprocesamiento básico
- Implementar aumento de datos (data augmentation)
- Realizar limpieza y control de calidad
- Entrenar un modelo CNN como validación del proceso

---

## Exploración del Dataset

Se realiza un análisis que incluye:
- Número total de imágenes y distribución por clase
- Formatos de imagen (JPG, PNG)
- Resoluciones de las imágenes
- Detección de archivos corruptos
- Evaluación visual de iluminación, fondo, orientación y ruido

---

## Análisis Estadístico

Para apoyar la normalización y el preprocesamiento de los datos se calcula:
- Media por canal RGB
- Desviación estándar por canal RGB
- Rango de valores de píxeles (0–255)

Además, se identifican imágenes extremadamente oscuras, brillantes o borrosas
como posibles valores atípicos.

---

## Preprocesamiento

Las imágenes se procesan de la siguiente manera:
- Conversión a formato RGB
- Redimensionamiento a 224 × 224 píxeles
- Normalización de valores al rango [0,1]
- Separación en conjuntos de entrenamiento y validación

---

## Aumento de Datos

Para reducir el sobreajuste y mejorar la generalización del modelo se aplican
técnicas de aumento de datos como:
- Rotación
- Desplazamiento horizontal y vertical
- Zoom
- Volteo horizontal

---

## Limpieza y Control de Calidad

Se implementan procesos para:
- Eliminar imágenes corruptas o no legibles
- Detectar y eliminar imágenes duplicadas
- Verificar la correcta asignación de etiquetas
- Comprobar la integridad de los archivos

---

## Modelo de Deep Learning

Se entrena un modelo **CNN (Convolutional Neural Network)** utilizando
**TensorFlow/Keras**, con capas convolucionales, pooling y una capa final
Softmax para la clasificación binaria.

---

## Tecnologías Utilizadas

- Python  
- Google Colab  
- TensorFlow / Keras  
- NumPy  
- Pandas  
- Matplotlib  
- Pillow  
- Kaggle API  

---

## Restricciones Cumplidas

- No se utiliza la librería `sklearn`
- Se emplean únicamente frameworks de Deep Learning

---

## Autora

**Amber Grijalba**  
Estudiante de Ingeniería Biomédica  
Universidad Latina de Panamá
