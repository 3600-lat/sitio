---
date: 2018-09-05T08:00:00-04:00
lastmod: 2018-09-05T08:00:00-04:00
title: ¿Como construir un mapa web en Cuatro (4) pasos?
draft: false
categories:
  - Visualización de datos
  - Mapas Web
  - Datos
cover:
  image: /images/umap_web.jpg
  caption: Mapa WEB
  style: normal
---

Publicar nuestros mapas en la web, a diferencia de la creación de mapas estáticos (por ejemplo un PDF), tiene la ventaja de poder llegar más rápidamente y a un público más amplio.
Basta con facilitar una dirección URL de nuestros mapas online a nuestros colegas, para que puedan verlos.
A pesar de que la creación de mapas web está estrechamente relacionada con la programación y tiene una curva de aprendizaje, existen algunas herramientas que podemos utilizar para hacer mapas interactivos de una forma sencilla

## ¿Que es un mapa Web?

Es una visualización interactiva de información geográfica que puede utilizar para contar historias y responder preguntas. Estos mapas contienen un mapa base, un conjunto de capas de datos (muchos de los cuales incluyen ventanas emergentes interactivas con información sobre los datos), una extensión y herramientas de navegación para el desplazamiento panorámico y el zoom. Muchos mapas también contienen símbolos escalados y otros elementos de estilo inteligentes que revelan datos a medida que interactúas con ellos.
Los mapas se pueden crear en unos pocos pasos sencillos y abrirse en navegadores Web estándar y dispositivos móviles principalmente.

Se pueden compartir a través de vínculos, se pueden integrar en sitios. Al compartir un mapa, el autor decide lo que quiere incluir en él.
Por ejemplo, incluir opciones para cambiar Fondos de mapa, ver una leyenda (si el mapa incluye una), ver detalles acerca del mapa, compartir, imprimir, medir y buscar ubicaciones en el mapa.
Los mapas incluidos en sitios web y compartidos a través de aplicaciones a menudo contienen un conjunto de herramientas en concreto para un fin determinado, como puede ser capturar información, editar entidades, etc.

Para nuestro ejemplo utilizaremos el servicio de [UMAP](https://umap.openstreetmap.fr/es/); que es un servicio que te permite visualizar y crear datos geográficos con fondos de mapa diseñados sobre de OpenStreetMap de manera ágil y embeber en tu sitio.
Asimismo, este servicio te permite :

- Elegir las capas de tu mapa
- Añadir puntos de interés (PDI): marcadores, líneas, polígonos...
- Eligir los colores y los iconos de los PDI
- Gestionar opciones del mapa: mostrar un mini-mapa, localizar al usuario al cargar...
- Importar por lotes datos geoestructurados (geojson, gpx, kml, osm...)
- Elegir las licencias de tus datos
- Embeber y compartir tu mapa

A continuación construiremos nuestro mapa web a partir de la siguiente secuencia:

{{< figure src="/images/mapa_web.jpg" alt="Cuatro pasos" >}}

### Primer Paso

{{< youtube cjW-Fh571Kk>}}

### Segundo Paso

{{< youtube y7Kaf9eRUXQ>}}

### Tercer Paso

{{< youtube dOa7iAQtFEs>}}

### Cuarto Paso

{{< youtube _Bc3XiV5v6s>}}

Aquí tienes el producto final:

http://umap.openstreetmap.fr/es/map/mapa-de-asaltos_245223#13/-16.5068/-68.0835

Para embeberlo aquí:

```html
<iframe
  width="100%"
  height="300px"
  frameBorder="0"
  allowfullscreen
  src="https://umap.openstreetmap.fr/es/map/mapa-de-asaltos_245223?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&allowEdit=false&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=undefined&captionBar=false"
  ></iframe>
<p><a href="https://umap.openstreetmap.fr/es/map/mapa-de-asaltos_245223">Ver pantalla completa</a></p>
```

El resultado es el siguiente:

<iframe
  width="100%"
  height="300px"
  frameBorder="0"
  allowfullscreen
  src="https://umap.openstreetmap.fr/es/map/mapa-de-asaltos_245223?scaleControl=false&miniMap=false&scrollWheelZoom=false&zoomControl=true&allowEdit=false&moreControl=true&searchControl=null&tilelayersControl=null&embedControl=null&datalayersControl=true&onLoadPanel=undefined&captionBar=false"
  ></iframe>
<p><a href="https://umap.openstreetmap.fr/es/map/mapa-de-asaltos_245223">Ver pantalla completa</a></p>

Finalmente te desafío a que construyas tu mapa web utilizando estos datos almacenados en [GeoBolivia](http://geo.gob.bo/download/?w=GobMunicipal&l=Museoswgs84) proveniente del Gobierno Autónomo Municipal de La Paz.

Si tienes alguna duda sobre el proceso no dudes en escribirnos a <a href="mailto:contacto@3600.lat">contacto@3600.lat</a> o por [nuestras redes sociales](https://3600.lat/contacto/) donde estaremos atentos a tus comentarios.

SaluDATOS...
