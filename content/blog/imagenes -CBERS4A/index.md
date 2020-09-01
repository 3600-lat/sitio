---
date: 2020-08-29T14:00:00-04:00
lastmod: 2020-08-30T19:00:00-04:00
title: Imágenes CIBERS 4A una alternativa para la planificación Urbana
draft: false
categories:
  - Imagenes
  - Web Services
  - Datos
slug: Imágenes-CIBERS4A-una-alternativa-para-la-planificación-Urbana 
cover:
  image: /images/Screenshot_0.png
  caption: Imagen CBERS4A de la ciudad de La Paz con resolución de 2m.
  style: normal
---

Sin duda unas de las limitaciones en los estudios urbanos era el nivel de resolución espacial de las imágenes satelitales ni mencionar la resolución temporal; nuestras opciones disponibles eran utilizando el catálogo de imágenes de google earth y la aplicación  [SAS-planet](http://www.sasgis.org/); sim embargo si bien cuentan con buena resolución espacial, solo cuenta con una banda NO permitiéndonos hacer combinaciones de bandas con otras regiones del espectro electromagnético.

En ese sentido, recientemente mediante el Programa de cooperación entre Brasil y China lanzaron a fines del año 2019 el satélite CBERS-4ª, cuya principal particularidad es la resolución espacial de 2 metros. Eso implica que es posible identificar objetos geográficos con mayor precisión como: trazado urbano, cuerpos de agua, áreas verdes, vías, etc.

{{< figure src="/images/Screenshot_1.png" alt="Catálogo de imágenes CBERS4A" >}}

Las características de las cámaras de CBERS-4A 

{{< figure src="/images/Screenshot_2.png" alt="Fuente: INPE" >}}

Para mayor información visitar el siguiente [link](http://www.cbers.inpe.br/sobre/cameras/cbers04a.php) 

A continuación, explicaremos brevemente como obtener estas imágenes y realizar composiciones para su posterior interpretación. Lo haremos con [QGIS]  (https://qgis.org/es/site/forusers/download.html) 

Para empezar ingresaremos al [catálogo de imágenes](http://www2.dgi.inpe.br/catalogo/explore) del [INPE](http://www.inpe.br/)

Seguidamente seleccionamos el área de interés (Por ejemplo, la ciudad de La Paz-Bolivia)
{{< figure src="/images/Screenshot_3.png" alt="Seleccionar área" >}}

Luego, seleccionamos las fechas y el % de nubosidad
{{< figure src="/images/Screenshot_4.png" alt="Configurando la búsqueda" >}}

Una vez realizado el Filtro, seleccionamos las imágenes CBERS4A_WPM_L4_DN (3/3) y añadimos a la cesta para su descarga (previamente debemos contar con una cuenta de registro)
{{< figure src="/images/Screenshot_5.png" alt="Imagen seleccionada" >}}
{{< figure src="/images/Screenshot_6.png" alt="Metadato" >}}

Genera un archivo de texto con las URL’s de las imágenes (5 bandas), donde la Banda 0 es la pancromática.

{{< figure src="/images/Screenshot_7.png" alt="URL's de descarga " >}}

Seguidamente, abrimos los archivos en QGIS
{{< figure src="/images/Screenshot_15.png" alt=" Interfaz QGIS" >}}

Luego vamos a las barra de Herramientas , seleccionar RASTER/Miscelanea/Construir raster virtual.
{{< figure src="/images/Screenshot_9.png" alt="Construir raster virtual" >}}

En el menú seleccionar Input layer y hacemos check en las bandas 1,2,3 para componer una banda RGB(321)y ejecutamos
{{< figure src="/images/Screenshot_10.png" alt="Composición de Banda RGB" >}}

Finalmente este raster virtual generado lo fusionamos con la BANDA 0 , haciendo un pansharpening. Para ello vamos a la CAJA DE HERRAMIENTAS DE PROCESO / Pansharpening
{{< figure src="/images/Screenshot_11.png" alt="Pansharpening" >}}

Y seleccionamos EJECUTAR
{{< figure src="/images/Screenshot_12.png" alt="Seleccionamos los Inputs" >}}

{{< figure src="/images/Screenshot_13.png" alt="Imagen final con resolución de 2m.">}}

Ahora si hacemos una composición 432
{{< figure src="/images/Screenshot_14.png" alt="Imagen final con resolución de 2m. en Falso color">}}

Vemos en infrarrojo , y podemos detectar cobertura vegetal en la ciudad de La Paz

Ya se cuenta con las  imágenes, ahora nos toca investigar y aprovecharlas al máximo. 


Aquí les comparto un primer video:

{{< youtube fO4kPG9MybQ >}}



Hasta la proxima.


R. Fernando Molina R.
[@rafemoro](https://twitter.com/rafemoro)
