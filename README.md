# 📊 E-Requête

## 📌 Présentation du projet
**E-Requête** est une application web développée avec **Streamlit**, permettant aux **data analysts** d’exécuter des **requêtes SQL pré-enregistrées** sur une **base PostgreSQL**. L'objectif est d'**automatiser les requêtes récurrentes**, d'**extraire** et d'**exporter facilement les données** au format **Excel et CSV**.

---

## 🎯 Objectifs
- ✅ **Interface utilisateur sécurisée** avec connexion et gestion des utilisateurs.
- ✅ **Exécution des requêtes SQL pré-enregistrées** en un clic.
- ✅ **Filtres dynamiques** (ex: sélection d’une période).
- ✅ **Téléchargement des résultats** en **CSV et Excel**.
- ✅ **Navigation multipage optimisée avec Streamlit**.

---

## ⚙️ Fonctionnalités principales
### 🔐 **Authentification & Sécurité**
- Connexion sécurisée via **nom d’utilisateur & mot de passe** (haché via `bcrypt`).
- **Gestion des sessions** via **cookies sécurisés**.
- **Déconnexion propre** pour réinitialiser la session.

### 📊 **Exécution des Requêtes SQL**
- Sélection d’une **requête pré-enregistrée** via un menu déroulant.
- **Gestion des filtres** (ex: sélection d'une période `date_debut` - `date_fin`).
- **Connexion à PostgreSQL via SQLAlchemy**.
- **Affichage interactif des résultats** sous forme de tableau.
- **Exportation des résultats en CSV et Excel**.

### 📂 **Navigation & Interface**
- 📌 **Page de connexion (`main.py`)** → Vérification des identifiants.
- 🏠 **Page d’accueil (`pages/home.py`)** → Accueil de l'utilisateur après connexion.
- 🔎 **Page des requêtes (`pages/requete.py`)** → Exécution des requêtes SQL.
- ⚙️ **Page des paramètres (`pages/parametres.py`)** → Gestion des utilisateurs et requêtes SQL.

---

## 🏗️ **Architecture technique**
### 🔹 **Technologies utilisées**
- 🐍 **Python 3** → Langage principal
- 🎨 **Streamlit** → Framework Web
- 🗄️ **PostgreSQL** → Base de données
- ⚡ **SQLAlchemy** → Connexion SQL sécurisée
- 🔐 **Streamlit Authenticator** → Gestion de l’authentification
- 📊 **Pandas** → Manipulation des données
- 📁 **ExcelWriter / CSV** → Export des données
- 🛠️ **YAML** → Configuration des utilisateurs

### 🔹 **Structure du projet**
