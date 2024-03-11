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

    



  
