# e-shop

Le but de cette exercice est de contruire une api pour un application e-commerce avec une dizaine de produits en utilisant Strapi.

## User stories

### 1. Admin

1. En tant qu'admin, je peux accéder à toutes les fonctionnalités du back office

### 2. Utilisateur connecté

1. En tant qu'utilisateur connecté, je peux créer, editer, supprimer des produits
2. En tant qu'utilisateur connecté, je peux créer, editer, supprimer des catégories
3. En tant qu'utilisateur connecté, je peux associer un catégorie à un produit
4. En tant qu'utilisateur connecté, je peux dissocier un catégorie d'un produit

### 3. Visiteur

1. En tant que visiteur, je peux consulter la listes des produits
2. En tant que visiteur, je peux consulter un produit
3. En tant que visiteur, je peux consulter la liste des catégories
4. En tant que visiteur, je peux consulter les produits liés à un catégories
5. En tant que visiteur, je peux voir les catégories lié à un produit

## Specs tech

### Product

- title (string) [required]
- description (string)
- image (???)
- price (text) [required]
- category (category) [one-to-many] [required]

### category

- label (string) [required]
- Products (Product) [many-to-one]

## Réaliser la partie Front end avec Gatsby, vuepress, jekyll ou next.js

## User stories supplémentaires

1. En tant que visiteur, je peux voir les produits classés par prix en ordre croissant

2. En tant que visiteur, je veux voir les 3 derniers produits saisis en page d'accueil