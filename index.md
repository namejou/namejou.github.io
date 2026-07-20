<section class="two-col">
  <aside class="left profile">
    <h1 class="profile-name">Nadia Mejou</h1>
    <img class="profile-photo" src="{{ '/assets/img/profile/profile_pic.jpg' | relative_url }}" alt="Mon portrait" />
    <p class="profile-city">Paris, France</p>
    <p class="profile-mail">nmejou@protonmail.com</p>
    <p class="profile-links">
<a href="#" target="_blank" rel="noopener">Resume</a> |
<a href="https://www.linkedin.com/in/nadia-mejou/" target="_blank" rel="noopener">LinkedIn</a> |
<a href="https://github.com/namejou/" target="_blank" rel="noopener">GitHub</a> |
<a href="#" target="_blank" rel="noopener">Tableau</a>
    </p>
    <p class="profile-bio">
      I am a Data & Analytics Manager focused on data governance, data quality, and business intelligence. I help organizations structure and leverage their data by designing reliable indicators, improving data processes, and building analytics solutions that support informed decisions.
    </p>
  </aside>

  <div class="section-title">
    <h2>Portfolio</h2>
    <div class="projects-list">
      {% assign projects = site.data.projects %}
      {% for project in projects %}
        <article class="project-card">
          <h3>{{ project.title }}</h3>
          <p class="project-description">{{ project.description }}</p>
          <div class="project-links">
            {% for link in project.links %}
              <a href="{{ link.url }}" target="_blank" rel="noopener">
                <img src="{{ link.badge }}" alt="{{ link.label }}">
              </a>
            {% endfor %}
          </div>
          <p class="project-skills">
            <em>Key Skills: {{ project.skills | join: ', ' }}</em>
          </p>
          <div class="project-summary">
            {{ project.summary | markdownify }}
          </div>
          <div class="project-image-wrapper">
            <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" class="project-image">
          </div>
        </article>
      {% endfor %}
    </div>
  </div>
</section>
