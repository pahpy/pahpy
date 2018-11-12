---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<h1>Mes publications</h1>

{% for publi in site.data.publis %}
  <h1><a href="{{ publi.url }}" target="_blank">{{ publi.title }}</a></h1>
  {{ publi.format }} • {{ publi.date }} • {{ publi.media }} • {{ publi.author }}
{% endfor %}