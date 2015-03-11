---
title: Culto
layout: page
category: culto 
author: Stefano
thumb:
image: campanile.jpg
description: Presentazione del culto
section: true
hide: false
---

Il trovarsi insieme per pregare, ascoltare una predicazione, cantare inni, celebrare la Cena del Signore o un battesimo si chiama per gli evangelici culto.

Dunque il culto è per gli evangelici quello che per altre confessioni cristiane è grosso modo la messa, la funzione, il servizio divino.

---------------------------

Le ultime meditazioni pubblicate:

<div class="posts">
    {% assign bene = 'ok' %}
    {% for post in site.posts limit:20 %}
    {% if post.tags contains 'Meditazione' %}
        {% if bene == 'ok' %}
            {% assign numero = numero | plus: 1 %}
<div class="post-teaser">
            {% include post-teaser.html %}
</div>
            {% if numero == 4 %}
                {% assign bene = 'nok' %}
            {% endif %}
        {% endif %}
    {% endif %}
    {% endfor %}
</div>
