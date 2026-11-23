# Cadrage du projet — Blog des Lauréats

> Ingénierie logicielle — Étape 2 : définition du produit et de son périmètre.

---

## 1. Contexte et valeur du projet

Les témoignages et conseils de carrière des lauréats circulent aujourd'hui sur des réseaux externes ou de manière informelle. Ils sont donc difficiles à retrouver et rarement conservés. Le **Blog des Lauréats** offrira un espace numérique institutionnel pour :

- Présenter les projets, parcours et expertises des lauréats.
- Partager avec les apprenants des expériences concrètes liées aux métiers.
- Mettre en valeur les compétences techniques et le dynamisme de la communauté.

---

## 2. Objectifs SMART

- **Spécifique :** créer une plateforme web pour rédiger, relire, publier et consulter des articles classés par catégorie.
- **Mesurable :** accueillir au moins 50 articles publiés au premier trimestre ; charger un article en moins de 300 ms en conditions normales ; adapter une interface accessible aux mobiles, tablettes et ordinateurs.
- **Atteignable :** livrer progressivement des fonctionnalités complètes et vérifiées lors de sprints Scrum de 80 heures.
- **Réaliste :** utiliser Laravel 13, MySQL, Tailwind CSS, Preline UI et Alpine.js pour limiter la complexité et la dette technique.
- **Temporel :** Sprint 0 pour le cadrage, l'infrastructure et les prototypes ; Sprint 1 pour le socle technique, la persistance et un premier parcours fonctionnel ; fin du cycle pour le déploiement en production.

---

## 3. Périmètre du MVP

### Inclus

- **Lecture publique :** accueil avec derniers articles, pages d'articles (auteur, date, catégorie), filtres thématiques, recherche textuelle simple et pagination.
- **Espace auteur :** inscription, connexion, réinitialisation du mot de passe, profil (nom, biographie, photo, liens LinkedIn et GitHub), tableau de bord, éditeur riche et statuts d'article (brouillon, soumis à modération, publié).
- **Administration et modération :** suivi des articles soumis, approbation et publication ou demande de correction motivée, gestion des catégories (création, modification, archivage), gestion des comptes et des rôles RBAC.

### Exclu

- Messagerie instantanée et chat ; les échanges passent par les profils externes.
- Abonnements payants, dons et commerce en ligne.
- Applications natives iOS et Android ; le site web adaptatif couvre les usages mobiles.
- Notes par étoiles et recommandations avancées par intelligence artificielle.
- Import et export automatisés depuis Medium, WordPress ou d'autres plateformes.

---

## 4. Contraintes et réussite

### Contraintes

- **Technique :** hébergement PHP/MySQL sans dépendance à des infrastructures propriétaires complexes ; contrôleurs légers et services métier ; rendu Blade enrichi par Alpine.js, sans SPA lourde.
- **RGPD :** consentement à la création du compte ; droits d'accès, de rectification et de suppression ; mots de passe hachés et protection contre les vulnérabilités courantes.
- **Accessibilité :** contraste WCAG AA, conception mobile-first et HTML5 sémantique compatible avec les lecteurs d'écran.

### Conditions de réussite

- Une rédaction et une soumission simples et rapides pour les lauréats.
- Une lecture claire et agréable pour les apprenants.
- Une modération éditoriale fluide.
