# Mineria de texto y procesamiento de lenguaje natural (NLP)

<br>

## Introducción

La minería de texto y el procesamiento de lenguaje natural son dos campos relacionados que se enfocan en extraer y analizar información a partir de texto escrito o hablado. Estos campos se han vuelto cada vez más importantes debido a la enorme cantidad de datos no estructurados que se generan a diario, y a la necesidad de obtener información útil a partir de ellos.

Por un lado, la mineria de texto se enfoca en detectar __tendencias, patrones o relaciones__ en los textos. Para esto se apoya de técnicas estadísticas y de Machine Learning. A raíz de ella han surgido un gran número de métodos como el análisis de sentimientos o la clasificación de documentos que permiten la obtención de insights o señales en datos tan complejos como lo pueden ser los conjuntos de texto.

En contra parte, el procesamiento de lenguaje natural se centra en el __entendimiento y comprensión__ del lenguaje humano. Al igual que la minería de texto, este emplea tecnicas tanto estadísticas como de machine learning. Mediante este se puede conseguir tareas como la traducción automática el análisis estructural del texto, la generación de lenguaje natural y humano y la respuesta automatica de preguntas por medio de, por ejemplo, chatbots.

Gracias a estas dos poderosas herramientas se han generado avances significativos en el análisis y la comprension de grandes conjuntos de texto y datos no estructurados, las cuales estan siendo empleados por diferentes campos del saber como la academia, la industria, la inteligencia artificial o el marketing. 

<br>

| Función            | Minería de Datos                              | Procesamiento del Lenguaje Natural       |
| ------------------|---------------------------------------------- | ---------------------------------------- |
| Objetivo           | Descubrir patrones y relaciones en los datos   | Comprender y generar lenguaje humano     |
| Tipo de datos      | Datos estructurados y no estructurados         | Texto escrito o hablado                  |
| Enfoque            | Análisis estadístico y aprendizaje automático | Análisis semántico y sintáctico          |
| Aplicaciones       | Análisis de mercado, detección de fraudes      | Traducción automática, chatbots, IA      |
| Técnicas           | Clustering, análisis de asociación            | Análisis semántico, procesamiento morfológico|
| Salida             | Patrones, relaciones entre los datos          | Respuestas en lenguaje natural            |
| Ejemplos de uso    | Análisis de ventas en línea, segmentación de clientes | Asistentes virtuales, análisis de sentimiento en redes sociales |

<br>

## Procesamiento de texto: preprocesamiento y normalización de datos de texto

El preprocesamiento y la normalización de datos de texto son técnicas importantes en el procesamiento del lenguaje natural. El objetivo de estas técnicas es transformar los datos de texto en una forma más procesable y significativa para los modelos de aprendizaje automático o para la aplicación de técnicas de minería de texto. A continuación te explico cada técnica:



1. **Preprocesamiento de datos de texto:**
El preprocesamiento de datos de texto consiste en la eliminación de información irrelevante o redundante y la transformación de los datos de texto en una forma más procesable. Algunas técnicas comunes de preprocesamiento son:

    * Tokenización: divide un texto en unidades más pequeñas llamadas tokens (palabras, frases, oraciones) para su posterior procesamiento.
    
    * Eliminación de signos de puntuación y caracteres especiales: elimina los signos de puntuación y los caracteres especiales del texto para reducir el ruido en los datos.

    * Eliminación de palabras vacías (stopwords): elimina las palabras comunes y sin significado que no aportan información relevante para el análisis, como artículos, pronombres y preposiciones.
    
    * Normalización de mayúsculas y minúsculas: convierte todas las letras del texto en mayúsculas o minúsculas para evitar que el modelo distinga entre palabras con mayúsculas y minúsculas.

<br>

2. **Normalización de datos de texto:**
La normalización de datos de texto consiste en la transformación del texto en una forma básica y que sea más significativa para el análisis y la comprensión. Algunas técnicas comunes de normalización son:

    * Lematización: implica reducir cada una de las palabras en el texto a su forma base (también denominado lemas), es decir, eliminando los sufijos y prefijos de la palabra. Por lo tanto, palabras como "saltando", "saltó" y "saltado" se reduce a "saltar", su forma base. El objetivo de esto es efectuar comparaciones mas precisas reduciendo multiples palabras que puedan significar lo mismo a solo una.

    * Stemming: implica reducir las palabras a su raíz (tambien denominado stems), eliminando los sufijos comunes. Por lo tanto, siguiendo el ejemplo anterior, la palabra "saltando" se reduciría a "salt". Su objetivo es similar al de la lematización pero puede ser más rápido, aunque menos intuitivo y podría, en el peor de los casos, generar resultados menos precisos en el sentido que las palabras pueden llegar a ser reducidas a formas que no son correctas.

    * Corrección ortográfica. implica corregir los errores ortográficos, de tal forma que no hayan diferentes palabras producto de una mala digitación u ortografía, por ejemplo, que no hayan palabras como "saltando" "zaltando" o "saltonda", devolviendolas todas a su forma correcta "saltando" y mejorando la precisíon y, por lo tanto, la confiabilidad del análisis.

    *   Eliminación de acentos: implica eliminar todas las tildes de las palabras, evitando tambien un sinumero de palabras similares.
    
Por lo tanto, el preprocesamiento y la normalización de texto son el primer paso en la transformación de texto a una forma más comprensible y relevante para la posterior ejecución de modelos de Machine learning y para diversas técnicas estadísticas sobre ellos, mejorando así la calidad y la precisión del análisis.

<br>

## Métodos de representación de texto

Después de realizar el preprocesamiento y la normalización, se obtiene un conjunto de documentos de texto limpios y procesados que se pueden utilizar para entrenar un modelo de aprendizaje automático o realizar otro tipo de análisis de texto. Sin embargo, la mayoría de los algoritmos de aprendizaje automático requieren que los datos estén en forma numérica, por lo que es necesario convertir el texto en una representación numérica.

Es aquí donde entran en juego los métodos de representación de texto, que transforman el texto en una forma numérica que los algoritmos de aprendizaje automático pueden entender y procesar.

Por ejemplo, la Bolsa de palabras convierte cada documento de texto en un vector de características donde cada dimensión del vector representa una palabra en el vocabulario y el valor de cada dimensión es la frecuencia de aparición de esa palabra en el documento. Las incrustaciones de palabras, por otro lado, asignan un vector numérico a cada palabra en el vocabulario que representa su significado semántico.

<br>

Existen diferentes métodos de representación de texto que se utilizan en el procesamiento de lenguaje natural. A continuación, se describen los más comunes:

1. **Bolsa de palabras (Bag of Words):** Este es uno de los métodos más simples y comunes para representar el texto. En este método, se crea un vector que representa la frecuencia de las palabras en el texto. Se construye un diccionario de palabras a partir del texto y se cuentan las ocurrencias de cada palabra. Cada palabra del diccionario se convierte en una dimensión en el vector y la frecuencia de aparición de cada palabra se convierte en el valor de esa dimensión.

    *Ejemplo:*

    *Supongamos que tenemos el siguiente texto: "Este es un ejemplo de texto de prueba". El diccionario generado a partir de este texto sería: {"este": 1, "es": 1, "un": 1, "ejemplo": 1, "de": 2, "texto": 1, "prueba": 1}. Cada palabra se convierte en una dimensión en el vector y su frecuencia de aparición se convierte en el valor de esa dimensión. Así, el vector resultante sería: [1, 1, 1, 1, 2, 1, 1].*

    *La idea detrás de la Bolsa de palabras es convertir cada palabra en una dimensión en un vector y contar cuántas veces aparece cada palabra en el texto para obtener la frecuencia de aparición. Esto nos permite representar el texto en un espacio vectorial de alta dimensión. En el ejemplo, la palabra "de" aparece dos veces en el texto, por lo tanto tiene el número 2, mientras que el resto de las palabras aparecen una sola vez y por eso tienen el número 1.*

    *Sin embargo, hay algunas limitaciones en el método de Bolsa de palabras, como por ejemplo, que no considera el orden de las palabras en el texto ni su contexto semántico, por lo que puede haber ambigüedades en la interpretación del texto.*

    <br>


2. **Incrustaciones de palabras (Word Embeddings):** Este método utiliza una técnica de aprendizaje profundo para representar las palabras en un espacio de características de dimensiones bajas. En lugar de representar cada palabra en un espacio de alta dimensión, las palabras se representan en un espacio continuo de baja dimensión, lo que permite que las palabras con significados similares se agrupen juntas en el espacio de características. Estas representaciones de palabras son útiles para tareas de análisis de sentimiento, traducción de idiomas, entre otros.

    *Ejemplo:*

    *Supongamos que tenemos el siguiente texto: "El perro corre detrás del gato". Las incrustaciones de palabras se crean utilizando una red neuronal que aprende las relaciones entre las palabras en un corpus de texto. En este caso, las palabras "perro" y "gato" estarían cerca en el espacio de características porque comparten características similares en términos de animales domésticos. Y "corre" estaría cerca de "detrás" porque ambas palabras suelen aparecer juntas en el texto.*

    <br>

3. **N-gramas:** En este método, se crean todas las secuencias contiguas de n palabras en el texto, que se convierten en características. El tamaño del n-grama se elige en función de la longitud del texto y del objetivo del análisis.

    *Ejemplo:*
    
    *Supongamos que tenemos el siguiente texto: "El perro corre detrás del gato". Si tomamos n=2, el conjunto de características generado sería: {"el perro": 1, "perro corre": 1, "corre detrás": 1, "detrás del": 1, "del gato": 1}. Si n=3, el conjunto de características sería: {"el perro corre": 1, "perro corre detrás": 1, "corre detrás del": 1, "detrás del gato": 1}.*

    <br>

4. **Representaciones basadas en subpalabras (Subword representations):** Este método representa las palabras como secuencias de subpalabras, lo que ayuda a capturar mejor la estructura de las palabras y a manejar mejor las palabras raras o desconocidas. Este enfoque también es útil en tareas de análisis de sentimiento, ya que los subpares de las palabras pueden ser fuertes indicadores del sentimiento.

    *Ejemplo:*
    
    *Supongamos que tenemos la palabra "comenzó" que no se encuentra en el vocabulario de la bolsa de palabras. Si utilizamos un modelo de representación basado en subpalabras, la palabra "comenzó" podría descomponerse en los siguientes subpares: {"co", "com", "ome", "men", "enz", "nzó"} y estos subpares se utilizarían para generar una representación de la palabra.*

Cada uno de estos métodos tiene sus ventajas y desventajas y se utilizan en diferentes aplicaciones de procesamiento de lenguaje natural. La elección del método dependerá del problema específico a resolver y del tipo de datos de texto que se esté analizando.

<br>

## Análisis de sentimientos

<!--- IMAGEN -->
![Imagen](https://www.meaningcloud.com/wp-content/uploads/2015/02/176964464-reduced.jpg "Análisis de sentimientos")


El análisis de sentimientos es una técnica novedosa de procesamiento de lenguaje natural que permite distinguir la actitud y la emoción expresada en un texto. La finalidad del análisis de sentimientos es clasificar el texto en diversas categorías como positivo, negativo o neutral, dependiendo de la manifestación de los sentimientos en el texto.

Para llevar a cabo el análisis de sentimientos, se emplean algoritmos de aprendizaje automático y técnicas de minería de texto, que permiten analizar el texto y establecer su polaridad o actitud. El enfoque más utilizado para el análisis de sentimientos es la clasificación supervisada, mediante el cual se entrena un modelo de aprendizaje automático con un conjunto de datos etiquetados con las categorías de sentimiento correspondientes.

Los datos etiquetados pueden ser revisados manualmente por humanos o etiquetados automáticamente por medio de técnicas de análisis de texto y minería de datos. Una vez que el modelo está entrenado, se puede utilizar para clasificar nuevos textos en las categorías de sentimiento que les corresponde.

El análisis de sentimientos se aplica en una gran cantidad de aplicaciones, tales como la monitorización de la reputación en línea de una marca o empresa, la evaluación de la satisfacción del cliente, la identificación de tendencias en las opiniones de los usuarios y la detección de noticias falsas o propaganda.

<br>

*Ejemplo:*

En el análisis de sentimientos, se puede ejemplificar el proceso de clasificación de comentarios de clientes de un hotel según su tono emocional. Para ello, se hace uso de un modelo de aprendizaje automático que ha sido previamente entrenado con un conjunto de datos etiquetados de comentarios de clientes, donde cada comentario se asocia a una categoría específica, como "excelente", "malo" o "neutral". De esta forma, al recibir un nuevo comentario como "Mi estancia en el hotel fue maravillosa, el personal fue extremadamente amable y servicial", el modelo lo clasificaría como un comentario positivo y lo ubicaría en su respectiva categoría.

Una vez que se completa el entrenamiento del modelo, se habilita la clasificación de nuevos comentarios de los clientes en las categorías apropiadas. Por ejemplo, si un nuevo comentario indica "Mi estancia en el hotel fue excepcional, el personal fue extremadamente amable y servicial", el modelo lo categorizaría como un comentario positivo.

<br>

*En general, el procedimiento que se sigue para el análisis de sentimientos es el siguiente:*

| Paso | Descripción |
| --- | --- |
| Paso 1 | Recopilar datos de texto relevantes, como comentarios de clientes, publicaciones en redes sociales, reseñas de productos, etc. |
| Paso 2 | Realizar el preprocesamiento y normalización de los datos de texto, incluyendo la eliminación de caracteres no deseados, la eliminación de stopwords, la lematización o el stemming, etc. |
| Paso 3 | Crear una representación de los datos de texto utilizando técnicas como la bolsa de palabras, incrustaciones de palabras o n-gramas. |
| Paso 4 | Dividir los datos en conjuntos de entrenamiento y prueba. |
| Paso 5 | Entrenar un modelo de aprendizaje automático utilizando el conjunto de entrenamiento etiquetado con las categorías de sentimiento correspondientes, utilizando algoritmos de clasificación supervisada como Naive Bayes, SVM, redes neuronales, etc. |
| Paso 6 | Evaluar el rendimiento del modelo utilizando el conjunto de prueba, midiendo métricas como la precisión, la exhaustividad y la puntuación F1. |
| Paso 7 | Utilizar el modelo entrenado para clasificar nuevos datos de texto en las categorías de sentimiento correspondientes, como positivo, negativo o neutral. |
| Paso 8 | Analizar los resultados y utilizarlos para tomar decisiones empresariales, mejorar la experiencia del cliente, etc. |

<br>

A continuación, se muestra un ejemplo de análisis de sentimientos ilustrando cada uno de los pasos mencionados anteriormente. Para esto se emplea el enfoque de análisis supervisado mediante el método de vectorización de bolsa de palabras. 

<br>

Se importan las librerias necesarias.

```python
import pandas as pd
from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer
from sklearn.linear_model import SGDClassifier
from sklearn.metrics import accuracy_score
from sklearn.model_selection import train_test_split
from nltk.corpus import stopwords
from nltk.stem import SnowballStemmer
```

<br>

Los primero que se hace es importar la base de datos. Para este ejemplo se debe descargar la base de datos de Sentimientos_empresa.csv, la cual está guardada en este mismo repositorio. Esta base contiene comentarios de empleados sobre de su nivel de satisfacción con la empresa en la cual trabajan, los cuales, a su vez, se encuentran etiquetados como positivo, negativo o neutral (Paso 1). Es importante cambiar la URL con la ruta en donde el lector haya guardado la base de datos.

```python
data = pd.read_csv('C:/Users/PC/Documents/Sentimientos_empresa.csv',
                   sep=";",
                   encoding='latin-1')

                   

X = data["comentario"]
y = data["sentimiento"]

data["comentario"]
```

<br>

A continuacion, se debe realizar el preprocesamiento y la normalización del texto, en este caso se realiza el stemming, la corrección ortográfica, la eliminación de acentos, la tokenización, y la eliminación de palabras vacias(stopwords), este último usando stopwords en español (Paso 2).

```python
stemmer = SnowballStemmer('spanish')
stopwords_es = stopwords.words('spanish')

def preprocess(text):
    text = text.lower()
    text = " ".join([stemmer.stem(word) for word in text.split() if word not in stopwords_es])
    return text
X = X.apply(preprocess)
```

<br>

Una vez normalizado el texto, este ya es más procesable y significativo para el análisis. Sin embargo, se debe transformar el texto a forma numérica de tal forma que pueda emplearse en un modelo de aprendizaje automático. Para esto se realiza algún método de representación de texto. En este caso se realiza la técnica de bolsa de palabras (Paso 3). 

```python
# Cuenta la frecuencia de las palabras
vectorizer = CountVectorizer(max_features=1000)
X_count = vectorizer.fit_transform(X)
```

```python
# Le otorga más importancia a las palabras que aparecen con menor frecuencia en el corpus
tfidf_transformer = TfidfTransformer()
X_tfidf = tfidf_transformer.fit_transform(X_count)
```

<br>

Como se va a entrenar un modelo de aprendizaje supervisado, los datos deben dividirse en dos, una para entrenar el modelo y otro para probarlo con datos que el modelo no conozca. Se entrena el modelo empleando algún algorítmo de machine learning que se adecue, en este caso se emplea el algoritmo de gradiente descendiente estocástico (Paso 4 y 5).

```python
X_train, X_test, y_train, y_test = train_test_split(X_tfidf, 
                                                    y, 
                                                    test_size=0.2, 
                                                    random_state=123)
```

<br>

```python
# Se entrena utilizando el algoritmo gradiente descendiente estocástico
clf = SGDClassifier(loss='log', 
                    random_state=123, 
                    max_iter=1000)

clf.fit(X_train, y_train)
```

<br>

Con los datos de prueba se evalua el rendimiento del modelo. Para este ejemplo se emplea la metrica de accuracy el cual mide las predicion correctas en relación al total de predicciones realizadas, esto es, el número porcentaje de comentarios clasificados correctamente como positivo, negativo o neutral (Paso 6).

```python
y_pred = clf.predict(X_test)
accuracy = accuracy_score(y_test, y_pred)

print("Exactitud:", accuracy)
```

<br>

Por último, se pone en funcionamiento el modelo entrenado para clasificar nuevos datos de texto en las categorías de sentimiento correspondientes, como positivo, negativo o neutral. Hay que aclarar que la base de datos empleada tiene muy pocos registros, por lo que la precisión puede no ser la mejor. Lo ideal para este tipo de modelos es entrenarlos con miles de registros distintos para que el modelo etiquete de mejor forma nuevos comentarios (Paso 7). 

```python
# Oración de prueba
sentence = "No estoy contento con mi trabajo actual, me siento triste y frustrado en estos momentos."

# Preprocesando la oración
preprocessed_sentence = preprocess(sentence)

# Transformando la oración preprocesada en un vector
vectorized_sentence = vectorizer.transform([preprocessed_sentence])

# Predecir el sentimiento de la oración vectorizada
predicted_sentiment = clf.predict(vectorized_sentence)

# Imprimir el resultado
print(predicted_sentiment)

```