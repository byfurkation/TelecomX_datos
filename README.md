![portada challenge](https://github.com/byfurkation/TelecomX_datos/blob/main/assets/portada%20challenge.png?raw=true)

# <h1 align="center"> TelecomX_datos - en Python </h1>
## <h1 align="center"> Desafío utilizando ETL, generación de gráficos e informe. </h1>

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

Has sido contratado como asistente de análisis de datos en Telecom X y formarás parte del proyecto "Churn de Clientes". La empresa enfrenta una alta tasa de cancelaciones y necesita comprender los factores que llevan a la pérdida de clientes.

Tu desafío será recopilar, procesar y analizar los datos, utilizando Python y sus principales bibliotecas para extraer información valiosa. A partir de tu análisis, el equipo de Data Science podrá avanzar en modelos predictivos y desarrollar estrategias para reducir la evasión.

**Requisitos:**

✅ Importar y manipular datos desde una API de manera eficiente.

✅ Aplicar los conceptos de ETL (Extracción, Transformación y Carga) en la preparación de los datos.

✅ Crear visualizaciones estratégicas para identificar patrones y tendencias.

✅ Realizar un Análisis Exploratorio de Datos (EDA) y generar un informe con insights relevantes.

## 2 La estructura del proyecto y organización de los archivos

Para llevar a cabo el presente análisis, se puede dividir en las siguientes etapas:

1️⃣ **Extracción de datos**

Los datos están disponibles en archivo JSON, y será necesario aplicarle una normalización a los datos en múltiples columnas.

2️⃣ **Explorar el conjunto de datos**

Ahora que has extraído los datos, es fundamental comprender la estructura del dataset y el significado de sus columnas. Esta etapa te ayudará a identificar qué variables son más relevantes para el análisis de evasión de clientes.

📌 Para facilitar este proceso, se creó un diccionario de datos con la descripción de cada columna, mismo que se encuentra en el repositorio bajo el nombre de "TelecomX_diccionario.md".

**Columnas más relevantes**

🎯 Objetivo asumido:

Analizar y predecir el "Churn" (si un cliente se va o se queda)

tenure (meses de contrato)
🧠 Relevancia: Refleja el tiempo de permanencia. Clientes con menor tenure son más propensos a irse.

🧪 Análisis: Puedes hacer histogramas, segmentaciones, correlaciones con Churn.

Contract (tipo de contrato: mensual, anual...)
🧠 Relevancia: Clientes con contrato mes a mes tienden a irse más fácilmente.

📊 Ideal para gráficos de barras o análisis de riesgo.

PaymentMethod (forma de pago)
💳 Pagos automáticos vs. manuales podrían influir.

🎯 A menudo se asocia a abandono por fricción en pagos.

Charges.Monthly y Charges.Total
💵 Clientes con cargos más altos pueden estar menos satisfechos.

También pueden indicar uso intensivo (más fidelidad).

Útiles para crear grupos de riesgo por gasto.

InternetService y servicios relacionados:
InternetService, OnlineSecurity, OnlineBackup, DeviceProtection, TechSupport, StreamingTV, StreamingMovies

🧠 Estos servicios son opcionales y reflejan nivel de compromiso y satisfacción.

Algunos modelos han demostrado que la combinación de servicios influye fuertemente en la retención.

PaperlessBilling
📥 Puede parecer menor, pero se ha encontrado correlación entre este tipo de facturación y cancelación: refleja preferencia por lo digital y menos fricción al cambiar de proveedor.

PhoneService y MultipleLines
🔁 Relacionados con fidelización: clientes que contratan más de un servicio tienden a quedarse más.

⚖️ Variables demográficas (prioridad media)

Estas no siempre son predictoras fuertes, pero pueden dar contexto:

SeniorCitizen: Algunos estudios muestran que personas mayores son más estables en sus servicios.

Partner y Dependents: Pueden reflejar estabilidad o necesidad de varios servicios.

gender: Usualmente no es significativa para Churn por sí sola, pero puede considerarse por completitud.

3️⃣**Análisis de Datos**

Se procede a realizar el análisis de las principales categorías de relevancia para determinar qué acciones tomar debido a la alta tasa de cancelaciones y comprender los factores que llevan a la pérdida de clientes. 

Se realiza un análisis descriptivo de los datos, calculando métricas como media, mediana, desviación estándar y otras medidas que ayuden a comprender mejor la distribución y el comportamiento de los clientes, del cual se logra obtener información sobre la permanencia en meses, cargos mensuales, cargos totales y cargo por día; ya que son las variables numéricas, susceptibles de aplicárceles el método de describe. 

Así mismo se realiza un análisis de la variable "churn" (evasión)  entre los clientes, el recuento de evasión por variables categóricas y numéricas (cliente_actual/evasión/churn vs genero, Ciudadano_mayor, pareja y dependientes); Variables contractuales (cliente_actual/evasión/churn vs Contrato, metodo_pago y facturacion_sin_papel); Servicios contratados (cliente_actual/evasión/churn vs variedad de servicios contratados); Variables continuas agrupadas por rangos (cliente_actual/evasión/churn vs meses de antigüedad, cargo mensual, y cargo total); y la correlación entre variables (cliente_actual/evasión/churn vs cuenta diaria y cantidad de servicios contratados). 


4️⃣**Visualizaciones**

Después de realizar los análisis, se debe transformar los resultados en visualizaciones que ayuden a comprender mejor los patrones y los insights encontrados.

A continuación se presentan unos ejemplos de los contenidos en el análisis, los cuales fueron generados mediante matplotlib y Seaborn.

 ![1. Distribución de Evasión de Clientes](https://github.com/byfurkation/TelecomX_datos/blob/main/assets/1.%20Distribución%20de%20Evasión%20de%20Clientes%20(Churn).png?raw=true)

 ![3. Relación entre Variables Personales y Evasión de Clientes](https://github.com/byfurkation/TelecomX_datos/blob/main/assets/3.%20Relaci%C3%B3n%20entre%20Variables%20Personales%20y%20Evasi%C3%B3n%20de%20Clientes.png?raw=True)

 ![5. Relación entre Servicios Contratados y Evasión de Clientes](https://github.com/byfurkation/TelecomX_datos/blob/main/assets/5.%20Relaci%C3%B3n%20entre%20Servicios%20Contratados%20y%20Evasi%C3%B3n%20de%20Clientes.png?raw=True)

 ![7. Distribución de Cargo por Día según Estado del Cliente](https://github.com/byfurkation/TelecomX_datos/blob/main/assets/7.%20Distribuci%C3%B3n%20de%20Cargo%20por%20D%C3%ADa%20seg%C3%BAn%20Estado%20del%20Cliente.png?raw=True)


5️⃣**Informe Final**

Con base en los análisis realizados y los gráficos generados, se debe sintetizar los hallazgos en un informe final, en este caso se ha llevado a cabo dentro de Google Colab, redactando un texto explicando las conclusiones y recomendaciones derivado de la alta tasa de evasión que se enfrenta.


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

Para Acceder al proyecto se necesita ingresar al repositorio alojado en Git Hub en la siguiente url: [https://github.com/byfurkation/telecomx](https://github.com/byfurkation/TelecomX_datos), dónde se deberá hacer clic sobre el archivo de nombre "AluraStoreLatam.ipynb".

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
