# TrabajoFinalOpenData
Este repositorio cumple la función de almacenar todos los archivos pertinentes a la entrega del trabajo práctico final de Open Data

## Codigo Fuente
Este codigo fuente puede dividirse en basicamente 3 partes principales:
  1. Importación de las librerías necesarias
  2. Scrapeado de las páginas seleccionadas
  3. Exportación de los datos a un archivo .csv

A continuación se procederá a explicar la función de cada uno de estos

### Importación de las librerías utilizadas
En este bloque de código se cumple estricatamente la necesidad de realizar un pequeño número de importaciones de librerías para el aprovechamiento de funciones especializadas para tablas (DataFrames) como la de la librería Pandas

### Scrapeado de las páginas seleccionadas
En este apartado se definen y ejecutan las funciones de scrapeado de páginas que corresponden, en este caso, a dos de los competidores más importantes para TECNOHAUS S.A. Estos son Nissei y Compulandia.

Se ha definido un apartado para cada una de estas empresas debido a que sus diferentes estructuras en la página web requieren diferentes métodos de scrapeado para funcionar correctamente.

Tal es el caso de Nissei, por ejemplo, donde fue necesario diseñar una función extra que defina la cantidad de paginaciones que tiene cada tipo de producto scrapeado.

En este bloque se realizan las búsquedas por cada tipo de producto y tienda por separado y todos estos resultados se guardan en distintos dataframes

### Exportación de los datos a un archivo .csv
Es en este último apartado donde de hecho se unen todos los dataframes creados previamente para cada producto de cada tienda por medio de métodos propios de la librería de Pandas

Posteriormente se aplica a este DataFrame resultante de la concatenación un método para exportarlo a un archivo en formato .csv y guardarlo en el entorno local
