---
layout: page
title: Chiesa
category: chiesa
social: false
section: true
image: SMartinoBondo.jpeg
---

Anche se le chiese hanno tanti difetti, il messaggio di salvezza di Gesù Cristo forma una comunità, non è solo qualcosa di individuale.

Per questo anche se nella storia della chiesa ci sono stati tanti errori, alle volte terribili, e altri errori saranno compiuti perché le chiese sono realtà umane, partecipare alla vita di una qualche chiesa e l’unica maniera per rispondere alla chiamata cristiana.

In questo senso nel Credo viene detto che si crede alla Chiesa, che si crede cioè che pur fra infedeltà e tradimenti, c’è un insieme di persone che vengono guidate dallo Spirito per annunciare nel mondo la Parola del Signore ed agire secondo la volontà di Dio.

Le persone che fanno parte della Chiesa di Cristo sono conosciute solo da Dio. E le chiese nel mondo sono viste come una parte della Chiesa di Cristo.
 
---------------------------

Gli ultimi post sul tema Chiesa:

<div class="posts">
    {% assign bene = 'ok' %}
    {% for post in site.posts limit:20 %}
    {% if post.tags contains 'Chiesa' %}
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
