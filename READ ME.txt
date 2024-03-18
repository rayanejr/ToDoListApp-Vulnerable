# Mon Application Web PHP

Ce projet est une simple application web développée en PHP et dockerisée pour une mise en œuvre facile. Elle utilise MySQL comme système de gestion de base de données et PHPMyAdmin pour une administration facile de la base de données via une interface web.

## Architecture

L'application est composée de trois services principaux :

- `web` : le service Apache avec PHP 8.0
- `db` : le service de base de données MySQL 8.0
- `phpmyadmin` : une interface web pour la gestion de la base de données MySQL

![Architecture de l'application](<VotrePhoto.png>)

## Prérequis

Avant de commencer, assurez-vous que vous avez Docker et Docker Compose installés sur votre machine.

- [Installer Docker](https://docs.docker.com/get-docker/)
- [Installer Docker Compose](https://docs.docker.com/compose/install/)

## Démarrage rapide

1. Clonez ce dépôt sur votre machine locale :

   ```bash
        git clone https://example.com/mon-repo.git
        cd mon-repo
   ```
2. Construisez et lancez les containers Docker :
    
    ```bash
        docker-compose up -d
   ```
3. Accédez à l'application web :

a. Application Web PHP : http://localhost:8000
b. PHPMyAdmin : http://localhost:8080

Utilisation
Vous pouvez modifier le code de l'application PHP dans le dossier local et voir les changements en direct en actualisant votre navigateur.

Pour interagir avec la base de données, utilisez PHPMyAdmin à l'adresse mentionnée ci-dessus.

4. Arrêt et nettoyage
Pour arrêter les services et nettoyer les ressources, exécutez :

    ```bash
        docker-compose down -v
        Cela arrêtera et supprimera les conteneurs, les réseaux par défaut, et le volume de la base de données.
    ```