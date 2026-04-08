---
title: Entradas
layout: post
icon: fas fa-stream
order: 40
toc: true
description: Todas las entradas del blog Diario de un parkinsoniano
---
Aquí puedes acceder a todas las entradas (también llamadas *posts*) del blog, publicadas hasta el momento, agrupadas en Relatos y en orden cronológico, gracias al trabajo de mi amiga Juana Zarranz.

Para leer una entrada, toca sobre ella con el dedo, o haz clic con el ratón.
<!-- Home Post List -->
{% for tag in site.tags %}

## {{ tag[0] | replace: '-', ' '}}

<ul>
    {% for post in tag[1] reversed %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
    