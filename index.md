---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

{% for publi in site.data.publis %}
  <div class="publi-container">
    <div class="media-logo-container">
      <img class="media-logo" src="assets/img/{{ publi.media }}.png" alt="{{ publi.media }}">
    </div>
    <div class="publi-info-container">
      <a href="{{ publi.url }}" target="_blank">{{ publi.title }}</a><br>
      <span class="description">{{ publi.format }} • {{ publi.date }} • {{ publi.media }} • {{ publi.author }}</span>
    </div>
  </div>
{% endfor %}