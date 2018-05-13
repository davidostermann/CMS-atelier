# Porfolio

Le projet consiste à mettre en place une API présentant vos différentes expériences en les présentant comme des études de cas (case studies).

Une études de cas présente le contexte initial, la réalisation, les difficultés et les acquis de l'expérience.

Une études de cas peut être n'importe quel type d'expérience dans le cadre de votre profession ou de vos études (projet, exercice, tutos, katas...)

## User stories

### 1. Admin

1. En tant qu'admin, je peux accéder à toutes les fonctionnalités du back office

### 2. Utilisateur connecté

1. En tant qu'utilisateur connecté, je peux créer, editer, supprimer des études de cas
2. En tant qu'utilisateur connecté, je peux créer, editer, supprimer des tags
3. En tant qu'utilisateur connecté, je peux associer un tag à un étude
4. En tant qu'utilisateur connecté, je peux dissocier un tag d'un étude

### 3. Visiteur

1. En tant que visiteur, je peux consulter la listes des études de cas
2. En tant que visiteur, je peux consulter un étude de cas
3. En tant que visiteur, je peux consulter la liste des tags
4. En tant que visiteur, je peux consulter les études de cas liés à un tags
5. En tant que visiteur, je peux voir les tags lié à un étude de cas

## Specs tech

### CaseStudy

- title (string)
- description (string)
- image (???)
- tags (tag) [many-to-many]

### tag

- label (string)
- caseStudies (CaseStudy) [many-to-many]

## Réaliser la partie Front end avec Gatsby, vuepress, jekyll ou next.js

## User stories supplémentaires

1. En tant que visiteur, je peux voir la liste des caseStudies classés par tag
2. En tant qu'utilisateur connecté, je peux spécifier un type (soit Technologie, soit Methodologie) au tags afin de pouvoir les attribuer une couleur.
