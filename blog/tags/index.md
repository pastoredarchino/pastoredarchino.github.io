---
layout: page
title: Tags
category: blog
social: false
description: sezione per migliorare la ricerca dei post con tags, autore e anno
---

Per migliorare la ricerca ecco i post raggruppati per Tag, cioé per l'argomento sotto cui rientra il tema trattato.

{% for tag in site.tags %}
<a style="float:left; margin: 0.5rem; font-size: {{ tag | last | size | times: 100 | divided_by: site.tags.size | plus: 70 }}%" href="/tags/{{ tag | first | slugize }}/">   {{ tag | first }} </a>
{% endfor %}

Se li volete per anno di pubblicazione, vedete qui: [Archivio]({{ site.baseurl }}/tags/archivio/).




