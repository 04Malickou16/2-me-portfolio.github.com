# Portfolio — Malick Kamara (BTS SIO, option SISR)

Portfolio statique en HTML/CSS/JS pur, prêt à être hébergé sur GitHub Pages.

Ce portfolio est conçu pour l'**épreuve E5 — Support et mise à disposition de services
informatiques** (coefficient 4, oral 40 min), conformément au dossier remis par le professeur
(*Dossier élève — Construire son portfolio professionnel, BTS SIO, session 2026-2027*).
Il doit démontrer, à travers des réalisations documentées, les 6 compétences du Bloc 1
(C1 à C6).

## Structure du site

```
index.html          → toute la page, organisée selon les rubriques attendues par le prof :
                       Accueil, Profil, Compétences, Réalisations, Veille, Stage, Formation,
                       Projets, Documentation, Projet professionnel, Contact
css/style.css        → styles
js/script.js         → menu mobile, année du footer, bouton retour en haut
assets/img/          → photo (photo.jpg)
assets/cv/           → CV en PDF (cv-malick.pdf)
```

## Important : la partie que Malick doit remplir lui-même

Les sections **Réalisations** et **Veille** contiennent des fiches *vides*, avec les champs
officiels du dossier (contexte, besoin, difficulté, diagnostic, solution, tests, bilan...).
Ce sont volontairement des modèles à compléter, et non du contenu inventé :

- à l'oral E5, le jury interroge sur le travail *personnellement* réalisé
  (« qu'avez-vous fait ? », « comment avez-vous diagnostiqué le problème ? »...) ;
- Malick doit donc remplir ces fiches lui-même, au fur et à mesure des séances 2, 3, 7 et 8
  du programme (inventaire des réalisations, fiche de réalisation, veille SLAM/SISR,
  transformation de la veille en expérimentation) ;
- une fois une fiche remplie dans `index.html`, pense aussi à cocher les compétences
  correspondantes (C1 à C6) dans le tableau de couverture de la section Compétences.

Pour ajouter une nouvelle fiche : duplique un bloc `<div class="fiche-card">...</div>`
existant dans `index.html` (section Réalisations ou Veille) et remplace les champs.

## À compléter

Marqué `<!-- TODO -->` dans `index.html` :

- **Réalisations** (2 fiches vides) et **Veille** (1 fiche vide) → à remplir avec Malick,
  au fil des séances (voir ci-dessus)
- **Stage de 1ère année** (section "Stage") → nom de l'entreprise, contexte, activités
  réalisées, bilan (dates déjà renseignées : 26 mai — 25 juin 2026)
- **Tableau de couverture des compétences** (section "Compétences") → à cocher une fois les
  fiches de réalisation remplies
- **3 technologies à maîtriser** (section "Profil") → à confirmer/ajuster avec Malick
- **Dépôt Git** (section "Profil") → lien à corriger une fois le dépôt GitHub créé
- **Liens LinkedIn / GitHub** (Contact) → non présents dans le CV
- **CV à jour** → le PDF actuel (`assets/cv/cv-malick.pdf`) date de la 1ère année de BTS
- Tes 3 projets (section "Projets") : titre, description, technos, lien GitHub
- Niveaux de compétences techniques (barres de progression, valeurs en %) → estimations
  à ajuster
- **Compétences à développer** (section "Projet professionnel") → à ajuster selon les
  besoins réels de Malick

## Aperçu en local

Ouvre simplement `index.html` dans ton navigateur, ou lance un petit serveur local :

```bash
python -m http.server 8000
```

puis va sur `http://localhost:8000`.

## Déploiement sur GitHub Pages

1. Crée un dépôt GitHub (ex: `portfolio`).
2. Pousse ce projet dedans :
   ```bash
   git init
   git add .
   git commit -m "Premier commit du portfolio"
   git branch -M main
   git remote add origin https://github.com/TON-PSEUDO/portfolio.git
   git push -u origin main
   ```
3. Sur GitHub : `Settings` → `Pages` → `Source` → sélectionne la branche `main` et le dossier `/ (root)`.
4. Ton site sera disponible à `https://TON-PSEUDO.github.io/portfolio/` après quelques minutes.
5. Mets à jour le lien "Dépôt Git" dans la section Profil du site avec l'URL réelle du dépôt.
