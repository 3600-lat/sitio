---
date: 2018-08-12T14:00:00-04:00
lastmod: 2018-08-16T19:00:00-04:00
title: Procesando imágenes satelitales con Software libre
draft: true
categories:
  - satelital
  - software libre
slug: procesando-imagenes-satelitales-con-software-libre
cover:
  image: /test/images/cubo.jpg
  caption: Rubik's Cube andino
  style: normal
---

## Introducción

Actualmente, la inmensa mayoría de los datos producidos por la actividad científica es analizada y procesada utilizando diversas herramientas de software, que abarcan desde la más sencilla planillade cálculos, hasta el más complejo de los sistemas desplegados en clusters. En las tareas más triviales,ciertos aspectos de las herramientas informáticas pueden pasar desapercibidos a los usuarios. 

Sin embargo, durante la ejecución de algoritmos complejos, resulta imprescindible que el investigador sepa exactamente qué operaciones se están realizando sobre sus datos. Tal situación de transparencia no se da cuando se utiliza un software que no permite acceder al código de procesamiento de manera explícita. Ni siquiera en el mejor de los casos, esto es, cuando se brinda documentación relativamente detallada, no es posible estar plenamente seguro de qué transformaciones se están operando sobre los datos. Por otra parte, es común que un investigador, debido a las particularidades de sus datos o de1sus objetivos de investigación, necesite desarrollar algoritmos de análisis y/o de procesamiento propios. 

Esta posibilidad de desarrollar algoritmos propios no siempre está incorporada en el software privativo. De allí que en la mayor parte de los casos, e independientemente de los elevados y a veces inalcanzables costos de las licencias, la elección de software libre y abierto resulte la elección más adecuada, puesto que permite al usuario ver y/o modificar las transformaciones que se operan sobre los datos en cada una de las etapas de procesamiento.

En ese sentido, el dia de hoy  compartiremos nuestra experiencia en el uso de [Quantum GIS (QGIS)](https://www.qgis.org/) es un sistema de información geográfica (SIG, o GIS por sus siglas en inglés)que permite trabajar con los formatos más clásicos de los entornos GIS: vector, raster y base de datos.Además, es posible agregarle complementos que permiten intercambiar información y funcionalidades con otras herramientas tales como GDAL/OGR. QGIS puede operarse a través de una interfaz gráficamuy intuitiva, pero, además, permite generar y utilizar scripts mediante una consola Python. Existen distintas versiones que se adaptan a una variedad de sistemas operativos. QGIS dispone de muy buena documentación oficial en distintos idiomas incluyendo el español. Además, cuenta distintos foros orientados a usuarios y a desarrolladores.

QGIS es un software de Sistemas de Informática (SIG) muy versátil para el manejo de datos espaciales tanto vectoriales como raster. Dentro de QGIS existe un ecosistema de complementos que implementan mayores funcionalidades para el análisis espacial. Uno de los últimos complementos es el [Semi Automatic Classification Plugin (SCP](https://goo.gl/vDFza4)) que tiene toda una serie de herramientas para el procesamiento de imágenes satelitales incluyendo la descarga de estas imágenes, la clasificación supervisada y el análisis espectral.

En este tutorial vamos a realizar una clasificación espectral con 10 categorías sobre una imagen recortada de Landsat 8 en la parte sur del Altiplano del Departamento de La Paz. Las bandas utilizadas en este tutorial son las bandas visibles y el infrarojo.
