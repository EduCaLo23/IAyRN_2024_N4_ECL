# Regresión Lineal

Objetivo.- Entrenar uno de los modelos de aprendizaje supervisado más simple: Regresión Lineal. 

Instrucciones.- 
- El estudiante generará un modelo de regresión lineal en Google Colab por medio del lenguaje de programación Python. Este modelo hará la predicción de la calificación de un grupo de estudiantes tomando en cuenta el número de horas dedicadas a estudiar. 
- El conjunto de datos se generará con la función “random” de Numpy de la siguiente manera:

np.random.seed(0)
horas_estudio = np.random.rand(100, 1) * 10 
calificaciones = 2 * horas_estudio + np.random.randn(100,1) * 2

- Durante el preprocesamiento de los datos, se utilizará la función “train_test_split” de la librería scikit-learn para generar los conjuntos de datos de entrenamiento (train_data, train_labels) y datos de prueba (test_data, test_label). Deberán de utilizar una relación de 80% para entrenamiento y 20% para prueba. 
- Se entrenará el modelo de regresión lineal con los datos de entrenamiento con la función “fit” de la librería scikit-learn. 
- Realizar predicciones con el conjunto de datos de prueba (train_data) y graficar el modelo de regresión lineal con estas predicciones. Se utilizará la función “mean_squared_error” de scikit-learn para calcular el error cuadrático medio, que será la métrica a utilizar para evaluar el desempeño del modelo durante la prueba. Se deberá mostrar dicho resultado. 

Recordar la estructura que se ha mencionado en clase para este tipo de proyectos:
  1. Cargar librerías
  2. Cargar datos
  3. Preprocesamiento de datos
  4. Selección y entrenamiento del modelo
  5. Prueba de modelo

# Árbol de decisiones

Objetivo.- Entrenar un árbol de decisión, modelo de aprendizaje supervisado. 

Instrucciones.- 
- El estudiante entrenará un modelo de árbol de decisión en Google Colab por medio del lenguaje de programación Python. Este modelo usará el conjunto de datos “Breast Cancer Wisconsin (Diagnostic)”; este conjunto de datos contiene características calculadas a partir de imágenes digitalizadas de tumores de cáncer de mama y el diagnóstico correspondiente (maligno o benigno).  El conjunto de datos es parte de la librería scikit-learn. Más información acerca de este conjunto de datos: https://medium.com/@shashmikaranam/exploratory-data-analysis-breast-cancer-wisconsin-diagnostic-dataset-6a3be9525cd 
Durante el preprocesamiento de los datos, se utilizará la función “train_test_split” de la librería scikit-learn para generar los conjuntos de datos de entrenamiento (train_data, train_labels) y datos de prueba (test_data, test_label). Deberán de utilizar una relación de 80% para entrenamiento y 20% para prueba. 
- Se entrenará el modelo árbol de decisión con los datos de entrenamiento con la función “fit” de la librería scikit-learn.  
- Realizar predicciones con el conjunto de datos de prueba (test_data).
- Se utilizará la función “accuracy” de scikit-learn para calcular la exactitud, que será la métrica a utilizar para evaluar el desempeño del modelo durante la prueba, así como la función “classification_report” que resume los resultados del desempeño del modelo durante la prueba. Se deberán de mostrar tales resultados.
- Se visualizará la representación gráfica del árbol de decisión. Utilizar resolución dpi = 300.

Recordar la estructura que se ha mencionado en clase para este tipo de proyectos:
  1. Cargar librerías
  2. Cargar datos
  3. Preprocesamiento de datos
  4. Selección y entrenamiento del modelo
  5. Prueba de modelo

# RNP 
Objetivo.- Entrenar un modelo de Red Neuronal Prealimentada (tipo feedforward).

Instrucciones.- 
- El estudiante entrenará un modelo de Red Neuronal Prealimentada en Google Colab por medio del lenguaje de programación Python. Este modelo usará el conjunto de datos MNIST; este conjunto de datos contiene imágenes de baja resolución con dígitos del 0 al 9 escritos a mano. El conjunto de datos es parte de la librería Keras. Más información acerca de este conjunto de datos: https://keras.io/api/datasets/mnist/  
Durante el preprocesamiento de los datos, se utilizará la función “load_data()” de la librería Keras para cargar el conjunto de datos y generar los conjuntos de entrenamiento (train_data, train_labels) y de prueba (test_data, test_label). Se puede utilizar la división de datos predeterminada por esta misma función.
- Se entrenará una red neuronal artificial prealimentada con los datos de entrenamiento utilizando la función “fit” de la librería tensorflow. El estudiante propondrá una estructura de red neuronal artificial prealimentada. La función de activación en la capa de salida deberá ser softmax. 
- Se establecerá el tipo de función de pérdida y optimizador a utilizar. La métrica a utilizar para evaluar el proceso de entrenamiento será la exactitud (accuracy).
- Utilizar la función “evaluate” para mostrar la exactitud de predicción del modelo con el conjunto de datos de prueba (test_data). 
- Realizar 5 diferentes predicciones con el conjunto de datos de prueba (test_data). En el resultado mostrar la predicción y el valor real. 

Recordar la estructura que se ha mencionado en clase para este tipo de proyectos:
  1. Cargar librerías
  2. Cargar datos
  3. Preprocesamiento de datos
  4. Selección y entrenamiento del modelo
  5. Prueba de modelo


# RNC
Objetivo.- Entrenar un modelo de Red Neuronal Convolucional.

Instrucciones.- 
- El estudiante entrenará un modelo de Red Neuronal Convolucional en Google Colab por medio del lenguaje de programación Python. Este modelo usará el conjunto de datos MNIST; este conjunto de datos contiene imágenes de baja resolución con dígitos del 0 al 9 escritos a mano. El conjunto de datos es parte de la librería Keras. Más información acerca de este conjunto de datos: https://keras.io/api/datasets/mnist/  
- Durante el preprocesamiento de los datos, se utilizará la función “load_data()” de la librería Keras para cargar el conjunto de datos y generar los conjuntos de entrenamiento (train_data, train_labels) y de prueba (test_data, test_label). Se puede utilizar la división de datos predeterminada por esta misma función.
- Se entrenará una red neuronal artificial prealimentada con los datos de entrenamiento utilizando la función “fit” de la librería tensorflow. El estudiante propondrá una estructura de red neuronal artificial prealimentada. La función de activación en la capa de salida deberá ser softmax. 
- Se establecerá el tipo de función de pérdida y optimizador a utilizar. La métrica a utilizar para evaluar el proceso de entrenamiento será la exactitud (accuracy).
- Utilizar la función “evaluate” para mostrar la exactitud de predicción del modelo con el conjunto de datos de prueba (test_data). 
- Realizar 5 diferentes predicciones con el conjunto de datos de prueba (test_data). En el resultado mostrar la predicción y el valor real. 

Responde las siguientes preguntas:
  ¿Cuántas épocas usaste para mejorar el rendimiento del modelo en comparación con la red neuronal prealimentada de la actividad 5? 
  ¿Obtuviste un mejor rendimiento con este modelo o con el de la actividad 5? ¿Por qué?

Recordar la estructura que se ha mencionado en clase para este tipo de proyectos:
  1. Cargar librerías
  2. Cargar datos
  3. Preprocesamiento de datos
  4. Selección y entrenamiento del modelo
  5. Prueba de modelo
