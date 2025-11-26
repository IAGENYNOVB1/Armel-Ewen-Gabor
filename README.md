# Armel-Ewen-Gabor
🛒 Liste de courses - Gestion avancée de liste de courses
Description:

C'est une application web front-end pour gérer vos listes de courses de manière intuitive et visuelle. Elle offre des fonctionnalités avancées telles que :

Ajout, édition et suppression d’articles

Gestion de quantités et catégories

Suivi des articles achetés et restants

Historique des articles ajoutés

Import/Export JSON des listes

Statistiques visuelles en temps réel

Mode sombre avec sauvegarde de préférence

L’application est entièrement basée sur HTML, CSS et JavaScript pur (sans framework) et utilise le localStorage pour persister les données.

Structure du projet
project-root/
│
├─ index.html             # Page principale de l'application
├─ README.md              # Documentation du projet
│
├─ /styles (optionnel)    # Dossier pour styles séparés (ici CSS intégré)
│   └─ main.css
│
├─ /scripts (optionnel)   # Dossier pour scripts séparés
│   └─ app.js
│
├─ /assets                # Images, icônes ou ressources statiques
│
└─ /data (optionnel)      # JSON exemple pour import/export

Points clés de la structure dans le code fourni

HTML

Contient la structure de la page, les onglets, les formulaires et la liste des articles.

Trois onglets principaux : Accueil, Historique, Import/Export.

CSS

Intégré directement dans le <head>.

Support du mode sombre et responsive design.

Animation pour les articles, transitions de boutons et messages de succès/erreur.

JavaScript

Contenu dans <script> à la fin du HTML.

Objet app centralise toutes les fonctionnalités :

init(), attacherEvenements(), afficherListe(), mettreAJourStats()

Gestion des articles, historique et stockage local.

Fonctions utilitaires : validation, formatage HTML, notifications success/erreur, thème sombre.

Gestion des onglets et import/export JSON.

Fonctionnalités principales
1️⃣ Gestion des articles

Ajouter un article avec nom, catégorie et quantité.

Modifier ou supprimer un article.

Marquer un article comme acheté.

Filtres par catégorie, état et recherche en temps réel.

2️⃣ Historique

Enregistre automatiquement les derniers articles ajoutés (max 50).

Affiche la date et la quantité pour chaque article.

Possibilité de vider l’historique.

3️⃣ Statistiques

Total d’articles, articles achetés et restants.

Progression en pourcentage.

4️⃣ Import / Export

Exporter la liste et l’historique au format JSON.

Importer depuis un JSON valide pour restaurer les données.

5️⃣ Thème sombre

Bascule dynamique entre clair et sombre.

Sauvegarde de la préférence dans le localStorage.

Utilisation

Ouvrir index.html dans un navigateur moderne (Chrome, Firefox, Edge).

Ajouter des articles via le formulaire en haut de l’onglet Accueil.

Filtrer ou rechercher les articles existants.

Basculer un article comme acheté en cochant la case correspondante.

Accéder à l’historique pour voir les articles ajoutés précédemment.

Importer ou exporter vos données via l’onglet Import/Export.

Activer le mode sombre via l’icône 🌙.

Fonctionnalités techniques avancées

Validation et sécurité

Nom d’article non vide et limité à 100 caractères.

Limite de 500 articles maximum.

Stockage

localStorage pour persister la liste (shoppingList_v2) et l’historique (shoppingHistory_v1).

Accessibilité

Messages d’erreur et de succès avec rôle alert.

Liste d’articles avec role="list" et role="listitem".

Contributions

Le projet peut être amélioré en ajoutant :

Tests unitaires pour les fonctions de validation et de gestion des articles.

TypeScript pour typage statique et meilleure maintenance.

Séparation CSS/JS dans des fichiers externes.

Support multi-utilisateur avec backend (API REST ou Firebase).

Licence

Ce projet est libre de droits et peut être utilisé ou modifié à volonté.
