# Clasificacion Dataset plantas
¿Se puede diferenciar una maleza de una plántula de cultivo?

La capacidad de hacerlo de manera efectiva puede significar mejores rendimientos de los cultivos y una mejor administración del medio ambiente.

El grupo de Procesamiento de Señales de la Universidad de Aarhus, en colaboración con la Universidad del Sur de Dinamarca, ha publicado recientemente un conjunto de datos que contiene imágenes de aproximadamente 960 plantas únicas pertenecientes a 12 especies en varias etapas de crecimiento.

Estamos organizando este conjunto de datos como una competencia de Kaggle para darle una exposición más amplia, para dar a la comunidad la oportunidad de experimentar con diferentes técnicas de reconocimiento de imágenes, así como para proporcionar un lugar para la polinización cruzada de ideas.

![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/9eb07fc4-ff83-4a02-a6bf-bf5ea4fe08af)

- **1** Red Neuronal Sencilla
    utilizando imagenes de 30x30 , en blanco y negro con 5544 imagenes para entrenar una red neuronal con una capa de entrada de 5000 neuronas, con         entradas de 900 pixeles por cada imagen , utilizando un optimizador de adam y una capa de salida de 12 neuronas ,además de una funcion de               activacion de softmax.
    la función de perdida utilizada es la cross entropy y las metricas utilizadas para observar la calidad del entrenaiento es el accuraccy.

    en la siguiente grafica observamos cuanto fue el accuracy del modelo con respecto a los EPOCHS Utilizados:

  ![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/8450dc32-8eaf-4db4-b9d8-598b773f7339)

    
