---
layout: home
title: Accueil
---

# Bonjour 👋
Bienvenue sur mon portfolio minimal.

{% for p in site.data.projects %}
- {{ p.title }}
{% endfor %}

<section class="projects">
  {% for p in site.data.projects %}
    {% include project-card.html project=p %}
  {% endfor %}
</section>
