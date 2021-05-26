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
    Ingénieur de formation et de profession, je m'intéresse aux questions agricoles, environnementales et économiques au travers de rapports, articles, conférences ou débats, en collaboration ponctuelle avec des médias ou des think-tanks. Je défends une société ouverte, guidée par la science et la raison, résolument écomoderniste, humaniste et libérale.
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