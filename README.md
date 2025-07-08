# TelecomX_datos
Desafío utilizando ETL, generación de gráficos e informe.


![Allura Store Banner](https://github.com/byfurkation/Allura_store/blob/main/assets/banner.png?raw=true)


# <h1 align="center"> Allura Store - en Python </h1>
## <h1 align="center"> Análisis de datos para tienda alura y decisiones estratégicas </h1>

![Static Badge](https://img.shields.io/badge/Data%20Analysis-Python-brightgreen?style=flat-square)

## Indice  

- [1 El propósito del análisis realizado](#1-el-propósito-del-análisis-realizado)

- [2 La estructura del proyecto y organización de los archivos](#2-La-estructura-del-proyecto-y-organización-de-los-archivos)

- [3 Ejemplos de gráficos e insights obtenidos](#3-Ejemplos-de-gráficos-e-insights-obtenidos)

- [4 Acceso al proyecto](#acceso-al-proyecto)

- [5 Instrucciones para ejecutar el notebook](#4-Instrucciones-para-ejecutar-el-notebook) 

- [6 Tecnologías utilizadas](#6-tecnologías-utilizadas)

- [7 Autor](#7-autor)

## 1 El propósito del análisis realizado
En este caso práctico, se plantea 

Para dicho fin se necesita: 
* Cargar y manipular datos CSV con la biblioteca Pandas.

* Crear visualizaciones de datos con la biblioteca Matplotlib.

* Analizar métricas como ingresos, reseñas y rendimiento de ventas.

**Requisitos:**

* Analizar datos de la tienda.

* Evaluar información como los ingresos, las categorías más vendidas, las reseñas de los clientes, los productos más vendidos y el envío promedio.

* Crear gráficos para visualización, mínimo de 3 gráficos diferentes, que pueden incluir gráficos de barras, circulares, de dispersión y otros.

* Enviar una recomendación: Después del análisis, escriba un texto explicando a qué tienda debería vender el Sr. João y por qué, basándose en los datos presentados.

## 2 La estructura del proyecto y organización de los archivos

Para llevar a cabo el presente análisis, se puede dividir en las siguientes etapas:

1️⃣ **Extracción de datos**

Los datos de cada tienda están disponibles en archivo JSON

2️⃣ **Explorar el conjunto de datos**

Es esencial explorar el conjunto de datos para comprender su estructura y contenido. Este paso permite identificar patrones, inconsistencias y las columnas más relevantes para los siguientes pasos.

El conjunto de datos se estructura de la siguiente forma: 

* Producto y Categoría: Artículos vendidos y sus calificaciones.
* Precio y Envío: Valores de venta y costos asociados.
* Fecha y ubicación de compra: Información temporal y geográfica.
* Evaluación de compra: Comentarios de clientes.
* Tipo de Pago y Cuotas: Métodos utilizados por los clientes.
* Coordenadas Geográficas: Ubicación de las transacciones. 

Una vez hecha esta exploración, nos permite comprender cuáles son las probables primeras actividades que necesitamos para cumplir el objetivo de nuestro análisis.

3️⃣**Análisis de Datos**

Se procede a realizar el análisis de las principales categorías de relevancia para determinar qué tienda debe de vender el señor Juan. Para este efecto se analizarán las siguientes columnas de los datos.



4️⃣**Visualizaciones**

Después de realizar los análisis, se debe transformar los resultados en visualizaciones que ayuden a comprender mejor los patrones y los insights encontrados.


5️⃣**Informe Final**

Con base en los análisis realizados y los gráficos generados, se debe sintetizar los hallazgos en un informe final, en este caso se ha llevado a cabo dentro de Google Colab, redactando un texto explicando a qué **tienda debe vender el Sr. Juan**, teniendo en cuenta todos los factores analizados, como:



6️⃣**Análisis  OPCIONAL** 



7️⃣ **Ejemplos de gráficos e insights obtenidos del desempeño geográfico OPCIONAL**


## 3 Ejemplos de gráficos e insights obtenidos



**Análisis de Ingresos Totales** 💸


**Conclusión:** 


**Distribución por Categorías de Productos**


**Conclusión:** 



**Productos Más Vendidos**


**Conclusión:**: 



## 4 Acceso al proyecto 

Para Acceder al proyecto se necesita ingresar al repositorio alojado en Git Hub en la siguiente url: https://github.com/byfurkation/Allura_store, dónde se deberá hacer clic sobre el archivo de nombre "AluraStoreLatam.ipynb".

![acceso_1](https://github.com/byfurkation/Allura_store/blob/main/assets/7_acceso.png?raw=true)

Al ingresar a la siguiente ventana nos encontraremos con lo siguiente, teniendo dos opciones para acceder al proyecto, la primera, será dar clic en la parte superior derecha en el botón que tiene una flecha hacia abajo para descargar el archivo y recuperarlo desde nuestra carpeta de descargas predeterminada, para posteriormente ir a la página https://colab.research.google.com/, o como segunda opción, dar clic sobre las letras que dicen "open in colab", lo cual nos llevará directamente al Notebook de Júpiter en Google colab. 

![acceso_1](https://github.com/byfurkation/Allura_store/blob/main/assets/7_acceso_2.png)

Si hemos seleccionado Descargar el proyecto podemos subirlo a Google Drive Y desde ahí vincularlo con Google Colab, para lo cual será necesario tener una cuenta de Google. Otra manera de subirlo será poniendo el link del repositorio, directamente en Google colab, o por último si lo hemos descargado subirlo desde la sección  "Subir", lo cual nos permitirá Buscar en nuestros archivos de nuestra computadora. 

![colab](https://github.com/byfurkation/Allura_store/blob/main/assets/8_colab_.png)

## 5 Instrucciones para ejecutar el notebook

Una vez dentro del proyecto encontraremos secciones de código, las cuales estando dentro de ellas, podremos ejecutarlo mediante la presión de los botones "shift" + "enter" o con el botón de Play que aparece a la izquierda del código. De esta manera si alguien quiere agregar código para realizar algún cálculo se puede llevar a cabo dentro de estas celdas o generar nuevas para correr otro código diferente, en el presente se utiliza python. 

## 6 Tecnologías utilizadas
* Python. Pandas y Matplotlib, para llevar a cabo ETL. 
* Jupiter Notebook en Google Colab.
* Github.

## 7 Autor

| [<img src="https://avatars.githubusercontent.com/u/194540551?s=200" width=115><br><sub>Christian Carvajal</sub>](https://github.com/byfurkation) |
| :---: |
