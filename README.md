# Mon Agence

Projet Docker Compose réalisé dans le cadre d'une formation DWWM chez BeWeb.

## Prérequis

- Docker Desktop installé et démarré sur votre machine
- Git

## Lancer le projet

Clonez le dépôt puis exécutez :

```bash
docker-compose up
```

Tous les services démarrent automatiquement. Aucune installation manuelle n'est nécessaire.

## Accès aux services

| Service | URL |
|---|---|
| Site frontend | http://localhost:8080 |
| phpMyAdmin | http://localhost:8090 |

## Identifiants base de données

| Paramètre | Valeur |
|---|---|
| Hôte | db |
| Base de données | users |
| Utilisateur | user |
| Mot de passe | user_password |
| Mot de passe root | root |

## Structure du projet

```
mon-agence/
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── Dockerfile
├── backend/
│   ├── app.sh
│   └── Dockerfile
├── docker-compose.yml
└── README.md
```

## Services Docker

- **frontend** : serveur Apache (httpd) servant une page HTML/CSS, accessible sur le port 8080
- **backend** : script Bash exécuté au démarrage du conteneur
- **db** : base de données MariaDB avec persistance des données via un volume Docker
- **phpmyadmin** : interface d'administration de la base de données, accessible sur le port 8090

## Gestion du projet

Tableau Trello : https://trello.com/b/74MCzNfm/projet-docker-compose-mon-agence
