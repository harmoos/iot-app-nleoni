# iot-app-nleoni

Ce dépôt public est la source GitOps de la partie 3 du projet
Inception of Things. Argo CD synchronise automatiquement ces trois ressources
dans le namespace `dev` :

- `deploy.yaml` : application `vloth2602/iot-app` ;
- `service.yaml` : accès interne sur le port `8888` ;
- `ingress.yaml` : accès externe via l'Ingress K3d.

Le déploiement commence avec le tag `v1`. Pour démontrer la synchronisation
automatique demandée par le sujet, remplacer `v1` par `v2` dans `deploy.yaml`,
puis committer et pousser le changement.
