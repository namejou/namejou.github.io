---
layout: default
title: Home
---

<button id="btn-fr">Français</button>
<button id="btn-en">English</button>

<div class="lang lang-fr">

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

<div class="lang lang-en" style="display:none;">

# 👋 Welcome !

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
    const btnFr = document.getElementById('btn-fr');
    const btnEn = document.getElementById('btn-en');
    const frSections = document.querySelectorAll('.lang-fr');
    const enSections = document.querySelectorAll('.lang-en');

    btnFr.addEventListener('click', () => {
      frSections.forEach(el => el.style.display = 'block');
      enSections.forEach(el => el.style.display = 'none');
    });

    btnEn.addEventListener('click', () => {
      frSections.forEach(el => el.style.display = 'none');
      enSections.forEach(el => el.style.display = 'block');
    });

    // Par défaut : anglais visible
    btnEn.click();
  });
</script>
