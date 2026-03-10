# Skill — Spring Boot 3

## Jakarta EE 10
- Toujours utiliser jakarta.* (jamais javax.*)

## Configuration
- Fichier de configuration : application.yml exclusivement (pas application.properties)

## Exposition REST
- Ne jamais exposer une entité JPA directement dans un controller
- Toujours utiliser des DTOs pour les requêtes et les réponses
- Versioning via le path : /api/v1/...
- Réponses avec ResponseEntity<T>

## Validation
- Annoter les DTOs de requête avec les contraintes Bean Validation (@NotBlank, @Positive, etc.)
- Activer la validation avec @Valid dans les controllers

## Gestion des erreurs
- Centraliser la gestion des erreurs dans un @RestControllerAdvice
- Ne jamais laisser remonter une exception non gérée

## Responsabilités
- Controllers : routage et mapping uniquement, aucune logique métier
