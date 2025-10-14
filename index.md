---
layout: home
title: Accueil
---

<!-- Fallback CSS (au cas où site.css n'est pas chargé) -->
<style>
.two-col{display:grid;grid-template-columns:320px 1fr;gap:40px;align-items:start}
.profile{position:sticky;top:24px}
.profile-photo{width:220px;height:220px;object-fit:cover;border-radius:50%;display:block;margin:0 0 16px}
.profile-name{font-size:32px;line-height:1.2;margin:0 0 8px}
.profile-bio{color:#444;margin:8px 0 12px}
.profile-links a{font-weight:600}
@media (max-width:900px){.two-col{grid-template-columns:1fr}.profile{position:static}.profile-photo{width:160px;height:160px}}
</style>

<section class="two-col">
  <aside class="left profile">
    <img class="profile-photo" src="{{ '/profile_pic.jpg' | relative_url }}" alt="Mon portrait" />
    <h1 class="profile-name">Ton Nom</h1>
    <p class="profile-bio">
      Petite bio en 2–3 phrases. Ce que tu fais, ton domaine, ton style.
    </p>
    <p class="profile-links">
      <a href="#" target="_blank" rel="noopener">Resume</a> |
      <a href="#" target="_blank" rel="noopener">LinkedIn</a> |
      <a href="https://github.com/nm-education" target="_blank" rel="noopener">GitHub</a> |
      <a href="#" target="_blank" rel="noopener">Tableau</a>
    </p>
  </aside>

  <div class="right content">
    <h2>Projets</h2>
    <!-- On ajoutera les cartes ici juste après -->
  </div>
</section>
