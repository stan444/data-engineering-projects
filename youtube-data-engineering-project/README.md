# Projet d'Analyse YouTube de Données par Darshil Parmar

## Introduction
Ce projet vise à gérer en toute sécurité, rationaliser et effectuer des analyses sur les données structurées et semi-structurées des vidéos YouTube, en se basant sur les catégories de vidéos et les métriques de tendance.
## Objectifs du Projet
1. **Ingestion des Données** — Construire un mécanisme pour ingérer des données provenant de différentes sources.
2. **Système ETL** — Nous recevons des données brutes, qu'il faut transformer en un format approprié.
3. **Lac de Données** — Comme nous recevrons des données de multiples sources, nous avons besoin d'un référentiel centralisé pour les stocker.
4. **Évolutivité** — Au fur et à mesure que la taille des données augmente, nous devons nous assurer que notre système évolue en conséquence.
5. **Cloud** — Nous ne pouvons pas traiter de vastes quantités de données sur un ordinateur local, nous devons donc utiliser le cloud, dans ce cas, AWS.
6. **Reporting** — Construire un tableau de bord pour répondre aux questions posées précédemment.

## Services Utilisés
1. **Amazon S3** : Amazon S3 est un service de stockage d'objets offrant une évolutivité, une disponibilité des données, une sécurité et des performances élevées.
2. **AWS IAM** : AWS Identity and Access Management (IAM) permet de gérer de manière sécurisée l'accès aux services et ressources AWS.
3. **QuickSight** : Amazon QuickSight est un service de business intelligence (BI) évolutif, sans serveur, et alimenté par le machine learning, conçu pour le cloud.
4. **AWS Glue** : Un service d'intégration de données sans serveur qui facilite la découverte, la préparation et la combinaison de données pour l'analyse, le machine learning et le développement d'applications.
5. **AWS Lambda** : Lambda est un service de calcul permettant d'exécuter du code sans créer ni gérer de serveurs.
6. **AWS Athena** : Athena est un service de requête interactive pour S3, dans lequel il n'est pas nécessaire de charger les données puisqu'elles restent dans S3.

## Jeu de Données Utilisé
Ce jeu de données Kaggle contient des statistiques (fichiers CSV) sur les vidéos YouTube populaires quotidiennes sur plusieurs mois. Jusqu'à 200 vidéos tendance sont publiées chaque jour pour plusieurs régions. Les données pour chaque région sont dans un fichier distinct. Les informations incluent le titre de la vidéo, le nom de la chaîne, l'heure de publication, les tags, les vues, les likes, les dislikes, la description et le nombre de commentaires. Un champ **category_id**, qui varie selon la région, est également inclus dans le fichier JSON associé.

[Jeu de données Kaggle](https://www.kaggle.com/datasets/datasnaek/youtube-new)

## Diagramme d'Architecture
![Diagramme d'Architecture](architecture.jpeg)

