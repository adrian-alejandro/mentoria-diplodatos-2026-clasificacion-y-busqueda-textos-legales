##### Universidad Nacional de Córdoba - Facultad de Matemática, Astronomía, Física y Computación
#### Diplomatura en Ciencia de Datos, Aprendizaje Automático y sus Aplicaciones

# Decodificando la Ley: Clasificación Inteligente y Búsqueda Semántica de Jurisprudencia Argentina

## Descripción
El acceso a la información legal y la jurisprudencia en Argentina presenta un desafío significativo debido al volumen, la complejidad léxica y la estructura no estandarizada de los documentos judiciales. Los sistemas de búsqueda tradicionales, basados en coincidencias exactas de palabras clave, a menudo fallan en capturar el "sentido" o contexto de una consulta, dificultando el trabajo de profesionales del derecho y el acceso a la información por parte de los ciudadanos.

Este proyecto propone el desarrollo de un pipeline integral de Procesamiento de Lenguaje Natural (NLP) y Machine Learning para procesar, clasificar y recuperar textos legales argentinos. Utilizando datos provenientes del Sistema Argentino de Información Jurídica (SAIJ), los estudiantes construirán un sistema capaz de agrupar temáticas automáticamente, predecir el fuero de un documento judicial y responder consultas mediante técnicas de búsqueda semántica.

El atractivo principal de esta mentoría es que ofrece un recorrido metodológico completo por el ciclo de vida de un proyecto de datos moderno, articulado en tres etapas prácticas claras: comenzando por la exploración y curación profunda de los textos legales de distinta naturaleza (sumarios sintetizados frente a fallos completos ruidosos), avanzando hacia la resolución conjunta de tareas de aprendizaje supervisado y no supervisado (descubrimiento de patrones latentes), para culminar con un desafío integrador que consiste en el diseño de un motor de búsqueda semántica para responder a las consultas de los usuarios, resolviendo así la etapa de recuperación y sentando la base técnica y conceptual sobre la cual escalar hacia un sistema RAG.

## Con este proyecto trataremos de responder algunas de las siguientes preguntas

- ¿Qué términos o expresiones legales diferencian claramente a un fallo de fuero laboral frente a uno civil o penal?
- ¿Existen conceptos o jerga institucional que cruzan todas las ramas del derecho por igual en nuestro dataset?
- ¿Hay fueros cuyas fronteras de vocabulario sean tan difusas que tienden a confundirse entre sí?
- ¿Cómo es la distribución de fallos por fueros? ¿Cómo varía entre los principales tribunales?
- ¿Qué nivel de solapamiento o ambigüedad se observa en la categorización de los fueros? ¿Qué implicancias tiene esto para diseñar nuestro modelo y qué estrategias podemos aplicar?
- ¿Existe algún desbalance de clases? ¿Cómo afecta esto a la capacidad predictiva del modelo y cómo podemos mitigarlo?
- ¿Se observa alguna tendencia en el volumen de fallos emitidos a lo largo del tiempo según el fuero o el tribunal de origen?
- ¿Qué agrupaciones temáticas latentes hay en los textos? ¿Se corresponden con las categorías legales predefinidas?
- ¿Es posible predecir a qué rama del derecho pertenece un documento leyendo exclusivamente su sumario?
- En una búsqueda de fallos, ¿cómo cambian los resultados obtenidos utilizando jerga técnica frente a una descripción coloquial de los hechos? ¿Qué ocurre con la relevancia de los documentos recuperados?

## Datos
En la carpeta `datos` se encuentran los datases que utilizaremos durante el proyecto:

1. **Dataset Estructurado**: Utilizaremos el repositorio [marianbasti/jurisprudencia-Argentina-SAIJ](https://huggingface.co/datasets/marianbasti/jurisprudencia-Argentina-SAIJ), el cual está alojado en HuggingFace y contiene miles de fallos y resoluciones judiciales obtenidas del repositorio público del [Sistema Argentino de Información Jurídica (SAIJ)](https://www.saij.gob.ar/). 
En la carpeta `datos` se encuentra una pequeña muestra aleatoria del dataset, el cual puede ser descargado en su totalidad utilizando la Jupyter notebook facilitado.

2. **Dataset Auxiliar (No-estructurado)**: Muestra de uso opcional que consiste en documentos judiciales crudos en formato PDF (descargados directamente de la página oficial del SAIJ), y sus respectivas extracciones en formato TXT y la Jupyter notebook utilizada para la extracción. Se pueden encontrar en la carpeta `datos/fallos`.

Adicionalmente, se facilita una Jupyter notebook con instrucciones básicas de descarga y lectura del dataset.

Consultar el archivo DISCLAIMER para más detalles sobre las fuentes del dataset y los términos de uso.