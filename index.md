---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
---

<h1>Bienvenue sur mon site !</h1>
<div class="intro-container">
  <div class="profile-picture-container">
    <img src="assets/img/pahpy.jpg" alt="Profile picture Laurent Pahpy">
  </div>
  <div class="welcome-message-container">
    Je m’appelle Laurent Pahpy et je suis analyste pour l’Institut de recherches économiques et fiscales (IREF). Ingénieur de formation, j’étudie comment l’économie de marché et la science permettent de construire une société plus juste et plus libre. 
  </div>
</div>

<!-- <br>
<h1>Mes derniers rapports</h1>
{% for publi in site.data.publis %}
  <div class="publi-container">
    {% if publi.format == "Rapport" %}
      <div class="media-logo-container">
        <img class="media-logo" src="assets/img/{{ publi.media }}.png" alt="{{ publi.media }}">
      </div>
      <div class="publi-info-container">
        <a href="{{ publi.url }}" target="_blank">{{ publi.title }}</a><br>
        <span class="description">{{ publi.format }} • {{ publi.date }} • {{ publi.media }} • {{ publi.author }}{% if publi.author2 != "" %}, {{ publi.author2 }}{% endif %}{% if publi.author3 != "" %}, {{ publi.author3 }}{% endif %}{% if publi.author4 != "" %}, {{ publi.author4 }}{% endif %}{% if publi.author5 != "" %}, {{ publi.author5 }}{% endif %}{% if publi.author6 != "" %}, {{ publi.author6 }}{% endif %}</span>
      </div>
    {% endif %}
  </div>
{% endfor %} -->

<br>
<h1>Mes articles, rapports, conférences et interventions médias</h1>
{% for publi in site.data.publis %}
  <div class="publi-container">
    <div class="media-logo-container">
      <img class="media-logo" src="assets/img/{{ publi.media }}.png" alt="{{ publi.media }}">
    </div>
    <div class="publi-info-container">
      <a href="{{ publi.url }}" target="_blank">{{ publi.title }}</a><br>
      <span class="description">{{ publi.format }} • {{ publi.date }} • {{ publi.media }} • {{ publi.author }}{% if publi.author2 != "" %}, {{ publi.author2 }}{% endif %}{% if publi.author3 != "" %}, {{ publi.author3 }}{% endif %}{% if publi.author4 != "" %}, {{ publi.author4 }}{% endif %}{% if publi.author5 != "" %}, {{ publi.author5 }}{% endif %}{% if publi.author6 != "" %}, {{ publi.author6 }}{% endif %}</span>
    </div>
  </div>
{% endfor %}