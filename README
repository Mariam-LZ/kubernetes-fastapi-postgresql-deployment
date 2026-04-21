# Kubernetes - Déploiement d'une application FastAPI avec PostgreSQL

Projet réalisé dans le cadre de la formation **DataScientest** - module **Kubernetes**.

## Objectif

Déployer sur Kubernetes une architecture composée de deux microservices :

- une application **FastAPI**
- une base de données **PostgreSQL**

Le projet avait pour objectif de mettre en place une infrastructure fiable, scalable et sécurisée en utilisant les objets natifs Kubernetes.

---

## Architecture technique

| Composant | Technologie |
|-----------|-------------|
| Orchestrateur | Kubernetes |
| Application | FastAPI |
| Base de données | PostgreSQL |
| Conteneurisation | Docker |
| Exposition externe | Ingress |
| Réseau interne | Services Kubernetes |
| Stockage | Persistent Volume Claim |
| Configuration | ConfigMaps |
| Secrets | Kubernetes Secrets |
| Sauvegarde cluster | ETCD Snapshot |

---

## Réalisations

### Déploiement de l'application

- Création du Dockerfile du service FastAPI
- Déploiement via `Deployment`
- Mise en place de **3 replicas**
- Exposition interne via `Service`
- Publication externe via `Ingress`
- Association à un sous-domaine personnalisé

### Déploiement de la base de données

- Déploiement PostgreSQL via `StatefulSet`
- Exposition via un service interne nommé `db`

Connexion utilisée :

```text
postgresql://admin:password@db:5432/storedb