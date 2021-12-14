# Sistema-de-Grillas
En este repositorio se pone a disposición el sistema de grillas para la aplicación de los protocolos oficiales de monitoreo

## Creación del sistema de grillas  

Se generaron dos sistemas de grillas, uno para el territorio continental e islas/islotes cercanos (continental de acá en adelante) y otro para la Isla del Coco. Ambos sistemas de grillas se crearon usando el programa QGIS 3.16.11 (QGIS.org, 2021), mediante la función Vectorial – Herramientas de Investigación- Crear Cuadrícula, con SRC CRTM05-EPSG 5367 y utilizando valores de Espaciado Horizontal y Espaciado Vertical de 1km x 1 km, 2km x 2km, 4km x 4km, y 8km x 8km. En el caso de la Isla del Coco, solo se generaron grillas de 1x1 km y 2x2 km. 

Para la grilla continental se utilizó una extensión de cuadrícula Xmin 280000, Ymin 888000, Xmax 660000, Ymax 1244000 (SINAC 2018) y para la grilla de la Isla del Coco, se utilizó la extensión de la capa Isla del Coco, Xmin 156147.2142, Ymin 164388.5675, Xmax 608238.1248, Ymax 616005.2418.

Posteriormente, mediante la función Vectorial – Herramientas de Geoproceso- Cortar, se cortaron las capas generadas con base a la capa “Delimitaciónterritorial2017 1:5mil”, para la grilla continental, y la capa Isla del Coco. 

Por último, todas las capas fueron reproyectadas a CR-SIRGAS-UTM zone 16N

