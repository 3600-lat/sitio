---
date: 2020-08-29T14:00:00-04:00
lastmod: 2020-08-30T19:00:00-04:00
title: \Imágenes CIBERS 4A una alternativa para la planificación Urbana
draft: true
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

Imagen 1




Las características de las cámaras de CBERS-4ª






Para mayor información visitar el siguiente [link](http://www.cbers.inpe.br/sobre/cameras/cbers04a.php) 

A continuación, explicaremos brevemente como obtener estas imágenes y realizar composiciones para su posterior interpretación. Lo haremos con [QGIS]  (https://qgis.org/es/site/forusers/download.html) 

Para empezar ingresaremos al [catálogo de imágenes](http://www2.dgi.inpe.br/catalogo/explore) del [INPE](http://www.inpe.br/)

Seguidamente seleccionamos el área de interés (Por ejemplo, la ciudad de La Paz-Bolivia)
(imagen3)

Luego, seleccionamos las fechas y el % de nubosidad
(imagen4)

Una vez realizado el Filtro, seleccionamos las imágenes CBERS4A_WPM_L4_DN (3/3) y añadimos a la cesta para su descarga (previamente debemos contar con una cuenta de registro)
(imagen5) y (imagen6)

Genera un archivo de texto con las URL’s de las imágenes (5 bandas), donde la Banda 0 es la pancromática.

(imagen7)




Seguidamente, abrimos los archivos en QGIS
(imagen8)


Luego vamos a las barra de Herramientas , seleccionar RASTER/Miscelanea/Cosntruir raster virtual.
(imagen9)

En el menú seleccionar Input layer y hacemos check en las bandas 1,2,3 para componer una banda RGB(321)y ejecutamos
(imagen10)

Finalmente este raster virtual generado lo fusionamos con la BANDA 0 , haciendo un pansharpening. Para ello vamos a la CAJA DE HERRAMIENTAS DE PROCESO / Pansharpening
(imagen11)
Y seleccionamos EJECUTAR
(imagen12)

(imagen13)

Ahora si hacemos una composición 432
(imagen14)

Vemos en infrarrojo , y podemos detectar cobertura vegetal en la ciudad de La Paz

Ya se cuenta con las  imágenes, ahora nos toca investigar y aprovecharlas al máximo. 





Actualmente, existen gran cantidad de sitios web para descargar imágenes satelitales. Este artículo brinda una guía de como descargar de manera facil, gratuita y segura. 
Por lo tanto cualquier persona (no especializada) pueda visualizar, consultar y calcular índices básicos de analisis del territorio.


Como mencionamos anteriorme a la fecha hay muchas fuentes para la descarga de imágenes satelitales, entre ellas existe el [EO Browser](https://apps.sentinel-hub.com/eo-browser/?lat=-4.83&lng=-71.41&zoom=5) que es un visor que nos permite visualizar imágenes provenientes de diferentes recursos satelitales  pudiendo seleccionar el momento temporal, la cobertura de nubes y realizar combinaciones de bandas personalizadas.

Este visor utiliza el fondo de mapa de  [OpenStreetMap](https://www.openstreetmap.org/#map=6/-16.267/-64.823), además se nutre hasta la fecha  de doce recursos satelitales diferentes con los que se puede realizar visualizaciones y combinaciones de bandas:

- Landsat 5 ESA
- Landsat 7 ESA
- Landsat 8 ESA
- Landsat 8 USGS
- Sentinel-1 GRD
- Sentinel-2 L1C
- Sentinel-2 L2A
- Sentinel-3 OLCI
- Sentinel-5P (BETA)
- Envisat Meris
- Proba-V
- GIBS

Deberemos seleccionar el recurso satelital e identificar las fechas para poder acceder al listado de archivos disponibles para la zona visualizada. Junto a las nuevas funciones del visor también se tiene  la opción de subida de archivos en formato KML o KMZ de las zonas en las que estamos interesados. De esta forma podremos identificar los límites espaciales del lugar de interés y realizar descargas concretas sin realizar búsquedas geográficas.

_¿Cómo descargar  imágenes de satélite con EO Browser?_

Aquí les comparto un primer video:

{{< youtube CamR_DDwcBw >}}


La lógica de funcionamiento no dista mucho del resto de visores. Una selección del recurso satelital, la fecha y la posibilidad de realizar composiciones RGB son las funciones básicas del visor para disponer de las imágenes satélites y los análisis multiespectrales que busquemos. Un sistema de memoria de imágenes permite archivar mosaicos en la sección My pins, pudiendo realizar comparaciones temporales entre imágenes mediante efecto split o por transparencia. Asimismo podemos generar un GIFT con todas las imágenes disponibles y de esta forma tener la posibilidad de realizar un análisis multitemporal de nuestra área de estudio 

La composición de imágenes, tanto a falso color como a color real, y la posibilidad de descargar las bandas de manera individual estará disponible (previo registro) desde la opción Analytical pudiendo seleccionar diferentes niveles de resolución, formato de archivo y sistema de referencia.

En nuestro siguiente video explicaremos estas funcionalidades.

{{< youtube LCTE3iV_Rco >}}  


Sin duda, el desarrollo tecnológico está permitiendo contar con estas herramientas via WEB que brinda a los usuarios (no especializados) acceder a datos satelitales, conocer su territorio, que hace 5 años era complicado. 

En las siguientes publicaciones iremos desglosando los diferentes recursos disponibles de esta plataforma y otras.



Hasta la proxima.