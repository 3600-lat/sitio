---
date: 2019-10-11T14:00:00-04:00
lastmod: 2019-10-11T19:00:00-04:00
title: Descargar datos Abiertos OpenStreetMap mediante QGIS3
draft: true
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

-Ventajas son muchas, estos datos son una primera aproximación de un territorio a intervenir (sobretodo en territorios con ausencia de información);
-Datos almacenados en una base de datos, permite su consulta ágil y rápida
-En cuanto a sus desventajas; es la heterogeneidad de la información (lugares con mucha información y otras con baja), eso significa contar con mayor cantidad de voluntarios que ayuden a la constante actualización y tambien la verificación (control de calidad) de la información capturada.

## ¿Cómo descargamos los datos de OSM?

De la siguiente manera:

- Primero ingreso a QGIS
- Seguidamente selecciono en la barra de menús la opción complementos/ Instalo la herramienta OSN
- Ingresa a la plataforma desarrollada sobre [I3GEO](https://softwarepublico.gov.br/gitlab/i3geo/i3geo/commit/63f28b011019104c2f1c29ae84dcaaf7ff6e6218) (Interface Integrada para Internet de Ferramentas de Geoprocessamento) es una aplicación para el desarrollo de mapas interactivos en la web, que integra varias aplicaciones de código abierto en una sola plataforma de desarrollo, principalmente Mapserver y OpenLayers. El programa se distribuye con licencia GPL (GNU General Public License), que permite acceder al código fuente y modificar, distribuir y compartir el software y fue creado por el Ministério do Meio Ambiente (MMA) de Brasil en 2004.
- Brinda la opción de visualizar por Departamentos (disperso, amanzanada), por supuesto nosotros elegiremos la opción AMANZANADA.
- Procedemos a la selección del área de interes como en el video se puede observar y generar el reporte en PDF ( la opción -XLS a mi no me funciona) sería ideal que la habiliten en *.CSV

Nosotros la utilizamos como una primera aproximación, validar información OFICIAL y desarrollar aplicaciones 



Aquí les comparto el proceso:

{{< youtube 8nr3SZM-Y9w >}}


Esta herramienta es super útil ojala puedan probarlo y generar los reportes que deseen, felicitar al INE por la plataforma falta aún mejorar los formatos de descarga y simplificar el proceso sería genial

Si tienes alguna duda sobre el proceso no dudes en escribirnos a contacto@3600.lat o por nuestras redes sociales donde estaremos atentos a tus comentarios.

SaluDATOS…

@rafemoro


