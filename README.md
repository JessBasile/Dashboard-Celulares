## Proyecto Data Analytics 

<img align="right" alt="Jess-perfil" width="150" src="https://github.com/JessBasile/Dashboard-Celulares/raw/main/imagenes/Jess-perfil.png">

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

A continuación, se describen las distintas tablas del modelo especificando las llaves primarias y foráneas.

+ ***Tabla Ventas:*** Contiene el detalle de las ventas discriminado el número de factura, cantidad, precio y costo. En el caso de la factura, articulo, marca, cliente y país figuran con sus abreviaciones.

`PK:` ID Venta Articulo
`FK:` ID Factura
`FK:` ID Articulo
`FK:` ID Marca
`FK:` ID Cliente
`FK:` ID Ciudad
`FK:` ID País
`FK:` ID Pago
`FK:` ID Tipo
