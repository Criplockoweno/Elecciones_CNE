
# Proyecto de Análisis de Resultados Electorales - Readme

Este proyecto se centra en el análisis de resultados electorales utilizando dos conjuntos de datos: "RESULTADOS_1V_PARROQUIA_2002" y "resultados a nivel parroquial - segunda vuelta". El objetivo principal es realizar una serie de tareas de procesamiento y manipulación de datos en ambos conjuntos para obtener información significativa y útil.

## Estructura del proyecto

El proyecto está organizado en varias etapas, cada una con tareas específicas a realizar. A continuación, se describe la estructura y los aspectos principales del proyecto:

1. **Carga y Preparación de Datos**
   - Se carga cada conjunto de datos ("cne2002resultadosV1" y "cne2002resultadosV2") en DataFrames separados.
   - Se realizan las transformaciones necesarias en cada conjunto de datos para limpiar y preparar los datos, como eliminar filas o columnas innecesarias, cambiar el tipo de datos de las columnas, etc.

2. **Mapeo de Códigos de Provincia**
   - Se carga un diccionario en formato CSV llamado "provincias_2002.csv" que relaciona los códigos de provincia con los nombres correspondientes.
   - Se realiza el mapeo de los códigos de provincia en la columna "PROVINCIA_CODIGO" de cada DataFrame utilizando el diccionario CSV.

3. **Manipulación de Datos de Votos por Género**
   - Se crean nuevas columnas en cada DataFrame para los votos masculinos y femeninos, extrayendo la información correspondiente de la columna "SEXO_DESCRIPCION".
   - Se eliminan las columnas innecesarias, como "SEXO_DESCRIPCION".

4. **Cálculo de Votos Totales por Candidato**
   - Se crea una nueva columna en cada DataFrame llamada "VOTOS_TOTALES" que suma los votos masculinos y femeninos de cada candidato.

5. **Agrupación de Datos y Suma de Votos por Tipo**
   - Se crean nuevas columnas en cada DataFrame para los votos nulos y votos en blanco, tanto para el género masculino como para el femenino.
   - Se realiza la agrupación de datos por tipo de voto y se suman los votos correspondientes para cada género en cada conjunto de datos.

6. **Combinación de Entradas para Candidatos**
   - Se combinan las entradas de cada candidato en cada DataFrame, preservando los valores en cada columna correspondiente (votos masculinos y femeninos) y rellenando los valores faltantes con ceros.

7. **Resultados y Análisis**
   - Se realizan análisis adicionales sobre los datos procesados en cada conjunto de datos y se obtiene información relevante, como el total de votos por provincia, el total de votos por tipo, etc.

## Requisitos y Dependencias

- Para ejecutar este proyecto, se requiere tener instalado Python (versión X.X o superior) y las siguientes bibliotecas:
  - pandas
  - numpy
  - matplotlib (opcional, para visualizaciones)

## Instrucciones de Uso

1. Descarga los conjuntos de datos "cne2002resultadosV1" y "cne2002resultadosV2" en formato CSV.
2. Asegúrate de tener todas las bibliotecas necesarias instaladas en tu entorno Python.
3. Ejecuta el código en un entorno de desarrollo o intérprete de Python, siguiendo las instrucciones y tareas descritas en el proyecto para cada conjunto de datos.
4. Observa los resultados y análisis obtenidos para cada conjunto de datos por separado.

## Contribuciones y Contacto

Este proyecto ha sido desarrollado por Kristian Mendoza. Si tienes alguna pregunta, sugerencia o contribución, no dudes en ponerte en contacto conmigo a través de [tu correo electrónico o medio de contacto].

¡Gracias por tu interés en este proyecto de análisis de resultados electorales!

