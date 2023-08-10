# Procesamiento del Lenguaje Natural

Este repositorio contiene los ejercicios resueltos para la asignatura de NLP de la Carrera de Especialización en Inteligencia Artificial (CEIA) de la Universidad de Buenos Aires (UBA).

## Contenido

### [Ejercicio 1](https://github.com/Federico-Delgado/PLN/tree/main/Ejercicio%201)
<img src="https://github.com/Federico-Delgado/PLN/blob/main/Imagenes/Ej1.jpg" width="700">

En este ejercicio se implementa la vectorizacion de documentos (Word2Vect) utilizando la libreria NumPy y ademas se tratan los siguientes temas:

- Obtención del vocabulario de un Corpus.
- Codificación mediante el método One-hot Encoding.
- Codificación mediante el método de Vector de Frecuencia o Term Frequency (TF).
- Codificación mediante el método TF-IDF (Term Frequency – Inverse Document Frequency).
- Comparación de similitud entre los documentos de un corpus utilizando la similitud coseno.

### [Ejercicio 2](https://github.com/Federico-Delgado/PLN/tree/main/Ejercicio%202)
<img src="https://github.com/Federico-Delgado/PLN/blob/main/Imagenes/Ej2.jpg" width="700">

En este ejercicio se implementa un bot simple para contestar preguntas de enfermedades medicas leves y ademas se tratan los siguientes temas:

- Desarrollo de un diccionario de entrada en archivo. [JSON](https://github.com/Federico-Delgado/PLN/blob/main/Ejercicio%202/intents.json)
- Preprocesamiento de datos utilizando Spacy: tokenización y lematización.
- Transformaciones empleando Bag of Words y One-Hot Encoding.
- Desarrollo de un modelo DNN con Keras para predecir la clase de pregunta y poder definir una respuesta.
- En la siguiente imagen se ven los resultados del entrenamiento de la red neuronal.

<img src="https://github.com/Federico-Delgado/PLN/blob/main/Imagenes/Res_Ej2.jpg" width="700">

### [Ejercicio 3](https://github.com/Federico-Delgado/PLN/tree/main/Ejercicio%203)
<img src="https://github.com/Federico-Delgado/PLN/blob/main/Imagenes/Ej3.jpg" width="700">

Se utilizará Gensim para crear embeddings customizados basado en un corpus extraido del primer volúmen del libro "*General Anatomy applied to physiology and medicine*" de Xavier Bichat, los cuáles se obtienen en la página de [Project Gutenberg](https://www.gutenberg.org/ebooks/56118).
En este notebook se tratan los siguientes temas:

- Preprocesamiento de datos.
- Creación de vectores empleando Word2Vec de Gensim.
- Ensayo del modelo empleando el método `most_similar` de Gensim para encontrar las palabras que más se relacionan con ciertas palabras de entrada.
- Visualización de agrupación de vectores.
- Operaciones con embeddings, realizando tests de analogía.

### [Ejercicio 4](https://github.com/Federico-Delgado/PLN/tree/main/Ejercicio%204)
<img src="https://github.com/Federico-Delgado/PLN/blob/main/Imagenes/Ej4.jpg" width="700">

En este notebook se implementa la predicción de próxima palabra utilizando un corpus extraido de los tres volúmenes del libro "*General Anatomy applied to physiology and medicine*" de Xavier Bichat, los cuáles se obtienen en la página de [Project Gutenberg](https://www.gutenberg.org/ebooks/search/?query=GENERAL+ANATOMY+APPLIED+TO+PHYSIOLOGY+AND+MEDICINE&submit_search=Go%21). 
Ademas se tratan los siguientes temas:

- Preprocesamiento de datos, utilizando tokenización y Word2Vec.
- División de secuencias de texto en una secuencia de entrada y una palabra target. Transformación de los datos de salida con One-hot Encoding.
- Entrenamiento de un modelo con Keras con capas de Embedding, capas LSTM y capas densas.
- Predicción de próxima palabra en secuencias.
- Generación de secuencias nuevas a partir de secuencias iniciales.

### [Ejercicio 5](https://github.com/Federico-Delgado/PLN/tree/main/Ejercicio%205)

<img src="https://github.com/Federico-Delgado/PLN/blob/main/Imagenes/Ej5.jpg" width="700">

En este notebook se utilizan las críticas de compradores de ropa del dataset de Kaggle [Women's E-Commerce Clothing Reviews](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews) para que el sistema determine la evaluación del comprador.

En particular se tratan los siguientes temas:

- Preprocesamiento de datos.
- División de los datos en set de entrenamiento y testeo. Se realiza oversampling al set de entrenamiento para tratar el desbalance de clases. 
- Entrenamiento de un modelo con Keras con capas de Embedding, capas LSTM bidireccionales, capas de dropout y capas densas.
- Entrenamiento de un modelo con Keras con capas de Embedding FastText, capas LSTM, capas de dropout y capas densas.
- Predicción del rating para diferentes reseñas de testeo empleando ambos modelos.
