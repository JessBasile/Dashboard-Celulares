
<p align="center">
    <img src="https://github.com/JessBasile/Dashboard-Celulares/blob/main/analitycs.gif?raw=true" alt="Descripción del GIF" style="width: 100%; max-width: 800px; height: auto;">
</p>

## Proyecto Data Analytics 

<img align="right" alt="Jess-perfil" width="200" src="https://github.com/JessBasile/Dashboard-Celulares/raw/main/imagenes/Jess-perfil.png">

***Título del proyecto:*** Análisis de satisfacción en ventas de celulares en la empresa Europe Mobile Distributors.

***Iniciativa de análisis:*** Mejora en la satisfacción de los clientes que manifiestan disconformidad.

***Autora:*** Jesica Brenda Basile

***Fecha de presentación:*** 16/03/2024

## Tabla de versiones

| VERSIÓN | FECHA       |
|---------|-------------|
| 1       | 30/12/2023  |
| 2       | 13/01/2024  |
| 3       | 24/02/2024  |
| 4       | 16/03/2024  |

## Introduccion

En las últimas décadas, el mercado de teléfonos celulares ha experimentado un crecimiento exponencial, convirtiéndose en un elemento fundamental en la vida moderna. La constante evolución tecnológica, la creciente conectividad y la versatilidad de los dispositivos han transformado la forma en que nos comunicamos, trabajamos y nos entretenemos.

El segmento de telefonía celular se caracteriza por una competencia intensa y una amplia variedad de opciones disponibles, sometida a constantes avances tecnológicos que provocan una rápida obsolescencia de los dispositivos, especialmente los de gama baja, lo que ha generado un aumento continuo en la demanda. Ser referente en este entorno es crucial para la permanencia y el crecimiento, en consecuencia, es importante priorizar la satisfacción al cliente como factor clave para triunfar y expandirse.
En este contexto, Europe Mobile Distributors, es una empresa especializada en la venta de teléfonos celulares en diversos países europeos, que intenta distinguirse por su compromiso con la satisfacción del cliente, la atención personalizada y la comunicación efectiva. La compañía alienta a los consumidores a valorar cada venta, como parte de su enfoque en la mejora continua, para incorporar los cambios necesarios y mantener una experiencia de alta calidad.

## Descripción de la temática

Basándonos en la temática, se busca analizar la información recopilada por Europe Mobile Distributors durante un período de tres años en sus ventas de teléfonos celulares, para valorar el nivel de satisfacción que manifiestan los clientes a través de reseñas asociadas a cada venta, utilizando una puntuación del 1 al 5, con la posibilidad de obtener una calificación nula para aquellos clientes que no proporcionaron valoraciones. Este análisis, no solo alcanza a evaluar la satisfacción de los clientes y correlacionar estos datos con el volumen de venta y las ganancias generadas, sino, adicionalmente, identificar los clientes que evidencian mayor insatisfacción con el fin de desarrollar estrategias comerciales que permitan mejorar la experiencia de esos consumidores e incrementar las ventas.

## Objetivo

El objetivo de este análisis es evaluar la satisfacción de los clientes y su correlación con el volumen y las ganancias de las ventas, a fin de identificar específicamente el nombre y ubicación de los clientes que evidencien mayor insatisfacción para que la empresa pueda desarrollar estrategias comerciales personalizadas con el propósito de mejorar la satisfacción de este grupo concreto de consumidores y aumentar su contribución porcentual al volumen total de ventas.

## Alcance

El dashboard diseñado permitirá acceder a la información sobre la satisfacción de los clientes de la empresa Europe Mobile Distributors ubicados en Europa durante un período de tres años en función de las ventas de teléfonos celulares efectuadas en sus distintas marcas y gamas.
Su utilización, permitirá identificar los nombres y el país de cada uno de los clientes insatisfechos durante el período específico comprendido desde enero del 2019 hasta septiembre del 2021. Estos datos permitirán deducir las estrategias más apropiadas y abordar los cambios necesarios para reducir esa insatisfacción.

## Usuario Final

El tablero de control se encuentra dirigido al nivel táctico, principalmente a los líderes de ventas de la firma Europe Mobile Distributors, dado que facilita la identificación de los clientes disconformes y la ubicación geográfica de los mismos, lo que permitirá al sector comercial diseñar e implementar estrategias para revertir la situación pudiendo generar un incremento en las ventas.

## Diagrama de Entidad-Relación

El diagrama de ER permite visualizar la relación de los datos y de las diferentes tablas. Dentro del mismo, se identifican las claves primarias y foráneas con todos los campos que contienen cada una de las tablas.

![Diagrama de Venta de Celulares](imagenes/Diagrama%20Venta%20Celulares.jpg)

## Herramientas tecnológicas implementadas

Para el presente trabajo se utilizaron los siguientes programas:
+ Excel para la lectura del dataset.
+ “Miro” para la creación del diagrama entidad-relación [https://miro.com/es/](https://miro.com/es/)
+ Word para la descripción del proyecto.
+ Power BI Desktop para la creación del tablero de control.

## Dataset

El dataset de Venta de Celulares fue elegido dentro de un grupo de opciones proporcionadas por el profesor a cargo de las clases del curso Martín Segovia, el cual no requería normalización dado que se encontraba óptimo para comenzar a trabajar.

## Listado de Tablas

A continuación, se describen las distintas tablas del modelo especificando [únicamente las llaves primarias y foráneas].

+ ***Tabla Ventas:*** Contiene el detalle de las ventas discriminado el número de factura, cantidad, precio y costo. En el caso de la factura, articulo, marca, cliente y país figuran con sus abreviaciones.

`PK:` ID Venta Articulo `FK:` ID Factura `FK:` ID Articulo `FK:` ID Marca `FK:` ID Cliente `FK:` ID Ciudad `FK:` ID País `FK:` ID Pago `FK:` ID Tipo

+ ***Tabla Artículos:*** Contiene la descripción del artículo, precio y costo, mientras que el artículo, la marca, la categoría, la RAM, almacenamiento y procesador figuran con sus abreviaciones.

`PK:` ID Articulo `FK:` ID Cat Articulo `FK:` ID RAM `FK:` ID Almacenamiento `FK:` ID Procesador 

+ ***Tabla Clientes:*** Contiene nombre del cliente, y abreviaciones de los clientes, ciudades, países y envío.

`PK:` ID Clientes `FK:` ID Envío

+ ***Tabla procesador:*** Contiene la descripción de los distintos procesadores, con sus abreviaciones campo ID Procesador.

`PK:` ID Procesador

+ ***Tabla Almacenamiento:*** Contiene los cuatro tamaños de almacenamiento 256GB, 128GB, 64GB y 32 GB con sus abreviaciones campo ID Almacenamiento.

`PK:` ID Almacenamiento

+ ***Tabla RAM:*** Contiene los cinco tamaños de memoria RAM 12GB, 8GB, 6GB, 4GB y 2GB con sus abreviaciones campo ID RAM.

`PK:` ID RAM

+ ***Tabla Categoría Artículo:*** Contiene las tres categorías de gama sobre los artículos Alta, Media y Baja con sus abreviaciones campo ID Categoría Articulo.

`PK:` ID Categoría Artículo

+ ***Tabla Tipo Pago:*** Contiene los cuatro diferentes medios de pago Efectivo, Crédito, Transferencia y Cheque con sus abreviaciones campo ID Pago.

`PK:` ID Pago

+ ***Tabla País:*** Contiene cinco países europeos España, Portugal, Italia, Francia y Alemania en los que se encuentran ubicados los clientes, con sus abreviaciones campo ID País.

`PK:` ID País

+ ***Tabla Ciudad:*** Contiene las distintas ciudades en las que se encuentran ubicados los clientes, con sus abreviaciones campo ID Ciudad.

`PK:` ID Ciudad.

+ ***Tabla Marca:*** Contiene las seis marcas Apple, Samsung, Google, Xiaomi, Huawei y Motorola de los artículos que se comercializan, con sus abreviaciones campo ID Marca.

`PK:` ID Marca

+ ***Tabla Facturas:*** Contiene los números de facturas y fechas de todas las ventas de celulares efectuadas en la compañía “Europe Mobile Distributors” desde el año 2019 al 2021 inclusive, con sus abreviaciones sobre las facturas, los pagos y los review.

`PK:` ID Factura `FK:` ID Review

+ ***Tabla Review:*** Contiene las puntuaciones None, 1, 2, 3, 4 y 5 sobre las valoraciones efectuadas por los clientes que revelan su satisfacción, donde None hace referencia a la ausencia de valoración por parte del consumidor.

`PK:` ID Review

## Listado de columnas por tablas

***VENTAS***

| CAMPO              | TIPO DE DATO    | TIPO DE CLAVE |
|--------------------|-----------------|---------------|
| ID Venta Artículos  | INT             | PK            |
| Nro Factura         | VARCHAR(20)     |               |
| ID Factura          | INT             | FK            |
| ID Articulo         | INT             | FK            |
| ID Marca            | INT             | FK            |
| ID Cliente          | INT             | FK            |
| ID Ciudad           | INT             | FK            |
| ID País             | INT             | FK            |
| Cantidad            | INT             |               |
| Precio USD          | DECIMAL(5,2)    |               |
| Coste USD           | DECIMAL(5,2)    |               |
| ID Pago             | INT             | FK            |
| ID Tipo             | INT             | FK            |

***ARTÍCULOS***

| CAMPO             | TIPO DE DATO    | TIPO DE CLAVE |
|-------------------|-----------------|---------------|
| ID Articulo       | INT             | PK            |
| ID Marca          | INT             |               |
| Des Articulo      | VARCHAR(100)    |               |
| Precio USD        | DECIMAL(5,2)    |               |
| Coste USD         | DECIMAL(5,2)    |               |
| ID Cat Articulo   | INT             | FK            |
| ID RAM            | INT             | FK            |
| ID Almacenamiento | INT             | FK            |
| ID Procesador     | INT             | FK            |


***CLIENTES***

| CAMPO           | TIPO DE DATO | TIPO DE CLAVE |
|-----------------|--------------|---------------|
| ID Cliente      | INT          | PK            |
| Nombre Cliente  | TEXT(50)     |               |
| ID Ciudad       | INT          |               |
| ID Pais         | INT          |               |
| ID Envio        | INT          | FK            |

***TIPOS DE CLIENTES***

| CAMPO       | TIPO DE DATO | TIPO DE CLAVE |
|-------------|--------------|---------------|
| ID Tipo     | INT          | PK            |
| Descripcion | TEXT(50)     |               |

***EMPRESAS ENVIO***

| CAMPO    | TIPO DE DATO | TIPO DE CLAVE |
|----------|--------------|---------------|
| ID Envio | INT          | PK            |
| Empresas | TEXT(50)     |               |

***PROCESADOR***

| CAMPO        | TIPO DE DATO   | TIPO DE CLAVE |
|--------------|----------------|---------------|
| ID Procesador| INT            | PK            |
| Procesador   | VARCHAR(100)   |               |

***ALMACENAMIENTO***

| CAMPO          | TIPO DE DATO   | TIPO DE CLAVE |
|----------------|----------------|---------------|
| ID Almacenamiento | INT          | PK            |
| Almacenamiento    | VARCHAR(50)  |               |

***RAM***

| CAMPO  | TIPO DE DATO   | TIPO DE CLAVE |
|--------|----------------|---------------|
| ID RAM | INT            | PK            |
| RAM    | VARCHAR(10)    |               |

***CATEGORIA ARTÍCULO***

| CAMPO             | TIPO DE DATO | TIPO DE CLAVE |
|-------------------|--------------|---------------|
| ID Cat Articulo   | INT          | PK            |
| Categoria Articulo| TEXT(10)     |               |

***TIPO DE PAGO***

| CAMPO         | TIPO DE DATO | TIPO DE CLAVE |
|---------------|--------------|---------------|
| ID Pago       | INT          | PK            |
| Tipo de Pago  | TEXT(50)     |               |

***PAÍS***

| CAMPO     | TIPO DE DATO | TIPO DE CLAVE |
|-----------|--------------|---------------|
| ID Pais   | INT          | PK            |
| Pais      | TEXT(50)     |               |

***CIUDAD***

| CAMPO      | TIPO DE DATO | TIPO DE CLAVE |
|------------|--------------|---------------|
| ID Ciudad  | INT          | PK            |
| Ciudad     | TEXT(50)     |               |

***MARCA***

| CAMPO      | TIPO DE DATO | TIPO DE CLAVE |
|------------|--------------|---------------|
| ID Ciudad  | INT          | PK            |
| Ciudad     | TEXT(50)     |               |

***FACTURAS***

| CAMPO        | TIPO DE DATO  | TIPO DE CLAVE |
|--------------|----------------|---------------|
| ID Factura   | INT            | PK            |
| Nro Factura  | VARCHAR(20)    |               |
| Fecha        | DATETIME       |               |
| ID Pago      | INT            |               |
| ID Review    | INT            | FK            |

***REVIEW***

| CAMPO      | TIPO DE DATO | TIPO DE CLAVE |
|------------|--------------|---------------|
| ID Review  | INT          | PK            |
| Review     | VARCHAR(10)  |               |

## Modificaciones abordadas en Power Query

Una vez exportadas las tablas en Power Bi y durante el proceso de elaboración del dashboard se identificó la necesidad de efectuar diversas modificaciones desde Power Query para mejorar la calidad de la información y exposición en el tablero de control.

## Transformaciones de las tablas

+ ***Tabla Empresas Envío:*** La modificación incorporada sobre la tabla envío consistió en la incorporación de una nueva columna denominada “Imagen”, cuyo tipo de dato es texto, y contiene los URL de imágenes en formato png para utilizarlas en la visualización ChicleySlicer. La fórmula condicional elaborada es la siguiente:
```sql
Imagen = if [ID Envio] = 1 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/DHL.png" else if [ID Envio] = 2 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/FEDEX.png" else if [ID Envio] = 3 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/UPS.png" else if [ID Envio] = 4 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/DB- SCHENKER.png" else if [ID Envio] = 5 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/TNT.png" else "Otro")
```

+ ***Tabla Facturas:*** Se incorporaron dos columnas “Tipo Review” y “Nivel Conformidad” con tipo de dato texto. En la primera se clasifican los ID Review en seis categorías a las que se les asigna un nombre específico, y en la segunda se agrupa en categorías más amplias, de acuerdo a las siguientes fórmulas:
```sql
Tipo Review = if [Tipo Review] = "Insatisfecho" or [Tipo Review] = "Poco Satisfecho" then "Disconforme" else if [Tipo Review] = "Satisfecho" or [Tipo Review] = "Muy Satisfecho" then "Conforme" else if [Tipo Review] = "Neutro" then "Neutro" else "Sin Reseña"
```
```sql
Nivel Conformidad = if [ID Review] = 1 then "Sin Calificar" else if [ID Review] = 2 then "Insatisfecho" else if [ID Review] = 3 then "Poco Satisfecho" else if [ID Review] = 4 then "Neutro" else if [ID Review] = 5 then "Satisfecho" else "Muy Satisfecho")
```

+ ***Tabla Marca:*** Se añadió una columna denominada “Logo”, cuyo tipo de dato es texto, y contiene los URL de imágenes en formato png para utilizarlas en la visualización ChicleySlicer. La fórmula utilizada es la siguiente:
```sql
Logo = if [ID Marca]= 1 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/APPLE.png" else if [ID Marca] = 2 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/SAMSUNG.png" else if [ID Marca] = 3 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/GOOGLE.png"else if [ID Marca] = 4 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/XIAOMI.png" else if [ID Marca] = 5 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/HUAWEI.png" else if [ID Marca] = 6 then "https://raw.githubusercontent.com/VanFolken/img_logos/main/MOTOROLA.png" else "Otro").
```

+ ***Tabla Ventas:*** Se insertaron dos columnas calculadas de tipo decimal que arrojan como resultados el Total Parcial Ventas y el Total Parcial Costos. Las fórmulas utilizadas son las siguientes:
```sql
Total Parcial Ventas = [Precio ud] * [Cantidad]
Total Parcial Costos = [Coste ud] * [Cantidad]
```

## Nuevas tablas incorporadas

Se incorporaron diversas tablas con distinta finalidad en DAX que son detalladas a continuación:

+ ***Tabla DAX Medidas:*** Es la tabla que contiene todas las medidas calculadas utilizadas para el diseño de las visualizaciones en el dashboard.

+ ***Tabla Calendario:*** Se trata de una tabla calculada que contiene un total de cuatro columnas cuyos datos abarcan desde enero 2019 a septiembre 2021 (se delimita el período, puesto que de lo contrario los gráficos con fechas mostraban datos nulos de noviembre a diciembre).
A continuación, se detallan las columnas con sus correspondientes fórmulas calculadas:
```sql
Fecha = CALENDAR(DATE(2019, 1, 1), DATE(2021, 9, 30))
Año = YEAR(Calendario[Fecha])
Mes número = MONTH(Calendario[Fecha])
Mes nombre = LEFT(UPPER(FORMAT(Calendario[Fecha], "MMM")), 1) & MID(FORMAT(Calendario[Fecha], "MMM"), 2, 2)
```

+ ***Tabla Aumento Costos:*** Se creó a través de un parámetro numérico bajo el cual se aplicó un formato porcentual y permite la creación de un segmentador que facilita la simulación de aumentos porcentuales sobre los costos totales.
```sql
Aumento de costos = GENERATESERIES(0, 1.01, 0.01)
Valor de aumento de costos = SELECTEDVALUE('Aumento Costos'[Aumento Costos])
```

+ ***Tabla Incremento Costo UPS:*** Fue creada a través de un parámetro numérico con un formato porcentual que permite la creación de un segmentador que facilita la simulación de aumentos porcentuales sobre una sola variable de los costos. La variable afectada es aquella que corresponde a los clientes que utilizan la empresa de envíos UPS (usuarios que manifestaron mayor insatisfacción, y puede presumirse una relación causal), con la finalidad de simular un escenario en el que Europe Mobile Distributors pueda responsabilizarse por la erogación del traslado.
```sql
Incremento Costo UPS = GENERATESERIES(0, 1.01, 0.01)
Valor de aumento de costos = SELECTEDVALUE('Incremento Costo UPS'[Incremento Costo UPS])
```

+ ***Tabla Descuento Gama Media:*** Se originó a través de un parámetro numérico con formato porcentual que permite la creación de un segmentador que facilita la simulación de descuentos porcentuales sobre una sola variable de las ventas. La variable afectada es aquella que corresponde a los clientes que adquieren artículos de gama media (sobre la que se identificó menor demanda), de ese modo, Europe Mobile Distributors puede simular el impacto que los descuentos pueden provocar en las ganancias con la finalidad de estimular las ventas.
```sql
Descuento de Gama Media =GENERATESERIES(0, 1.01, 0.01)
Valor de Descuento Gama Media = SELECTEDVALUE('Descuento Gama Media'[Descuento Gama Media])
```

+ ***Tabla Atributos sobre la Cantidad Vendida:*** Se trata de una tabla creada a través de un parámetro de campo que permite la creación de un segmentador que filtra la cantidad total vendida por marca o por país, según corresponda.
```sql
Atributos sobre la Cantidad Vendida = {("Marca Articulo", NAMEOF('Marca'[Marca Articulo]), 0), ("País", NAMEOF('Pais'[País]), 1)}
```

+ ***Tabla Ventas Agrupadas:*** Es una tabla creada con la finalidad de agrupar las ventas de acuerdo al número de ID Venta Artículo, para ser utilizada en los cálculos estadísticos, es decir, medidas de tendencia central.
```sql
Ventas Agrupadas = SUMMARIZE(Ventas, Ventas[ID Vta Articulos], "Valor Venta Agrupada", SUM(Ventas[Total Parcial Ventas]))
```

## Diagrama de entidad-relación en Power Bi

<img align="right" alt="PBI-logo" width="150" src="https://github.com/JessBasile/Dashboard-Celulares/raw/main/imagenes/PBI-logo.png">

El diagrama de ER fue modificado respecto el diseño original, puesto que, durante la elaboración del tablero, se detecto la necesidad de cambiar algunas relaciones entre tablas. Se trasladaron las relaciones de las tablas de “Envio” y “Ciudad” hacia “Clientes” (en lugar de Ventas como estaba inicialmente). El cambio se implementó por el descubrimiento de la existencia de clientes inactivos que no figuraban en la tabla de hechos, y eso evitaba que pudiera conocerse la ubicación geográfica de los mismos.

![Diagrama de PBI](imagenes/DER-PBI.png)

## Medidas calculadas

Se crearon un total de 32 medidas calculadas diferentes. Las mismas se encuentran agrupadas en dos carpetas dentro de “DAX Medidas” y sus nombres fueron elegidos acorde a los datos que proporcionan en las visualizaciones.

![Medidas Calculadas](imagenes/medidas-calculadas.png)

A continuación, se detalla la fórmula de calculo sobre cada medida y su finalidad específica.

---
***Medida:*** _Cantidad Total Vendida_
```sql
VAR _cantidadtotalvendida = SUM(Ventas[Cantidad]) RETURN
IF(ISBLANK(_cantidadtotalvendida), 0, _cantidadtotalvendida)
```
***Finalidad:*** Esta medida fue creada a través de una variable para sumar la cantidad total vendida de la columna Cantidad que se encuentra en la tabla Ventas. Al final de la fórmula se aplica una restricción, para que en caso que el resultado sea “en blanco” de cero y al segmentar figure el número en lugar de la palabra.

---
***Medida:*** _Cantidad Total Vendida Año Anterior_
```sql 
CALCULATE([Cantidad Total Vendida], DATEADD(Calendario[Fecha], -1, YEAR))
```
***Finalidad:*** Esta medida permite calcular la cantidad vendida acumulada hasta el año anterior, para ser utilizada en la visualización “Scroller” del mapa que figura en la página productos que permite mostrar numéricamente ese escenario comparativo.

---
***Medida:*** _Cliente Activos_
```sql 
VAR _activos = CALCULATE(DISTINCTCOUNT('Ventas'[ID Cliente])) RETURN
IF(ISBLANK(_activos), 0, _activos)
```
***Finalidad:*** A través de la introducción de una variable, esta medida calcula la cantidad de clientes a los que se les realizaron ventas, asegurándose de no contar clientes de forma duplicada. Al final de la fórmula se aplica una restricción, para que en caso que el resultado sea “en blanco” de cero y al segmentar figure el número en lugar de la palabra.

---
***Medida:*** _Clientes Inactivos_
```sql
VAR _inactivos = ([Total Clientes] - [Clientes Activos]) RETURN
IF(HASONEVALUE('Tipos Cliente'[ID Tipo]), 0,
IF(ISBLANK(_inactivos), 0, _inactivos))
```
***Finalidad:*** Esta medida se realiza a través de una variable que resta dos medidas calculadas generadas anteriormente, y permite obtener la cantidad de clientes a los que no se les efectuaron ventas, puesto que figuran en la tabla Clientes, pero no en la tabla Ventas. Asimismo, se coloca una restricción solicitando que se evalúe si en la tabla Tipos de Cliente existe un valor que especifique el tipo del que se trata, y si no lo hay que arroje el valor cero.
Esta restricción se incorporó dado que los clientes inactivos solo figuran en la tabla Clientes, y los Tipos de clientes solo figuran en la tabla Ventas, en consecuencia, no puede saberse la clase de cliente que son los inactivos. Por último, al final de la fórmula también figura otra restricción, para que en caso que el resultado sea “en blanco” de cero y al segmentar figure el número en lugar de la palabra.

---
***Medida:*** _Costo Total Desglosado por Empresa de Envío_
```sql
VAR _DHL = CALCULATE(SUMX(FILTER('Ventas', RELATED('Clientes'[ID Envio]) = 1), 'Ventas'[Total Parcial Costos]))
VAR _Fedex = CALCULATE(SUMX(FILTER('Ventas', RELATED('Clientes'[ID Envio]) = 2), 'Ventas'[Total Parcial Costos]))
VAR _UPS = CALCULATE(SUMX(FILTER('Ventas', RELATED('Clientes'[ID Envio]) = 3), 'Ventas'[Total Parcial Costos])) * (1 + 'Incremento Costo UPS'[Valor de Incremento Costo UPS])
VAR _Schenker = CALCULATE(SUMX(FILTER('Ventas', RELATED('Clientes'[ID Envio]) = 4), 'Ventas'[Total
Parcial Costos]))
VAR _TNT = CALCULATE(SUMX(FILTER('Ventas', RELATED('Clientes'[ID Envio]) = 5), 'Ventas'[Total Parcial Costos]))
VAR _TotalCostos = _DHL + _Fedex + _UPS + _Schenker + _TNT
RETURN
IF(ISBLANK(_TotalCostos), 0, _TotalCostos * (1 + 'Aumento Costos'[Valor de Aumento Costos]))
```
***Finalidad:*** Se crearon en total de 6 variables, dentro de las cuales 5 corresponden a los costos de los productos que se venden a los clientes que utilizan determinadas empresas de envío. Sobre la empresa UPS se aplica un parámetro numérico que permite incrementarlo a través de una segmentación. La última variable, realiza una suma de todas las anteriores y en su retorno también se aplica un parámetro numérico que permite incrementar el total de los costos para explorar futuros
escenarios. Por último, al final de la fórmula también figura otra restricción, para que en caso que el resultado sea “en blanco” de cero y al segmentar figure el número en lugar de la palabra.

---
***Medida:*** _Disconformes_
```sql
VAR _disconforme = CALCULATE(COUNTROWS('Facturas'), 'Facturas'[ID Review] > 1 && 'Facturas'[ID Review] < 4)
RETURN
IF(ISBLANK(_disconforme), 0, _disconforme)
```
***Finalidad:*** Esta medida a través de una variable cuenta la cantidad de facturas que tienen un ID Review mayor a 1 y menor a 4, puesto que los ID Review 2 y 3 son los clientes “Insatisfechos” y “Poco Satisfechos” considerados como disconformes. Al final de la fórmula se aplica una restricción, para que en caso que el resultado sea “en blanco” de cero y al segmentar figure el número en lugar de la palabra.

---
***Medida:*** _Disconformes Año Anterior_
```sql 
CALCULATE([Disconformes], DATEADD(Calendario[Fecha], -1, YEAR))
```
*** Finalidad:*** Esta medida busca obtener la cantidad acumulada en años anteriores de clientes disconformes para ser utilizada en una visualización KPI que permita observar esa comparación.

---
***Medida:*** _Etiqueta Positiva_
```sql
IF([Disconformes] = 0, UNICHAR(128994), BLANK())
```
***Finalidad:*** Esta medida fue creada con la finalidad de utilizarse como una etiqueta en visualizaciones donde se requiere una indicación visual para manifestar alguna situación en particular. En el dashboard elaborado se utiliza en el gráfico donde se muestra el total de reseñas en comparación a las reseñas disconformes para indicar (con un círculo verde) los meses en los que no hubo reseñas negativas. El código 128994 fue extraído de la página web [https://www.vertex42.com/ExcelTips/unicode-symbols.html](https://www.vertex42.com/ExcelTips/unicode-symbols.html).

---
***Medida:*** _Ganancia Total_
```sql 
[Venta Total Desglosada por Gama] - [Costo Total Desglosado por Empresa Envio]
```
***Finalidad:*** Esta medida se calcula restando dos medidas calculadas anteriormente, para obtener como resultado la ganancia total del período analizado.

