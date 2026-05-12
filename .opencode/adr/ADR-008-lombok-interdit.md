# ADR-008 — Lombok interdit

## Statut
Accepté

## Contexte
Lombok est souvent utilisé pour réduire le boilerplate Java (getters, setters, builders, etc.).
Avec Java 25, les records natifs couvrent les mêmes besoins de manière plus explicite et sans dépendance externe.

## Décision
Lombok est interdit dans ce projet.

## Conséquences
- Utiliser les records Java 25 à la place de @Data, @Value, @Builder, @Getter, @Setter
- Le code est plus lisible et ne dépend pas d'un processeur d'annotations externe
- Pas de risque de compatibilité entre Lombok et les futures versions du JDK
- Légèrement plus verbeux pour les classes mutables, mais les classes mutables sont à éviter (cf. règle d'immutabilité)
