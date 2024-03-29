# Exploracion-de-datos-Y-PCA
| DEPARTAMENTO | PIB en Millones (X1) | Población (X2) | PIB per cápita en Millones (X3) |
|--------------|-----------------------|----------------|----------------------------------|
| Amazonas     | 1067855.672           | 76589          | 13.94267678                      |
| Antioquia    | 212514957.4           | 6407102        | 33.16865524                      |
| Arauca       | 8548114.653           | 262174         | 32.60473828                      |
| Atlántico    | 63764770.77           | 2535517        | 25.1486268                       |
| Bogotá D.C.  | 357258620.8           | 7412566        | 48.19634938                      |
| Bolívar      | 51404352.37           | 2070110        | 24.83170091                      |
| Boyacá       | 38858162.12           | 1217376        | 31.91960588                      |
| Caldas       | 23953112.45           | 998255         | 23.9949837                       |
| Caquetá      | 5461366.78            | 401849         | 13.59059443                      |
| Casanare     | 23660657.37           | 420504         | 56.26737766                      |
| Cauca        | 25758151.71           | 1464488        | 17.58850309                      |
| Cesar        | 37523918.98           | 1200574        | 31.25498218                      |
| Chocó        | 6001844.915           | 534826         | 11.2220515                       |
| Córdoba      | 24991953.76           | 1784783        | 14.00279685                      |
| Cundinamarca | 91945942.28           | 2919060        | 31.49847632                      |
| Guainía      | 497704.0127           | 48114          | 10.34426597                      |
| Guaviare     | 1123857.696           | 82767          | 13.57857232                      |
| Huila        | 24011616.06           | 1100386        | 21.82108466                      |
| La Guajira                               | 22262575.88           | 880560         | 25.28229295                      |
| Magdalena                                | 19738417.36           | 1341746        | 14.710994                        |
| Meta                                     | 58439500.07           | 1039722        | 56.20685151                      |
| Nariño                                   | 21775426.15           | 1630592        | 13.35430699                      |
| Norte de Santander                       | 23056874.23           | 1491689        | 15.45689097                      |
| Putumayo                                 | 5616558.269           | 348182         | 16.13109888                      |
| Quindío                                  | 11941644.16           | 539904         | 22.11808795                      |
| Risaralda                                | 23786362.42           | 943401         | 25.21341659                      |
| San Andrés, Providencia y Santa Catalina | 2125410.333           | 61280          | 34.68358898                      |
| Santander                                | 92276678.16           | 2184837        | 42.23504003                      |
| Sucre                                    | 11516270.76           | 904863         | 12.7270877                       |
| Tolima                                   | 30438180.15           | 1330187        | 22.8826324                       |
| Valle del Cauca                          | 139863153.5           | 4475886        | 31.2481492                       |
| Vaupés                                   | 381851.6785           | 40797          | 9.359797989                      |
| Vichada                                  | 956576.6785           | 107808         | 8.872965629                      |

Datos:
Media (Promedio):
  - promedio_PIB_DEPARTAMENTOS: 44318861.80599092
  - promedio_POBLACION: 1462378.606060606
  - promedio_PIB_per_capita: 24.407855870242425

Mediana:
  - La mediana de los datos es 17.0

Desviación Estándar:
  - Desviación estándar de PIB en Millones: 71673456.53928636
  - Desviación estándar de Población: 1705549.0329603895
  - Desviación estándar de PIB per cápita en Millones: 12.766733645850927

Moda:
  - No hay moda en los datos

Para el PIB en millones y la población:
- Covarianza: 113,233,718,703,629.06
- Correlación: 0.9552502783564497

Para el PIB en millones y el PIB per cápita en millones:
- Covarianza: 466,198,063.93045557
- Correlación: 0.5254075147557418
- Covarianza: La covarianza es una medida de la relación lineal entre dos variables. Indica si las variables tienden a aumentar o disminuir juntas. Si la covarianza es positiva, significa que las dos variables tienden a aumentar o disminuir juntas. Si es negativa, significa que una variable tiende a aumentar mientras que la otra tiende a disminuir. Sin embargo, la covarianza no proporciona información sobre la fuerza o la intensidad de la relación entre las variables. Por lo tanto, es difícil interpretar su magnitud en términos de la fuerza de la relación.

-Correlación: La correlación, por otro lado, es una medida estandarizada que indica la fuerza y la dirección de la relación lineal entre dos variables. A diferencia de la covarianza, la correlación está limitada a valores entre -1 y 1. Un coeficiente de correlación cercano a 1 indica una relación lineal positiva fuerte, mientras que un coeficiente cercano a -1 indica una relación lineal negativa fuerte. Un coeficiente de correlación cercano a 0 indica una relación débil o nula. Por lo tanto, la correlación no solo indica la dirección de la relación, sino también la fuerza de la relación entre las variables.

2. **PCA**:
-Matriz de covarianza:

|          | Variable 1 | Variable 2 | Variable 3 |
|----------|------------|------------|------------|
| Variable 1 | 1.03125    | 0.98510185 | 0.5418265  |
| Variable 2 | 0.98510185 | 1.03125    | 0.4212694  |
| Variable 3 | 0.5418265  | 0.4212694  | 1.03125    |

| EigenValues |
|-------------|
| 2.36491665  |
| 0.03659132  |
| 0.69224202  |

| EigenVectores|
|---------------------------|
| -0.64120229               |
| -0.61751702               |
| -0.45555718               |

| Datos Proyectados |
|-------------------|
|  1.28167345       |
| -3.66356153       |
|  0.46923492       |
| -0.59807495       |
| -5.89277461       |
| -0.30317836       |
| -0.13250718       |
|  0.37062885       |
|  1.13492648       |
| -0.58372383       |
|  0.41495487       |
| -0.09012447       |
|  1.16695117       |
|  0.4340836        |
| -1.22521294       |
|  1.42771627       |
|  1.292087         |
|  0.41132039       |
|  0.38261347       |
|  0.61904339       |
| -1.12516417       |
|  0.54349679       |
|  0.50673639       |
|  1.06118998       |
|  0.71628864       |
|  0.34816069       |
|  0.52611842       |
| -1.34731502       |
|  0.92626206       |
|  0.22997664       |
| -2.22387303       |
|  1.46713265       |
|  1.45491398       |

-Error:Error Cuadrático Medio (MSE): 0.2286218284334619

-Varianza Explicada = 2.36491665 / (2.36491665 + 0.03659132 + 0.69224202) ≈ 0.7639

3.**PCA**

  -Calcular la mean face. Que es la cara con el promedio de los pixeles y
    visualizarla
    ![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/0b8f5c1e-6a02-4e5c-b9e2-e1be999beb2b)

  -¿Cuántos componentes se deben utilizar para mantener el 90% de las características?: se deben utilizar 46 componentes

  -Crear una tabla para mostrar las primeras 5 caras utilizando, la mean face + los datos reconstruidos utilizando la primera componente, después con 3 componentes, después con las primeras 20 componentes, después con las componentes que explican el 95% de la varianza y por último con el numero de componentes que tiene el 99% de la varianza. ¿Qué se puedeconcluir de los resultados?:
  
  ![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/a20ef5b4-3b89-43ac-8c76-e7d65ea9b4e9)
  se concluye que entre mas componentes yo utilize y se los sume a la media mejor se vera la cara ,ademas de que con 161 componentes ya estoy representando con exactitud el 99% de los datos por lo tanto es irrelevantes utilizar mas de 161 componentes.

  4.**Utilizando el dataset del proyecto data/CARS.csv**

  -Para las variables categóricas un gráfico de barras. Categoría numero de observaciones:
  ![newplot](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/281c8f38-1c68-40b4-b1f1-58e7a53e1b56)
  
  ![newplot (1)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/4748717f-9ff8-47be-a6cb-9630d98541fa)
  
  ![newplot (2)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/5c9f745c-4320-42b7-ac35-d1ec0cbd2e95)
  
  ![newplot (3)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/1431a970-5d41-44f9-ab10-124f8778fbd2)

  ![newplot (4)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/0bac5d9a-0b88-4518-99a6-f67d5b202f27)

  -Para las variables numéricas crear histogramas. Listar los modelos de carros que están más lejos de 5 estándares de desviación, y serían considerados outliers. Hacer test de si es una distribución normal o no:
  ![newplot (5)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/fc312f4a-8a69-49d7-9cf1-292fa7c86d70)

  ![newplot (6)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/fcc147aa-4f69-4e69-b2c8-9e4faffe9176)

  ![newplot (7)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/a40f0c0e-b6a0-4520-9623-afbf9d4ed477)

  ![newplot (8)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/763c0378-003b-44a0-b0f0-2411e58a5776)

  ![newplot (9)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/ee2e7996-93a6-4dca-91cc-feef96ad36f8)

  Modelos de automóviles con valores atípicos (más de 5 desviaciones estándar) en MPG_City:
  150    Insight 2dr (gas/electric)
  373      Prius 4dr (gas/electric)

  Modelos de automóviles con valores atípicos (más de 5 desviaciones estándar) en MPG_Highway:
  150    Insight 2dr (gas/electric)

  It is not normal MPG_City
  It is not normal MPG_Highway
  It is not normal Weight
  It is not normal Wheelbase
  It is normal Length

  -Variables categóricas debes crear un boxplot. Explique cómo interpreta el gráfico:
  ![newplot (10)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/6808ff24-db42-4f15-a3ae-67bcda53819b)

  ![newplot (11)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/a94470ed-e37f-4bb3-917d-e7498a49459e)

  ![newplot (12)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/1ae21c81-08c4-4ad0-8883-63f433c524bd)

  ![newplot (13)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/cee7c49d-99c8-4625-9a67-aabb66bf543a)

  ![newplot (14)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/2bc3c2f7-885b-4ef4-b745-70e8dd95abba)

  los boxplot me sirven para ver la variabilidad de los datos , si la caja es muy pequeña es por que quiere decir que los datos estan muy concentrados alrededor de la media o la mediana de los datos , por otro lado si el bigote es muy grande me representa que hay muchos datos que son  muy diferentes a los datos ubicados en el primer quartil o en el tercer quartil , es decir donde se ubica el 25% de los datos o donde se ubica el 75% de los datos , por otro lado si la caja es muy grande quiere decir que hay datos muy diferentes a los datos de la media o la mediana y por ultimos si los bigotes y la caja son muy grandes hay demasiada variabilidad en los datos.

  -Variables numéricas vas a crear un scatter plot.Explique cómo interpreta el gráfico:
  ![newplot (15)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/628723ec-d249-47ec-893d-425059371b75)

  ![newplot (16)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/081756f4-e80b-40cf-bfbb-fd42820942a6)

  ![newplot (17)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/6fc87b10-dc21-4224-b947-074072b01d15)

  ![newplot (18)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/3a3b8e21-4760-4611-bb57-2b61ab8394ab)

  ![newplot (19)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/a2fd655f-d726-4014-af3b-6424ae6015be)

  -Cree la matriz de correlación, cuales son las variables más importantes para explicar la variabilidad de MPG_City. Explique por qué el coeficiente es negativo o positivo:
  ![newplot (20)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/6f44a7e9-96ab-49fb-8151-152b19141eb9)

  la variable mas importante para explicar la variabilidad de MPG_City es MPG_Highway , dado que explica su variabilidad en un 94,1 % , ademas de que los ceficientes son negativos o postivos para decir que son inversamentes propocional o propocional en la misma direccion , en otra palabras el signo solo me dice si crece una la otra también crece o si decrece una la otra decrece.

  -¿Cuál es el valor de variable categórica con mayor correlación?:

  Variable categórica con la mayor correlación: Invoice

  -Cree la matriz de correlación nuevamente removiendo todas los modelos de carro que fueron catalogados como un outlier:
  -Matriz Original:
    
|               | Invoice   | EngineSize | Cylinders | Horsepower | MPG_City  | ... |
|---------------|-----------|------------|-----------|------------|-----------|-----|
| Invoice       | 1.000000  | 0.564498   | 0.645226  | 0.823746   | -0.470442 | ... |
| EngineSize    | 0.564498  | 1.000000   | 0.908002  | 0.787435   | -0.709471 | ... |
| Cylinders     | 0.645226  | 0.908002   | 1.000000  | 0.810341   | -0.684402 | ... |
| Horsepower    | 0.823746  | 0.787435   | 0.810341  | 1.000000   | -0.676699 | ... |
| MPG_City      | -0.470442 | -0.709471  | -0.684402 | -0.676699  | 1.000000  | ... |
| ...           | ...       | ...        | ...       | ...        | ...       | ... |

- Matriz Filtrada:
  
|               | Invoice   | EngineSize | Cylinders | Horsepower | MPG_City  | ... |
|---------------|-----------|------------|-----------|------------|-----------|-----|
| Invoice       | 1.000000  | 0.564498   | 0.645226  | 0.823746   | -0.470442 | ... |
| EngineSize    | 0.564498  | 1.000000   | 0.908002  | 0.787435   | -0.709471 | ... |
| Cylinders     | 0.645226  | 0.908002   | 1.000000  | 0.810341   | -0.684402 | ... |
| Horsepower    | 0.823746  | 0.787435   | 0.810341  | 1.000000   | -0.676699 | ... |
| MPG_City      | -0.470442 | -0.709471  | -0.684402 | -0.676699  | 1.000000  | ... |
| ...           | ...       | ...        | ...       | ...        | ...       | ... |


No se observan cambios siginificativos en la correlacion , por lo que la correlacion no es sensible a los outliers.













  








    



  
