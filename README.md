Clasificación de Prendas de Ropa — Fashion-MNIST (CNN con TensorFlow)

Este proyecto implementa una red neuronal convolucional (CNN) utilizando TensorFlow/Keras para clasificar imágenes del dataset Fashion-MNIST, el cual contiene 70,000 imágenes en escala de grises distribuidas en 10 categorías de prendas de vestir.
El objetivo del proyecto es demostrar el uso de redes neuronales convolucionales para resolver un problema real de visión por computadora.

Objetivos del Proyecto

Cargar y explorar el dataset Fashion-MNIST.

Preprocesar y normalizar las imágenes.

Construir una arquitectura de red neuronal convolucional.

Entrenar y validar el modelo.

Evaluar su rendimiento en datos de prueba.

Visualizar predicciones generadas por el modelo.

Dataset: Fashion-MNIST

El dataset contiene imágenes en escala de grises (28x28 px) pertenecientes a las siguientes 10 clases:

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
Arquitectura del Modelo

El modelo implementado consiste en una red neuronal convolucional con la siguiente estructura:

Capa Conv2D con 32 filtros y activación ReLU

Capa MaxPooling2D

Capa Conv2D con 64 filtros y activación ReLU

Capa MaxPooling2D

Capa Flatten

Capa Dense con 128 unidades y activación ReLU

Capa Dropout (para reducir sobreajuste)

Capa Dense final con 10 unidades y activación softmax

Total de parámetros entrenables: 225,034
Precisión final en el conjunto de prueba: aproximadamente 90.37 %

Resultados del Modelo
Rendimiento General

El modelo entrenado alcanzó una exactitud de prueba de:

Accuracy en test: 0.9037 (aprox. 90.37 %)

Este resultado indica que el modelo es capaz de identificar prendas del dataset con un alto nivel de precisión.

Curvas de Entrenamiento

Se observaron mejoras progresivas en el rendimiento del modelo a lo largo de las épocas:

Accuracy (Entrenamiento)
Epoch 1 → 0.7777  
Epoch 5 → 0.8959  
Epoch 10 → 0.9205  

Accuracy (Validación)
Epoch 1 → 0.8647  
Epoch 5 → 0.9135  
Epoch 10 → 0.9135  


La validación se mantuvo cercana al desempeño de entrenamiento, lo que indica una buena generalización sin sobreajuste significativo.

Ejemplos de Predicciones

Ejemplos representativos del comportamiento del modelo:

Imagen	Clase real	Predicción
Ankle boot	Ankle boot	Correcta
T-shirt/top	T-shirt/top	Correcta
Pullover	Pullover	Correcta
Trouser	Trouser	Correcta
Coat	Coat	Correcta
Sneaker	Sneaker	Correcta
Dress	Dress	Correcta

El modelo clasifica correctamente la mayoría de los ejemplos visualizados, confirmando su buen desempeño.

Interpretación de Resultados

El modelo aprende patrones visuales relevantes para cada clase.

La precisión se estabiliza alrededor del 91 %.

Las curvas de entrenamiento muestran una convergencia adecuada.

Las predicciones indican un comportamiento robusto y confiable.

Instrucciones para Ejecutar el Proyecto
1. Clonar el repositorio
git clone https://github.com/EmilianoCR2006/clasificacion-ropa-fashion-mnist.git

2. Instalar dependencias
pip install tensorflow numpy matplotlib scikit-learn

3. Ejecutar el notebook
jupyter notebook Proyecto1.ipynb

Tecnologías Utilizadas

Python

TensorFlow / Keras

NumPy

Matplotlib

Scikit-Learn

Jupyter Notebook

Licencia

Este proyecto está distribuido bajo la licencia MIT, lo que permite su uso y modificación siempre que se brinde atribución correspondiente.

Autor

EmilianoCR2006
Proyecto académico de clasificación de imágenes mediante redes neuronales convolucionales.
