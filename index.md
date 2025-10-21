<section class="two-col">
  <aside class="left profile">
    <h1 class="profile-name">Nadia Medjdoub</h1>
    <img class="profile-photo" src="{{ '/assets/img/profile/profile_pic.jpg' | relative_url }}" alt="Mon portrait" />
    <p class="profile-city">Paris, France</p>
    <p class="profile-phone">(+33)699201222</p>
    <p class="profile-mail">nadia.mejou@gmail.com</p>
    <p class="profile-links">
<a href="#" target="_blank" rel="noopener">Resume</a> |
<a href="https://www.linkedin.com/in/nadia-medjdoub/" target="_blank" rel="noopener">LinkedIn</a> |
<a href="https://github.com/namejou/" target="_blank" rel="noopener">GitHub</a> |
<a href="#" target="_blank" rel="noopener">Tableau</a>
    </p>
    <p class="profile-bio">
      I am a Data & Insights Manager with deep expertise in academic information systems and a strong focus on the higher education sector. My background blends data engineering, analytics, and applied data science to drive impactful, data-informed strategies for universities and educational institutions.
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
