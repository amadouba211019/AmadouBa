<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Amadou Ba — Économiste</title>

<meta name="description"
      content="Portfolio professionnel d'Amadou Ba, titulaire d'un Master 2 en Analyse économique et quantitative.">

<style>

/* =========================================================
   RESET
========================================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #ffffff;
    color: #111111;
    line-height: 1.6;
}

a {
    color: inherit;
    text-decoration: none;
}

button {
    font-family: inherit;
}

/* =========================================================
   VARIABLES
========================================================= */

:root {
    --black: #111111;
    --dark: #181818;
    --gray: #666666;
    --light-gray: #eeeeee;
    --lighter: #f7f7f7;
    --white: #ffffff;
    --border: #dddddd;
}

/* =========================================================
   CONTAINER
========================================================= */

.container {
    width: min(1120px, 92%);
    margin: auto;
}

/* =========================================================
   NAVBAR
========================================================= */

.navbar {
    position: sticky;
    top: 0;
    z-index: 1000;

    background: rgba(255,255,255,0.95);
    backdrop-filter: blur(10px);

    border-bottom: 1px solid var(--border);
}

.nav-inner {
    height: 72px;

    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    font-size: 20px;
    font-weight: 800;
    letter-spacing: -0.5px;
}

.nav-links {
    display: flex;
    gap: 28px;
    list-style: none;
}

.nav-links a {
    font-size: 14px;
    color: #555;
    transition: 0.2s;
}

.nav-links a:hover {
    color: #000;
}

.menu-button {
    display: none;
    border: 0;
    background: none;
    font-size: 25px;
    cursor: pointer;
}

/* =========================================================
   HERO
========================================================= */

.hero {
    padding: 110px 0 90px;
    border-bottom: 1px solid var(--border);
}

.hero-grid {
    display: grid;
    grid-template-columns: 1.4fr 0.6fr;
    gap: 80px;
    align-items: end;
}

.eyebrow {
    font-size: 13px;
    text-transform: uppercase;
    letter-spacing: 2px;
    color: var(--gray);
    margin-bottom: 20px;
}

.hero h1 {
    font-size: clamp(46px, 7vw, 82px);
    line-height: 0.98;
    letter-spacing: -4px;
    margin-bottom: 30px;
    max-width: 850px;
}

.hero h1 span {
    color: #777;
}

.hero-description {
    max-width: 680px;
    font-size: 19px;
    color: #555;
}

.hero-buttons {
    display: flex;
    gap: 12px;
    margin-top: 32px;
    flex-wrap: wrap;
}

.btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;

    padding: 13px 20px;

    border: 1px solid #111;
    font-size: 14px;

    transition: 0.2s;
}

.btn-primary {
    background: #111;
    color: white;
}

.btn-primary:hover {
    background: white;
    color: #111;
}

.btn-secondary:hover {
    background: #111;
    color: white;
}

.hero-meta {
    border-left: 1px solid #ccc;
    padding-left: 30px;
}

.meta-item {
    margin-bottom: 25px;
}

.meta-number {
    font-size: 30px;
    font-weight: 800;
}

.meta-label {
    color: #666;
    font-size: 14px;
}

/* =========================================================
   SECTIONS
========================================================= */

section {
    padding: 90px 0;
    border-bottom: 1px solid var(--border);
}

.section-header {
    display: grid;
    grid-template-columns: 180px 1fr;
    gap: 50px;
    margin-bottom: 55px;
}

.section-number {
    font-size: 13px;
    color: #777;
    text-transform: uppercase;
    letter-spacing: 1.5px;
}

.section-title {
    font-size: 42px;
    letter-spacing: -2px;
    line-height: 1.1;
}

.section-intro {
    margin-top: 15px;
    color: #666;
    max-width: 700px;
}

/* =========================================================
   ABOUT
========================================================= */

.about-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 70px;
}

.about-text {
    font-size: 18px;
    color: #444;
}

.about-text p {
    margin-bottom: 20px;
}

.about-facts {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1px;
    background: var(--border);
    border: 1px solid var(--border);
}

.fact {
    background: white;
    padding: 25px;
}

.fact strong {
    display: block;
    margin-bottom: 7px;
}

.fact span {
    font-size: 14px;
    color: #666;
}

/* =========================================================
   PROJECTS
========================================================= */

.projects {
    display: flex;
    flex-direction: column;
    gap: 25px;
}

.project {
    border: 1px solid var(--border);
    padding: 35px;

    display: grid;
    grid-template-columns: 70px 1fr;
    gap: 25px;

    transition: 0.25s;
}

.project:hover {
    border-color: #111;
    transform: translateY(-2px);
}

.project-number {
    font-size: 14px;
    color: #888;
}

.project h3 {
    font-size: 28px;
    letter-spacing: -1px;
    margin-bottom: 10px;
}

.project-type {
    font-size: 13px;
    text-transform: uppercase;
    letter-spacing: 1px;
    color: #777;
    margin-bottom: 18px;
}

.project p {
    color: #555;
    max-width: 780px;
}

.tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-top: 22px;
}

.tag {
    border: 1px solid #ccc;
    padding: 6px 10px;
    font-size: 12px;
}

/* =========================================================
   SKILLS
========================================================= */

.skills-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1px;
    background: var(--border);
    border: 1px solid var(--border);
}

.skill {
    background: white;
    padding: 30px;
    min-height: 180px;
}

.skill h3 {
    font-size: 18px;
    margin-bottom: 15px;
}

.skill p {
    color: #666;
    font-size: 14px;
}

/* =========================================================
   EXPERIENCE
========================================================= */

.timeline {
    border-left: 1px solid #ccc;
    margin-left: 8px;
}

.experience {
    position: relative;
    padding: 0 0 50px 40px;
}

.experience:last-child {
    padding-bottom: 0;
}

.experience::before {
    content: "";
    width: 9px;
    height: 9px;

    position: absolute;
    left: -5px;
    top: 7px;

    background: #111;
    border-radius: 50%;
}

.experience-date {
    font-size: 13px;
    color: #777;
    margin-bottom: 8px;
}

.experience h3 {
    font-size: 23px;
    margin-bottom: 4px;
}

.experience-company {
    color: #666;
    margin-bottom: 12px;
}

.experience p {
    max-width: 720px;
    color: #555;
}

/* =========================================================
   EDUCATION
========================================================= */

.education {
    display: grid;
    grid-template-columns: 150px 1fr;
    gap: 35px;

    padding: 25px 0;

    border-top: 1px solid var(--border);
}

.education:last-child {
    border-bottom: 1px solid var(--border);
}

.education-date {
    color: #777;
    font-size: 14px;
}

.education h3 {
    font-size: 20px;
}

.education p {
    color: #666;
    margin-top: 5px;
}

/* =========================================================
   LANGUAGES
========================================================= */

.languages {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 15px;
}

.language {
    padding: 25px;
    border: 1px solid var(--border);
}

.language strong {
    display: block;
    margin-bottom: 5px;
}

.language span {
    color: #777;
    font-size: 14px;
}

/* =========================================================
   CONTACT
========================================================= */

.contact {
    padding: 100px 0;
    text-align: center;
}

.contact h2 {
    font-size: clamp(40px, 7vw, 76px);
    letter-spacing: -3px;
    line-height: 1;
    margin-bottom: 25px;
}

.contact p {
    color: #666;
    margin-bottom: 35px;
}

.contact-links {
    display: flex;
    justify-content: center;
    gap: 12px;
    flex-wrap: wrap;
}

/* =========================================================
   FOOTER
========================================================= */

footer {
    padding: 30px 0;
    color: #777;
    font-size: 13px;
}

.footer-inner {
    display: flex;
    justify-content: space-between;
    gap: 20px;
}

/* =========================================================
   DARK MODE
========================================================= */

body.dark {
    background: #111;
    color: #eee;
}

body.dark .navbar {
    background: rgba(17,17,17,0.95);
    border-color: #333;
}

body.dark .nav-links a,
body.dark .hero-description,
body.dark .meta-label,
body.dark .section-intro,
body.dark .about-text,
body.dark .fact span,
body.dark .project p,
body.dark .skill p,
body.dark .experience-date,
body.dark .experience-company,
body.dark .experience p,
body.dark .education-date,
body.dark .education p,
body.dark .language span,
body.dark .contact p,
body.dark footer {
    color: #aaa;
}

body.dark .hero,
body.dark section {
    border-color: #333;
}

body.dark .btn {
    border-color: #eee;
}

body.dark .btn-primary {
    background: #eee;
    color: #111;
}

body.dark .btn-primary:hover {
    background: #111;
    color: #eee;
}

body.dark .btn-secondary:hover {
    background: #eee;
    color: #111;
}

body.dark .hero-meta {
    border-color: #444;
}

body.dark .about-facts,
body.dark .skills-grid {
    background: #333;
    border-color: #333;
}

body.dark .fact,
body.dark .skill {
    background: #111;
}

body.dark .project,
body.dark .education,
body.dark .language {
    border-color: #333;
}

body.dark .project:hover {
    border-color: #eee;
}

body.dark .tag {
    border-color: #444;
}

body.dark .timeline {
    border-color: #444;
}

body.dark .experience::before {
    background: #eee;
}

/* =========================================================
   MOBILE
========================================================= */

@media (max-width: 800px) {

    .nav-links {
        position: absolute;
        top: 72px;
        left: 0;
        right: 0;

        display: none;
        flex-direction: column;

        padding: 25px;

        background: white;
        border-bottom: 1px solid #ddd;
    }

    body.dark .nav-links {
        background: #111;
        border-color: #333;
    }

    .nav-links.active {
        display: flex;
    }

    .menu-button {
        display: block;
    }

    .hero {
        padding: 75px 0;
    }

    .hero-grid {
        grid-template-columns: 1fr;
        gap: 45px;
    }

    .hero h1 {
        font-size: 54px;
        letter-spacing: -3px;
    }

    .hero-meta {
        border-left: none;
        border-top: 1px solid #ccc;
        padding: 25px 0 0;
    }

    .section-header {
        grid-template-columns: 1fr;
        gap: 15px;
    }

    .section-title {
        font-size: 36px;
    }

    .about-grid {
        grid-template-columns: 1fr;
        gap: 40px;
    }

    .skills-grid {
        grid-template-columns: 1fr;
    }

    .languages {
        grid-template-columns: 1fr 1fr;
    }

    .education {
        grid-template-columns: 1fr;
        gap: 8px;
    }

    .project {
        grid-template-columns: 1fr;
        gap: 12px;
    }

    .footer-inner {
        flex-direction: column;
    }
}

</style>
</head>

<body>

<!-- =====================================================
     NAVIGATION
===================================================== -->

<header class="navbar">

<div class="container nav-inner">

<a href="#" class="logo">Amadou Ba</a>

<nav>
<ul class="nav-links" id="navLinks">

<li><a href="#about">À propos</a></li>
<li><a href="#projects">Travaux</a></li>
<li><a href="#skills">Compétences</a></li>
<li><a href="#experience">Expérience</a></li>
<li><a href="#education">Formation</a></li>
<li><a href="#contact">Contact</a></li>

</ul>
</nav>

<button class="menu-button" id="menuButton">
☰
</button>

</div>

</header>


<!-- =====================================================
     HERO
===================================================== -->

<main>

<section class="hero">

<div class="container hero-grid">

<div>

<div class="eyebrow">
Économiste · Analyse quantitative · Données
</div>

<h1>
Je transforme les données économiques en
<span>analyses utiles.</span>
</h1>

<p class="hero-description">

Je suis <strong>Amadou Ba</strong>, titulaire d’un
Master 2 en Analyse économique et quantitative.
Je m’intéresse à l’analyse économique, à
l’économétrie, aux politiques publiques et
à l’exploitation des données pour éclairer
la prise de décision.

</p>

<div class="hero-buttons">

<a href="#projects" class="btn btn-primary">
Voir mes travaux →
</a>

<a href="mailto:amadouba211019@gmail.com"
   class="btn btn-secondary">
Me contacter
</a>

</div>

</div>


<div class="hero-meta">

<div class="meta-item">

<div class="meta-number">M2</div>

<div class="meta-label">
Analyse économique et quantitative
</div>

</div>


<div class="meta-item">

<div class="meta-number">UGB</div>

<div class="meta-label">
Université Gaston Berger
</div>

</div>


<div class="meta-item">

<div class="meta-number">Sénégal</div>

<div class="meta-label">
Tivaouane
</div>

</div>

</div>

</div>

</section>


<!-- =====================================================
     ABOUT
===================================================== -->

<section id="about">

<div class="container">

<div class="section-header">

<div class="section-number">
01 — À propos
</div>

<div>

<h2 class="section-title">
Économie, données et décision.
</h2>

<p class="section-intro">
Une approche orientée vers l’analyse quantitative,
la compréhension des phénomènes économiques
et la production d’informations utiles à la décision.
</p>

</div>

</div>


<div class="about-grid">

<div class="about-text">

<p>
Mon parcours est centré sur l’économie appliquée
et l’analyse quantitative. Ma formation m’a permis
de développer des compétences en traitement,
analyse et interprétation des données économiques.
</p>

<p>
Je m’intéresse particulièrement aux questions
de dette publique, de croissance économique,
de finances publiques, de politiques économiques
et de développement.
</p>

<p>
Je souhaite mettre ces compétences au service
d’organisations qui utilisent les données et
l’analyse économique pour prendre de meilleures
décisions.
</p>

</div>


<div class="about-facts">

<div class="fact">

<strong>Formation</strong>

<span>
Master 2 Analyse économique et quantitative
</span>

</div>


<div class="fact">

<strong>Domaine</strong>

<span>
Économie appliquée
</span>

</div>


<div class="fact">

<strong>Économétrie</strong>

<span>
Stata · R · EViews · Scilab
</span>

</div>


<div class="fact">

<strong>Données</strong>

<span>
Excel · Analyse quantitative
</span>

</div>

</div>

</div>

</div>

</section>


<!-- =====================================================
     PROJECTS
===================================================== -->

<section id="projects">

<div class="container">

<div class="section-header">

<div class="section-number">
02 — Travaux
</div>

<div>

<h2 class="section-title">
Travaux & recherches
</h2>

<p class="section-intro">
Quelques axes de travail autour de l’économie,
de l’économétrie et de l’analyse des politiques publiques.
</p>

</div>

</div>


<div class="projects">


<!-- PROJECT 01 -->

<article class="project">

<div class="project-number">
01
</div>

<div>

<div class="project-type">
Mémoire · Économétrie
</div>

<h3>
Efficacité de l’endettement du Sénégal
</h3>

<p>

Analyse économétrique de la relation entre
l’endettement public et les performances
économiques du Sénégal. Étude de la dynamique
de la dette et de ses effets sur la croissance
à travers des modèles économétriques.

</p>

<div class="tags">

<span class="tag">Économie</span>
<span class="tag">Dette publique</span>
<span class="tag">Économétrie</span>
<span class="tag">Stata</span>
<span class="tag">ARDL</span>

</div>

</div>

</article>


<!-- PROJECT 02 -->

<article class="project">

<div class="project-number">
02
</div>

<div>

<div class="project-type">
Analyse économique
</div>

<h3>
Dette publique & croissance
</h3>

<p>

Analyse de la relation entre la dette publique,
l’investissement, l’ouverture commerciale,
l’inflation et la croissance économique.

</p>

<div class="tags">

<span class="tag">Analyse macroéconomique</span>
<span class="tag">Données</span>
<span class="tag">Régression</span>
<span class="tag">Stata</span>

</div>

</div>

</article>


<!-- PROJECT 03 -->

<article class="project">

<div class="project-number">
03
</div>

<div>

<div class="project-type">
Suivi · Évaluation
</div>

<h3>
Analyse et suivi de projets
</h3>

<p>

Intérêt professionnel pour le suivi-évaluation,
la gestion de projets, l'analyse des indicateurs
et l'utilisation des données pour mesurer les
résultats des interventions.

</p>

<div class="tags">

<span class="tag">Suivi-évaluation</span>
<span class="tag">Gestion de projet</span>
<span class="tag">Indicateurs</span>
<span class="tag">Excel</span>

</div>

</div>

</article>

</div>

</div>

</section>


<!-- =====================================================
     SKILLS
===================================================== -->

<section id="skills">

<div class="container">

<div class="section-header">

<div class="section-number">
03 — Compétences
</div>

<div>

<h2 class="section-title">
Ce que je peux apporter.
</h2>

<p class="section-intro">
Des compétences quantitatives combinées à une
formation en économie appliquée.
</p>

</div>

</div>


<div class="skills-grid">

<div class="skill">

<h3>Analyse économique</h3>

<p>
Analyse macroéconomique, économie appliquée,
finances publiques et analyse des politiques
économiques.
</p>

</div>


<div class="skill">

<h3>Économétrie & données</h3>

<p>
R, Stata, EViews, Scilab et Excel pour
le traitement, l'analyse et l'interprétation
des données.
</p>

</div>


<div class="skill">

<h3>Gestion de projet</h3>

<p>
Gestion, évaluation et suivi-évaluation
de projets et appui à la prise de décision.
</p>

</div>


<div class="skill">

<h3>Analyse quantitative</h3>

<p>
Modélisation, analyse statistique et
interprétation des résultats économétriques.
</p>

</div>


<div class="skill">

<h3>Bureautique</h3>

<p>
Microsoft Word et Excel pour la production
de rapports et le traitement des données.
</p>

</div>


<div class="skill">

<h3>Communication</h3>

<p>
Français courant, Wolof, Puular courant
et anglais de bon niveau.
</p>

</div>

</div>

</div>

</section>


<!-- =====================================================
     EXPERIENCE
===================================================== -->

<section id="experience">

<div class="container">

<div class="section-header">

<div class="section-number">
04 — Expérience
</div>

<div>

<h2 class="section-title">
Expérience professionnelle
</h2>

<p class="section-intro">
Des expériences combinant gestion financière,
communication et engagement associatif.
</p>

</div>

</div>


<div class="timeline">


<div class="experience">

<div class="experience-date">
2023 — 2024
</div>

<h3>
Comptable
</h3>

<div class="experience-company">
Tivaouane Basket Club · Tivaouane
</div>

<p>
Suivi des dépenses et recettes du club.
Élaboration de bilans financiers et de
rapports budgétaires. Appui à la prise
de décision financière.
</p>

</div>


<div class="experience">

<div class="experience-date">
2023 — 2024
</div>

<h3>
Community Manager
</h3>

<div class="experience-company">
Tivaouane Basket Club · Tivaouane
</div>

<p>
Gestion et animation des réseaux sociaux
du club. Promotion des activités sportives,
amélioration de la visibilité et contribution
à la mobilisation des supporters et partenaires.
</p>

</div>


<div class="experience">

<div class="experience-date">
2020 — 2022
</div>

<h3>
Vice-président
</h3>

<div class="experience-company">
Association And Defar Ndoutt · Tivaouane
</div>

<p>
Coordination d’activités communautaires
et sociales. Participation à la gestion
de projets locaux et actions de solidarité
en faveur des populations vulnérables.
</p>

</div>


</div>

</div>

</section>


<!-- =====================================================
     EDUCATION
===================================================== -->

<section id="education">

<div class="container">

<div class="section-header">

<div class="section-number">
05 — Formation
</div>

<div>

<h2 class="section-title">
Parcours académique
</h2>

</div>

</div>


<div class="education">

<div class="education-date">
2024 — 2025
</div>

<div>

<h3>
Master 2 — Analyse économique et quantitative
</h3>

<p>
Université Gaston Berger · Saint-Louis
</p>

</div>

</div>


<div class="education">

<div class="education-date">
2022 — 2023
</div>

<div>

<h3>
Licence en Économie Appliquée
</h3>

<p>
Université Gaston Berger · Saint-Louis
</p>

</div>

</div>


<div class="education">

<div class="education-date">
2019 — 2020
</div>

<div>

<h3>
Baccalauréat
</h3>

<p>
Groupe scolaire Abdou Aziz Dabakh · Tivaouane
</p>

</div>

</div>


<div class="education">

<div class="education-date">
2015 — 2016
</div>

<div>

<h3>
Brevet de fin d’études moyennes — BFEM
</h3>

<p>
CEM Habib Sy · Tivaouane
</p>

</div>

</div>

</div>

</section>


<!-- =====================================================
     LANGUAGES
===================================================== -->

<section>

<div class="container">

<div class="section-header">

<div class="section-number">
06 — Langues
</div>

<div>

<h2 class="section-title">
Communication
</h2>

</div>

</div>


<div class="languages">

<div class="language">
<strong>Français</strong>
<span>Courant</span>
</div>

<div class="language">
<strong>Wolof</strong>
<span>Courant</span>
</div>

<div class="language">
<strong>Puular</strong>
<span>Courant</span>
</div>

<div class="language">
<strong>Anglais</strong>
<span>Bon niveau</span>
</div>

</div>

</div>

</section>


<!-- =====================================================
     CONTACT
===================================================== -->

<section id="contact" class="contact">

<div class="container">

<div class="eyebrow">
07 — Contact
</div>

<h2>
Construisons quelque chose d’utile.
</h2>

<p>
Vous recherchez un économiste pour une étude,
une analyse de données, un projet ou une mission
de suivi-évaluation ?
</p>

<div class="contact-links">

<a href="mailto:amadouba211019@gmail.com"
   class="btn btn-primary">
amadouba211019@gmail.com
</a>

<a href="tel:+221772503248"
   class="btn btn-secondary">
+221 77 250 32 48
</a>

</div>

</div>

</section>

</main>


<!-- =====================================================
     FOOTER
===================================================== -->

<footer>

<div class="container footer-inner">

<div>
© <span id="year"></span> Amadou Ba
</div>

<div>
Économiste · Sénégal
</div>

</div>

</footer>


<!-- =====================================================
     JAVASCRIPT
===================================================== -->

<script>

/* Année automatique */

document.getElementById("year").textContent =
    new Date().getFullYear();


/* Menu mobile */

const menuButton =
    document.getElementById("menuButton");

const navLinks =
    document.getElementById("navLinks");

menuButton.addEventListener("click", () => {

    navLinks.classList.toggle("active");

});


/* Fermer le menu après clic */

document.querySelectorAll(".nav-links a").forEach(link => {

    link.addEventListener("click", () => {

        navLinks.classList.remove("active");

    });

});


/* Mode sombre */

const darkButton = document.createElement("button");

darkButton.innerHTML = "◐";

darkButton.title = "Changer le thème";

darkButton.style.cssText = `
    border: 0;
    background: none;
    cursor: pointer;
    font-size: 20px;
    margin-left: 20px;
`;

document.querySelector(".nav-inner").appendChild(darkButton);

darkButton.addEventListener("click", () => {

    document.body.classList.toggle("dark");

    localStorage.setItem(
        "darkMode",
        document.body.classList.contains("dark")
    );

});


/* Restaurer le thème */

if (localStorage.getItem("darkMode") === "true") {

    document.body.classList.add("dark");

}

</script>

</body>
</html>
