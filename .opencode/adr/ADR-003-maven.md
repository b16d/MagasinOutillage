# ADR-003 — Maven

## Statut
Accepté

## Contexte
Le projet nécessite un outil de build et de gestion des dépendances.
Les alternatives considérées sont Maven et Gradle.

## Décision
Utiliser Maven comme build system, avec le group ID `fr.magasinoutillage`.

## Conséquences
- Configuration déclarative via `pom.xml`, lisible et bien documentée
- Large compatibilité avec les outils CI/CD et les IDE
- Gestion des dépendances mature via Maven Central
- Moins flexible que Gradle pour les builds complexes
- Syntaxe XML plus verbeuse que le DSL Kotlin de Gradle
