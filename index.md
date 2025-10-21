---
layout: home
title: Portfolio
---

<section class="two-col">
  <aside class="left profile">
    <h1 class="profile-name">Nadia Mejou</h1>
    <img class="profile-photo" src="{{ '/assets/img/profile/profile_pic.jpg' | relative_url }}" alt="Mon portrait" />
    <p class="profile-city"> 
      Paris, France
    </p>
    <p class="profile-phone">
      (+33)699201222
    </p>
    <p class="profile-mail">
      nadia.mejou@gmail.com
    </p>
    <p class="profile-links">
      <a href="#" target="_blank" rel="noopener">Resume</a> |
      <a href="#" target="_blank" rel="noopener">LinkedIn</a> |
      <a href="https://github.com/nm-education" target="_blank" rel="noopener">GitHub</a> |
      <a href="#" target="_blank" rel="noopener">Tableau</a>
    </p>
    <p class="profile-bio">
      I am a Data & Insights Manager with deep expertise in academic information systems and a strong focus on the higher education sector. My background blends data engineering, analytics, and applied data science to drive impactful, data-informed strategies for universities and educational institutions.
    </p>
  </aside>

  <div class="section-title">
    <h2>Portfolio</h2>
    <div class="section-title">
  <h2>Portfolio</h2>
  <div class="projects-list">
    {% assign projets = site.data.projects %}
    {% for projet in projets %}
      <article class="project-card">
        <h3>{{ projet.title }}</h3>
        <img src="{{ projet.image | relative_url }}" alt="{{ projet.title }}">
        <p>{{ projet.description }}</p>
        <ul class="skills-list">
          {% for skill in projet.skills %}
            <li>{{ skill }}</li>
          {% endfor %}
        </ul>
        <div class="project-links">
          {% for link in projet.links %}
            <a href="{{ link.url }}" target="_blank" rel="noopener">
              {% if link.badge %}
                <img src="{{ link.badge }}" alt="{{ link.label }}" class="badge" />
              {% else %}
                {{ link.label }}
              {% endif %}
            </a>
          {% endfor %}
        </div>
      </article>
    {% endfor %}
  </div>
</div>

  </div>
</section>
