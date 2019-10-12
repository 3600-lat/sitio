---
date: 2019-10-12T14:00:00-04:00
lastmod: 2019-10-12T19:00:00-04:00
title: Descargar datos Abiertos OpenStreetMap mediante QGIS3
draft: false
categories:
  - OSM
  - Web Services
  - Datos
slug: Descargar-datos-Abiertos-OpenStreetMap-mediante-QGIS3

cover:
  image: /images/osm_download.jpg
  caption: Descarga datos OSM en QGIS3
  style: normal
---

[OpenStreetMap](https://www.openstreetmap.org/#map=14/-16.5297/-68.1108), de un tiempo a esta parte se ha convertido en una herramienta fundamental para nuestro trabajo, mucha gente ayuda a su actualización de manera voluntaria, pero su gran potencial
es en la oportunidad que nos brinda para su descarga, con su respectiva licencia abierta.

Ahora pasaremos a describir este proceso para su respectiva descarga y comprender sus ventajas y limitaciones al respecto.

- Ventajas son muchas, estos datos son una primera aproximación de un territorio a intervenir (sobretodo en territorios con ausencia de información);
- Datos almacenados en una base de datos, permite su consulta ágil y rápida
- En cuanto a sus desventajas; es la heterogeneidad de la información (lugares con mucha información y otras con baja), eso significa contar con mayor cantidad de voluntarios que ayuden a la constante actualización y tambien la verificación (control de calidad) de la información capturada.

## ¿Cómo descargamos los datos de OSM?

De la siguiente manera:

- Primero ingresamos a [QGIS](https://www.qgis.org/es/site/) 
- Seguidamente selecciono en la barra de menús la opción complementos/ Instalo la herramienta [OSMDownloader](https://github.com/lcoandrade/OSMDownloader)
- Una vez instalado, verificamos el icono de descarga, le hacemos click y; 
- seleccionamos el área a descargar (podemos utilizar una geometria del área de estudio)
- y listo, guardamos en el formato deseado (mejor si es geopackage :)


Aquí les comparto el proceso:

{{< youtube 8nr3SZM-Y9w >}}


Nosotros la utilizamos estos datos de OSM como una primera aproximación, validar información OFICIAL y desarrollar aplicaciones, y simultaneamente vamos actualizando sectores que aún faltan completar

Agradecer a todos los voluntarios y desarrolladores que apoyan a OpenStreetMap, hay mucho por hacer si quieres ser un mapeador de OSM visita este [link](https://learnosm.org/es/) les ayudará mucho.

Si tienes alguna duda sobre el proceso no dudes en escribirnos a contacto@3600.lat o por nuestras redes sociales donde estaremos atentos a tus comentarios.

SaluDATOS…

@rafemoro


