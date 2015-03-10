---
layout:
permalink: sitemap.xml
---

<?xml version="1.0" encoding="UTF-8"?>
<urlset xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://www.sitemaps.org/schemas/sitemap/0.9 http://www.sitemaps.org/schemas/sitemap/0.9/sitemap.xsd" xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
  {% for post in site.posts %}
  <url>
    <loc>http://darchino.ch/pastore/{{ post.url }}</loc>
    {% if post.lastmod == null %}
    <lastmod>{{ post.date | date_to_xmlschema }}</lastmod>
    {% else %}
    <lastmod>{{ post.lastmod | date_to_xmlschema }}</lastmod>
    {% endif %}
    <changefreq>weekly</changefreq>
    <priority>1.0</priority>
  </url>
  {% endfor %}
  {% for page in site.pages %}
    {% if page.url != '/404/' %}
  <url>
    <loc>http://darchino.ch/pastore/{{ page.url }}</loc>
  </url>
    {% endif %}
  {% endfor %}
</urlset>


