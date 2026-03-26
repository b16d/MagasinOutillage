# ADR-007 — Liquibase

## Statut
Accepté

## Contexte
Le projet nécessite un outil de gestion des migrations de base de données.
Sans outil dédié, les évolutions du schéma sont difficiles à tracer et à reproduire entre environnements.

## Décision
Utiliser Liquibase pour gérer les migrations de base de données.
Les changelogs seront écrits en YAML et stockés dans `src/main/resources/db/changelog/`.

## Conséquences
- Migrations versionnées et tracées dans le code source
- Reproductibilité garantie entre les environnements (dev, test, prod)
- Compatible avec H2 en développement et toute base relationnelle en production
- Intégration native avec Spring Boot (exécution automatique au démarrage)
- Toute modification du schéma doit passer par un changelog Liquibase (jamais de DDL manuel)
