# Procesamiento del Lenguaje Natural

**UNIVERSIDAD DE BUENOS AIRES**

**ESPECIALIZACION EN INTELIGENCIA ARTIFICIAL**

Docente: Rodrigo Cárdenas
Alumno: Albachiaro Leandro

En este repositorio se encontrarán y detallarán los conocimientos adquiridos durante la materia Procesamiento del Lenguaje Natural, como también cada uno de los desafíos superados y una breve explicación de los mismos.

## Desafío 1 - Vectorización de documentos
<img src="https://miro.medium.com/v2/resize:fit:1400/0*B3rOPw4OVDRSqpU8">

En este desafío se aplican los conceptos de vectorización, aplicando los siguientes métodos:

  * One Hot Encoding
  * Vectores de Frecuencia
  * TF - IDF

Luego se realiza la comparación de documentos utilizando dichos métodos en conjunto con la Similitud de coseno.

[Link a la carpeta del desafío](https://github.com/LeandroAlbachiaro/Entregas_PLN/tree/da3a032e14586bf70601c75554f305a28dbb0d65/Desafio_1)

## Desafío 2 - Bots de información

<img src="https://www.lavanguardia.com/andro4all/hero/2021/04/Mejores-bots-Telegram.jpg?width=768&aspect_ratio=16:9&format=nowebp" width="700" height="300">

En este desafío se introducen los conceptos de preprocesamiento de texto, tokenización y lematización, que se utilizan para programar un bot de respuestas automáticas a través de la libreria de nltk en conjunto con un corpus de wikipedia.

[Link a la carpeta del desafío](https://github.com/LeandroAlbachiaro/Entregas_PLN/tree/da3a032e14586bf70601c75554f305a28dbb0d65/Desafio_2)

## Desafío 3 - Embeddings
<img src="https://miro.medium.com/v2/resize:fit:2000/1*SYiW1MUZul1NvL1kc1RxwQ.png" width="700" height="300">

En este desafío utilizamos el libro "Don Quijote de la Mancha", el cual luego de ser preprocesado a través de los métodos vistos anteriormente, se entrenó un modelo para generar vectores que sintetizan la proximidad que tienen las palabras dentro del corpus.

Luego se procede a ensayar, buscando las palabras que más se relacionan entre sí y haciendo un test de analogías.

Finalmente se visualizan los vectores generados utilizando tecnicas de reducción de dimensionalidad y se concluye en que los embeddings logran captar correctamente el significado semántico de las palabras.

[Link a la carpeta del desafío](https://github.com/LeandroAlbachiaro/Entregas_PLN/tree/da3a032e14586bf70601c75554f305a28dbb0d65/Desafio_3)

## Desafío 4 - Predicción de próxima palabra
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSgxdyQin7ncY-md1VaOsUqx9C4sJwOoyBovWUHltsZ1e6V8Le3OLrqxkz82m8UxPiqLFg&usqp=CAU" width="600" height="250">

Habiendo ya aprendido los métodos de preprocesamiento y de generación de embeddings, en este desafío creamos los primeros modelos de RNN y BRNN que se utilizan para predecir la siguiente palabra de una oración, en este caso se utilizó el libro "Los Miserables" como corpus.

Los resultados no fueron satisfactorios, debido a que estos modelos tienden a predecir las palabras más comunes del vocabulario, como por ejemplo los conectores.

Cabe aclarar que el rendimiento de estos modelos puede mejorar utilizando corpus mucho mas grandes y también con embeddings y modelos preentrenados. 

[Link a la carpeta del desafío](https://github.com/LeandroAlbachiaro/Entregas_PLN/tree/da3a032e14586bf70601c75554f305a28dbb0d65/Desafio_4)

## Desafío 5 - Análisis de sentimientos
<img src="https://1.bp.blogspot.com/-C03j8yr-Xds/XcxXmpG5biI/AAAAAAAAB90/yQJ49G3nEscdgrSGTSW_ODHvfRIrr19xgCPcBGAYYCw/s1600/shutterstock_1073953772-860x9999.jpg" width="600" height="300">

En este desafío contamos con un dataset de opiniones de un local de E-commerce que se encuentra desbalanceado, para comparar resultados, se entrenaron 4 modelos en total con las siguientes características:

 * Dataset desbalanceado y embeddings propios.
 * Dataset desbalanceado y embeddings preentrenados.
 * Dataset balanceado y embeddings propios.
 * Dataset balanceado y embeddings preentrenados

Debido al desbalance de datos se utilizó la métrica F1-score y se concluyó que el modelo con el dataset balanceado y embeddings propios fue el de mejor rendimiento.

[Link a la carpeta del desafío](https://github.com/LeandroAlbachiaro/Entregas_PLN/tree/da3a032e14586bf70601c75554f305a28dbb0d65/Desafio_5)

## Desafío 6 - Bot QA
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT6G8rU7A_PzHNsIEA9ZD92c1an6X1Xwhl5u_TZK3ilBHo5FncUp9XkO_SGjqKyI6-weRU&usqp=CAU" width="300" height="300">

En el último desafío aplicamos todos los conocimientos adquiridos en la materia, utilizando un set de datos de ConvAI2 (Conversational Intelligence Challenge 2), construimos un BOT para responder preguntas de un usuario.

Para esto, se realiza el preprocesamiento correspondiente, se utilizan embeddings de Glove y se entrena un modelo basado en el esquema encoder-decoder con capas LSTM.

Luego se realizan inferencias para testear el funcionamiento del mismo.

[Link a la carpeta del desafío](https://github.com/LeandroAlbachiaro/Entregas_PLN/tree/aeadc95df2ff84859aec06f57b6ac96f89f1ad3a/Desafio_6)
