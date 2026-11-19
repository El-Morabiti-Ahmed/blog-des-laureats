# Dossier du Rapport de Projet (`rapport/`)

Ce dossier héberge le rapport technique et académique du projet Blog des Lauréats (Solicode Tanger).

## 1. Organisation modulaire

Le rapport est découpé en chapitres indépendants dans le sous-dossier `chapitres/` pour faciliter la rédaction progressive. Chaque fichier porte le numéro de sa position, suivi d'un nom dérivé de son titre (`1.remerciement.md`, `2.table-des-matieres.md`, ..., `25.chapitre-2-conclusion.md`). Le numéro fixe l'ordre du rapport sans configuration :

- `1.remerciement.md` : remerciement.
- `2.table-des-matieres.md` : table des matières, remplie automatiquement par le script.
- `3.chapitre-1-introduction.md` : introduction.
- Les chapitres `4` à `9` couvrent le contexte, le cahier des charges et la méthodologie.
- `10.planification.md` : organisation des sprints.
- Les chapitres `11` à `15` couvrent la branche fonctionnelle et l'analyse fonctionnelle.
- Les chapitres `16` à `18` couvrent la branche technique, la stack et l'architecture.
- Les chapitres `19` à `22` couvrent le prototype et la conception.
- `23.realisation.md` et `24.interfaces.md` : réalisation et interfaces.
- `25.chapitre-2-conclusion.md` : conclusion et perspectives.

Les chapitres encore vides contiennent seulement leur titre de niveau 1 : le script le reprend tel quel.

## 2. Compilation automatique

Le fichier unique consolidé `rapport.md` est généré automatiquement à partir des chapitres à l'aide d'un script Node.js réutilisable sur n'importe quel projet :

- Script : `concat-chapitres.js`
- Commande directe : `node concat-chapitres.js`
- Ou via npm : `npm run build`

Le script ne contient aucune liste de chapitres : il détecte tous les fichiers `.md` du dossier, les trie par ordre naturel du nom (préfixe numérique puis alphabet) et les numérote de 1 à N dans le rapport généré. Les titres sont repris du titre de niveau 1 présent dans le fichier, sinon déduits du nom du fichier.

Les titres sont insérés tels quels, sans numérotation : le fichier `23.realisation.md` produit `# Réalisation`, et non `# Chapitre 23 : Réalisation`.

La table des matières est elle aussi générée : le chapitre qui contient le marqueur `<!-- SOMMAIRE -->` reçoit à cet endroit la liste des titres de tous les autres chapitres.

Options disponibles :

- `--chapters <dossier>` : dossier des chapitres (`chapitres/` par défaut).
- `--output <fichier>` : fichier généré (`rapport.md` par défaut).
- `--title <texte>` : titre du rapport (`Rapport de Projet` par défaut).
- `--marp` : ajoute l'en-tête Marp au fichier généré.

## 3. Guide de rédaction

- Rédiger ou modifier les chapitres dans le sous-dossier `chapitres/`.
- Pour placer un chapitre à un endroit précis, commencer son nom de fichier par le numéro d'ordre voulu (`12.titre-du-chapitre.md`).
- Chaque fichier commence par son titre de niveau 1 (`# Titre du chapitre`) : ce titre est repris tel quel dans le rapport.
- Le fichier `2.table-des-matieres.md` ne contient que son titre et le marqueur `<!-- SOMMAIRE -->` : ne pas écrire la liste à la main.
- Lancer le script de compilation après chaque modification pour mettre à jour `rapport.md`.
- Respecter les règles générales : zéro tableau Markdown, liens relatifs et français professionnel.
