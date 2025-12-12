🧠 Clasificación de Prendas de Ropa — Fashion-MNIST (CNN con TensorFlow)

Este proyecto implementa una red neuronal convolucional (CNN) usando TensorFlow/Keras para clasificar imágenes del dataset Fashion-MNIST, compuesto por 70,000 imágenes en escala de grises de 10 categorías de ropa.

🎯 Objetivos del proyecto

Cargar y explorar el dataset Fashion-MNIST

Preprocesar y normalizar las imágenes

Construir una arquitectura CNN eficiente

Entrenar y validar el modelo

Evaluar su rendimiento en datos no vistos

Visualizar predicciones reales vs predichas

📂 Dataset: Fashion-MNIST

El dataset contiene 10 clases de ropa:

Clase	Etiqueta
0	T-shirt/top
1	Trouser
2	Pullover
3	Dress
4	Coat
5	Sandal
6	Shirt
7	Sneaker
8	Bag
9	Ankle boot
🧱 Arquitectura del Modelo (Resumen)

Conv2D (32 filtros) + ReLU

MaxPooling2D

Conv2D (64 filtros) + ReLU

MaxPooling2D

Flatten

Dense(128) + ReLU

Dropout(0.3)

Dense(10, softmax)

📌 Total de parámetros entrenables: 225,034
📌 Precisión final en el conjunto de prueba: ≈ 90.3%

📊 Resultados

El modelo alcanzó un 90%+ de accuracy clasificando correctamente la mayoría de las prendas.

Incluye visualización de:

Imágenes de entrenamiento

Predicciones del modelo

Comparación Real vs Predicho
-Como ejecutar el proyecto
Clonar el repositorio
git clone https://github.com/EmilianoCR2006/clasificacion-ropa-fashion-mnist.git

-Instalar dependencias
pip install tensorflow numpy matplotlib scikit-learn

-Abrir el notebook
jupyter notebook Proyecto1.ipynb

 Tecnologías usadas

Python

TensorFlow / Keras

NumPy

Matplotlib

Scikit-Learn

Jupyter Notebook

Licencia

Este proyecto está bajo la licencia MIT, lo que permite uso libre del código con atribución.

Autor

EmilianoCR2006
Proyecto personal / portafolio de Deep Learning.
