# TP1 - (2026)

COMPLÉTER ET ADAPTER CE README

Ceci est ma solution pour le TP1. Ce défi m'a permis de concevoir un ou plusieurs composants d'interface moderne, performant et pleinement accessible, sans dépendre de frameworks ou de préprocesseurs.

## Sommaire

- [TP1 - (2026)](#tp1---2026)
  - [Sommaire](#sommaire)
  - [Présentation](#présentation)
    - [Le défi : des composants accessibles](#le-défi--des-composants-accessibles)
    - [Liens](#liens)
  - [Mon Processus](#mon-processus)
    - [Technologies utilisées](#technologies-utilisées)
    - [Ce que j'ai appris](#ce-que-jai-appris)
    - [Développement continu](#développement-continu)
  - [Auteur](#auteur)

## Présentation
![version table](images/screencapture-127-0-0-1-5500-index-html-2026-09-23-20_03_13.png)
![version mobile](images/screencapture-127-0-0-1-5500-index-html-2026-09-23-20_03_39.png)
### Le défi : des composants accessibles

Les utilisateurs doivent être capables de :

- Consulter le site sur n'importe quel écran (ordinateur, tablette, smartphone) avec une mise en page fluide.
- Voir les états de survol (hover) et de focus clavier pour tous les éléments interactifs de la page.
- Ouvrir et fermer le menu mobile à l'aide d'un bouton qui bascule textuellement ("Menu" / "Fermer") et graphiquement (Hamburger / Croix).
- Naviguer de manière accessible : le menu mobile doit respecter les normes WCAG (fermeture avec la touche `Échap`, gestion des attributs `aria-expanded` et `aria-hidden`).
- Utiliser les filtres avec des cases à cocher stylisées, alignées et accessibles au clavier.

### Liens

- URL de la solution : [Lien vers mon dépôt GitHub](https://github.com/elatifir/tp1-base-2026)
- URL du site en direct : [Lien vers GitHub Pages](https://elatifir.github.io/tp1-base-2026/)

## Mon Processus

- **Analyse de la maquette** : identification des composants (header, filtres, grille produits, pagination, footer) et de leurs états (hover, focus, actif, masqué).
- **Structuration HTML sémantique** : utilisation de `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`
- **Responsive** : media queries à `64rem`, `70rem`, `80rem` pour adapter la grille produits et le menu.
- **Accessibilité** : focus visibles (`:focus-visible`), `sr-only` pour les textes cachés, `aria-label` sur les boutons icônes.
### Technologies utilisées

- **HTML5** – Balisage sémantique (`<nav>`, `<header>`, `<main>`).
- **CSS3 Moderne (Architecture 2026)** – Utilisation des couches de cascade natives (`@layer`) pour isoler les styles, et du _Nesting_ (imbrication) natif pour la lisibilité.
- **Méthodologie BEM** – Nomenclature stricte des classes pour éviter les conflits de spécificité.
- **JavaScript Vanille** – Script épuré (syntaxe `let` et fonctions classiques pour débutant) axé sur l'accessibilité ARIA.
- **Google Fonts** – Polices `Barlow`, `Barlow Condensed`, `Barlow Semi Condensed`, `Noto Sans JP`.

### Ce que j'ai appris
- Nommer mes classes avec BEM : un nom clair et prévisible pour chaque classe, ce qui évite les conflits.
- Penser mobile d'abord, puis agrandir avec des media queries.
- Utiliser (`<time datetime="2017">`) pour les dates'
- Utiliser (`<picture>`) avec srcset et media pour servir différentes tailles d'images selon la largeur d'écran.
- Nommer les images de façon descriptive (men_AirForceFlynit_01_w446.jpg plutôt que img1.jpg).
- Optimiser les images avant de les intégrer (poids, format, dimensions).
- Un badge « Nouveau » positionné en absolute sur l'image produit.
- Une grille produits qui passe de 1 → 2 → 3 colonnes selon l'écran.
- Vérifier le HTML avec le validateur W3C.
- Utilisation de :has() pour adapter la grille quand les filtres sont masqués.

### Développement continu
Pour mes prochains projets, je souhaite :
- Comprendre en profondeur les rôles ARIA et quand les utiliser (ou ne pas les utiliser).
- Adopter une approche mobile-first systématique.
- Documenter mon code avec des commentaires utiles.

## Auteur
 Rhita Elatifi