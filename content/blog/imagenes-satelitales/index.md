---
date: 2018-08-12T14:00:00-04:00
lastmod: 2018-08-16T19:00:00-04:00
title: Descargando imagenes satelitales de Bolivia 
draft: false
categories:
  - Imagenes
  - Web Services
  - Datos
slug: procesando-imagenes-satelitales-con-software-libre
cover:
  image: /images/eobrowser.jpg
  caption: Interfaz EOBrowser
  style: normal
---
Actualmente, existen gran cantidad de sitios web para descargar imágenes satelitales. Este artículo brinda una guía de como descargar de manera facil, gratuita y segura. 
Por lo tanto cualquier persona (no especializada) pueda visualizar, consultar y calcular índices básicos de analisis del territorio.


Como mencionamos anteriorme a la fecha hay muchas fuentes para la descarga de imágenes satelitales, entre ellas existe el [EO Browser](https://apps.sentinel-hub.com/eo-browser/?lat=-4.83&lng=-71.41&zoom=5) que es un visor que nos permite visualizar imágenes provenientes de diferentes recursos satelitales  pudiendo seleccionar el momento temporal, la cobertura de nubes y realizar combinaciones de bandas personalizadas.

Este visor utiliza el fondo de mapa de  OpenStreetMap, además se nutre hasta la fecha de 12 recursos satelitales diferentes con los que se puede realizar visualizaciones y combinaciones de bandas:

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

Aquí les comparto un primer video

{{< youtube CamR_DDwcBw >}}


La lógica de funcionamiento no dista mucho del resto de visores. Una selección del recurso satelital, la fecha y la posibilidad de realizar composiciones RGB son las funciones básicas del visor para disponer de las imágenes satélites y los análisis multiespectrales que busquemos. Un sistema de memoria de imágenes permite archivar mosaicos en la sección My pins, pudiendo realizar comparaciones temporales entre imágenes mediante efecto split o por transparencia. Asimismo podemos generar un GIFT con todas las imágenes disponibles y de esta forma tener la posibilidad de realizar un análisis multitemporal de nuestra área de estudio 

La composición de imágenes, tanto a falso color como a color real, y la posibilidad de descargar las bandas de manera individual estará disponible (previo registro) desde la opción Analytical pudiendo seleccionar diferentes niveles de resolución, formato de archivo y sistema de referencia.

En nuestro siguiente video explicaremos estas funcionalidades.

{{< youtube LCTE3iV_Rco >}}  


Sin duda, el desarrollo tecnológico está permitiendo contar con estas herramientas via WEB que brinda a los usuarios (no especializados) acceder a datos satelitales, conocer su territorio, que hace 5 años era complicado. 

En las siguientes publicaciones iremos desglosando los diferentes recursos disponibles de esta plataforma y otras.

Hasta la proxima

