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
docker-compose up --build -d
```

## Feuille de Route Détaillée (Étapes d'Apprentissage Prévues)

Ce projet évoluera en suivant ces étapes :

1.  **Projet simple (sans base de données externe, juste Django et SQLite)**
    *   Objectif : Maîtriser la configuration Docker et le pipeline de base.

2.  **Projet avec base de données PostgreSQL**
    *   Objectif : Apprendre à composer plusieurs services (application + base de données) avec Docker Compose.

3.  **Projet avec des fichiers médias**
    *   Objectif : Configurer la gestion et le service des fichiers médias (uploads utilisateurs) directement sur le serveur, en utilisant des volumes Docker et  Nginx pour les servir.

4.  **Projet avec Celery**
    *   Objectif : Comprendre le fonctionnement de Celery pour les tâches asynchrones et Celery Beat pour les tâches planifiées, et les intégrer dans l'environnement Docker Compose.

5.  **Mise en Production Complète et Automatisation**
    *   Installation de Docker sur le VPS.
    *   Configuration du proxy Nginx avec Docker Compose sur le serveur.
    *   Pointer le nom de domaine vers le serveur.
    *   Créer un pipeline GitHub Actions pour le build et le déploiement automatiques.
---

Ce projet est un voyage d'apprentissage. Suivez les commits pour voir l'évolution 😉

By djokodev 😊.