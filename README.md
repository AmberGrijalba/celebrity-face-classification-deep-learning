# Celebrity-face-classification-deep-learning
Clasificación de imágenes con Deep Learning (TensorFlow)
# Celebrity Face Classification – Deep Learning

# Celebrity Face Classification – Deep Learning

Proyecto de **Clasificación de Imágenes** desarrollado como parte de la  
**Inteligencia Artificial (UDH-B1-001-IMP-42A-25-03-G3)**.

El objetivo del proyecto es realizar un **análisis completo de un dataset de imágenes**
y aplicar técnicas de **Deep Learning** para clasificar rostros de celebridades,
utilizando únicamente **TensorFlow/Keras** (sin uso de `sklearn`).

---

## 📌 Dataset

Se utiliza el dataset público de Kaggle:

**Celebrity Face Image Dataset**  
🔗 https://www.kaggle.com/datasets/vishesh1412/celebrity-face-image-dataset

Del dataset original se seleccionan únicamente **dos clases**:
- Natalie Portman
- Scarlett Johansson

---

## 🎯 Objetivos del Proyecto

- Realizar una **exploración general del dataset**
- Analizar la **distribución de imágenes por clase**
- Evaluar tamaños, resoluciones y formatos
- Detectar imágenes corruptas o vacías
- Analizar el **balance de clases**
- Realizar **análisis estadístico por canal RGB**
- Detectar valores atípicos (imágenes muy oscuras, brillantes o borrosas)
- Aplicar **preprocesamiento básico**
- Implementar **aumento de datos (data augmentation)**
- Realizar **limpieza y control de calidad**
- Entrenar un modelo CNN básico como validación del proceso

---

## 🔍 Exploración del Dataset

Se realiza un análisis que incluye:

- Número total de imágenes
- Distribución por clase
- Formatos de imagen (JPG, PNG)
- Resoluciones (ancho × alto)
- Detección de imágenes corruptas
- Evaluación visual de:
  - Iluminación
  - Fondo
  - Orientación
  - Ruido

---

## 📊 Análisis Estadístico

Para apoyar la normalización y el preprocesamiento, se calcula:

- Media por canal RGB
- Desviación estándar por canal RGB
- Rango de valores de píxeles (0–255)

También se detectan **valores atípicos**, tales como:
- Imágenes extremadamente oscuras o brillantes
- Imágenes potencialmente desenfocadas

---

## ⚙️ Preprocesamiento

Las imágenes son procesadas de la siguiente manera:

- Conversión a RGB
- Redimensionamiento a **224 × 224**
- Normalización al rango **[0,1]**
- División en conjuntos de entrenamiento y validación

---

## 🔄 Aumento de Datos (Data Augmentation)

Para reducir el sobreajuste y mejorar la generalización del modelo, se aplican:

- Rotación
- Desplazamiento horizontal y vertical
- Zoom
- Volteo horizontal

---

## 🧹 Limpieza y Control de Calidad

Se implementan procesos para:

- Eliminar imágenes corruptas o no legibles
- Detectar y eliminar imágenes duplicadas mediante hash
- Verificar consistencia de etiquetas por carpeta
- Confirmar integridad de archivos

---

## 🧠 Modelo de Deep Learning

Se entrena un modelo **CNN (Convolutional Neural Network)** básico utilizando
**TensorFlow/Keras**, con las siguientes características:

- Capas convolucionales y pooling
- Función de activación ReLU
- Capa final Softmax para clasificación binaria
- Optimización con Adam
- Métrica de evaluación: Accuracy

> El entrenamiento del modelo se incluye como validación del pipeline completo,
aunque el enfoque principal del proyecto es el análisis y procesamiento de datos.

---

## 🛠️ Tecnologías Utilizadas

- Python
- Google Colab
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- PIL (Pillow)
- Kaggle API

---

## 🚫 Restricciones Cumplidas

- ❌ No se utiliza `sklearn`
- ✅ Uso exclusivo de frameworks de Deep Learning

---

## 🌐 Enlace al Proyecto

Este proyecto forma parte del portafolio académico y puede ser consultado en:

🔗 **Repositorio GitHub:**  
https://github.com/TU_USUARIO/celebrity-face-classification-deep-learning

---

## 👩‍🎓 Autora

**Amber Grijalba**  
Estudiante de Ingeniería Biomédica  
Universidad Latina de Panamá
