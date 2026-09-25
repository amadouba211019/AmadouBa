
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

 <img src="photo.jpg" alt="Amadou Ba — Économiste">

<meta name="description" content="Portfolio d'Amadou Ba — Économie appliquée, économétrie et analyse de données.">

<!-- POLICES -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Manrope:wght@600;700;800&display=swap" rel="stylesheet">

<!-- ICONES -->
<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">

<style>

/* =====================================================
   VARIABLES
===================================================== */

:root{
    --black:#111111;
    --dark:#1b1b1b;
    --white:#ffffff;
    --cream:#f5f2ec;
    --cream-dark:#e9e5dc;
    --gray:#666666;
    --border:#d8d4cc;
}


/* =====================================================
   RESET
===================================================== */

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
    scroll-padding-top:90px;
}

body{
    font-family:"DM Sans",sans-serif;
    background:var(--cream);
    color:var(--black);
    line-height:1.6;
}

a{
    text-decoration:none;
    color:inherit;
}

img{
    max-width:100%;
}

.container{
    width:min(1180px,90%);
    margin:auto;
}


/* =====================================================
   NAVIGATION
===================================================== */

nav{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:1000;

    background:rgba(245,242,236,.94);
    backdrop-filter:blur(14px);

    border-bottom:1px solid rgba(0,0,0,.08);
}

.nav-inner{
    height:78px;

    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    font-family:"Manrope",sans-serif;
    font-size:21px;
    font-weight:800;
    letter-spacing:-1px;
}

.logo span{
    font-weight:400;
}

.nav-links{
    display:flex;
    align-items:center;
    gap:30px;
    list-style:none;
}

.nav-links a{
    font-size:14px;
    font-weight:600;
    transition:.3s;
}

.nav-links a:hover{
    opacity:.5;
}


/* =====================================================
   HERO
===================================================== */

.hero{
    min-height:100vh;

    display:flex;
    align-items:center;

    padding:150px 0 100px;
}

.hero-grid{
    display:grid;
    grid-template-columns:1.4fr .6fr;
    gap:80px;
}

.eyebrow{
    font-size:12px;
    font-weight:700;
    letter-spacing:2px;
    text-transform:uppercase;

    margin-bottom:30px;
}

.hero h1{
    font-family:"Manrope",sans-serif;

    font-size:clamp(50px,7vw,95px);
    line-height:.95;

    letter-spacing:-6px;
}

.hero h1 span{
    display:block;
}

.hero-text{
    max-width:700px;

    margin-top:35px;

    font-size:20px;
    color:#444;
}

.hero-description{
    max-width:680px;

    margin-top:18px;

    color:#555;
}

.btn{
    display:inline-flex;
    align-items:center;
    gap:12px;

    margin-top:35px;

    padding:15px 22px;

    background:var(--black);
    color:white;

    font-size:14px;
    font-weight:700;

    transition:.3s;
}

.btn:hover{
    background:#333;
    transform:translateY(-3px);
}


/* =====================================================
   RESULTS
===================================================== */

.stats{
    border-top:1px solid var(--border);
    border-bottom:1px solid var(--border);
}

.stats-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
}

.stat{
    padding:35px 25px;

    border-right:1px solid var(--border);
}

.stat:last-child{
    border-right:none;
}

.stat-number{
    font-family:"Manrope",sans-serif;
    font-size:23px;
    font-weight:800;

    margin-bottom:7px;
}

.stat-title{
    font-weight:700;
}

.stat p{
    color:var(--gray);
    font-size:14px;
}


/* =====================================================
   SECTIONS
===================================================== */

section{
    padding:120px 0;
}

.section-header{
    display:flex;
    justify-content:space-between;
    align-items:flex-start;

    margin-bottom:70px;
}

.section-number{
    font-size:12px;
    font-weight:700;
    letter-spacing:2px;
}

.section-title{
    font-family:"Manrope",sans-serif;

    font-size:clamp(42px,5vw,70px);

    line-height:1;
    letter-spacing:-4px;
}


/* =====================================================
   ABOUT
===================================================== */

.about-grid{
    display:grid;
    grid-template-columns:.7fr 1.3fr;
    gap:100px;
}

.about-label{
    font-size:12px;
    font-weight:700;
    letter-spacing:2px;
    text-transform:uppercase;
}

.about-text{
    max-width:760px;

    font-size:20px;
}

.about-text p{
    margin-bottom:24px;
}

.skills{
    display:flex;
    flex-wrap:wrap;
    gap:9px;

    margin-top:35px;
}

.skill{
    padding:8px 13px;

    border:1px solid var(--border);

    background:#faf8f4;

    font-size:13px;
}


/* =====================================================
   TRAVAUX
===================================================== */

.projects{
    border-top:1px solid var(--border);
}

.project{
    display:grid;
    grid-template-columns:100px 1fr 60px;

    gap:30px;

    padding:45px 0;

    border-top:1px solid var(--border);

    transition:.3s;
}

.project:last-child{
    border-bottom:1px solid var(--border);
}

.project:hover{
    padding-left:12px;
}

.project-number{
    font-family:"Manrope",sans-serif;
    font-size:18px;
    font-weight:800;
}

.project-category{
    margin-bottom:14px;

    font-size:12px;
    font-weight:700;

    letter-spacing:1px;
    text-transform:uppercase;
}

.project h3{
    font-family:"Manrope",sans-serif;

    font-size:31px;
    line-height:1.2;

    letter-spacing:-1px;

    margin-bottom:18px;
}

.project-description{
    max-width:720px;

    color:#555;

    margin-bottom:12px;
}

.tags{
    display:flex;
    flex-wrap:wrap;
    gap:8px;

    margin-top:20px;
}

.tag{
    padding:6px 9px;

    border:1px solid var(--border);

    font-size:12px;
}

.project-arrow{
    font-size:28px;

    transition:.3s;
}

.project:hover .project-arrow{
    transform:translate(5px,-5px);
}


/* =====================================================
   LABS
===================================================== */

.labs{
    background:var(--black);
    color:white;
}

.labs .section-title{
    color:white;
}

.labs-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);

    gap:1px;

    background:#333;
}

.lab{
    min-height:310px;

    padding:45px;

    background:var(--black);
}

.lab-number{
    font-size:12px;
    opacity:.5;
}

.lab h3{
    font-family:"Manrope",sans-serif;

    font-size:27px;

    margin:40px 0 18px;
}

.lab p{
    color:#aaa;
}

.lab .tag{
    border-color:#444;
    color:#bbb;
}


/* =====================================================
   FORMATION
===================================================== */

.education{
    border-top:1px solid var(--border);
}

.education-list{
    border-top:1px solid var(--border);
}

.education-item{
    display:grid;
    grid-template-columns:170px 1fr 180px;

    gap:40px;

    padding:35px 0;

    border-bottom:1px solid var(--border);
}

.education-date{
    font-size:14px;
    color:var(--gray);
}

.education h3{
    font-family:"Manrope",sans-serif;

    font-size:24px;

    margin-bottom:5px;
}

.education p{
    color:#555;
}

.education-place{
    text-align:right;

    font-size:14px;
    color:var(--gray);
}


/* =====================================================
   EXPERIENCE
===================================================== */

.experience{
    border-top:1px solid var(--border);
}

.experience-item{
    display:grid;
    grid-template-columns:190px 1fr 120px;

    gap:40px;

    padding:40px 0;

    border-top:1px solid var(--border);
}

.experience-item:last-child{
    border-bottom:1px solid var(--border);
}

.experience-company{
    font-weight:700;
}

.experience h3{
    font-family:"Manrope",sans-serif;

    font-size:25px;

    margin-bottom:10px;
}

.experience p{
    max-width:680px;
    color:#555;
}

.experience-date{
    text-align:right;
    color:var(--gray);
    font-size:14px;
}


/* =====================================================
   ANALYSES
===================================================== */

.analysis-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);

    gap:20px;
}

.analysis-card{
    padding:40px;

    border:1px solid var(--border);

    transition:.3s;
}

.analysis-card:hover{
    background:white;
    transform:translateY(-5px);
}

.analysis-card h3{
    font-family:"Manrope",sans-serif;

    font-size:27px;

    margin-bottom:12px;
}


/* =====================================================
   CONTACT
===================================================== */

.contact{
    background:var(--cream-dark);
}

.contact-grid{
    display:grid;
    grid-template-columns:1fr 1fr;

    gap:80px;
}

.contact h2{
    font-family:"Manrope",sans-serif;

    font-size:clamp(43px,5vw,70px);

    line-height:1;

    letter-spacing:-4px;
}

.contact-text{
    max-width:600px;

    margin-top:25px;

    color:#555;

    font-size:18px;
}

.contact-info{
    display:flex;
    flex-direction:column;
    justify-content:center;
}

.contact-link{
    padding:18px 0;

    border-bottom:1px solid #aaa;

    font-family:"Manrope",sans-serif;

    font-size:22px;
    font-weight:700;

    transition:.3s;
}

.contact-link:hover{
    padding-left:10px;
}


/* =====================================================
   RESEAUX SOCIAUX
===================================================== */

.social-title{
    margin-top:50px;

    font-size:12px;
    font-weight:700;

    text-transform:uppercase;
    letter-spacing:2px;
}

.socials{
    display:flex;
    gap:12px;

    margin-top:20px;
}

.social{
    width:50px;
    height:50px;

    display:flex;
    align-items:center;
    justify-content:center;

    border:1px solid #aaa;

    font-size:20px;

    transition:.3s;
}

.social:hover{
    background:var(--black);
    color:white;
    border-color:var(--black);

    transform:translateY(-4px);
}


/* =====================================================
   FOOTER
===================================================== */

footer{
    background:var(--black);
    color:white;

    padding:35px 0;
}

.footer-inner{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.footer-logo{
    font-family:"Manrope",sans-serif;
    font-weight:800;
}

footer p{
    color:#aaa;
    font-size:13px;
}


/* =====================================================
   MOBILE
===================================================== */

@media(max-width:900px){

    .nav-links{
        display:none;
    }

    .hero-grid,
    .about-grid,
    .contact-grid{
        grid-template-columns:1fr;
        gap:45px;
    }

    .stats-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .stat:nth-child(2){
        border-right:none;
    }

    .stat:nth-child(3),
    .stat:nth-child(4){
        border-top:1px solid var(--border);
    }

    .labs-grid{
        grid-template-columns:1fr;
    }

    .education-item{
        grid-template-columns:1fr;
        gap:8px;
    }

    .education-place{
        text-align:left;
    }

    .experience-item{
        grid-template-columns:1fr;
        gap:10px;
    }

    .experience-date{
        text-align:left;
    }

    .analysis-grid{
        grid-template-columns:1fr;
    }
}


@media(max-width:600px){

    section{
        padding:80px 0;
    }

    .hero{
        padding-top:130px;
    }

    .hero h1{
        font-size:49px;
        letter-spacing:-3px;
    }

    .hero-text{
        font-size:17px;
    }

    .stats-grid{
        grid-template-columns:1fr;
    }

    .stat{
        border-right:none !important;
        border-top:1px solid var(--border);
    }

    .stat:first-child{
        border-top:none;
    }

    .section-header{
        margin-bottom:45px;
    }

    .project{
        grid-template-columns:45px 1fr;
        gap:15px;
    }

    .project-arrow{
        display:none;
    }

    .project h3{
        font-size:25px;
    }

    .about-text{
        font-size:18px;
    }

    .contact h2{
        font-size:45px;
    }

    .contact-link{
        font-size:18px;
    }

    .footer-inner{
        flex-direction:column;
        align-items:flex-start;
        gap:10px;
    }

}

</style>
</head>


<body>


<!-- =====================================================
     NAVIGATION
===================================================== -->

<nav>

<div class="container nav-inner">

<a href="#accueil" class="logo">
AMADOU <span>BA</span>
</a>

<ul class="nav-links">

<li>
<a href="#about">À propos</a>
</li>

<li>
<a href="#travaux">Travaux</a>
</li>

<li>
<a href="#labs">Labs</a>
</li>

<li>
<a href="#formation">Formation</a>
</li>

<li>
<a href="#experience">Expérience</a>
</li>

<li>
<a href="#contact">Contact</a>
</li>

</ul>

</div>

</nav>



<!-- =====================================================
     HERO
===================================================== -->

<header class="hero" id="accueil">

<div class="container hero-grid">

<div>

<div class="eyebrow">
ÉCONOMIE APPLIQUÉE · ÉCONOMÉTRIE · ANALYSE DE DONNÉES
</div>

<h1>
Économie.
<span>Données.</span>
Décision.
</h1>

<p class="hero-text">
J’analyse les données économiques, construis des modèles
économétriques et transforme les résultats en informations utiles.
</p>

<p class="hero-description">

Je suis <strong>Amadou Ba</strong>, titulaire d’un
<strong>Master 2 en Analyse économique et quantitative</strong>
à l’Université Gaston Berger de Saint-Louis.

Je m’intéresse à l’économie appliquée, à l’économétrie,
aux finances publiques et à l’analyse des politiques économiques.

</p>

<a href="#travaux" class="btn">

Voir mes travaux

<i class="fa-solid fa-arrow-down"></i>

</a>

</div>

</div>

</header>



<!-- =====================================================
     RESULTS
===================================================== -->

<section class="stats">

<div class="container stats-grid">


<div class="stat">

<div class="stat-number">
Master 2
</div>

<div class="stat-title">
Analyse économique et quantitative
</div>

<p>
Université Gaston Berger
</p>

</div>


<div class="stat">

<div class="stat-number">
UGB
</div>

<div class="stat-title">
Université Gaston Berger
</div>

<p>
Saint-Louis, Sénégal
</p>

</div>


<div class="stat">

<div class="stat-number">
Économétrie
</div>

<div class="stat-title">
Outils
</div>

<p>
Stata · R · EViews · Scilab
</p>

</div>


<div class="stat">

<div class="stat-number">
Recherche
</div>

<div class="stat-title">
Mémoire
</div>

<p>
Efficacité de l’endettement du Sénégal
</p>

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
01 / ABOUT
</div>

<h2 class="section-title">
À propos
</h2>

</div>


<div class="about-grid">

<div>

<div class="about-label">
Profil
</div>

</div>


<div class="about-text">

<p>
Mon orientation actuelle est l’analyse économique quantitative,
avec un intérêt particulier pour l’économétrie, les données
macroéconomiques et les politiques publiques.
</p>

<p>
Je travaille avec <strong>Stata, R, EViews, Scilab et Excel</strong>
pour traiter, analyser et interpréter des données économiques.
</p>

<p>
Je m’intéresse notamment à la dette publique, à la croissance,
aux finances publiques et aux questions de développement.
</p>

<p>
Je cherche à transformer les données et les résultats
économétriques en analyses claires et utiles à la décision.
</p>


<div class="skills">

<span class="skill">Stata</span>
<span class="skill">R</span>
<span class="skill">EViews</span>
<span class="skill">Scilab</span>
<span class="skill">Excel</span>
<span class="skill">Économétrie</span>
<span class="skill">Analyse de données</span>
<span class="skill">Séries temporelles</span>

</div>

</div>

</div>

</div>

</section>



<!-- =====================================================
     TRAVAUX
===================================================== -->

<section class="projects" id="travaux">

<div class="container">

<div class="section-header">

<div class="section-number">
02 / SELECTED WORK
</div>

<h2 class="section-title">
Travaux
</h2>

</div>



<!-- TRAVAIL 01 -->

<article class="project">

<div class="project-number">
01
</div>

<div>

<div class="project-category">
Recherche économique · Économétrie
</div>

<h3>
L’impact de la dette publique sur l’investissement
</h3>

<p class="project-description">

Étude économétrique consacrée à l’analyse de l’impact
de la dette publique sur l’investissement au Sénégal.

</p>

<p class="project-description">

L’objectif est d’examiner la relation entre l’endettement
public et l’investissement à partir de données
macroéconomiques, en mobilisant des outils d’analyse
économétrique et de séries temporelles.

</p>

<div class="tags">

<span class="tag">Stata</span>
<span class="tag">Économétrie</span>
<span class="tag">Séries temporelles</span>
<span class="tag">Dette publique</span>
<span class="tag">Investissement</span>

</div>

</div>

<div class="project-arrow">
↗
</div>

</article>



<!-- TRAVAIL 02 -->

<article class="project">

<div class="project-number">
02
</div>

<div>

<div class="project-category">
Analyse économique · Recherche
</div>

<h3>
Dette publique & croissance économique
</h3>

<p class="project-description">

Une analyse de la relation entre l’endettement public,
la croissance économique, l’investissement et plusieurs
variables macroéconomiques.

</p>

<div class="tags">

<span class="tag">Stata</span>
<span class="tag">Régression</span>
<span class="tag">Données macroéconomiques</span>
<span class="tag">Analyse quantitative</span>

</div>

</div>

<div class="project-arrow">
↗
</div>

</article>



<!-- TRAVAIL 03 -->

<article class="project">

<div class="project-number">
03
</div>

<div>

<div class="project-category">
Gestion · Suivi-évaluation
</div>

<h3>
Suivi & évaluation de projets
</h3>

<p class="project-description">

Travaux et intérêt professionnel autour du suivi,
de l’évaluation et de la gestion de projets,
avec une approche orientée vers les données
et les indicateurs de résultats.

</p>

<div class="tags">

<span class="tag">Gestion de projet</span>
<span class="tag">Suivi-évaluation</span>
<span class="tag">Excel</span>
<span class="tag">Analyse</span>

</div>

</div>

<div class="project-arrow">
↗
</div>

</article>


</div>

</section>



<!-- =====================================================
     LABS
===================================================== -->

<section class="labs" id="labs">

<div class="container">

<div class="section-header">

<div class="section-number">
03 / LABS & ANALYSES
</div>

<h2 class="section-title">
Labs
</h2>

</div>


<div class="labs-grid">


<div class="lab">

<div class="lab-number">
01
</div>

<h3>
Dette publique du Sénégal
</h3>

<p>
Analyses et visualisations autour de l'évolution de
la dette publique, du déficit et de leurs implications
pour les finances publiques.
</p>

<div class="tags">

<span class="tag">Économie publique</span>
<span class="tag">Données</span>
<span class="tag">Analyse quantitative</span>

</div>

</div>



<div class="lab">

<div class="lab-number">
02
</div>

<h3>
Énergie & finances publiques
</h3>

<p>
Réflexions quantitatives sur les subventions énergétiques,
les dépenses publiques et les mécanismes de financement.
</p>

<div class="tags">

<span class="tag">Économie de l’énergie</span>
<span class="tag">Politiques publiques</span>
<span class="tag">Données</span>

</div>

</div>



<div class="lab">

<div class="lab-number">
03
</div>

<h3>
Économétrie appliquée
</h3>

<p>
Expérimentations et analyses utilisant des modèles
économétriques pour étudier des phénomènes économiques.
</p>

<div class="tags">

<span class="tag">Stata</span>
<span class="tag">R</span>
<span class="tag">EViews</span>
<span class="tag">Séries temporelles</span>

</div>

</div>


</div>

</div>

</section>



<!-- =====================================================
     FORMATION
===================================================== -->

<section class="education" id="formation">

<div class="container">

<div class="section-header">

<div class="section-number">
04 / EDUCATION
</div>

<h2 class="section-title">
Formation
</h2>

</div>


<div class="education-list">


<!-- MASTER -->

<div class="education-item">

<div class="education-date">
2024 — 2025
</div>

<div>

<h3>
Master 2 — Analyse économique et quantitative
</h3>

<p>
Formation en analyse économique, économétrie,
statistiques et méthodes quantitatives.
</p>

</div>

<div class="education-place">
Université Gaston Berger<br>
Saint-Louis
</div>

</div>



<!-- LICENCE -->

<div class="education-item">

<div class="education-date">
2022 — 2023
</div>

<div>

<h3>
Licence — Économie appliquée
</h3>

<p>
Formation en économie appliquée et analyse économique.
</p>

</div>

<div class="education-place">
Université Gaston Berger<br>
Saint-Louis
</div>

</div>



<!-- BAC -->

<div class="education-item">

<div class="education-date">
Baccalauréat
</div>

<div>

<h3>
Baccalauréat
</h3>

<p>
Diplôme de fin d’études secondaires.
</p>

</div>

<div class="education-place">
Sénégal
</div>

</div>


</div>

</div>

</section>



<!-- =====================================================
     ANALYSES
===================================================== -->

<section>

<div class="container">

<div class="section-header">

<div class="section-number">
05 / ANALYSES
</div>

<h2 class="section-title">
Écrits
</h2>

</div>


<div class="analysis-grid">


<div class="analysis-card">

<h3>
Analyses économiques
</h3>

<p>
Dette publique · Croissance · Finances publiques
</p>

</div>


<div class="analysis-card">

<h3>
Recherche
</h3>

<p>
Économétrie · Politiques publiques · Données
</p>

</div>


</div>

</div>

</section>



<!-- =====================================================
     EXPERIENCE
===================================================== -->

<section class="experience" id="experience">

<div class="container">

<div class="section-header">

<div class="section-number">
06 / EXPERIENCE
</div>

<h2 class="section-title">
Expérience
</h2>

</div>



<div class="experience-item">

<div class="experience-company">
Tivaouane Basket Club
</div>

<div>

<h3>
Comptable
</h3>

<p>
Suivi des dépenses et recettes, élaboration de bilans
financiers et de rapports budgétaires, avec appui
à la prise de décision financière.
</p>

</div>

<div class="experience-date">
2023 — 2024
</div>

</div>



<div class="experience-item">

<div class="experience-company">
Tivaouane Basket Club
</div>

<div>

<h3>
Community Manager
</h3>

<p>
Gestion et animation des réseaux sociaux, promotion
des activités sportives et contribution à la mobilisation
des supporters et partenaires.
</p>

</div>

<div class="experience-date">
2023 — 2024
</div>

</div>



<div class="experience-item">

<div class="experience-company">
Association And Defar Ndoutt
</div>

<div>

<h3>
Vice-président
</h3>

<p>
Coordination d’activités communautaires et sociales,
participation à la gestion de projets locaux et actions
de solidarité.
</p>

</div>

<div class="experience-date">
2020 — 2022
</div>

</div>


</div>

</section>



<!-- =====================================================
     CONTACT
===================================================== -->

<section class="contact" id="contact">

<div class="container contact-grid">


<div>

<h2>
Construisons quelque chose d’utile.
</h2>

<p class="contact-text">

Vous avez un projet d’étude, une analyse économique,
une mission de suivi-évaluation ou un projet nécessitant
une approche quantitative ?

</p>


<div class="social-title">
Follow me on
</div>


<div class="socials">


<!-- X -->

<a
href="https://x.com/amadou_at_tijan?s=11"
target="_blank"
rel="noopener noreferrer"
class="social"
aria-label="X"
>

<i class="fa-brands fa-x-twitter"></i>

</a>



<!-- LINKEDIN -->

<a
href="https://www.linkedin.com/in/amadou-ba-037159374/"
target="_blank"
rel="noopener noreferrer"
class="social"
aria-label="LinkedIn"
>

<i class="fa-brands fa-linkedin-in"></i>

</a>



<!-- FACEBOOK -->

<a
href="https://www.facebook.com/share/1Lmk3AGCWk/"
target="_blank"
rel="noopener noreferrer"
class="social"
aria-label="Facebook"
>

<i class="fa-brands fa-facebook-f"></i>

</a>



<!-- INSTAGRAM -->

<a
href="https://www.instagram.com/amadou_at_tijani/"
target="_blank"
rel="noopener noreferrer"
class="social"
aria-label="Instagram"
>

<i class="fa-brands fa-instagram"></i>

</a>


</div>

</div>



<div class="contact-info">

<a
href="mailto:amadouba211019@gmail.com"
class="contact-link"
>

amadouba211019@gmail.com

</a>


<a
href="tel:+221772503248"
class="contact-link"
>

+221 77 250 32 48

</a>

</div>


</div>

</section>



<!-- =====================================================
     FOOTER
===================================================== -->

<footer>

<div class="container footer-inner">

<div class="footer-logo">
AMADOU BA
</div>

<p>
© 2026 Amadou Ba — Économie appliquée & analyse quantitative
</p>

</div>

</footer>


</body>
</html>
