# ADR-004 — H2 In-Memory

## Statut
Accepté

## Contexte
Le projet nécessite une base de données pour la phase de développement.
L'objectif est de démarrer rapidement sans infrastructure externe.

## Décision
Utiliser H2 en mode in-memory pour l'environnement de développement.

## Conséquences
- Aucune installation ou configuration de base de données requise
- Démarrage rapide, idéal pour le développement et les tests
- La base de données est réinitialisée à chaque redémarrage de l'application
- Non adapté à la production (données non persistées, pas de scalabilité)
- Migration vers une base de données persistante (PostgreSQL, MySQL) à prévoir pour la production
