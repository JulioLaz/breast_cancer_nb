CÁNCER DE MAMA

PREDICCIÓN PARA LA DETERMINACIÓN DE TUMORES MAMARIOS SEGÚN SU CONDICIÓN DE BENIGNO O MALIGNO

imagen ilustrativa de la app

¿Sabías que el cáncer de mama representa el 25% de todos
los casos de cáncer diagnosticados entre las mujeres?


¡El cáncer de mama sigue siendo una de las
principales causas de muerte en las mujeres!


La detección temprana a través de mamografías y la conciencia sobre el autoexamen de senos son
importantes para mejorar las tasas de supervivencia.



Este proyecto de ciencia de datos con machine learning utilizando Logistic Regression predice si un tumor es maligno o benigno de acuerdo al conjunto de datos (30 features) obtenidos de las características que se calculan a partir de una imagen digitalizada de una aspiración con aguja fina (PAAF) de una masa mamaria. Describen características de los núcleos celulares presentes en la imagen.


Fuente de datos:
https://www.kaggle.com/uciml/breast-cancer-wisconsin-data

La base de datos tiene 569 muestras, con un target (diagnóstico) que presenta la siguiente distribución:



Observamos que la distribución de la característica diagnóstico presenta una buena distribución prácticamente de 60:40.


Entre las principales características, podemos observar su distribución:











En la siguiente gráfica de puntos, podemos observar que a medida que aumenta el radio observado la tendencia es a tumor maligno:






Scores obtenidas con los distintos modelos de machine learning




Por lo tanto, los modelos con mejor puntuación son Logistic Regression y MLP Classifier. Pero después de evaluar las métricas y la estabilidad de los modelos, consideré elegir Logistic Regression:





Es importante destacar en primer lugar Recall con 98.41%, lo que sugiere una buena predicción para los tumores malignos distinguiendo con mucha certeza los falsos negativos (es decir tumores que son malignos pero que se predicen como benignos) Observamos con claridad en la matriz de confusión donde los verdaderos positivos son 62 contra los falsos negativos que son 1. Por otra parte la exactitud con un 98.25% indica que predice con mucha certeza los verdaderos negativos, es decir los tumores benignos.


Conclusión: 

La predicción tiene una buena performance de acuerdo a la evaluación de las métricas. El modelo de Logistic Regression nos ayuda a determinar de forma confiable los tumores, evitando los falsos negativos.

Te invito a probar la app:
https://breast-cancer-6c5r.onrender.com



¡El cuidado y la prevención ayudan a salvar vidas!
Autor: Julio A. Lazarte
