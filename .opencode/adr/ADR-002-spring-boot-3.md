# ADR-002 — Spring Boot 3

## Statut
Accepté

## Contexte
Le projet nécessite un framework web pour exposer une API REST en Java.
Plusieurs options ont été considérées : Spring Boot 3, Quarkus, Micronaut.

## Décision
Utiliser Spring Boot 3 comme framework web.

## Conséquences
- Écosystème mature et très large adoption dans l'industrie
- Support Jakarta EE 10 (jakarta.* au lieu de javax.*)
- Intégration native avec Spring Data JPA, Spring Security, Spring Validation
- Démarrage plus lent qu'un framework cloud-native (Quarkus/Micronaut)
- Consommation mémoire plus élevée qu'une alternative AOT
