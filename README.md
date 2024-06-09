# readme_file 

New-Focus-Web

1️/ Technologie Frontend

Framework : React.js

Gestion d'état : Redux

Outil de Build : npm

Backend

Environnement : Node.js v12

Base de données : MongoDB

Déploiement

Outil CI précédent : Gitlab-CI (désormais obsolète)

2️/ Structure du Projet

La structure suivante permettra au projet de croître efficacement et de faciliter sa maintenance.

Structure du Frontend

├── src

│   ├── assets

│   │  ├── fonts

│   │  ├── images

├── json

│   │  ├── svg

│   ├── containers

│   │  ├── feature

│   │  │  ├── constante

│   │  │  ├── index

│   │  │  ├── message

│   │  │  ├── reducer

│   │  │  ├── saga

│   ├── helpers

│   ├── translations

│   ├── utils

│   │  ├── focus-ui-kit

│   │  │  ├── Axios

│   │  │  ├── messages

│   │  │  ├── Protected

│   │  │  ├── roles

│   │  │  ├── utils

│   ├── App.jsx

│   ├── reducers.jsx

│   ├── sagas.jsx

│   ├── store.jsx

│   ├── index.jsx

3️/ Exécution du Projet

Configuration du Frontend

-Cloner le Répertoire

git clone https://gitlab.com/focus2/new-focus-web

Installation

Accédez au répertoire du projet et installez les dépendances :

cd new-focus-web

npm install

Compilation et Démarrage

Pour compiler et construire le projet pour la production :

npm run build:prod

Pour démarrer le serveur de développement :

npm start

Adresse par défaut : http://localhost:3000

Identifiants

Login : abounsir@maltem.com

Mot de passe : password

Dépannage

Si vous rencontrez des problèmes, essayez les commandes suivantes :

rm package-lock.json

rm -R node_modules

npm cache clean --force

npm install

Pour plus d'assistance, contactez abounsir@maltem.com.

Configuration du Backend

Cloner le Répertoire

git clone https://gitlab.com/focus2/focus-backend.git

Installation

Accédez au répertoire du projet backend et installez les dépendances :

cd focus-backend

npm install

Configuration

Configurez la connexion MongoDB dans src/config/db.cfg.js :

MongoDB local :

const LOCAL_DB = "mongodb://127.0.0.1:27017/test"

MongoDB distant :

const REMOTE_DB = "mongodb+srv://doadmin:password@db-mongodb-fra1-dev-8b08ba06.mongo.ondigitalocean.com/admin?tls=true&authSource=admin"

Assurez-vous que toutes les variables nécessaires sont définies dans le fichier .env.

Exécution

Pour démarrer le serveur :

npm start

Ou utilisez nodemon pour les redémarrages automatiques :

npx nodemon

Visitez http://localhost:4000/backend/api/v1 pour voir l'application Express.

Dépannage
Si les problèmes persistent, essayez les commandes suivantes :

rm package-lock.json
rm -R node_modules
npm cache clean --force
npm install
Assurez-vous que l'URI MongoDB est correctement configuré dans src/config/db.cfg.js.

Ce projet a été initialisé avec Create React App.

En Savoir Plus
Documentation de Create React App
Documentation de React
Documentation du Backend Focus
Pour des scripts et configurations supplémentaires, consultez la documentation de Create React App.
