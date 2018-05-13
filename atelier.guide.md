# Atelier guidé : Strapi Gatsby

## Brief

Créer un système de blog

## User stories

### 1. Admin

1. En tant qu'admin, je peux accéder à toutes les fonctionnalités du back office

### 2. Utilisateur connecté

1. En tant qu'utilisateur connecté, je peux créer, editer, supprimer des articles
2. En tant qu'utilisateur connecté, je peux créer, editer, supprimer des tags
3. En tant qu'utilisateur connecté, je peux associer un tag à un article
4. En tant qu'utilisateur connecté, je peux dissocier un tag d'un article

### 3. Visiteur

1. En tant que visiteur, je peux consulter la listes des articles
2. En tant que visiteur, je peux consulter un article
3. En tant que visiteur, je peux voir l'auteur de l'article
4. En tant que visiteur, je peux voir la liste des articles d'un auteur
5. En tant que visiteur, je peux consulter la liste des tags
6. En tant que visiteur, je peux consulter les articles liés à un tags
7. En tant que visiteur, je peux voir les tags lié à un article

## Modèle de donnée : Entités et associations

### User

- firstName
- lastName
- email

(Nous utiliserons l'entité `user` de Strapi )

### Article

- title (string) [required]
- resume (string) [required]
- content (text)
- author (user) [one-to-many] [required]

### tag

- label (string) [required]
- articles (article) [many-to-many]

## Implémentation

### Strapi

- User story 1
  - Créer un projet avec strapi
  - Créer l'utilisateur `Admin`

- User story 2
  - Créer l'entité `article` et son association avec `user`
  - Créer l'entité `tags` et son association avec `article`
  - Créer des tags via le dashboard
  - Créer des articles via le dashboard
  - Donner les droits CRUD sur `article` et `tag` aux utilisateurs connectés

- User story 3
  - Donner les droits `find`et `find one` sur les API de l'entité `article` aux visiteurs
  - Donner les droits `find`et `find one` sur les API de l'entité `tag` aux visiteurs
  - tester les API  public `/article` `/article/slug`

### Gatsby

- User story 3
  - Créer un projet avec gatsby
  - accéder à l'interface graphQL afin de tester les API en graphQL
  - Ajouter la liste des articles à la homepage
  - Créer une page article
  - Créer une page auteur
  - Créer une page tags