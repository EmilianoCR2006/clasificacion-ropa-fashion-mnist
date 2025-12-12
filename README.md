lasificación de Prendas de Ropa — Fashion-MNIST (CNN con TensorFlow)

Este proyecto implementa una red neuronal convolucional (CNN) utilizando TensorFlow/Keras para clasificar imágenes del dataset Fashion-MNIST, el cual contiene 70,000 imágenes en escala de grises, divididas en 10 categorías de prendas de vestir.

Objetivos del proyecto

Cargar y explorar el dataset Fashion-MNIST.

Preprocesar y normalizar las imágenes.

Construir una arquitectura de red neuronal convolucional.

Entrenar y validar el modelo.

Evaluar el rendimiento en datos de prueba.

Visualizar predicciones generadas por el modelo.

Dataset: Fashion-MNIST

El dataset contiene 10 categorías de prendas:

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

Las imágenes tienen resolución de 28x28 píxeles en escala de grises.

Arquitectura del Modelo

La arquitectura implementada se compone de las siguientes capas:

Capa Conv2D con 32 filtros y activación ReLU.

Capa MaxPooling2D.

Capa Conv2D con 64 filtros y activación ReLU.

Capa MaxPooling2D.

Capa Flatten para aplanar los mapas de características.

Capa Dense con 128 unidades y activación ReLU.

Capa Dropout para reducir sobreajuste.

Capa Dense final con 10 unidades y activación softmax para la clasificación.

Total de parámetros entrenables: 225,034
Precisión final en el conjunto de prueba: aproximadamente 90.3%

Resultados

El modelo entrenado logra una precisión superior al 90% en el conjunto de prueba.
También incluye visualización de:

Imágenes del dataset.

Comparaciones de etiquetas reales vs. predichas por el modelo.

Instrucciones para ejecutar el proyecto
1. Clonar el repositorio
git clone https://github.com/EmilianoCR2006/clasificacion-ropa-fashion-mnist.git

2. Instalar dependencias necesarias
pip install tensorflow numpy matplotlib scikit-learn

3. Ejecutar el notebook
jupyter notebook Proyecto1.ipynb

Tecnologías utilizadas

Python

TensorFlow / Keras

NumPy

Matplotlib

Scikit-Learn

Jupyter Notebook

Licencia

Este proyecto está distribuido bajo la licencia MIT, lo cual permite el uso y modificación del código con atribución correspondiente.

Autor

EmilianoCR2006
Proyecto académico enfocado en la aplicación de redes neuronales convolucionales para clasificación de imágenes.
