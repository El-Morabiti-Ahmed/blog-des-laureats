---
marp: true
theme: default
paginate: true
size: 16:9
---

<!-- _class: lead -->

# Comprendre Agile & Scrum

### Application au projet Portail e-Sport

- **Apprenant** : El Morabiti Ahmed
- **Encadrant** : ESSARRAJ Fouad

**Projet technique :** Gestion des jeux e-Sport  
**Technologies :** HTML · Tailwind CSS · JavaScript · PHP · JSON

---

# 1. Pourquoi abandonner le Cycle en V ?

### Le Cycle en V

- Tout est planifié au début du projet.
- Le développement suit un plan précis.
- Les tests et la validation arrivent principalement après le développement.

**Problème :** si le besoin change, modifier le projet peut devenir compliqué et coûteux.

### L'approche Agile

- Développer progressivement.
- Tester régulièrement.
- Recueillir des retours.
- Améliorer le produit à chaque étape.

**Exemple :** commencer par afficher et ajouter des jeux, puis améliorer le portail selon les besoins.

---

# 2. Les 4 valeurs Agile

Le Manifeste Agile privilégie :

| Priorité | Valeur |
|---|---|
| 1 | Les individus et leurs interactions plutôt que les processus et outils |
| 2 | Un logiciel fonctionnel plutôt qu'une documentation exhaustive |
| 3 | La collaboration avec le client plutôt que la négociation contractuelle |
| 4 | L'adaptation au changement plutôt que le suivi strict d'un plan |

Cela ne signifie pas que les outils, la documentation, les contrats ou les plans sont inutiles.

**L'objectif :** privilégier ce qui apporte réellement de la valeur au projet.

---

# 3. Les 3 piliers de Scrum

Scrum repose sur trois principes :

### Transparence
Le travail, les problèmes et l'avancement doivent être visibles pour tous.

**Portail e-Sport :** un tableau permet de voir les tâches terminées, en cours et à faire.

### Inspection
Vérifier régulièrement le produit et le travail réalisé.

**Portail e-Sport :** tester l'ajout d'un jeu et vérifier que les données sont enregistrées.

### Adaptation
Modifier l'organisation ou le produit lorsque des problèmes sont détectés.

**Portail e-Sport :** corriger un bug ou améliorer le formulaire après un retour utilisateur.

---

# 4. Les 3 rôles Scrum

### Product Owner (PO)
Définit les besoins du produit et organise les fonctionnalités selon leur priorité.

**Exemple :** prioriser l'affichage des jeux et leur ajout avant des fonctionnalités secondaires.

### Scrum Master (SM)
Aide l'équipe à appliquer Scrum, facilite son organisation et aide à résoudre les blocages.

**Exemple :** identifier les difficultés techniques et améliorer la communication.

### Développeurs
Conçoivent, développent, testent et livrent un incrément fonctionnel.

**Exemple :** créer l'interface, l'API PHP, les classes et le stockage JSON.

---

# 5. Les 5 événements Scrum

### 1. Sprint
Une période de travail limitée durant laquelle l'équipe cherche à atteindre un objectif précis.

### 2. Sprint Planning
L'équipe choisit les tâches et définit l'objectif du Sprint.

### 3. Daily Scrum
Un point quotidien court pour suivre l'avancement et identifier les blocages.

### 4. Sprint Review
Présentation du produit réalisé et collecte des retours.

### 5. Sprint Retrospective
L'équipe analyse son organisation et décide comment s'améliorer.

---

# 6. Application Scrum au Portail e-Sport

### Vision du produit

Créer une application web simple permettant de consulter et gérer une liste de jeux e-Sport.

### Besoins principaux

- Consulter les jeux enregistrés.
- Ajouter un nouveau jeu.
- Indiquer son nom et sa plateforme.
- Enregistrer les données sans recharger la page.
- Informer l'utilisateur du résultat de son action.

**L'objectif est d'obtenir une application simple, fonctionnelle et évolutive.**

---

# 7. Sprint 1 — Construire le MVP

### Sprint Goal

> Créer une première version fonctionnelle du Portail e-Sport permettant d'afficher les jeux et d'en ajouter de nouveaux.

### Les fonctionnalités retenues

- **Feature 1 :** Afficher les jeux depuis le fichier JSON.
- **Feature 2 :** Ajouter un jeu avec son nom et sa plateforme.
- **Feature 3 :** Enregistrer les données et actualiser le tableau sans rechargement.

### Pourquoi ces fonctionnalités ?

Elles représentent le cœur du projet et permettent d'obtenir rapidement une première version utilisable.

---

# 8. Organisation et réalisation du Sprint

### Sprint Planning
Sélectionner les fonctionnalités prioritaires et répartir le travail.

### Daily Scrum
Faire un point sur l'avancement, les difficultés et les prochaines tâches.

### Développement

- HTML / Tailwind CSS : interface.
- JavaScript : formulaire, DOM et requêtes Fetch.
- PHP POO : traitement des données.
- API : communication frontend / backend.
- JSON : stockage des jeux.

### Sprint Review
Démontrer l'affichage et l'ajout d'un jeu.

### Sprint Retrospective
Identifier les difficultés et proposer des améliorations pour le prochain Sprint.

---

# 9. Incrément et Definition of Done (DoD)

### Incrément

Une version fonctionnelle du Portail e-Sport à la fin du Sprint.

L'utilisateur peut :

- Voir les jeux enregistrés.
- Ajouter un jeu.
- Retrouver le jeu ajouté dans le tableau.
- Recevoir une notification de succès ou d'erreur.

### Definition of Done

Une fonctionnalité est terminée lorsque :

- Le code fonctionne correctement.
- Les données sont correctement enregistrées.
- Les erreurs principales sont gérées.
- L'interface est utilisable.
- Les tests sont validés.

---

<!-- _class: lead -->

# Conclusion

Scrum permet de développer progressivement un produit, de vérifier régulièrement son fonctionnement et d'améliorer son organisation grâce aux retours.

**Pour le Portail e-Sport :** commencer par un MVP fonctionnel, puis enrichir l'application Sprint après Sprint.

### Transparence · Inspection · Adaptation