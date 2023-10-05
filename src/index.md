---
layout: base.njk
title: Mi Blog
---

# {{ title }}

- El segundo mas cabron de los cabroncitos

![Banner perfil]({{ '/static/img/bannerPerfil.png' | url }})

[Acerca]({{ '/acerca' | url }})

## Blog

### Mis Juegos Favoritos

{% for juego in collections.juegos %}

- [{{juego.data.title}}]({{ juego.url | url }})

{% endfor %}

### Mis Series Favoritas

{% for serie in collections.series %}

- [{{serie.data.title}}]({{ serie.url | url }})

{% endfor %}

### Mis Peliculas Favoritas

{% for pelicula in collections.peliculas %}

- [{{pelicula.data.title}}]({{ pelicula.url | url }})

{% endfor %}
