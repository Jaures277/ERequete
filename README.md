# ERequete
Le projet E-Requête est une application web développée avec Streamlit permettant aux data analysts d’exécuter des requêtes SQL pré-enregistrées sur une base de données PostgreSQL. L’objectif est d’automatiser les requêtes fréquentes et de faciliter l’extraction et le téléchargement des données sous différents formats (Excel, CSV).

2. Objectifs du projet
✅ Offrir une interface utilisateur sécurisée avec un système de connexion et de gestion des utilisateurs.
✅ Simplifier l'exécution des requêtes SQL pré-enregistrées via une interface intuitive.
✅ Permettre le filtrage dynamique (ex: sélection de dates pour les requêtes avec période).
✅ Automatiser l’exportation des résultats en CSV et Excel.
✅ Gérer la navigation via un système multipage avec Streamlit.
3. Fonctionnalités attendues
3.1 Authentification et Sécurité
🔐 Connexion sécurisée via nom d’utilisateur & mot de passe (stockés de manière hachée dans config.yaml).
🍪 Gestion des sessions via cookies pour maintenir la connexion.
🚪 Déconnexion propre pour réinitialiser la session.
3.2 Exécution des requêtes SQL
🔎 Sélection d’une requête pré-enregistrée dans une liste déroulante.
📅 Gestion des filtres dynamiques (ex: sélection d’une période avec date_debut et date_fin).
⚙️ Exécution des requêtes SQL sur PostgreSQL avec SQLAlchemy.
📊 Affichage des résultats sous forme de tableau interactif.
📥 Téléchargement des résultats en CSV et Excel.
3.3 Gestion des pages
📌 Page de connexion (main.py)

Vérification des identifiants et redirection vers l’accueil.
🏠 Page d’accueil (pages/home.py)

Affichage du nom de l’utilisateur connecté.
Navigation vers les autres pages.
Bouton "Se déconnecter".
📋 Page d’exécution des requêtes (pages/requete.py)

Sélection et exécution des requêtes SQL.
Exportation des résultats.
⚙️ Page des paramètres (pages/parametres.py)

Ajout/modification des requêtes SQL.
Gestion des utilisateurs.
4. Architecture technique
4.1 Technologies utilisées
🐍 Python 3 - Langage principal
🎨 Streamlit - Framework web
🗄️ PostgreSQL - Base de données principale
⚡ SQLAlchemy - Connexion à la base de données
🔐 Streamlit Authenticator - Gestion de l'authentification
📝 Pandas - Manipulation et affichage des données
📁 ExcelWriter / CSV - Exportation des fichiers
🛠️ YAML - Configuration des utilisateurs
