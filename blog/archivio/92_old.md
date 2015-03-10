---
layout: page
title: Anni precedenti
category: blog
social: false
---
In questo pagina sono raccolti post scritti prima del 2010. 
Non sono tutti i post, ma quelli che per qualche motivo sembravano ancora di un qualche interesse.

<ul>
  {% for post in site.posts %}
   {% assign anno = post.date | date: "%Y" %}
   {% if anno == '2005' or anno == '2006' or anno == '2007' or anno == '2008'or anno == '2009' %}
       <li><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
{% assign m = post.date | date: "%-m" %}
({{ post.date | date: "%-d" }}
{% case m %}
  {% when '1' %}gennaio
  {% when '2' %}febbraio
  {% when '3' %}marzo
  {% when '4' %}aprile
  {% when '5' %}maggio
  {% when '6' %}giugno
  {% when '7' %}luglio
  {% when '8' %}agosto
  {% when '9' %}settembre
  {% when '10' %}ottobre
  {% when '11' %}novembre
  {% when '12' %}dicembre
{% endcase %} 
{{ post.date | date: "%Y" }})
 <a style="color:gray" href="{{ site.baseurl }}/blogs/0{{ post.author }}">{{ post.author }}</a>
 {% for tag in post.tags %}
 <a style="color:gray" href="{{ site.baseurl }}/blogs/tags/{{ tag }}">{{ tag }}</a>
{% endfor %}
</li>
   {% endif %} 
  {% endfor %}
</ul>


 
