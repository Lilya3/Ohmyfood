# Ohmyfood

Projet 3 réalisé dans le cadre de la formation **Intégrateur Web d’OpenClassrooms**.

L’objectif était d’intégrer en mobile first le site d’**Ohmyfood**, une entreprise fictive de réservation de menus gastronomiques, puis d’enrichir l’interface avec des animations CSS réalisées sans JavaScript.

## Présentation du projet

Ohmyfood permet aux utilisateurs de découvrir une sélection de restaurants parisiens et de consulter leur menu avant leur arrivée.

Cette première version du site comprend :

- une page d’accueil présentant le fonctionnement du service ;
- une sélection de quatre restaurants ;
- une page de menu dédiée à chaque restaurant ;
- une interface responsive adaptée aux mobiles, tablettes et ordinateurs ;
- plusieurs animations et transitions réalisées uniquement avec CSS et Sass.

## Restaurants présentés

- **La palette du goût**
- **La note enchantée**
- **À la française**
- **Le délice des sens**

Chaque page présente les entrées, les plats et les desserts du restaurant, ainsi qu’un bouton de commande.

## Travail réalisé

- intégration des maquettes avec une approche mobile first ;
- création de la page d’accueil et des quatre pages de menu ;
- mise en place d’une navigation entre les différentes pages ;
- adaptation de l’affichage aux écrans plus larges avec des media queries ;
- organisation des styles dans plusieurs fichiers Sass ;
- utilisation de variables pour les couleurs, les polices, les tailles et les ombres ;
- compilation du code SCSS dans une feuille de style CSS ;
- intégration d’animations et de transitions sans JavaScript ;
- utilisation d’une convention de nommage inspirée de BEM.

## Animations et interactions

### Écran de chargement

Un loader recouvre temporairement la page d’accueil lors de son ouverture. Il combine :

- une animation de rotation ;
- un masque couvrant l’intégralité de l’écran ;
- une disparition automatique après le chargement.

### Boutons principaux

Les boutons utilisent un dégradé reprenant les couleurs principales de l’identité graphique. Leur apparence s’éclaircit au survol grâce aux fonctions de couleur Sass.

### Boutons « J’aime »

Les cœurs présents sur les cartes et les pages de restaurant peuvent être activés. Le remplissage coloré apparaît progressivement grâce à une transition CSS.

### Apparition des menus

Les éléments des menus apparaissent progressivement avec un décalage entre chaque étape. Les délais d’animation sont générés avec une boucle Sass `@for`.

### Sélection d’un plat

Au survol d’un plat :

- son prix se déplace ;
- une zone de validation turquoise apparaît depuis la droite ;
- une coche confirme visuellement la sélection ;
- les textes trop longs sont raccourcis avec des points de suspension.

## Technologies utilisées

- HTML5
- CSS3
- Sass / SCSS
- Flexbox
- Media queries
- Animations `@keyframes`
- Transitions et transformations CSS
- Font Awesome
- Google Fonts — Roboto et Shrikhand

Le projet ne contient aucun framework et n’utilise pas JavaScript.

## Identité graphique

| Élément | Valeur |
| --- | --- |
| Couleur principale | `#9356DC` |
| Couleur secondaire | `#FF79DA` |
| Couleur tertiaire | `#99E2D0` |
| Titres et logo | Shrikhand |
| Textes | Roboto |

## Responsive design

Le site a été développé selon une approche mobile first :

- les styles de base ciblent les écrans mobiles ;
- à partir de `768px`, les cartes, les menus, le footer et les différentes sections adoptent une mise en page adaptée aux tablettes et aux ordinateurs ;
- le contenu principal est limité en largeur sur les grands écrans afin de conserver une lecture confortable.

## Branche du projet

- **`main`** : contient la version finalisée du site et les fichiers Sass compilés.

## Installation et lancement

Le site est statique et ne nécessite aucune dépendance pour être consulté.

1. Clonez le dépôt :

```bash
git clone <URL_DU_DEPOT>
```

2. Placez-vous dans le dossier du projet :

```bash
cd Ohmyfood
```

3. Ouvrez `index.html` dans votre navigateur ou lancez-le avec **Live Server** dans Visual Studio Code.

## Compilation Sass

Le fichier CSS compilé est déjà inclus dans le dépôt. Pour modifier les sources SCSS, Sass doit être installé sur votre machine.

Compilation unique :

```bash
sass sass/main.scss sass/main.css
```

Compilation automatique pendant le développement :

```bash
sass --watch sass/main.scss:sass/main.css
```

## Structure du projet

```text
Project-3-Ohmyfood/
├── assets/                    # Logo, icônes et illustrations SVG
├── restaurants/               # Photographies des restaurants
├── sass/
│   ├── _base.scss             # Styles globaux et typographie
│   ├── _button.scss           # Boutons et animation des cœurs
│   ├── _footer.scss           # Pied de page
│   ├── _header.scss           # En-tête et navigation
│   ├── _index.scss            # Page d’accueil et loader
│   ├── _menu.scss             # Pages de restaurant et animations
│   ├── _variables.scss        # Variables du design system
│   ├── main.scss              # Point d’entrée Sass
│   └── main.css               # Feuille de style compilée
├── index.html                 # Page d’accueil
├── a_la_francaise.html        # Menu À la française
├── la_note_enchantee.html     # Menu La note enchantée
├── la_palette_du_gout.html    # Menu La palette du goût
└── le_delice_des_sens.html    # Menu Le délice des sens
```

## Compétences travaillées

- intégrer une maquette avec HTML et CSS ;
- développer une interface selon l’approche mobile first ;
- créer une navigation entre plusieurs pages ;
- organiser et maintenir des styles avec Sass ;
- utiliser des variables, l’imbrication et les boucles Sass ;
- concevoir des animations avec `@keyframes` ;
- créer des transitions et des effets interactifs sans JavaScript ;
- adapter une interface aux différentes tailles d’écran ;
- respecter une identité graphique sur l’ensemble d’un site.

## Contexte

Projet pédagogique réalisé dans le cadre de la formation **Intégrateur Web** d’OpenClassrooms.
