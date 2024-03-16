# Projet ETL Twitter

Ce projet contient un DAG Airflow pour extraire, transformer et charger (ETL) des tweets à partir de l'API Twitter, et les stocker dans le service de stockage cloud AWS S3.

## Description

Ce DAG Airflow est conçu pour récupérer les tweets d'un utilisateur spécifique sur Twitter, en l'occurrence '@elonmusk', les transformer en un format CSV, et les stocker dans un bucket AWS S3.

## Contenu du Projet

- `twitter_dag.py`: Le script Python contenant le DAG Airflow pour orchestrer le processus ETL.
- `twitter_etl.py`: Le script Python contenant la logique d'extraction, transformation et chargement (ETL) des tweets depuis l'API Twitter, et le stockage dans AWS S3.
- `README.md`: Ce fichier, fournissant une description du projet.
- `twitter_commands.sh`: Un script bash (s'il est pertinent) contenant des commandes utiles pour l'utilisation ou la configuration du projet.
- Autres fichiers ou répertoires pertinents.

## Configuration

Avant d'exécuter le DAG Airflow, assurez-vous d'avoir configuré les clés d'accès de l'API Twitter dans le script `twitter_etl.py`. De plus, configurez les informations d'authentification AWS pour accéder à S3.

## Installation

1. Cloner ce dépôt : `git clone https://github.com/votre-utilisateur/twitter-etl.git`
2. Installer les dépendances : `pip install -r requirements.txt`

## Utilisation

1. Configurez les clés d'accès de l'API Twitter dans `twitter_etl.py`.
2. Configurez les informations d'authentification AWS dans `twitter_etl.py` pour accéder à S3.
3. Lancez le DAG Airflow en exécutant le script `twitter_dag.py`.
4. Consultez le bucket S3 spécifié dans le script pour récupérer les fichiers CSV contenant les données extraites et transformées.

## Stockage dans AWS S3

Les données extraites et transformées sont automatiquement stockées dans un bucket S3 spécifié dans le script `twitter_etl.py`. Assurez-vous que l'utilisateur exécutant le DAG a les autorisations appropriées pour écrire dans le bucket S3.

## Auteur

[@makavelli666](https://github.com/makavelli666)

## Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.
