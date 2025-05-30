# 🍷 Proyecto de Clasificación de Calidad de Vinos con Redes Neuronales

> Un proyecto de Inteligencia Artificial para predecir la calidad del vino como verdaderos sommeliers digitales 🍇🧠

![vino](https://img.icons8.com/color/96/wine-bottle.png)

## 🎯 Objetivo

Desarrollar modelos de clasificación utilizando redes neuronales para predecir la **calidad del vino** (clases 4 y 5) a partir de sus características físicas y categóricas. Se comparan diferentes arquitecturas para determinar cuál ofrece el mejor rendimiento.

## 🧪 Arquitecturas evaluadas

| Modelo             | Capas ocultas  | Activación | Descripción                           |
| ------------------ | -------------- | ---------- | ------------------------------------- |
| 💡 Perceptrón      | 0              | Sigmoide   | Modelo lineal sin capas ocultas       |
| 🧱 1 Capa oculta   | 1 (n entradas) | Sigmoide   | Mismo número de neuronas que entradas |
| 🧠 3 Capas ocultas | 3 x 3 neuronas | Sigmoide   | Arquitectura profunda                 |

## 🔍 Etapas del proyecto

### 📊 1. Análisis Exploratorio

* Visualización de distribuciones
* Correlaciones entre variables
* Distribución de clases

### 🧹 2. Preprocesamiento

* Limpieza de valores nulos ❌
* Dumificación de variables categóricas 🔤
* Normalización de datos 📏
* **Tratamiento de outliers** (método IQR) 🚫📈

### ⚖️ 3. Rebalanceo de Clases

* La clase 5 fue subrepresentada.
* Se **triplicaron los ejemplos** de clase 5 para igualar la clase 4.

### 🧠 4. Entrenamiento

* Red neuronal construida con **TensorFlow / Keras**
* Activación: `sigmoid` en todas las neuronas ocultas
* Salida: `softmax`
* Optimizador: `Adam` con `learning_rate=0.001`
* EarlyStopping con `patience=10` 🔁

### 📈 5. Evaluación y Comparación

* Métricas: **Accuracy**, **Precision**, **Recall**, **F1-score**
* Visualización: Matriz de confusión ↔↓
* El modelo con **1 capa oculta** obtuvo el mejor F1 general 🏆

## 📦 Dataset

[📂 Kaggle: Spanish Wine Quality Dataset](https://www.kaggle.com/datasets/fedesoriano/spanish-wine-quality-dataset)

## 👥 Integrantes

* 👨‍💻 Juan Martín Sánchez
* 👨‍💻 Juan Esteban Camargo
* 👨‍💻 Santiago Martínez
* 👨‍💻 Juan Esteban Garzón

## 👨‍🏫 Profesor

**Julio Omar Palacio Niño**
Pontificia Universidad Javeriana 🏛️

## 🛠 Tecnologías usadas

* Python 3 🐍
* TensorFlow / Keras 🤖
* Pandas / NumPy 🧮
* Matplotlib / Seaborn 🎨
* Google Colab 🚀

## 📝 Licencia

Este proyecto fue realizado con fines académicos. El uso externo debe contar con autorización de los autores o del docente de la asignatura.

---

> "Las redes neuronales no saben de vino... pero aprenden muy rápido" 🍷🧠
