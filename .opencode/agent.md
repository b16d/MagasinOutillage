# Agent — MagasinOutillage

## Contexte
Back-end d'un service de vente d'outillage en ligne.

## Stack technique
- Java 25
- Spring Boot 3
- Maven (group ID : fr.magasinoutillage)
- Base de données : H2 (in-memory, développement)
- Migrations : Liquibase (changelogs en YAML)
- Architecture : Monolithique — Clean Architecture (ports & adapters)

## Règles générales
- Langue du code (classes, méthodes, variables) : anglais
- Langue de la prose (commentaires, messages d'erreur, commits) : français
- Respecter strictement les règles définies dans chaque skill
- Toute nouvelle décision d'architecture doit faire l'objet d'un ADR dans `.opencode/adr/`

## Skills actifs
- java
- spring-boot
- clean-arch
- commit

## Workflow Git
- Avant chaque commit, créer une branche dédiée avec un nom explicite (ex: feat/catalogue-product-entity)
- Rédiger le détail du commit : message court (50 chars max) + description des changements
- Ne jamais faire de push — le push est effectué par l'utilisateur
