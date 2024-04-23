Utilizar la base de datos ‘pruebas_saber_2023_scores.xlsx’ saque el promedio por institucion educativa de los puntajes por cada competencia. Es decir , las siguientes
columnas.

| INST_NOMBRE_INSTITUCION                                 | MOD_LECTURA_CRITICA_PUNT | MOD_COMPETEN_CIUDADA_PUNT | MOD_INGLES_PUNT | MOD_COMUNI_ESCRITA_PUNT | PUNT_GLOBAL |
|---------------------------------------------------------|---------------------------|----------------------------|-----------------|--------------------------|-------------|
| CENTRO DE EDUCACION MILITAR-BOGOTÁ D.C.                | 140.000000                | 89.000000                  | 172.000000      | 158.000000               | 143.000000  |
| COLEGIO DE ESTUDIOS SUPERIORES DE ADMINISTRACION-CESA-BOGOTÁ D.C. | 187.285714     | 189.571429                | 213.285714      | 174.428571               | 188.142857  |
| COLEGIO MAYOR DE ANTIOQUIA-MEDELLIN                    | 142.661972                | 137.821596                | 145.258216      | 145.328638               | 142.394366  |
| COLEGIO MAYOR DE NUESTRA SEÑORA DEL ROSARIO-BOGOTÁ D.C.| 181.581901                | 181.940435                | 199.011455      | 162.762887               | 178.395189  |
| COLEGIO MAYOR DEL CAUCA-POPAYAN                        | 137.677596                | 128.234973                | 142.546448      | 144.786885               | 137.644809  |
| ...                                                     | ...                       | ...                        | ...             | ...                      | ...         |
| UNIVERSIDAD TECNOLOGICA DE PEREIRA - ITP-PEREIRA       | 156.645094                | 145.832985                | 162.039666      | 145.720251               | 153.371608  |
| UNIVERSIDAD TECNOLOGICA DEL CHOCO"DIEGO LUIS CORDOBA"-QUIBDO | 120.780965           | 107.649283                | 118.887875      | 122.267275               | 116.397653  |
| UNIVERSIDAD-COLEGIO MAYOR DE CUNDINAMARCA-BOGOTÁ D.C. | 154.793233                | 145.127820                | 153.289474      | 146.759398               | 150.387218  |
| UNIVERSITARIA AGUSTINIANA- UNIAGUSTINIANA-BOGOTÁ D.C.  | 144.581651                | 131.590826                | 154.227523      | 141.267890               | 142.963303  |
| UNIVERSITARIA VIRTUAL INTERNACIONAL-BOGOTÁ D.C.        | 137.221477                | 128.932886                | 147.107383      | 142.281879               | 137.147651  |
  
  Crear 5 clusters. Seleccione colocar el centroide de cada cluster, describa que significada cada cluster. Colocar el nombre d ela institucion mas     cercana al centroide.

https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/blob/main/Tarea%202/K_means.xlsx

Realizar la exploración de los datos correlación, scatter plots, boxplots e histogramas
        ![newplot (24)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/4b5fee05-6b49-4c3d-a171-8dee5bc0469e)
        ![newplot (25)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/6f24c740-c6c4-4191-8022-d9b7bf6722c9)
        ![newplot (26)](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/f81b340b-aecd-4ebb-bb82-ec058a67acb7)
  1.2. Existen nulos?, ¿cómo se deben imputar?
        si existen nulos dentro del dataframe , se deben eliminar con el metodo fillna de la libreria pandas
  1.3. Crear dummy variables para incluirlas en la correlación
        ![image](https://github.com/juanruiz7468/Exploraci-n-de-datos-Y-PCA/assets/126533316/310ad6cc-b877-4ec1-a447-8387f8637390)
        
  1.4. Crear una correlación, que variables tienen un efecto positivo en el puntaje y cuales un efecto negativo.
  
  1.1. ¿Qué variables son importantes para predecir el valor?
  
        - ESTU_ESTADOCIVIL_Soltero
        - ESTU_ESTADOCIVIL_Unión libre
        - ESTU_VALORMATRICULAUNIVERSIDAD_Más de 7 millones
        - ESTU_PAGOMATRICULAPADRES_Si
        - ESTU_PAGOMATRICULAPROPIO_Si
        - ESTU_COMOCAPACITOEXAMENSB11_Repasó por cuenta propia
        - ESTU_TIPODOCUMENTOSB11_TI
        - FAMI_EDUCACIONPADRE_Ninguno
        - FAMI_EDUCACIONPADRE_Postgrado
        - FAMI_EDUCACIONPADRE_Primaria incompleta
        - FAMI_EDUCACIONMADRE_Postgrado
        - FAMI_EDUCACIONMADRE_Primaria incompleta
        - FAMI_TIENEHORNOMICROOGAS_Si
        - FAMI_TIENEMOTOCICLETA_Si
        - FAMI_TRABAJOLABORPADRE_Trabaja como profesional (por ejemplo médico, abogado, ingeniero)
        - FAMI_TRABAJOLABORMADRE_Trabaja como profesional (por ejemplo médico, abogado, ingeniero)
        - ESTU_VLRULTIMOSEMESCURSADO_Entre un millón y 3 millones de pesos
        - ESTU_VLRULTIMOSEMESCURSADO_Más de 7 millones
        - INST_NOMBRE_INSTITUCION_FUNDACIÓN DE EDUCACIÓN SUPERIOR SAN JOSÉ - FESSANJOSÉ - BOGOTÁ D.C.
        - INST_NOMBRE_INSTITUCION_UNIVERSIDAD NACIONAL DE COLOMBIA - BOGOTÁ D.C.
        - ESTU_METODO_PRGM_DISTANCIA VIRTUAL
        - ESTU_METODO_PRGM_PRESENCIAL
        - INST_CARACTER_ACADEMICO_INSTITUCIÓN UNIVERSITARIA
        - INST_CARACTER_ACADEMICO_UNIVERSIDAD
        - ESTU_MCPIO_PRESENTACION_BOGOTÁ D.C.
        - ESTU_DEPTO_PRESENTACION_BOGOTÁ
        - INST_COD_INSTITUCION
        - ESTU_SNIES_PRGMACADEMICO
        - ESTU_NSE_INDIVIDUAL
        - ESTU_NSE_IES
        - edad
        
    2.2. Entrenar un modelos de regresión
    
| Variable | Coeficiente | Error estándar | t     | P>|t|   | Intervalo de confianza (95%) |
|----------|-------------|-----------------|-------|---------|-------------------------------|
| const    | 150.9882    | 4.670           | 32.334| 0.000   | [141.834, 160.143]           |
| ESTU_ESTADOCIVIL_Soltero | -1.3693 | 1.605    | -0.853| 0.394   | [-4.515, 1.777]             |
| ESTU_ESTADOCIVIL_Unión libre | -4.8700 | 1.832 | -2.658| 0.008   | [-8.462, -1.278]           |
| ...      | ...         | ...             | ...   | ...     | ...                           |
| edad     | -0.2863     | 0.078           | -3.693| 0.000   | [-0.438, -0.134]            |



  2.3. ¿Cuál es el mejor R squared? Cuál es el MAPE y el MSE.
  
        training mse error:787.0441320191331
        training MAPE error:0.16826065130562573

  3. Remueva las variables que nos son relevantes
     
        ESTU_ESTADOCIVIL_Unión libre
        ESTU_VALORMATRICULAUNIVERSIDAD_Más de 7 millones
        ESTU_PAGOMATRICULAPADRES_Si
        ESTU_PAGOMATRICULAPROPIO_Si
        ESTU_COMOCAPACITOEXAMENSB11_Repasó por cuenta propia
        ESTU_TIPODOCUMENTOSB11_TI
        FAMI_EDUCACIONPADRE_Ninguno
        FAMI_EDUCACIONPADRE_Postgrado
        FAMI_EDUCACIONMADRE_Primaria incompleta
        FAMI_TIENEHORNOMICROOGAS_Si
        FAMI_TIENEMOTOCICLETA_Si
        INST_NOMBRE_INSTITUCION_UNIVERSIDAD NACIONAL DE COLOMBIA-BOGOTÁ D.C.
        ESTU_METODO_PRGM_PRESENCIAL
        INST_CARACTER_ACADEMICO_UNIVERSIDAD
        ESTU_MCPIO_PRESENTACION_BOGOTÁ D.C.
        ESTU_DEPTO_PRESENTACION_BOGOTÁ
        INST_COD_INSTITUCION
        ESTU_NSE_IES
        edad

     
  5. Utilizando los datos de test medir el MAPE y el MSE de test. Qué tan diferentes son las métricas de training.
        test mse error:1160.835235350644
        test MAPE error:0.20672507574194635

     
  7. Describa en palabras que dice el modelo cuales son los principales hallazgos.
        el modelo es bueno ya que presenta un MAPE 20,67% y un mean square error del 33,94% para test lo cual esta alejado de una regresion perfecta          , pero esta bien.

Utilizar los datos para crear un modelo de KNN que permita predecir el puntaje por estudiante. Utilizar el dataset de la carpeta datos. ‘Pruebas_saber_2023.xlsx’ y las mismas transformaciones dle punto anterior.
    1) Hacer pruebas con 5, 10, 20 y 30 vecinos. Seleccione el numero de vecinos basado en el error de test MSE.


    
|   | MSE Train | MAPE Train | MSE Test | MAPE Test | Vecinos |
|---|-----------|------------|----------|-----------|---------|
| 0 | 610.420   | 0.146      | 914.107  | 0.183     | 5       |
| 1 | 684.289   | 0.156      | 846.441  | 0.177     | 10      |
| 2 | 732.497   | 0.162      | 824.524  | 0.175     | 20      |
| 3 | 752.367   | 0.164      | 818.616  | 0.174     | 30      |


    2) Describa cual es mejor modelo entre la regresion o el knn
    
        El Knn es mejor dado que , para el MAPE en test fue menor alrededor 17,4% si se toman 30 vecinos lo cual disminuye el error casi en un 3% ,
        ademas que el Mean Square Error tambien fue menor de un 28,61% una disminucion de casi un 5%.
    


        


        





        
