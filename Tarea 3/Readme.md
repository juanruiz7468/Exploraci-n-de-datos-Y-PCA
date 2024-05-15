# Clasificacion Dataset plantas
¿Se puede diferenciar una maleza de una plántula de cultivo?

La capacidad de hacerlo de manera efectiva puede significar mejores rendimientos de los cultivos y una mejor administración del medio ambiente.

El grupo de Procesamiento de Señales de la Universidad de Aarhus, en colaboración con la Universidad del Sur de Dinamarca, ha publicado recientemente un conjunto de datos que contiene imágenes de aproximadamente 960 plantas únicas pertenecientes a 12 especies en varias etapas de crecimiento.

Estamos organizando este conjunto de datos como una competencia de Kaggle para darle una exposición más amplia, para dar a la comunidad la oportunidad de experimentar con diferentes técnicas de reconocimiento de imágenes, así como para proporcionar un lugar para la polinización cruzada de ideas.

![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/9eb07fc4-ff83-4a02-a6bf-bf5ea4fe08af)

- **1** Red Neuronal Sencilla:
    utilizando imagenes de 30x30 , en blanco y negro con 5544 imagenes para entrenar una red neuronal con una capa de entrada de 5000 neuronas, con         entradas de 900 pixeles por cada imagen , utilizando un optimizador de adam y una capa de salida de 12 neuronas ,además de una funcion de               activacion de softmax.
    la función de perdida utilizada es la cross entropy y las metricas utilizadas para observar la calidad del entrenaiento es el accuraccy.

    en la siguiente grafica observamos cuanto fue el accuracy del modelo con respecto a los EPOCHS Utilizados:

  ![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/8450dc32-8eaf-4db4-b9d8-598b773f7339)

    solo obtuvimos un accuracy de casi el 20% , lo cual es muy bajo.

- **2** Red Convolucionales:
  
          utilizando las mismas imagenes con el mismo tamaño y tambien en blanco y negro , se diseña una red convulucional que aprenda lo mas                    importante de las imagenes.La arquitectura de la red convulucional es la primera capa de entrada una convolucion en dos dimensiones
          de imagenese 30 x 30 con un solo canal ,una funcion de activacion de relu y 32 filtros. para la siguiente capa se hizo un maxpooling
          en 2 dimensiones con kernels de 2x2 , en las siguientes capas se siguieron los mismos pasos solo se aumentaron el numero de filtros en las            etapas de convolucion.
  
          por ultimo se paso la imagen de cada filtro a un vector para luego entrarla a una red neuronal , que en su primera capa de entrada tiene              5000 neuronas y en la capa de salida 12 ( siguiendo los mismos parametros que la red neuronal anteriros , solo cambia el optimizador que en
          este caso es el rmsprop).
  
          obtuvimos los siguientes resultados medidas para los datos de entrenamiento y la metrica del accuracy:
  
![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/6449fc3d-93a6-47ef-b357-f4b0e84a55d1)


    
