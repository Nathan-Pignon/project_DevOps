# Project DevOps - Maxime MARTIN & Nathan PIGNON

**Environnement de dev : https://tpdevopsdev.web.app/**

**Environnement de prod : https://tpdevopsprod.web.app/**

## Triggers

Les scripts de déploiement se déclenchent par un push sur la branche Master pour le développement, et par la publication d'une nouvelle feature pour le déploiement en production.

## Tests

Dans les deux environnements, des tests sont effectués pour valider de manière unitaire, ainsi que la qualité et la sécurité du code. La réussite de ces tests est nécessaire pour accéder à la partie suivante.

## Build et déploiement

Une fois les tests validés, les workers réalisent le build et le déclenchement du déploiement du projet.

Nous avons fait le choix de déployer sur Firebase afin de pouvoir héberger le projet, et gérer facilement les deux environnements de déploiement.

## Notification sur Discord

Nous avons choisi, une fois la réussite du déploiement, de déclencher un message automatisé sur Discord pour nous informer de cette réussite, ainsi que certaines informations permettant de situer facilement le commit déclencheur ou la release. 