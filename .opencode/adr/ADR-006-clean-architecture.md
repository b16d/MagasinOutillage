# ADR-006 — Clean Architecture (Ports & Adapters)

## Statut
Accepté

## Contexte
Le projet nécessite un pattern d'organisation du code clair et maintenable.
Les alternatives considérées sont l'architecture en couches (N-tiers), DDD et Clean Architecture.

## Décision
Adopter la Clean Architecture avec le pattern Ports & Adapters.
Chaque domaine est organisé en trois couches : `domain`, `application`, `infrastructure`.

## Conséquences
- Le domaine métier est totalement indépendant du framework (testable sans Spring)
- Les dépendances pointent toujours vers l'intérieur (domain ne dépend de rien)
- Facilite les tests unitaires des use cases sans infrastructure
- Permet de remplacer un adapter (ex: H2 → PostgreSQL) sans toucher au domaine
- Légère verbosité supplémentaire par rapport à une architecture N-tiers classique
