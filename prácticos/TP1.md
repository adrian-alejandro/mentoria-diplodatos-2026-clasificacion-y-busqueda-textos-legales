##### Universidad Nacional de Córdoba - Facultad de Matemática, Astronomía, Física y Computación
#### Diplomatura en Ciencia de Datos, Aprendizaje Automático y sus Aplicaciones

### Decodificando la Ley: Clasificación Inteligente y Búsqueda Semántica de Jurisprudencia Argentina

## Entrega 07/08 - Práctico 1 de análisis y visualización

Nuestro objetivo será entender el corpus e identificar qué información tenemos y qué preguntas pueden ser respondidas. Abordaremos esta práctica en tres partes: 
- exploración de datos estructurados, 
- exploración de los textos, y 
- visualización de resultados y conclusiones preliminares.

En la primera, centraremos el análisis en la estructura del dataset, evaluando la distribución de fueros y tribunales. Indagaremos si hay valores faltantes, si hay desbalance de clases y cuál es la evolución temporal. Nos preguntaremos qué áreas legales están más o menos representadas, si existen sesgos temporales y si hay tribunales sobrerrepresentados. Aquí identificaremos la variable objetivo (target), que usaremos para predecir.

Por otro lado, analizaremos los campos de texto, seleccionando el campo que consideremos más adecuado, y nos centraremos en la distribución de la longitud de los textos, el tamaño del vocabulario, los términos más frecuentes y los n-gramas. Buscaremos qué palabras caracterizan a cada fuero, cuáles son compartidas y cuáles son distintivas, evaluando cómo cambia esto al remover *“palabras vacías”* (stopwords). Opcionalmente, exploraremos el dataset de fallos completos contrastando la longitud, la riqueza del vocabulario y la presencia de ruido frente a los campos de texto.

Finalmente, armaremos un reporte visual con los hallazgos preliminares.
