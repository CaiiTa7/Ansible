 # 🌐 Serveur Quark Dockerisé avec Reverse Proxy Nginx
 ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
 ![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
 ![Alpine](https://img.shields.io/badge/Alpine%20Linux-0D597F?style=for-the-badge&logo=alpinelinux&logoColor=white)
 
Ce projet configure et déploie le serveur web Quark pour du contenu statique, derrière un reverse proxy Nginx, en utilisant Docker et Docker Compose.
 ## 📋 Table des Matières
- [🌐 Serveur Quark Dockerisé avec Reverse Proxy Nginx](#-serveur-quark-dockerisé-avec-reverse-proxy-nginx)
  - [📋 Table des Matières](#-table-des-matières)
  - [🚀 Fonctionnalités](#-fonctionnalités)
  - [📦 Structure du Projet](#-structure-du-projet)
  - [🔧 Prérequis](#-prérequis)
  - [📄 Instructions d'Installation](#-instructions-dinstallation)
  - [🔍 Vérification](#-vérification)
  - [📜 Licence](#-licence)

 ## 🚀 Fonctionnalités
 - **Léger:** Utilise Alpine Linux pour un environnement minimal.
 - **Reverse Proxy:** Déploie Nginx pour gérer les requêtes des clients et les rediriger vers le serveur Quark.
 - **Scalable:** Facilement configurable et évolutif grâce à Docker Compose.
 - **Déploiement Simple:** Mise en place rapide avec une configuration minimale.
 ## 📦 Structure du Projet
 ```plaintext
 .

├── Dockerfile             # Dockerfile pour construire l'image du serveur Quark
├── docker-compose.yml     # Fichier de configuration Docker Compose
├── nginx.conf             # Fichier de configuration Nginx pour le reverse proxy
├── root                   # Répertoire contenant les fichiers statiques
│   └── index.html         # Fichier HTML principal à servir
└── README.md              # Fichier README du projet

 ```
## 🔧 Prérequis

* Docker installé sur votre machine. [Installer Docker]()
* Docker Compose installé. [Installer Docker Compose]()

## 📄 Instructions d'Installation

1. **Cloner le dépôt :**

   ```bash
   git clone https://votre-url-depot.git
   cd votre-repertoire-depot
   ```

2. **Construire et démarrer les services :**

   ```bash
   docker-compose up -d
   ```

   Cette commande construira l'image du serveur Quark et démarrera les services Quark et Nginx.

3. **Accéder à l'application :**

   Ouvrez votre navigateur web et allez sur `http://localhost/`.

## 🔍 Vérification

Pour s'assurer que tout fonctionne correctement, vous pouvez vérifier les logs des services :

```bash
docker-compose logs quark
docker-compose logs nginx
```

## 📜 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE]() pour plus de détails.
