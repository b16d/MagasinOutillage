# Skill — Java 25

## Fonctionnalités modernes à utiliser
- Records pour les value objects et DTOs (immutables par nature)
- Sealed interfaces/classes pour modéliser des résultats ou états finis
- Pattern matching : switch avec guards, instanceof avec destructuring
- Text blocks pour les chaînes multilignes (SQL, JSON de test, etc.)
- Virtual threads (Thread.ofVirtual()) pour les opérations I/O bloquantes

## Null safety
- Ne jamais retourner null
- Utiliser Optional<T> pour les valeurs potentiellement absentes
- Ne jamais passer null en paramètre

## Immutabilité
- Champs final par défaut
- Collections non-modifiables (List.of, Map.of, Collections.unmodifiableList)

## Conventions de nommage
- Classes : PascalCase
- Méthodes et variables : camelCase
- Constantes : UPPER_SNAKE_CASE
- Packages : tout en minuscules, sans underscore

## Imports
- Toujours explicites (pas de wildcard import java.util.*)
