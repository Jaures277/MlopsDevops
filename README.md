# MlopsDevops

## Objectif 
Mettre en place une chaîne complète MLOps en intégrant l'ensemble des pratiques DevOps et les outils spécifiques au Machine Learning, en utilisant une approche d'Infrastructure as Code (IaC) et de CI/CD.

## Description du Projet
Ce projet consiste à construire une chaîne complète MLOps pour un modèle de machine learning. L’objectif est d'intégrer les pratiques DevOps en utilisant une approche Infrastructure as Code (IaC) et des pipelines CI/CD pour faciliter le développement, le déploiement et la surveillance d’un modèle ML.

## Les principaux composants sont :

Infrastructure Cloud : Provisionnée sur AWS avec Terraform et configurée avec Ansible.
Application ML : API de prédiction construite autour d'un modèle ML (entraînement et versioning des modèles avec MLflow).
Pipeline CI/CD : Automatisé avec GitHub Actions pour les tests, le build et le déploiement.
Monitoring : Métriques d'infrastructure et de performance du modèle via Prometheus et visualisation avec Grafana.
Architecture Technique
Voici un aperçu de l'architecture générale :

Infrastructure : Provisionnée sur AWS avec Terraform et configurée via Ansible pour l’installation des dépendances.
Application : Un modèle de machine learning conteneurisé avec Docker, déployé et accessible via une API REST (Flask ou FastAPI).
CI/CD : Pipeline GitHub Actions pour automatiser les tests, le build Docker et le déploiement en production.
Monitoring : Prometheus pour la collecte des métriques et Grafana pour la visualisation.

## Technologies Utilisées

### Technologie	Description
Docker	Conteneurisation des services pour un déploiement simplifié et portable.
Terraform	Infrastructure as Code pour provisionner les ressources sur AWS.
Ansible	Gestion de la configuration des serveurs.
MLflow	Suivi des expérimentations et versioning des modèles.
GitHub Actions	Automatisation du pipeline CI/CD.
Prometheus	Monitoring des métriques d'infrastructure et de performance des modèles.
Grafana	Visualisation des métriques collectées.

## Prérequis
Compte AWS (ou autre fournisseur cloud supporté)
Docker installé localement
Accès à GitHub pour configurer les GitHub Actions
Clé SSH pour accéder aux serveurs (si nécessaire)
Terraform et Ansible installés sur votre machine
Installation et Déploiement
