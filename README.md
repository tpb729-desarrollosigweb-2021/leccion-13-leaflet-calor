# Leaflet - mapas de calor (*heat maps*)
## Leaflet.heat
El complemento [Leaflet.heat](https://github.com/Leaflet/Leaflet.heat) simplifica la elaboración de [mapas de calor (*heat maps*)](https://es.wikipedia.org/wiki/Mapa_de_calor).

Para utilizarse, primero debe incluirse el enlace al archivo JavaScript del complemento. 

```html
<head>
  ...
  script src="https://cdnjs.cloudflare.com/ajax/libs/leaflet.heat/0.2.0/leaflet-heat.js"></script>
</head>
```

Para generar el mapa de calor, debe crearse un objeto de la clase ```L.heatLayer```.

```javascript
  coordenadas = geodata.features.map(feat => feat.geometry.coordinates.slice().reverse());
  var capa_carnivora_calor = L.heatLayer(coordenadas, {radius: 30, blur: 1});
```

En el sitio de Leaflet.heat puede encontrar más información acerca de [como personalizar el mapa de calor](https://github.com/Leaflet/Leaflet.heat#reference).

Puede ver un ejemplo de un mapa de puntos agrupados con íconos personalizados en [https://tpb729-desarrollosigweb-2021.github.io/ejemplo-mapa-leaflet-calor/](https://tpb729-desarrollosigweb-2021.github.io/ejemplo-mapa-leaflet-calor/).

**Ejercicios**  
1. Utilice una capa de puntos de sus tareas para generar un mapa de calor.
