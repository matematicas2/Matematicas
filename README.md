# Proyecto Integrador sobre Procesamiento de Texto

### Equipo de trabajo
Los integrantes del equipo son:
-  Camila Mejía Quintero
-  Sara Mira Puerta
-  Juan David Jurado Tapias
-  Alirio Rodriguez Mesías

## I. Descripción
### Introducción
En este repositorio se encuentra disponibles los archivos con el código y la respectiva documentación que corresponde al Proyecto Integrador de la Maestría en Analítica y Ciencia de Datos de la cohorte 2019-1 en la  Universidad EAFIT.

### Descripción del Problema
A partir de un conjunto muy grande (Big data) de documentos tipo texto (Para este proyecto se cuenta con 980 archivos, habiendo quitando un documento escrito en aleman) y los metadatos sobre dichos documentos, realizar un sistema/aplicación para la ingesta, almacenamiento, indexación, búsqueda, recuperación, navegación y visualización de documentos. 

### Descripción de la Solución
Para el primer seguimiento se cubrirá las siguientes fases:
 * Pre-procesamiento: Limpieza de los archivos y generación de métricas.
 * Procesamiento:   <b> Falta completar por parte de Camila </b>
 * Almacenamiento:  <b> Falta completar por parte de Camila </b>


## II. Arquitectura del Código

El código para la preparación de los datos se divide en dos secciones principales. La primera sección es el Pre-procesamiento de los datos, y la segúnda sección es el procesamiento de los datos, en esta se usan las técnicas básicas de preparación de los datos. 

### Sección 1: Pre-procesamiento

El objetivo es eliminar la mayor cantidad de información obsoleta que contiene cada dato de texto, y generar datos de texto de menor dimensión. La sección contiene los siguientes ordenados:

1. Importación de las librerías necesarias: numpy, re, os y collections. 
2. Llamado de los datos input (datasetIn) y se genera una carpeta de outputs "salida" para guardar los datos de texto de menor dimensión (datasetout).
3. Eliminación de la imformación obsoleta. Por ejemplo: textos en paréntesis, números, direcciones de páginas web y correos electronicos y las secciónes de bibliografía de los artículos.
4. Reconstrucción de los datos en formato .txt para su posterior tratamiento en procesamiento. 
5. Guardado de los nuevos datos en la carpeta de salida.
6. Reducción de la información se puede verificar en el archivo .xls generado. 

### Sección 2: Procesamiento

El objetivo es generar el bag of words de todo el dataset generado en la sección anterior. La sección contiene los siguientes ordenados:

1. Carga de las librerías necesarias para el procesamiento de datos: ntkl, pandas, sklearn, CountVectorizer , pickle. 
2. Formación de las reglas para aplicar la tokenización y eliminación de stopwords, entre otros elementos identificados. 
3. Formación de las reglas para aplicar las tecnicas de stemming y lemmatización. 
4. Lectura de los datos .txt guardados en la carpeta de salida, generada en el pre.procesamiento, se seleccionan los archivos en inglés (existe un documento en alemán). 
5. Implementación de las técnicas de tokenización, stemming y lemmatización a los artículos en inglés, 
6. Construcción del vocabulario.
7. Construcción de Bag of Words.

## III. Guía de Uso
#### Estructura de Directorios
- En la subcarpeta papers-txt del directorio datasets se encuentran los 980 archivos en formato txt que se deben procesar.
- En la subcarpeta salida del directorio datasets se encuentran los 980 archivos en formato txt que se obtienen después de realizar la fase de pre-procesamiento.
- En el directorio raíz están los archivos en formato Jupyter Notebook con las diferentes rutinas para hacer las siguientes operaciones:
  * Archivo preprocessing_data.ipynb, tiene las rutinas del <b>Pre-procesamiento</b> de los archivos de texto, se realizan las siguientes acciones: <br>
    a. Eliminar URL o email.<br>
    b. Eliminar cualquier contenido entre paréntesis o corchetes<br>
    c. Eliminar abreviaciones("et al.", "i.i.e.","i.e"), apóstrofes y guiónes<br>
    d Eliminar los caracteres que NO sean letras o vocales acentuadas<br>
    e. Eliminar palabras o números de un caracter de longitud 1<br>
  Como resultado de este procesamiento se logra en promedio (para los 981 archivos) eliminar aproximadamente el 19% de las palabras en los archivos iniciales.
  * Archivo processing_data.ipynb, tiene las rutinas del <b>Procesamiento</b> de los archivos de texto, se realizan las siguientes acciones:<br>
    a. <b> Falta completar por parte de Camila </b><br>
    b. <b> Falta completar por parte de Camila </b><br>
    c. <b> Falta completar por parte de Camila </b><br>
    d. <b> Falta completar por parte de Camila </b><br>
    e. Eliminar palabras o números de un caracter de longitud 1<br>
