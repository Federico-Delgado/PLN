# Natural Language Processing

## Predicción de próxima palabra

<img width="2116" alt="nextword" src="https://github.com/tmonreal/Natural_Language_Processing/assets/84754265/0a3145f8-3510-45a5-848e-16e0bd54faf1">

En este notebook se implementa la predicción de próxima palabra utilizando un corpus extraido de los tres volúmenes del libro "*General Anatomy applied to physiology and medicine*" de Xavier Bichat, 
los cuáles se obtienen en la página de [Project Gutenberg](https://www.gutenberg.org/ebooks/search/?query=GENERAL+ANATOMY+APPLIED+TO+PHYSIOLOGY+AND+MEDICINE&submit_search=Go%21). En particular, en este notebook se tratan los siguientes temas:

- Preprocesamiento de datos, utilizando tokenización y Word2Vec.
- División de secuencias de texto en una secuencia de entrada y una palabra target. Transformación de los datos de salida con One-hot Encoding.
- Entrenamiento de un modelo con Keras con capas de Embedding, capas LSTM bidireccionales y capas densas.
- Predicción de próxima palabra en secuencias dentro del contexto fisiológico.
- Generación de secuencias nuevas a partir de secuencias iniciales.
