# Skill — Clean Architecture

## Structure par domaine
```
src/main/java/fr/magasinoutillage/
└── {domain}/
    ├── domain/
    │   ├── model/         ← entités et value objects
    │   ├── port/          ← interfaces (ports entrants et sortants)
    │   └── exception/     ← exceptions métier
    ├── application/
    │   └── usecase/       ← use cases (services d'application)
    └── infrastructure/
        ├── persistence/   ← adapter sortant (JPA)
        └── web/           ← adapter entrant (REST controller + DTOs)
```

## Règles de dépendance
- domain : aucune dépendance vers Spring, JPA ou tout autre framework
- application : dépend uniquement de domain ; orchestre via les ports
- infrastructure : implémente les ports ; dépend de domain et application
- La règle absolue : les dépendances pointent toujours vers l'intérieur

## Ports
- Les interfaces (ports) sont définies dans domain/port/
- Les implémentations (adapters) sont dans infrastructure/

## Tests
- Les use cases (application) se testent sans Spring context (tests unitaires purs)
- Les adapters se testent avec des tests d'intégration ciblés
- Stack de test : JUnit 5 + AssertJ + Mockito
