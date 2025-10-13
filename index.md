---
layout: default
title: Accueil
---

<nav>
  <a href="#" id="link-fr" style="font-weight:bold;">Français</a> |
  <a href="#" id="link-en">English</a>
</nav>

<div id="fr" style="display:block;" markdown="1">
  
# 👋 Bienvenue !

Travail en cours — contenu bientôt disponible.

## Mes projets

- **Visualisation de données** : Tableau de bord des affaires académiques utilisant Power BI  
- **Qualité & Intégration des données** : Amélioration de la fiabilité du système d’information académique avec Talend  
- **Gestion des données** : Modélisation basée sur enquêtes du lien entre compétences acquises et exigences du premier emploi (Snowflake & Tableau)  
- **Traitement automatique du langage naturel (TALN)** : Traitement automatisé des réponses ouvertes des enquêtes  

## Contactez-moi

[Envoyez-moi un e-mail](mailto:nadia.medjdoub@hotmail.com)

</div>

<div id="en" style="display:none;" markdown="1">

# 👋 Welcome!

Work in progress — content coming soon.

## My projects

- **Data Visualization**: Academic Affairs Dashboard using Power BI  
- **Data Quality & Integration**: Improved reliability of the Academic Information System using Talend  
- **Data Management**: Survey-based modeling of the match between student-acquired skills and first job requirements (Snowflake & Tableau)  
- **Natural Language Processing (NLP)**: Automated processing of open-ended survey responses

## Contact me

[Send me an email](mailto:nadia.medjdoub@hotmail.com)

</div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const linkFr = document.getElementById('link-fr');
    const linkEn = document.getElementById('link-en');
    const fr = document.getElementById('fr');
    const en = document.getElementById('en');

    linkFr.addEventListener('click', function(e) {
      e.preventDefault();
      fr.style.display = 'block';
      en.style.display = 'none';
      linkFr.style.fontWeight = 'bold';
      linkEn.style.fontWeight = 'normal';
    });

    linkEn.addEventListener('click', function(e) {
      e.preventDefault();
      en.style.display = 'block';
      fr.style.display = 'none';
      linkEn.style.fontWeight = 'bold';
      linkFr.style.fontWeight = 'normal';
    });
  });
</script>
