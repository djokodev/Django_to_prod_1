# Parcours d'Apprentissage Déploiement Django

Bienvenue, Ce projet sert de fil rouge pour un apprentissage pratique et progressif de la mise en production d'applications Django. L'objectif est de maîtriser la containerisation avec Docker, la configuration d'un proxy Nginx, l'intégration de services comme PostgreSQL et Celery, et l'automatisation du déploiement via un pipeline CI/CD avec GitHub Actions.


## Contexte et Objectif Global

Ce projet est entrepris dans le cadre d'un accompagnement visant à acquérir des compétences solides en déploiement d'applications. 


## Prérequis

Avant de commencer, assurez-vous d'avoir installé les outils suivants sur votre machine :

*   [Git](https://git-scm.com/)
*   [Docker Engine](https://docs.docker.com/engine/install/)
*   [Docker Compose](https://docs.docker.com/compose/install/)


## Technologies Utilisées

*   **Framework Backend :** Python, Django
*   **Base de données :** SQLite, PostgresSql
*   **Tâches Asynchrones  :** Celery, Celery Beat 
*   **Containerisation :** Docker, Docker Compose\


## Installation & Lancement du Projet

Voici les étapes pour cloner, configurer et lancer ce projet :

```bash
# 1. Cloner le dépôt
git clone https://github.com/djokodev/django_to_prod.git
cd django_to_prod
```

# 2. Variables d'environnement

Crée un fichier ```.env``` à la racine du projet, puis :

- Ouvre le fichier ```.env.example```

- Copie tout son contenu

- Colle-le dans le fichier ```.env```

Remplace les valeurs par défaut par les tiennes


# 3. Lancer l’application avec Docker Compose
```bash
docker-compose up --build -d
```

Ce projet est un voyage d'apprentissage. Suivez les commits pour voir l'évolution 😉

By djokodev 😊.