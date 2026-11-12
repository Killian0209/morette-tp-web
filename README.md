# RANDOM ADVENTURE GAME

Jeu d'aventure loufoque en **HTML / CSS**, réalisé par **Killian MORETTE** dans le cadre d'un TP web.

Tu incarnes Mega Man et tu traverses une suite de scènes complètement incohérentes (village d'Astérix, stade de l'OM, Paris, Europa Park, Fortnite, IKEA…). À chaque scène, une question : la bonne réponse te fait avancer, la mauvaise t'envoie sur la page **perdu**.

## Lancer le jeu

Aucune installation n'est nécessaire.

1. Télécharger ou cloner le dépôt.
2. Ouvrir `index.html` dans un navigateur.
3. Cliquer sur **Jouer**.

## Pages principales

| Page | Rôle |
|------|------|
| `index.html` | Menu principal (Jouer / À propos) |
| `apropos.html` | Crédits du jeu |
| `scene01.html` à `scene13.html` | Scènes du parcours principal |
| `challenge.html` → `scene_exp.html` | Branche « challenge » (le vaisseau) |
| `scene_alt.html` → `sceneAlt2.html` | Branche « bobo » (scène alternative) |
| `win.html` | Victoire |
| `winb.html` | Victoire alternative (« bobo ») |
| `perdu.html` | Défaite |

Toute mauvaise réponse mène à `perdu.html`. Les pages `perdu`, `win` et `winb` proposent un lien **Retourner au menu** vers `index.html`.

Le schéma complet, avec toutes les réponses et les liens cachés, est dans **`arbre_navigation.pdf`**.

## Liens cachés

Deux passages ne se trouvent pas en lisant simplement les boutons :

- `scene_alt.html` : un des mots de la phrase est un lien.
- `scene13.html` : un bouton sans texte mène à la victoire.

## Structure du projet

```
morette-tp-web/
├── index.html, apropos.html
├── scene01.html … scene13.html
├── scene_exp.html, scene_alt.html, sceneAlt2.html
├── challenge.html
├── win.html, winb.html, perdu.html
├── style.css, style1.css … style13.css   (styles des scènes)
├── apropos.css, challenge.css, perdu.css,
│   scene_alt.css, scene_alt2.css, scene_exp.css,
│   win.css, winb.css
├── arbre_navigation.pdf                  (arbre de navigation)
└── assets/
    ├── background/                       (images de fond)
    ├── icons/                            (personnages et images de réponses)
    ├── police/                           (police AdventureTime)
    └── sounds/
```

## Technologies

- HTML5
- CSS3
- Aucune dépendance, aucun JavaScript

## Auteur

Killian MORETTE
