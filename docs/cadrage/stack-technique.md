---
marp: true
theme: default
paginate: true
style: |
  section {
    font-size: 25px;
  }
---

# Blog des Lauréats
## Documentation de la stack technique

Choix technologiques et justification

---

# 1. Analyse des besoins

Le Blog des Lauréats doit répondre à plusieurs besoins techniques :

- **Performance :** chargement rapide des pages.
- **Modularité :** code organisé et facile à maintenir.
- **Sécurité :** protection des données et des utilisateurs.
- **Responsive design :** adaptation aux différents écrans.
- **Mobilité :** consultation des articles depuis un smartphone.

---

# 2. Backend — Laravel

Nous avons choisi Laravel comme framework backend.

- Architecture **MVC** pour organiser le code.
- **Eloquent ORM** pour gérer la base de données.
- **Blade** pour créer des vues dynamiques.
- Protection contre les attaques courantes.
- Middleware pour gérer l'authentification et les accès.

Laravel permet de développer une application robuste, sécurisée et évolutive.

---

# 3. Base de données — MySQL

MySQL est notre système de gestion de base de données relationnelle.

- Organisation des données dans des tables.
- Relations entre utilisateurs, articles et catégories.
- Intégrité des données.
- Transactions fiables grâce aux propriétés ACID.
- Compatibilité avec Laravel via PDO et Eloquent.

Il permet de stocker et gérer les données de manière structurée.

---

# 4. Frontend — Tailwind CSS & Preline UI

### Tailwind CSS
- Classes utilitaires pour styliser rapidement les pages.
- Design cohérent et personnalisable.
- Adaptation aux différents formats d'écran.

### Preline UI
- Composants d'interface prêts à l'emploi.
- Gain de temps dans le développement.
- Interfaces modernes et accessibles.

Ces outils facilitent la création d'une interface responsive.

---

# 5. Interactivité — Alpine.js

Alpine.js permet d'ajouter des interactions directement dans le HTML.

- Gestion des menus et des boutons.
- Interactions dynamiques.
- Code JavaScript léger.
- Intégration naturelle avec Blade.

Il évite d'utiliser un framework frontend complexe pour des besoins simples.

---

# 6. Application mobile — NativePHP

NativePHP permet de développer une application mobile à partir de l'écosystème PHP et Laravel.

- Création d'une application Android.
- Réutilisation de la logique métier Laravel.
- Réutilisation des modèles, contrôleurs et vues existants lorsque compatibles.
- Consultation des articles depuis un smartphone.

Il évite de maintenir deux projets totalement séparés, comme Laravel et Flutter.

---

# 7. Qualité & Tests — TDD

Nous utilisons une approche TDD (Test Driven Development).

- Écrire les tests avant ou pendant le développement.
- Tests unitaires pour les composants.
- Tests fonctionnels pour les fonctionnalités.
- Vérification à chaque modification.

Outils : PHPUnit / Pest.

Cette méthode permet de détecter les erreurs plus tôt et de maintenir un code fiable.

---

# 8. Environnement de développement

Notre environnement repose sur les outils suivants :

- **Windows** — système d'exploitation.
- **PowerShell** — terminal de développement.
- **Composer** — gestion des dépendances PHP.
- **Node.js / npm** — gestion des outils frontend.
- **Android Studio** — SDK et émulateur Android.
- **Git** — versionnement du code.

Un agent IA est utilisé comme copilote pour aider à la recherche, au débogage et aux tests, tout en gardant le développeur responsable du code.

---

# Conclusion

Cette stack technologique répond aux besoins du Blog des Lauréats.

Elle offre :

- Une architecture organisée.
- Une base de données fiable.
- Une interface responsive.
- Des interactions légères.
- Une solution mobile.
- Un développement plus simple à maintenir et à faire évoluer.

**L'objectif :** créer une application cohérente, accessible et évolutive, sur web et mobile.