# Cadrage du projet — Blog des Lauréats

> Livrable d'ingénierie logicielle — Étape 2 : cadrage et périmètre du produit.

---

## 1. Contexte et valeur

Les retours d'expérience et conseils de carrière des lauréats sont aujourd'hui dispersés sur des réseaux sociaux externes ou partagés de façon informelle, sans être conservés durablement. Le **Blog des Lauréats**, média numérique institutionnel et convivial, permettra de :

- Documenter les réalisations, parcours et expertises professionnelles des lauréats.
- Donner aux apprenants accès à des témoignages concrets.
- Valoriser l'excellence technique et le dynamisme de la communauté.

---

## 2. Objectifs SMART

- **Spécifique (S) :** proposer une plateforme web autonome pour rédiger, relire, publier et consulter des articles professionnels classés par catégorie.
- **Mesurable (M) :** accueillir au moins 50 articles publiés au premier trimestre ; charger un article en moins de 300 ms en conditions normales ; offrir une interface accessible et responsive sur mobile, tablette et ordinateur.
- **Atteignable (A) :** avancer par sprints Scrum de 80 heures, avec des fonctionnalités livrées en parcours complets et testées de bout en bout.
- **Réaliste (R) :** s'appuyer sur Laravel 13, MySQL, Tailwind CSS, Preline UI et Alpine.js afin de limiter la complexité et la dette architecturale.
- **Temporel (T) :** Sprint 0 pour finaliser le cadrage, l'infrastructure et les prototypes ; Sprint 1 pour le socle technique, la persistance et une première fonctionnalité opérationnelle ; fin du cycle pour le déploiement en production.

---

## 3. Périmètre du MVP

### Inclus

- **Consultation publique :** accueil mettant en avant les derniers articles ; pages détaillées avec typographie soignée et métadonnées (auteur, date, catégorie) ; filtres thématiques, recherche textuelle simple et pagination.
- **Espace auteur lauréat :** inscription, connexion et réinitialisation du mot de passe ; profil (nom, biographie, photo, liens LinkedIn et GitHub) ; tableau de bord personnel ; éditeur riche épuré ; statuts d'article : brouillon, soumis à modération ou publié.
- **Administration et modération :** tableau de suivi des articles soumis ; validation et publication ou demande de correction motivée ; gestion des catégories (création, modification, archivage), des utilisateurs et des rôles RBAC.

### Exclu du MVP

- Messagerie instantanée et chat ; les contacts passent par les profils externes.
- Abonnements payants, dons et monétisation e-commerce.
- Applications natives iOS et Android ; le site web responsive couvre les usages mobiles.
- Notes par étoiles et recommandations prédictives par IA.
- Import et export automatisés d'articles depuis Medium, WordPress ou d'autres plateformes.

---

## 4. Contraintes et facteurs de réussite

### Contraintes

- **Technique :** hébergement PHP/MySQL classique, sans dépendance à des infrastructures propriétaires complexes ; architecture en deux couches (contrôleurs minces et services métier) ; rendu Blade enrichi par Alpine.js, sans SPA lourde côté client.
- **RGPD :** consentement explicite à la création du compte ; droits d'accès, de rectification et de suppression des données personnelles ; mots de passe hachés et protection contre les vulnérabilités courantes.
- **Accessibilité et ergonomie :** contraste WCAG AA, conception mobile-first lisible sur smartphone et HTML5 sémantique compatible avec les lecteurs d'écran.

### Facteurs clés de réussite

- Un parcours de rédaction simple et rapide pour les lauréats.
- Une expérience de lecture claire pour les apprenants.
- Une modération éditoriale fluide.
