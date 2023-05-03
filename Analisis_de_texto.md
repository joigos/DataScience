# Mineria de texto y el procesamiento de lenguaje natural (NLP)

<br>

## Introducción

La minería de texto y el procesamiento de lenguaje natural son dos campos relacionados que se enfocan en extraer y analizar información a partir de texto escrito o hablado. Estos campos se han vuelto cada vez más importantes debido a la enorme cantidad de datos no estructurados que se generan a diario, y a la necesidad de obtener información útil a partir de ellos.

La minería de texto implica el uso de técnicas estadísticas y de aprendizaje automático para extraer información significativa de grandes conjuntos de texto. Esto puede incluir la identificación de patrones, tendencias y relaciones entre diferentes conjuntos de datos. La minería de texto se utiliza en una variedad de campos, desde la análisis de sentimiento en las redes sociales hasta la clasificación de documentos en una biblioteca digital.

Por otro lado, el procesamiento de lenguaje natural se enfoca en la comprensión de la lengua humana por parte de las máquinas. Esto incluye tareas como la traducción automática, el análisis sintáctico y semántico, la generación de lenguaje natural y la respuesta automática a preguntas. El procesamiento de lenguaje natural también utiliza técnicas de aprendizaje automático y estadísticas para mejorar la precisión de los resultados.

En conjunto, la minería de texto y el procesamiento de lenguaje natural son herramientas poderosas para el análisis y la comprensión de grandes cantidades de datos no estructurados. Estas técnicas pueden ser aplicadas en una variedad de campos, incluyendo la investigación académica, la industria, el marketing y la inteligencia artificial.

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


En resumen, la minería de datos y el procesamiento del lenguaje natural son dos campos diferentes que tienen enfoques y objetivos distintos, aunque ambos utilizan técnicas estadísticas y de aprendizaje automático para extraer información útil a partir de grandes conjuntos de datos. La minería de datos se enfoca en la identificación de ___patrones y relaciones___ en datos estructurados y no estructurados, mientras que el procesamiento del lenguaje natural se enfoca en la ___comprensión y generación___ de lenguaje humano. Ambos campos tienen aplicaciones útiles en diferentes áreas de la investigación académica y la industria.

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
La normalización de datos de texto consiste en la transformación del texto en una forma estandarizada y más significativa para el análisis. Algunas técnicas comunes de normalización son:

    * Lematización: reduce las palabras a su forma base (lemas) para eliminar las diferencias de inflexión y derivación, y reducir la complejidad de los datos. En este proceso, se utiliza un diccionario léxico para transformar una palabra a su lema correspondiente, eliminando los sufijos y prefijos. Por ejemplo, las palabras "corriendo", "corre" y "corrido" se reducirían todas a su lema base "correr". Esto puede ser útil para analizar grandes cantidades de texto y para hacer comparaciones más precisas entre diferentes palabras.
    
    * Stemming: reduce las palabras a su raíz o raíces (stems) para eliminar las diferencias de inflexión y derivación, y reducir la complejidad de los datos.  Esto se hace aplicando reglas específicas que eliminan sufijos comunes. Por ejemplo, la palabra "corriendo" se reduciría a "corr", mientras que la palabra "corre" se reduciría a "corr" también. Aunque esta técnica es más simple y rápida que la lematización, puede producir resultados menos precisos ya que algunas palabras pueden ser reducidas a formas que no son lemas válidos.

    * Corrección ortográfica: corrige los errores de ortografía para mejorar la precisión y confiabilidad de los datos.
    
    * Remoción de acentos y diacríticos: elimina los acentos y diacríticos de las letras para evitar la variabilidad en los datos de texto.

En resumen, el preprocesamiento y la normalización de datos de texto son importantes para garantizar que los datos de texto sean más procesables y significativos para los modelos de aprendizaje automático y para las técnicas de minería de texto. Estas técnicas son útiles para reducir el ruido y la complejidad en los datos, mejorar la precisión y confiabilidad de los análisis, y garantizar una comprensión adecuada del texto.

<br>

*Ejemplo de este proceso:*

> Oración: "El perro marrón saltó sobre el gran tronco caído en el río."

<br>

1. **Preprocesamiento de datos de texto:**

    * Tokenización: ['El', 'perro', 'marrón', 'saltó', 'sobre', 'el', 'gran', 'tronco', 'caído', 'en', 'el', 'río', '.']

    * Eliminación de signos de puntuación y caracteres especiales: ['El', 'perro', 'marrón', 'saltó', 'sobre', 'el', 'gran', 'tronco', 'caído', 'en', 'el', 'río']

    * Eliminación de palabras vacías (stopwords): ['perro', 'marrón', 'saltó', 'gran', 'tronco', 'caído', 'río']

    * Normalización de mayúsculas y minúsculas: ['perro', 'marrón', 'saltó', 'gran', 'tronco', 'caído', 'río']

<br>

2. **Normalización de datos de texto:**

    * Lematización: ['perro', 'marrón', 'saltar', 'grande', 'tronco', 'caído', 'río']

    * Stemming: ['perr', 'marrón', 'saltó', 'gran', 'tronc', 'caíd', 'rí']

    * Corrección ortográfica: ['perro', 'marrón', 'saltó', 'gran', 'tronco', 'caído', 'río']

    * Remoción de acentos y diacríticos: ['perro', 'marron', 'salto', 'gran', 'tronco', 'caido', 'rio']

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

El análisis de sentimientos es una técnica de procesamiento de lenguaje natural que se utiliza para determinar la actitud o la emoción expresada en un texto. El objetivo del análisis de sentimientos es clasificar el texto en una de varias categorías, como positivo, negativo o neutral, en función de la expresión de sentimientos en el texto.

Para realizar el análisis de sentimientos, se utilizan algoritmos de aprendizaje automático y técnicas de minería de texto para analizar el texto y determinar su polaridad o actitud. El enfoque más común para el análisis de sentimientos es la clasificación supervisada, en la que se entrena un modelo de aprendizaje automático utilizando un conjunto de datos etiquetados con las categorías de sentimiento correspondientes.

Los datos etiquetados pueden ser revisados manualmente por humanos o etiquetados automáticamente utilizando técnicas de análisis de texto y minería de datos. Una vez que se ha entrenado el modelo, se puede utilizar para clasificar nuevos textos en las categorías de sentimiento correspondientes.

El análisis de sentimientos se utiliza en una amplia gama de aplicaciones, como la monitorización de la reputación en línea de una marca o empresa, la evaluación de la satisfacción del cliente, la identificación de tendencias en las opiniones de los usuarios y la detección de noticias falsas o propaganda.

<br>

*Ejemplo:*

Un ejemplo de análisis de sentimientos podría ser la clasificación de los comentarios de los clientes de un hotel en positivos, negativos o neutrales. El modelo de aprendizaje automático se entrena utilizando un conjunto de datos etiquetados de comentarios de clientes, donde cada comentario se etiqueta con la categoría correspondiente, por ejemplo, "Excelente", "Malo" o "Neutral".

Una vez que el modelo se entrena, se puede utilizar para clasificar nuevos comentarios de clientes en las categorías correspondientes. Por ejemplo, si un nuevo comentario dice "Mi estancia en el hotel fue fantástica, el personal fue muy amable y atento", el modelo lo clasificaría como un comentario positivo.

Del mismo modo, si otro comentario dice "Mi experiencia en el hotel fue terrible, la habitación estaba sucia y el servicio era pésimo", el modelo lo clasificaría como un comentario negativo.

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



<br>

## Extracción de información

<!--- IMAGEN -->
![Imagen](https://mug-it.org.ar/multimedios/imgs/17674_620.jpg "Extracción de información")

La extracción de información es una tarea de procesamiento de lenguaje natural que implica la identificación y extracción de información relevante y estructurada de datos de texto no estructurados. Esta tarea puede involucrar la identificación de entidades, relaciones y eventos en el texto.

* **La identificación de entidades** implica la identificación de palabras o frases en el texto que se refieren a __objetos__, lugares, personas, organizaciones, etc. Las entidades pueden ser identificadas mediante el uso de técnicas como la coincidencia de patrones, el etiquetado de partes del discurso, el análisis sintáctico, etc. Una vez que se identifican las entidades, se pueden extraer características relevantes como nombres, ubicaciones, fechas, etc.


* **La identificación de relaciones** implica la identificación de las __conexiones__ entre las entidades en el texto. Por ejemplo, si un texto habla sobre una empresa adquiriendo otra empresa, se podría identificar una relación de "adquisición" entre dos entidades, una que representa la empresa adquirente y otra que representa la empresa adquirida. Las relaciones pueden ser identificadas mediante el análisis de patrones lingüísticos y semánticos, la resolución de correferencia, etc.


* **La identificación de eventos** implica la identificación de __acciones__ o sucesos que ocurren en el texto. Por ejemplo, si un texto habla sobre un accidente automovilístico, se podría identificar un evento de "accidente automovilístico". Los eventos pueden ser identificados mediante el análisis de verbos, la identificación de patrones lingüísticos, etc.

La extracción de información puede ser útil para una variedad de aplicaciones, como la minería de datos, la clasificación de documentos, el análisis de riesgos, la vigilancia de la competencia, etc. Al utilizar técnicas de extracción de información, es posible automatizar la identificación de información importante y estructurada en grandes conjuntos de datos de texto, lo que permite a las empresas tomar decisiones informadas basadas en datos.

<br>

*Ejemplo:*

Un ejemplo de extracción de información podría ser la identificación de entidades y relaciones en un conjunto de noticias financieras. Supongamos que tenemos una serie de noticias financieras que hablan sobre fusiones y adquisiciones de empresas. Podríamos utilizar técnicas de procesamiento de lenguaje natural para identificar las empresas involucradas en las fusiones y adquisiciones, así como la naturaleza de las relaciones entre ellas.

Por ejemplo, si una noticia habla sobre que "Apple adquiere a la empresa X", podríamos utilizar técnicas de extracción de información para identificar que Apple es la empresa adquiriente y la empresa X es la empresa adquirida. Además, podríamos identificar características adicionales como el valor de la transacción, la fecha de la transacción, etc.

Esto puede ser útil para los inversores que buscan tomar decisiones informadas sobre las acciones de las empresas involucradas en las fusiones y adquisiciones. Además, la información estructurada y organizada obtenida a través de la extracción de información puede ser utilizada para construir bases de datos de inteligencia empresarial o para alimentar modelos de aprendizaje automático que puedan hacer predicciones sobre futuras fusiones y adquisiciones.

<br>

*En general, el procedimiento que se sigue para la extracción de información es el siguiente:*

| Paso | Descripción |
| --- | --- |
| 1 | **Identificación de entidades:** Identificar todas las entidades relevantes en el texto, tales como personas, organizaciones, lugares, etc. |
| 2 | **Normalización:** Normalizar las entidades para asegurar que estén escritas de la misma forma en todo el texto. |
| 3 | **Identificación de relaciones:** Identificar las relaciones entre las entidades, tales como "X adquiere a Y" o "Z es el CEO de W". |
| 4 | **Estructuración de la información:** Estructurar la información identificada en una forma que permita su análisis y procesamiento, tal como una base de datos o un grafo. |
| 5 | **Validación y verificación:** Validar y verificar la información extraída para asegurar su precisión y completitud. |
| 6 | **Aplicaciones:** Utilizar la información extraída para diversas aplicaciones, como análisis de riesgos, toma de decisiones, o entrenamiento de modelos de aprendizaje automático. |
