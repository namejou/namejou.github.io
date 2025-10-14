---
layout: home
title: Accueil
---

# Bonjour 👋
Bienvenue sur mon portfolio minimal.

<section class="projects">
  {% for p in site.data.projects %}
    {% include project-card.html project=p %}
  {% endfor %}
</section>
